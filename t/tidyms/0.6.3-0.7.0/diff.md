# Comparing `tmp/tidyms-0.6.3.tar.gz` & `tmp/tidyms-0.7.0.tar.gz`

## Comparing `tidyms-0.6.3.tar` & `tidyms-0.7.0.tar`

### file list

```diff
@@ -1,106 +1,116 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 tidyms-0.6.3/.coveragerc
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 tidyms-0.6.3/.readthedocs.yml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tidyms-0.6.3/MANIFEST.in
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tidyms-0.6.3/Makefile
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 tidyms-0.6.3/TODO.md
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 tidyms-0.6.3/pruebas.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 tidyms-0.6.3/requirements.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tidyms-0.6.3/test_requirements.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 tidyms-0.6.3/tox.ini
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/Makefile
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/api.rst
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/bokeh_plots.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/chem.rst
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/conf.py
--rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/data-curation.rst
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/descriptors.csv
--rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/feature-correspondence.rst
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/fileio.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/fileio_tutorial.rst
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/glossary.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/index.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/installation.rst
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/mzml.rst
--rw-r--r--   0        0        0    15021 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/peak-picking.rst
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/preprocessing-steps.csv
--rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/processing_datasets.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/quickstart.rst
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/requirements.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/tutorials.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/examples/custom_peak_descriptors.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/examples/roi-creation.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/plots/dbscan-clustering.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/plots/dbscan-parameters.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/plots/gmm-clustering.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/plots/peak-definition.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/plots/peak-detection-example.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/plots/peak_detection_baseline_example.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 tidyms-0.6.3/docs/plots/roi-definition.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/__init__.py
--rw-r--r--   0        0        0    15157 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/_batch_corrector.py
--rw-r--r--   0        0        0    11115 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/_build_data_matrix.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/_constants.py
--rw-r--r--   0        0        0    19106 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/_filter_functions.py
--rw-r--r--   0        0        0    17013 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/_mzml.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/_names.py
--rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/_plot_bokeh.py
--rw-r--r--   0        0        0    20037 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/annotation.py
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/assay.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/consensus_annotation.py
--rw-r--r--   0        0        0    57865 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/container.py
--rw-r--r--   0        0        0    14387 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/correspondence.py
--rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/fileio.py
--rw-r--r--   0        0        0    10049 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/fill_missing.py
--rw-r--r--   0        0        0    43419 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/filter.py
--rw-r--r--   0        0        0    26243 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/lcms.py
--rw-r--r--   0        0        0    21095 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/peaks.py
--rw-r--r--   0        0        0    36103 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/raw_data_utils.py
--rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/simulation.py
--rw-r--r--   0        0        0    14829 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/utils.py
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/validation.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/__init__.py
--rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/_envelope_utils.py
--rw-r--r--   0        0        0    25516 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/_formula_generator.py
--rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/atoms.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/elements.json
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/envelope_finder.py
--rw-r--r--   0        0        0    25557 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/envelope_tools.py
--rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/formula.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/formula_generator_utils.pyx
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/isotope_distribution_utils.pyx
--rw-r--r--   0        0        0    28834 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/isotopes.json
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/mmi_finder.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tidyms-0.6.3/src/tidyms/chem/utils.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/conftest.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/integration/test_assay_real_data.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/integration/test_real_raw_data.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_annotation.py
--rw-r--r--   0        0        0    21242 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_assay.py
--rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_batch_corrector.py
--rw-r--r--   0        0        0    16102 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_build_data_matrix.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_consensus_annotation.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_correspondence.py
--rw-r--r--   0        0        0    17149 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_data_container.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_fileio.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_fill_missing.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_filter.py
--rw-r--r--   0        0        0     9222 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_lcms.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_peaks.py
--rw-r--r--   0        0        0    32420 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_raw_data_utils.py
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_utils.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_validation.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_chem/test_atoms.py
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_chem/test_envelope_finder.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_chem/test_formula.py
--rw-r--r--   0        0        0    20397 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_chem/test_formula_generator.py
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_chem/test_isotope_distributions.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_chem/test_isotope_scorer.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 tidyms-0.6.3/tests/unit/test_chem/test_mmi_finder.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tidyms-0.6.3/.gitignore
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 tidyms-0.6.3/LICENSE
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 tidyms-0.6.3/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 tidyms-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 tidyms-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 tidyms-0.7.0/.coveragerc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tidyms-0.7.0/.flake8
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 tidyms-0.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tidyms-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tidyms-0.7.0/Makefile
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 tidyms-0.7.0/TODO.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tidyms-0.7.0/conftest.py
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 tidyms-0.7.0/prueba.ipynb
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tidyms-0.7.0/pruebas.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 tidyms-0.7.0/requirements.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tidyms-0.7.0/test_requirements.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 tidyms-0.7.0/tox.ini
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/api.rst
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/bokeh_plots.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/chem.rst
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/data-curation.rst
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/descriptors.csv
+-rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/feature-correspondence.rst
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/fileio.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/fileio_tutorial.rst
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/glossary.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/index.rst
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/installation.rst
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/mzml.rst
+-rw-r--r--   0        0        0    15044 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/peak-picking.rst
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/preprocessing-steps.csv
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/processing_datasets.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/quickstart.rst
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/requirements.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/tutorials.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0  2719101 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/examples/DARTMS_processing.ipynb
+-rw-r--r--   0        0        0   464433 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/examples/DARTMS_processing_ParameterOptimization.ipynb
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/examples/custom_peak_descriptors.py
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/examples/defined_spots_supervised.tsv
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/examples/roi-creation.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/plots/dbscan-clustering.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/plots/dbscan-parameters.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/plots/gmm-clustering.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/plots/peak-definition.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/plots/peak-detection-example.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/plots/peak_detection_baseline_example.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 tidyms-0.7.0/docs/plots/roi-definition.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/__init__.py
+-rw-r--r--   0        0        0    15003 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/_batch_corrector.py
+-rw-r--r--   0        0        0    11115 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/_build_data_matrix.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/_constants.py
+-rw-r--r--   0        0        0    17547 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/_filter_functions.py
+-rw-r--r--   0        0        0    17214 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/_mzml.py
+-rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/_plot_bokeh.py
+-rw-r--r--   0        0        0    63922 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/assay.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/consensus_annotation.py
+-rw-r--r--   0        0        0    57004 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/container.py
+-rw-r--r--   0        0        0    14387 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/correspondence.py
+-rw-r--r--   0        0        0   230965 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/dartms.py
+-rw-r--r--   0        0        0    38093 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/fileio.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/fill_missing.py
+-rw-r--r--   0        0        0    42488 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/filter.py
+-rw-r--r--   0        0        0    31241 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/lcms.py
+-rw-r--r--   0        0        0    21152 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/peaks.py
+-rw-r--r--   0        0        0    37111 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/raw_data_utils.py
+-rw-r--r--   0        0        0    12659 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/simulation.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/utils.py
+-rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/validation.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/annotation/__init__.py
+-rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/annotation/annotation.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/annotation/annotation_data.py
+-rw-r--r--   0        0        0     8551 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/annotation/envelope_finder.py
+-rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/annotation/mmi_finder.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/assay/assay_processor.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/__init__.py
+-rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/_envelope_utils.py
+-rw-r--r--   0        0        0    25516 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/_formula_generator.py
+-rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/atoms.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/elements.json
+-rw-r--r--   0        0        0    25557 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/envelope_tools.py
+-rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/formula.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/formula_generator_utils.pyx
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/isotope_distribution_utils.pyx
+-rw-r--r--   0        0        0    28834 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/isotopes.json
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tidyms-0.7.0/src/tidyms/chem/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/integration/test_assay_real_data.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/integration/test_real_raw_data.py
+-rw-r--r--   0        0        0    22251 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_assay.py
+-rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_batch_corrector.py
+-rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_build_data_matrix.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_consensus_annotation.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_correspondence.py
+-rw-r--r--   0        0        0    17090 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_data_container.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_fileio.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_fill_missing.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_filter.py
+-rw-r--r--   0        0        0    12761 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_lcms.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_peaks.py
+-rw-r--r--   0        0        0    32060 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_raw_data_utils.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_validation.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/annotation/test_annotation.py
+-rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/annotation/test_envelope_finder.py
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/annotation/test_mmi_finder.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_chem/test_atoms.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_chem/test_formula.py
+-rw-r--r--   0        0        0    20397 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_chem/test_formula_generator.py
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_chem/test_isotope_distributions.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 tidyms-0.7.0/tests/unit/test_chem/test_isotope_scorer.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 tidyms-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 tidyms-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 tidyms-0.7.0/README.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 tidyms-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 tidyms-0.7.0/PKG-INFO
```

### Comparing `tidyms-0.6.3/docs/Makefile` & `tidyms-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/api.rst` & `tidyms-0.7.0/docs/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -64,7 +64,8 @@
     tidyms.peaks
     tidyms.raw_data_utils
     tidyms.utils
     tidyms.chem.atoms
     tidyms.chem.envelope_tools
     tidyms.chem.formula
 
+    tidyms.dartms
```

### Comparing `tidyms-0.6.3/docs/bokeh_plots.py` & `tidyms-0.7.0/docs/bokeh_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     filename = "NZ_20200227_039.mzML"
     dataset = "test-nist-raw-data"
     ms.fileio.download_tidyms_data(dataset, [filename])
     path = Path(ms.fileio.get_tidyms_path())
     path = path.joinpath(dataset, filename)
 
-    ms_data = ms.MSData(
+    ms_data = ms.MSData.create_MSData_instance(
         path,
         ms_mode="centroid",
         instrument="qtof",
         separation="uplc"
     )
     mz_list = np.array([189.0734])
     return ms.make_chromatograms(ms_data, mz_list)[0]
```

### Comparing `tidyms-0.6.3/docs/chem.rst` & `tidyms-0.7.0/docs/chem.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/conf.py` & `tidyms-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/data-curation.rst` & `tidyms-0.7.0/docs/data-curation.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/feature-correspondence.rst` & `tidyms-0.7.0/docs/feature-correspondence.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/fileio.rst` & `tidyms-0.7.0/docs/fileio.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 --------
 
 Raw MS data in the mzML format can be read through the :class:`~tidyms.MSData`
 object.
 
 .. code-block:: python
 
-    ms_data = ms.MSData(
+    ms_data = ms.MSData.create_MSData_instance(
         filename,
         ms_mode="centroid",
         instrument="qtof",
         separation="uplc"
     )
 
 It is necessary to specify if the data is in centroid or profile mode using the
```

### Comparing `tidyms-0.6.3/docs/glossary.rst` & `tidyms-0.7.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/index.rst` & `tidyms-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/installation.rst` & `tidyms-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/mzml.rst` & `tidyms-0.7.0/docs/mzml.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/peak-picking.rst` & `tidyms-0.7.0/docs/peak-picking.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     import numpy as np
     import tidyms as ms
 
     filename = "NZ_20200227_039.mzML"
     dataset = "test-nist-raw-data"
     ms.fileio.download_tidyms_data(dataset, [filename], download_dir=".")
 
-    ms_data = ms.MSData(
+    ms_data = ms.MSData.create_MSData_instance(
         filename,
         ms_mode="centroid",
         instrument="qtof",
         separation="uplc"
     )
```

### Comparing `tidyms-0.6.3/docs/processing_datasets.rst` & `tidyms-0.7.0/docs/processing_datasets.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/quickstart.rst` & `tidyms-0.7.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/examples/custom_peak_descriptors.py` & `tidyms-0.7.0/docs/examples/custom_peak_descriptors.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/examples/roi-creation.py` & `tidyms-0.7.0/docs/examples/roi-creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,10 +11,14 @@
 ftp.cwd(sample_path)
 with open(filename, "wb") as fin:
     ftp.retrbinary("RETR " + filename, fin.write)
 ftp.close()
 
 # specifying instrument and separation used in the experiments provides better
 # default values for several functions used in
-ms_data = ms.MSData(filename, ms_mode="centroid", instrument="qtof",
-                    separation="uplc")
+ms_data = ms.MSData.create_MSData_instance(
+    filename, 
+    ms_mode="centroid", 
+    instrument="qtof",
+    separation="uplc"
+    )
 roi_list = ms_data.make_roi()
```

### Comparing `tidyms-0.6.3/docs/plots/dbscan-clustering.py` & `tidyms-0.7.0/docs/plots/dbscan-clustering.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/plots/dbscan-parameters.py` & `tidyms-0.7.0/docs/plots/dbscan-parameters.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/plots/gmm-clustering.py` & `tidyms-0.7.0/docs/plots/gmm-clustering.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/plots/peak-definition.py` & `tidyms-0.7.0/docs/plots/peak-definition.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/plots/peak-detection-example.py` & `tidyms-0.7.0/docs/plots/peak-detection-example.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/plots/peak_detection_baseline_example.py` & `tidyms-0.7.0/docs/plots/peak_detection_baseline_example.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/docs/plots/roi-definition.py` & `tidyms-0.7.0/docs/plots/roi-definition.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/__init__.py` & `tidyms-0.7.0/src/tidyms/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 from . import fill_missing
 from . import consensus_annotation
 from .container import DataContainer
 from .fileio import MSData
 from .lcms import Chromatogram, MSSpectrum
 from .assay import Assay
 from .raw_data_utils import *
-from . import annotation
+from . import dartms
+from .annotation import annotation
 
 utils.create_tidyms_dir()
 SETTINGS = utils.get_settings()
 
 if SETTINGS["bokeh"]["apply_theme"]:
     from bokeh.themes import Theme as _Theme
     from bokeh.io import curdoc as _curdoc
     theme = SETTINGS["bokeh"]["theme"]
     _curdoc().theme = _Theme(json=theme)
 
 if utils.is_notebook():
     from bokeh.plotting import output_notebook as _output_notebook
-    _output_notebook()
+
+    _output_notebook()
```

### Comparing `tidyms-0.6.3/src/tidyms/_batch_corrector.py` & `tidyms-0.7.0/src/tidyms/_batch_corrector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,82 @@
 import numpy as np
 import pandas as pd
 from scipy.interpolate import interp1d
 from statsmodels.nonparametric.smoothers_lowess import lowess
 from sklearn.model_selection import LeaveOneOut, ShuffleSplit, GridSearchCV
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.utils.validation import check_X_y
+from sklearn.exceptions import NotFittedError
 from joblib import Parallel, delayed
-from typing import List, Optional, Tuple
+from typing import Optional, Tuple
 from tqdm.notebook import tqdm
 from functools import partial
 
-MIN_LOESS_SIZE = 4      # the minimum number of points necessary to use LOESS
+MIN_LOESS_SIZE = 4  # the minimum number of points necessary to use LOESS
 
 
 def find_invalid_samples(
-    sample_metadata: pd.DataFrame,
-    sample_class: List[str],
-    qc_class: List[str]
+    sample_metadata: pd.DataFrame, sample_class: list[str], qc_class: list[str]
 ) -> pd.Index:
     """
     Finds samples that cannot be corrected using LOESS batch correction.
 
     Parameters
     ----------
     sample_metadata : DataFrame
         sample metadata from a DataContainer
-    sample_class : List[str]
+    sample_class : list[str]
         Classes where the correction is going to be applied.
-    qc_class : List[str]
+    qc_class : list[str]
         Classes used to estimate the correction factor.
 
     Returns
     -------
     invalid_samples = pd.Index
 
     """
     invalid_samples = pd.Index([])
     for name, gdf in sample_metadata.groupby("batch"):
+        gdf: pd.DataFrame
         qc_mask = gdf["class"].isin(qc_class)
         sample_mask = gdf["class"].isin(sample_class)
         qc_order = gdf.loc[qc_mask, "order"]
-        sample_order = gdf.loc[sample_mask, "order"]    # type: pd.Series
+        sample_order = gdf.loc[sample_mask, "order"]  # type: pd.Series
         min_qc_order = qc_order.min()
         max_qc_order = qc_order.max()
         n_qc = qc_order.size
         if n_qc >= MIN_LOESS_SIZE:
-            mask = (
-                    (sample_order < min_qc_order) |
-                    (sample_order > max_qc_order)
-            )
+            mask = (sample_order < min_qc_order) | (sample_order > max_qc_order)
             rm_index = mask[mask].index
         else:
             rm_index = gdf.index
         invalid_samples = invalid_samples.union(rm_index)
     return invalid_samples
 
 
 def find_invalid_features(
     data_matrix: pd.DataFrame,
     sample_metadata: pd.DataFrame,
-    sample_class: List[str],
-    qc_class: List[str],
+    sample_class: list[str],
+    qc_class: list[str],
     threshold: float,
-    min_detection_rate: float
+    min_detection_rate: float,
 ) -> pd.Index:
     """
     Remove features detected in a low number of QC samples.
 
     Parameters
     ----------
     data_matrix : DataFrame
         data matrix from a DataContainer
     sample_metadata : DataFrame
         sample metadata from a DataContainer
-    sample_class : List[str]
+    sample_class : list[str]
         Classes where the correction is going to be applied.
-    qc_class : List[str]
+    qc_class : list[str]
         Classes used to estimate the correction factor.
     threshold : positive number
         Minimum value to consider a feature detected.
     min_detection_rate : number between 0 and 1
         Minimum fraction of samples where a feature was detected
 
     Returns
@@ -87,76 +84,73 @@
     invalid_features : pd.Index
 
     """
     invalid_features = pd.Index([])
     for name, gdf in sample_metadata.groupby("batch"):
         qc_mask = gdf["class"].isin(qc_class)
         sample_mask = gdf["class"].isin(sample_class)
-        qc_order = gdf.loc[qc_mask, "order"]    # type: pd.Series
+        qc_order = gdf.loc[qc_mask, "order"]  # type: pd.Series
         sample_order = gdf.loc[sample_mask, "order"]
         min_sample_order = sample_order.min()
         max_sample_order = sample_order.max()
 
         # first block: qc samples before any study samples
         first_block_samples = qc_order < min_sample_order
         first_block_samples = first_block_samples[first_block_samples].index
         first_block_n = data_matrix.loc[first_block_samples, :]
         first_block_n = (first_block_n > threshold).sum()
 
         # middle block: qc sample measured between study samples
-        middle_block_samples = ((qc_order > min_sample_order) |
-                                (qc_order < max_sample_order))
+        middle_block_samples = (qc_order > min_sample_order) | (qc_order < max_sample_order)
         middle_block_samples = middle_block_samples[middle_block_samples].index
         middle_block_n = data_matrix.loc[middle_block_samples, :]
         middle_block_n = (middle_block_n > threshold).sum()
 
         # last block: qc samples after all study samples
         last_block_samples = qc_order > max_sample_order
         last_block_samples = last_block_samples[last_block_samples].index
         last_block_n = data_matrix.loc[last_block_samples, :]
         last_block_n = (last_block_n > threshold).sum()
 
         total = first_block_n + middle_block_n + last_block_n
         valid_blocks = (
-            (first_block_n > 0) &
-            (middle_block_n > 0) &
-            (last_block_n > 0)
-        )    # type: pd.Series
-        valid_n = (total >= MIN_LOESS_SIZE)
+            (first_block_n > 0) & (middle_block_n > 0) & (last_block_n > 0)
+        )  # type: pd.Series
+        valid_n = total >= MIN_LOESS_SIZE
         n_rows = qc_order.size
-        valid_dr = (total / n_rows) >= min_detection_rate   # type: pd.Series
+        valid_dr = (total / n_rows) >= min_detection_rate  # type: pd.Series
         invalid_mask = ~(valid_n & valid_blocks & valid_dr)
         rm_features = invalid_mask[invalid_mask].index
         invalid_features = invalid_features.union(rm_features)
     return invalid_features
 
 
 def correct_batches(
     data_matrix: pd.DataFrame,
     sample_metadata: pd.DataFrame,
-    sample_class: List[str],
-    qc_class: List[str],
+    sample_class: list[str],
+    qc_class: list[str],
     threshold: float = 0.0,
     frac: Optional[float] = None,
     first_n: Optional[int] = None,
     n_jobs: Optional[int] = None,
-    verbose: bool = True
+    verbose: bool = True,
 ) -> pd.DataFrame:
     """
     Inter-batch correction using LOESS smoothing.
 
     Parameters
     ----------
     data_matrix : DataFrame
         data matrix from a DataContainer
     sample_metadata : DataFrame
         sample metadata from a DataContainer
-    sample_class : List[str]
+    sample_class : list[str]
         Classes where the correction is going to be applied.
-    qc_class : List[str]
+    qc_class : list[str]
         Classes used to estimate the correction factor.
     threshold : positive number
         Minimum value to consider a feature detected. Features in QC samples
         above this value are used to compute the correction factor.
     frac : Number between 0 and 1.0 or None, default=None
         frac value passed to LOESS function. If None, value is optimized for
         each feature using cross validation.
@@ -176,19 +170,15 @@
     corrected: DataFrame
         Data matrix with the correction applied.
 
     """
     # data matrix is split into columns, and each column is split according to
     # the number of batches.
     iterator = _split_data_matrix(
-        data_matrix,
-        sample_metadata,
-        sample_class,
-        qc_class,
-        threshold
+        data_matrix, sample_metadata, sample_class, qc_class, threshold
     )
 
     if verbose:
         n_ft = data_matrix.shape[1]
         n_batch = sample_metadata["batch"].unique().size
         desc = "Correcting {} features in {} batches".format(n_ft, n_batch)
         total = _get_tqdm_total(data_matrix, sample_metadata)
@@ -196,36 +186,33 @@
 
     # intra-batch correction
     corrector_func = partial(_correct_intra_batch, first_n=first_n, frac=frac)
     func = delayed(corrector_func)
     data = Parallel(n_jobs=n_jobs)(func(x) for x in iterator)
     data_corrected = _rebuild_data_matrix(data_matrix.shape, data)
     data_corrected = pd.DataFrame(
-        data=data_corrected,
-        index=data_matrix.index,
-        columns=data_matrix.columns
+        data=data_corrected, index=data_matrix.index, columns=data_matrix.columns
     )
     # inter-batch correction
-    data_corrected = _inter_batch_correction(
-        data_corrected, sample_metadata, qc_class
-    )
+    data_corrected = _inter_batch_correction(data_corrected, sample_metadata, qc_class)
 
     return data_corrected
 
 
 class _LoessCorrector(BaseEstimator, RegressorMixin):
     """
     Intra-batch corrector implementation using sklearn.
 
     Parameters
     ----------
     frac : number between 0 and 1, default=0.66
         Fraction of samples used for local regressions
 
     """
+
     def __init__(self, frac: float = 0.66):
         """
         Constructor function.
 
         """
 
         self.frac = frac
@@ -233,46 +220,45 @@
 
     def fit(self, X, y):
 
         # Check that X and y have correct shape
         X, y = check_X_y(X, y)
         # Store the classes seen during fit
         x = X.flatten()
-        y_fit = lowess(
-            y, x, frac=self.frac, is_sorted=True, return_sorted=False
-        )
+        y_fit = lowess(y, x, frac=self.frac, is_sorted=True, return_sorted=False)
         fill = (y[0], y[-1])
-        self.interpolator_ = interp1d(
-            x, y_fit, fill_value=fill, bounds_error=False)
+        self.interpolator_ = interp1d(x, y_fit, fill_value=fill, bounds_error=False)
         return self
 
     def predict(self, X):
+        if self.interpolator_ is None:
+            raise NotFittedError
         xf = X.flatten()
         x_interp = self.interpolator_(xf)
         return x_interp
 
 
 def _split_data_matrix(
-        data_matrix: pd.DataFrame,
-        sample_metadata: pd.DataFrame,
-        sample_class: List[str],
-        qc_class: List[str],
-        threshold: float
+    data_matrix: pd.DataFrame,
+    sample_metadata: pd.DataFrame,
+    sample_class: list[str],
+    qc_class: list[str],
+    threshold: float,
 ):
     """
     Yields chunks of the data matrix and the order array associated with the
     data. Aux function to correct_batches.
 
     Parameters
     ----------
     data_matrix : DataFrame
     sample_metadata : DataFrame
-    sample_class : List[str]
+    sample_class : list[str]
         classes where the correction will be applied
-    qc_class : List[str]
+    qc_class : list[str]
         classes used to create the correction
     threshold : positive number
         Minimum value to consider a feature detected.
     Yields
     -------
     row_start : int
         index of row where x starts.
@@ -305,17 +291,15 @@
             x = X[index + start_index, column]
             ft_train_index = train_index[x[train_index] >= threshold]
             yield start_index, column, order, x, ft_train_index, predict_index
         start_index += g.shape[0]
 
 
 def _correct_intra_batch(
-        args: Tuple,
-        frac: Optional[float] = None,
-        first_n: Optional[int] = None
+    args: Tuple, frac: Optional[float] = None, first_n: Optional[int] = None
 ) -> Tuple[np.ndarray, np.ndarray, int]:
     """
     Apply LOESS correction on features in a batch. Aux function to
     correct_batches.
 
     Parameters
     ----------
@@ -358,25 +342,25 @@
         x_mean = x[train_index[:first_n]].mean()
     else:
         x_mean = x[train_index].mean()
 
     # compute corrected values
     x_qc = corrector.predict(x_predict)
     factor = np.zeros_like(x_qc)
-    # correct nans in zero values and negative values generated during LOESS
+    # correct nan in zero values and negative values generated during LOESS
     is_positive = x_qc > 0
     factor = np.divide(x_mean, x_qc, out=factor, where=is_positive)
     corrected = y_predict * factor
     x[predict_index] = corrected
 
     index = np.arange(x.size) + start_index
     return x, index, column
 
 
-def _rebuild_data_matrix(shape, data: List[Tuple]) -> np.ndarray:
+def _rebuild_data_matrix(shape, data: list[Tuple]) -> np.ndarray:
     """
     Rebuilds the data matrix from the processed output. Aux function to\
     correct_batches.
 
     Parameters
     ----------
     shape : tuple
@@ -391,17 +375,15 @@
     Xr = np.zeros(shape=shape, dtype=float)
     for x, index, column in data:
         Xr[index, column] = x
     return Xr
 
 
 def _inter_batch_correction(
-        data_matrix: pd.DataFrame,
-        sample_metadata: pd.DataFrame,
-        qc_class: List[str]
+    data_matrix: pd.DataFrame, sample_metadata: pd.DataFrame, qc_class: list[str]
 ) -> pd.DataFrame:
     """
     corrects the mean in each batch to a common mean. Aux function to
     correct_batches.
 
     Parameters
     ----------
@@ -417,21 +399,20 @@
     batch = sample_metadata["batch"]
     qc_batch = batch[qc_mask]
     n_batches = batch.unique().size
     if n_batches == 1:
         res = data_matrix
     else:
         factor = _get_inter_batch_correction_factor(qc_dm, qc_batch)
-        res = data_matrix.groupby(batch).apply(lambda x: x * factor[x.name])
+        res = data_matrix.groupby(batch, group_keys=False).apply(lambda x: x * factor[x.name])
     return res
 
 
 def _get_inter_batch_correction_factor(
-        data_matrix: pd.DataFrame,
-        batch: pd.Series
+    data_matrix: pd.DataFrame, batch: pd.Series
 ) -> pd.DataFrame:
     """
     Estimates a correction factor for inter-batch correction. Aux function to
     _inter_batch_correction.
 
     """
     inter_batch_mean = data_matrix.mean()
@@ -469,16 +450,15 @@
         n_points = 5
         frac = np.linspace(min_frac, 1.0, n_points)
 
     grid_params = {"frac": frac}
     return grid_params
 
 
-def _get_tqdm_total(
-        data_matrix: pd.DataFrame, sample_metadata: pd.DataFrame) -> int:
+def _get_tqdm_total(data_matrix: pd.DataFrame, sample_metadata: pd.DataFrame) -> int:
     """
     Computes the number of items to compute a percentage in the progress bar.
 
     """
     _, n_ft = data_matrix.shape
     n_batch = sample_metadata["batch"].unique().size
     total = n_batch * n_ft
```

### Comparing `tidyms-0.6.3/src/tidyms/_build_data_matrix.py` & `tidyms-0.7.0/src/tidyms/_build_data_matrix.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/_constants.py` & `tidyms-0.7.0/src/tidyms/_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from typing import Final, List
 
-# TODO: merge with _names.py
+
 # separation modes
 HPLC: Final[str] = "hplc"
 UPLC: Final[str] = "uplc"
-LC_MODES: Final[List[str]] = [UPLC, HPLC]
+DART: Final[str] = "None/DART"
+LC_MODES: Final[List[str]] = [UPLC, HPLC, DART]
 SEPARATION_MODES: Final[List[str]] = LC_MODES + []
 
 # instruments
 QTOF: Final[str] = "qtof"
 ORBITRAP: Final[str] = "orbitrap"
 MS_INSTRUMENTS: Final[List[str]] = [QTOF, ORBITRAP]
 
 # MS mode
 CENTROID: Final[str] = "centroid"
 PROFILE: Final[str] = "profile"
 MS_MODES: Final[List[str]] = [CENTROID, PROFILE]
 
+# Data loading
+MEMORY: Final[str] = "memory"
+INFILE: Final[str] = "file"
+SIMULATED: Final[str] = "simulated"
+DATA_LOAD_MODES: Final[List[str]] = [MEMORY, INFILE, SIMULATED]
+DEFAULT_DATA_LOAD_MODE = INFILE
+
 # feature descriptors
 FEATURE: Final[str] = "feature"
 MZ: Final[str] = "mz"
 RT_START: Final[str] = "rt start"
 RT_END: Final[str] = "rt end"
 RT: Final[str] = "rt"
 RT_STD: Final[str] = "rt std"
@@ -29,25 +37,50 @@
 HEIGHT: Final[str] = "height"
 SNR: Final[str] = "snr"
 MZ_STD: Final[str] = "mz_std"
 ROI_INDEX: Final[str] = "roi_index"
 FT_INDEX: Final[str] = "ft_index"
 MERGED: Final[str] = "merged"
 
+# chromatogram names
+BASELINE: Final[str] = "baseline"
+NOISE: Final[str] = "noise"
+SPINT: Final[str] = "spint"  # spectral intensity
+ROI_FEATURE_LIST: Final[str] = "features"
+TIME: Final[str] = "time"
+SCAN: Final[str] = "scan"
+MODE: Final[str] = "mode"
+
+# peak names
+START: Final[str] = "start"
+APEX: Final[str] = "apex"
+END: Final[str] = "end"
+
 # isotopologue envelope annotation
 ENVELOPE_LABEL: Final[str] = "envelope_label"
 ENVELOPE_INDEX: Final[str] = "envelope_index"
 CHARGE: Final[str] = "charge"
 
 # sample metadata
-SAMPLE: Final[str] = "sample_"
-CLASS: Final[str] = "class_"
-ORDER: Final[str] = "order_"
-BATCH: Final[str] = "batch_"
-LABEL: Final[str] = "cluster_"
+SAMPLE: Final[str] = "sample"
+CLASS: Final[str] = "class"
+ORDER: Final[str] = "order"
+BATCH: Final[str] = "batch"
+LABEL: Final[str] = "cluster"
+ID: Final[str] = "id"
+DILUTION: Final[str] = "dilution"
+TYPE: Final[str] = "type"
+
+# sample types
+QC_TYPE: Final[str] = "qc"
+DQC_TYPE: Final[str] = "dqc"
+STUDY_TYPE: Final[str] = "sample"
+BLANK_TYPE: Final[str] = "blank"
+SAMPLE_TYPES: Final[list[str]] = [QC_TYPE, STUDY_TYPE, BLANK_TYPE, DQC_TYPE]
+
 
 # assay file and dir names
 ROI_DIR: Final[str] = "roi"
 FT_DIR: Final[str] = "feature"
 MANAGER_FILENAME: Final[str] = "metadata.pickle"
 FT_TABLE_FILENAME: Final[str] = "feature-table.pickle"
 DATA_MATRIX_FILENAME: Final[str] = "data-matrix.pickle"
@@ -68,9 +101,9 @@
     EXTRACT_FEATURES,
     DESCRIBE_FEATURES,
     ANNOTATE_ISOTOPOLOGUES,
     ANNOTATE_ADDUCTS,
     BUILD_FEATURE_TABLE,
     MATCH_FEATURES,
     MAKE_DATA_MATRIX,
-    FILL_MISSING
+    FILL_MISSING,
 ]
```

### Comparing `tidyms-0.6.3/src/tidyms/_filter_functions.py` & `tidyms-0.7.0/src/tidyms/_filter_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,49 +4,20 @@
 
 import numpy as np
 import pandas as pd
 from scipy.interpolate import CubicSpline, interp1d
 from statsmodels.nonparametric.smoothers_lowess import lowess
 from typing import List, Callable, Union, Optional
 from .utils import mad
-from ._names import *
+from . import _constants as c
 
 
-# def input_na(df: pd.DataFrame, classes: pd.Series, mode: str) -> pd.DataFrame:
-#     """
-#     Fill missing values.
-#
-#     Parameters
-#     ----------
-#     df : pd.DataFrame
-#     classes: ps.Series
-#     mode : {'zero', 'mean', 'min'}
-#
-#     Returns
-#     -------
-#     filled : pd.DataFrame
-#     """
-#     if mode == "zero":
-#         return df.fillna(0)
-#     elif mode == "mean":
-#         return (df.groupby(classes)
-#                 .apply(lambda x: x.fillna(x.mean()))
-#                 .droplevel(0))
-#     elif mode == "min":
-#         return (df.groupby(classes)
-#                 .apply(lambda x: x.fillna(x.min()))
-#                 .droplevel(0))
-#     else:
-#         msg = "mode should be `zero`, `mean` or `min`"
-#         raise ValueError(msg)
-
-
-def average_replicates(data: pd.DataFrame, sample_id: pd.Series,
-                       classes: pd.Series,
-                       process_classes: List[str]) -> pd.DataFrame:
+def average_replicates(
+    data: pd.DataFrame, sample_id: pd.Series, classes: pd.Series, process_classes: List[str]
+) -> pd.DataFrame:
     """
     Group samples by id and computes the average.
 
     Parameters
     ----------
     data: pd.DataFrame
     sample_id: pd.Series
@@ -58,26 +29,30 @@
     """
     include_samples = classes[classes.isin(process_classes)].index
     exclude_samples = classes[~classes.isin(process_classes)].index
     mapper = sample_id[include_samples].drop_duplicates()
     mapper = pd.Series(data=mapper.index, index=mapper.values)
     included_data = data.loc[include_samples, :]
     excluded_data = data.loc[exclude_samples, :]
-    averaged_data = (included_data.groupby(sample_id[include_samples])
-                     .mean())
+    averaged_data = included_data.groupby(sample_id[include_samples]).mean()
     averaged_data.index = averaged_data.index.map(mapper)
     result = pd.concat((averaged_data, excluded_data)).sort_index()
     return result
 
 
-def correct_blanks(df: pd.DataFrame, classes: pd.Series,
-                   corrector_classes: List[str], process_classes: List[str],
-                   factor: float = 1.0, robust: bool = True,
-                   mode: Union[str, Callable] = "mean",
-                   process_blanks: bool = False) -> pd.DataFrame:
+def correct_blanks(
+    df: pd.DataFrame,
+    classes: pd.Series,
+    corrector_classes: List[str],
+    process_classes: List[str],
+    factor: float = 1.0,
+    robust: bool = True,
+    mode: Union[str, Callable] = "mean",
+    process_blanks: bool = False,
+) -> pd.DataFrame:
     """
     Correct samples using blanks.
 
     Parameters
     ----------
     df : pandas.DataFrame
         Data to correct.
@@ -102,18 +77,20 @@
     if robust:
         mean_func = lambda x: x.median()
         std_func = mad
     else:
         mean_func = lambda x: x.mean()
         std_func = lambda x: x.std()
 
-    corrector = {"max": lambda x: x.max(),
-                 "mean": lambda x: mean_func(x),
-                 "lod": lambda x: mean_func(x) + 3 * std_func(x),
-                 "loq": lambda x: mean_func(x) + 10 * std_func(x)}
+    corrector = {
+        "max": lambda x: x.max(),
+        "mean": lambda x: mean_func(x),
+        "lod": lambda x: mean_func(x) + 3 * std_func(x),
+        "loq": lambda x: mean_func(x) + 10 * std_func(x),
+    }
     if hasattr(mode, "__call__"):
         corrector = mode
     else:
         corrector = corrector[mode]
     samples = df[classes.isin(process_classes)]
     blanks = df[classes.isin(corrector_classes)]
 
@@ -124,16 +101,17 @@
     if process_blanks:
         corrected_blanks = blanks - correction
         corrected_blanks[(blanks - factor * correction) < 0] = 0
         df[classes.isin(corrector_classes)] = corrected_blanks
     return df
 
 
-def _loocv_loess(x: pd.Series, y: pd.Series, interpolator: Callable,
-                 frac: Optional[float] = None) -> tuple:
+def _loocv_loess(
+    x: pd.Series, y: pd.Series, interpolator: Callable, frac: Optional[float] = None
+) -> tuple:
     """
     Helper function for batch_correction. Computes loess correction with LOOCV.
 
     Parameters
     ----------
     x: pd.Series
     y: pd.Series
@@ -147,15 +125,15 @@
     corrected: pd.Series
         LOESS corrected data
     """
     if frac is None:
         # valid frac values, from 4/N to 1/N, where N is the number of corrector
         # samples.
         frac_list = [k / x.size for k in range(4, x.size + 1)]
-        rms = np.inf    # initial value for root mean square error
+        rms = np.inf  # initial value for root mean square error
         best_frac = 1
         for frac in frac_list:
             curr_rms = 0
             for loocv_index in x.index[1:-1]:
                 y_temp = y.drop(loocv_index)
                 x_temp = x.drop(loocv_index)
                 y_loess = lowess(y_temp, x_temp, return_sorted=False, frac=frac)
@@ -164,60 +142,65 @@
             if rms > curr_rms:
                 best_frac = frac
                 rms = curr_rms
         frac = best_frac
     return lowess(y, x, return_sorted=False, frac=frac)
 
 
-def _generate_batches(df: pd.DataFrame, run_order: pd.Series, batch: pd.Series,
-                      classes: pd.Series, corrector_classes: List[str],
-                      process_classes: List[str]):
-    batch_order = (pd.concat((batch, run_order), axis=1)
-                   .sort_values([_sample_batch, _sample_order]))
-    grouped = batch_order.groupby(_sample_batch)
+def _generate_batches(
+    df: pd.DataFrame,
+    run_order: pd.Series,
+    batch: pd.Series,
+    classes: pd.Series,
+    corrector_classes: List[str],
+    process_classes: List[str],
+):
+    batch_order = pd.concat((batch, run_order), axis=1).sort_values([c.BATCH, c.ORDER])
+    grouped = batch_order.groupby(c.BATCH)
     for n_batch, group in grouped:
         df_batch = df.loc[group.index, :]
         classes_batch = classes[group.index]
         process_df = df_batch.loc[classes_batch.isin(process_classes), :]
         corrector_df = df_batch.loc[classes_batch.isin(corrector_classes), :]
         process_order = run_order[process_df.index]
         corrector_order = run_order[corrector_df.index]
-        batch_order = (run_order[corrector_df.index.union(process_df.index)]
-                       .sort_values())
+        batch_order = run_order[corrector_df.index.union(process_df.index)].sort_values()
         corrector_df = corrector_df.set_index(corrector_order).sort_index()
         process_df = process_df.set_index(process_order).sort_index()
         yield corrector_df, process_df, batch_order
 
 
-def get_outside_bounds_index(data: Union[pd.Series, pd.DataFrame], lb: float,
-                             ub: float) -> pd.Index:
+def get_outside_bounds_index(
+    data: Union[pd.Series, pd.DataFrame], lb: float, ub: float
+) -> pd.Index:
     """
     return index of columns with values outside bounds.
     Parameters
     ----------
     data: pd.Series or pd.DataFrame
     lb: float
         lower bound
     ub: float
         upper bound
     Returns
     -------
 
     """
-    result = ((data < lb) | (data > ub))
+    result = (data < lb) | (data > ub)
     if isinstance(data, pd.DataFrame):
         result = result.all()
     if result.empty:
         return pd.Index([])
     else:
         return result[result].index
 
 
-def batch_ext(order: pd.Series, batch: pd.Series, classes: pd.Series,
-              class_list: List[str], ext: str) -> pd.Series:
+def batch_ext(
+    order: pd.Series, batch: pd.Series, classes: pd.Series, class_list: List[str], ext: str
+) -> pd.Series:
     """
     get minimum/maximum order of samples of classes in class_list. Auxiliary
     function to be used with BatchChecker / FeatureCheckerBatchCorrection
     Parameters
     ----------
     order: pandas.Series
         run order
@@ -233,30 +216,35 @@
     Returns
     -------
     pd.Series with the corresponding min/max order with batch as index.
     """
     func = {"min": lambda x: x.min(), "max": lambda x: x.max()}
     func = func[ext]
 
-    ext_order = (order
-                 .groupby([classes, batch])
-                 .apply(func)
-                 .reset_index()
-                 .groupby(classes.name)
-                 .filter(lambda x: x.name in class_list)
-                 .groupby(batch.name)
-                 .apply(func)[order.name])
+    ext_order = (
+        order.groupby([classes, batch])
+        .apply(func)
+        .reset_index()
+        .groupby(classes.name)
+        .filter(lambda x: x.name in class_list)
+        .groupby(batch.name)
+        .apply(func)[order.name]
+    )
     return ext_order
 
 
-def check_qc_prevalence(data_matrix: pd.DataFrame,
-                        batch: pd.Series, classes: pd.Series,
-                        qc_classes: List[str], sample_classes: List[str],
-                        threshold: float = 0,
-                        min_qc_dr: float = 0.9) -> pd.Index:
+def check_qc_prevalence(
+    data_matrix: pd.DataFrame,
+    batch: pd.Series,
+    classes: pd.Series,
+    qc_classes: List[str],
+    sample_classes: List[str],
+    threshold: float = 0,
+    min_qc_dr: float = 0.9,
+) -> pd.Index:
     """
     Remove features with low detection rate in the QC samples. Also check that
     each feature is detected in the first and last block (this step is necessary
     interpolate the bias contribution to biological samples).
 
     Aux function to use in the BatchCorrector Pipeline.
 
@@ -272,20 +260,21 @@
 
     Returns
     -------
     index of invalid features
     """
     invalid_features = pd.Index([])
     for batch_number, batch_class in classes.groupby(batch):
-        block_type, block_number = \
-            make_sample_blocks(batch_class, qc_classes, sample_classes)
+        block_type, block_number = make_sample_blocks(batch_class, qc_classes, sample_classes)
         qc_blocks = block_number[block_type == 0]
-        block_prevalence = (data_matrix.loc[qc_blocks.index]
-                            .groupby(qc_blocks)
-                            .apply(lambda x: (x > threshold).any()))
+        block_prevalence = (
+            data_matrix.loc[qc_blocks.index]
+            .groupby(qc_blocks)
+            .apply(lambda x: (x > threshold).any())
+        )
 
         # check start block
         start_block_mask = block_prevalence.loc[qc_blocks.iloc[0]]
         tmp_rm = data_matrix.columns[~start_block_mask]
         invalid_features = invalid_features.union(tmp_rm)
 
         # check end block
@@ -299,18 +288,24 @@
         batch_min_qc_dr = max(4 / n_blocks, min_qc_dr)
         tmp_rm = data_matrix.columns[qc_prevalence < batch_min_qc_dr]
         invalid_features = invalid_features.union(tmp_rm)
 
     return invalid_features
 
 
-def loess_interp(ft_data: pd.Series, order: pd.Series, qc_index: pd.Index,
-                 sample_index: pd.Index, frac: float, interpolator: Callable,
-                 n_qc: Optional[int] = None, method: str = "multiplicative"
-                 ) -> pd.Series:
+def loess_interp(
+    ft_data: pd.Series,
+    order: pd.Series,
+    qc_index: pd.Index,
+    sample_index: pd.Index,
+    frac: float,
+    interpolator: Callable,
+    n_qc: Optional[int] = None,
+    method: str = "multiplicative",
+) -> pd.Series:
     """
     Applies LOESS-correction interpolation on a feature. Auxiliary function of
     batch_corrector_func
 
     Parameters
     ----------
     ft_data: pd.Series
@@ -333,16 +328,15 @@
 
     qc_median = ft_data[qc_index[:n_qc]].median()
     # if there are several 0 values the median may be 0, this prevent against
     # such cases
     if np.isclose(qc_median, 0.0):
         qc_median = ft_data[qc_index[:n_qc]].mean()
 
-    qc_loess = _loocv_loess(order[qc_index], ft_data[qc_index], interpolator,
-                            frac=frac)
+    qc_loess = _loocv_loess(order[qc_index], ft_data[qc_index], interpolator, frac=frac)
     interp = interpolator(order[qc_index], qc_loess)
 
     if method == "additive":
         bias = interp(order[sample_index]) - qc_median
         ft_data[sample_index] -= bias
     elif method == "multiplicative":
         qc_smooth = interp(order[sample_index])
@@ -357,20 +351,25 @@
         ft_data[sample_index] *= factor
     else:
         msg = "Valid methods are `additive` or `multiplicative`."
         raise ValueError(msg)
     return ft_data
 
 
-def batch_corrector_func(df_batch: pd.DataFrame, order: pd.Series,
-                         classes: pd.Series, frac: float,
-                         interpolator: Callable, qc_classes: List[str],
-                         sample_classes: List[str],
-                         n_qc: Optional[int] = None,
-                         method: str = "multiplicative") -> pd.DataFrame:
+def batch_corrector_func(
+    df_batch: pd.DataFrame,
+    order: pd.Series,
+    classes: pd.Series,
+    frac: float,
+    interpolator: Callable,
+    qc_classes: List[str],
+    sample_classes: List[str],
+    n_qc: Optional[int] = None,
+    method: str = "multiplicative",
+) -> pd.DataFrame:
     """
     Applies LOESS correction - interpolation on a single batch. Auxiliary
     function of interbatch_correction.
 
     Parameters
     ----------
     df_batch: pandas.DataFrame
@@ -389,31 +388,36 @@
     -------
     pandas.DataFrame
     """
     qc_index = classes.isin(qc_classes)
     qc_index = qc_index[qc_index].index
     sample_index = classes.isin(sample_classes)
     sample_index = sample_index[sample_index].index
-    df_batch.loc[sample_index, :] = \
-        (df_batch.apply(loess_interp,
-                        args=(order, qc_index, sample_index, frac,
-                              interpolator),
-                        n_qc=n_qc, method=method))
+    df_batch.loc[sample_index, :] = df_batch.apply(
+        loess_interp,
+        args=(order, qc_index, sample_index, frac, interpolator),
+        n_qc=n_qc,
+        method=method,
+    )
     return df_batch
 
 
-def interbatch_correction(df: pd.DataFrame, order: pd.Series, batch: pd.Series,
-                          classes: pd.Series, corrector_classes: List[str],
-                          process_classes: List[str],
-                          frac: Optional[float] = None,
-                          interpolator: Optional[str] = "splines",
-                          n_qc: Optional[int] = None,
-                          process_qc: bool = True,
-                          method: str = "multiplicative"
-                          ) -> pd.DataFrame:
+def interbatch_correction(
+    df: pd.DataFrame,
+    order: pd.Series,
+    batch: pd.Series,
+    classes: pd.Series,
+    corrector_classes: List[str],
+    process_classes: List[str],
+    frac: Optional[float] = None,
+    interpolator: Optional[str] = "splines",
+    n_qc: Optional[int] = None,
+    process_qc: bool = True,
+    method: str = "multiplicative",
+) -> pd.DataFrame:
     r"""
     Correct instrument response drift using LOESS regression [1, 2]
     and center each batch to a common mean.
 
     Parameters
     ----------
     df : pandas.DataFrame
@@ -451,15 +455,15 @@
     References.
     -----
     .. [1] W B Dunn *et al*, "Procedures for large-scale metabolic profiling of
     serum and plasma using gas chromatography and liquid chromatography coupled
     to mass spectrometry", Nature Protocols volume 6, pages 1060–1083 (2011).
     .. [2] D Broadhurst *et al*, "Guidelines and considerations for the use of
     system suitability and quality control samples in mass spectrometry assays
-    applied in untargeted clinical metabolomic studies.", Metabolomics,
+    applied in untargeted clinical metabolomics studies.", Metabolomics,
     2018;14(6):72. doi: 10.1007/s11306-018-1367-3
 
     Notes
     -----
     The correction is applied as described by Broadhurst in [2]. Using QC
     samples a correction is generated for each feature in the following way:
     The signal of a Quality control can be described in terms of three
@@ -480,27 +484,32 @@
 
     if process_qc:
         # add QC classes to process classes
         process_classes = corrector_classes + process_classes
         process_classes = list(set(process_classes))
 
     def corrector_helper(df_group):
-        return batch_corrector_func(df_group, order[df_group.index],
-                                    classes[df_group.index], frac,
-                                    interp_func, corrector_classes,
-                                    process_classes, n_qc=n_qc,
-                                    method=method)
+        return batch_corrector_func(
+            df_group,
+            order[df_group.index],
+            classes[df_group.index],
+            frac,
+            interp_func,
+            corrector_classes,
+            process_classes,
+            n_qc=n_qc,
+            method=method,
+        )
 
     # intra batch correction
     corrected = df.groupby(batch).apply(corrector_helper)
 
     # inter batch mean alignment
     def batch_mean_func(df_group):
-        batch_mean = (df_group[classes[df_group.index].isin(corrector_classes)]
-                      .mean())
+        batch_mean = df_group[classes[df_group.index].isin(corrector_classes)].mean()
         is_process_sample = classes[df_group.index].isin(process_classes)
         if method == "additive":
             df_group[is_process_sample] -= batch_mean
         else:
             batch_mean[batch_mean <= 0] = np.nan
             df_group[is_process_sample] /= batch_mean
             df_group.fillna(0)
@@ -514,30 +523,31 @@
     else:
         corrected.loc[process_mask, :] *= global_median
     corrected[corrected < 0] = 0
 
     return corrected
 
 
-def make_sample_blocks(classes: pd.Series, corrector_classes: List[str],
-                       process_classes: List[str]):
+def make_sample_blocks(
+    classes: pd.Series, corrector_classes: List[str], process_classes: List[str]
+):
     """
     groups samples into blocks of consecutive samples of the same type
     aux function in BatchCorrector pipeline.
 
     each class is assigned to each one of three possible sample blocks:
     0 if the sample is mapped as QC, 1 if the sample is mapped as a
     sample, and 2 otherwise.
 
     Each block is assigned an unique number.
     """
     class_to_block_type = dict()
-    for c in classes.unique():
-        if c in corrector_classes:
-            class_to_block_type[c] = 0
-        elif c in process_classes:
-            class_to_block_type[c] = 1
+    for cl in classes.unique():
+        if cl in corrector_classes:
+            class_to_block_type[cl] = 0
+        elif cl in process_classes:
+            class_to_block_type[cl] = 1
         else:
-            class_to_block_type[c] = 2
+            class_to_block_type[cl] = 2
     block_type = classes.map(class_to_block_type)
     block_number = (block_type.diff().fillna(0) != 0).cumsum()
     return block_type, block_number
```

### Comparing `tidyms-0.6.3/src/tidyms/_mzml.py` & `tidyms-0.7.0/src/tidyms/_mzml.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
 NEGATIVE_POLARITY = "MS:1000129"
 POSITIVE_POLARITY = "MS:1000130"
 # time units
 SECONDS = "UO:0000010"
 MINUTES = "UO:0000031"
 
 # data types
-FLOAT16 = "MS:1000521"
-FLOAT32 = "MS:1000518"
+FLOAT16 = "UNKNOWN" ## TODO check "MS:1000521"
+FLOAT32 = "MS:1000521"
 FLOAT64 = "MS:1000523"
 INT32 = "MS:1000519"
 INT64 = "MS:1000522"
 DATA_TYPES = {
     FLOAT16: np.float16,
     FLOAT32: np.float32,
     FLOAT64: np.float64,
@@ -177,15 +177,19 @@
         filename,
         spectra_offset,
         chromatogram_offset,
         index_offset,
         n,
         "spectrum"
     )
-    elements = list(fromstring(xml_str))
+    try:
+        elements = list(fromstring(xml_str))
+    except:
+        print("error", xml_str) 
+        raise "laskjf"
     spectrum = dict()
     for el in elements:
         tag = el.tag
         if tag == "cvParam":
             accession = el.attrib.get("accession")
             if accession == MS_LEVEL:
                 spectrum["ms_level"] = int(el.attrib.get("value"))
@@ -328,17 +332,18 @@
     data = None
     kind = None
     units = None
     dtype = None
     for e in element:
         tag = e.tag
         if tag == "binary":
-            data = e.text
-        else:
+            data = e.text if e.text is None else e.text.strip()
+        elif tag == "cvParam":
             accession = e.attrib.get("accession")
+            value = e.attrib.get("name")
             if accession in UNSUPPORTED_COMPRESSION:
                 msg = "Currently only zlib compression is supported."
                 raise NotImplementedError(msg)
             elif accession == ZLIB:
                 has_zlib_compression = True
             elif accession == INT_ARRAY:
                 kind = "spint"
```

### Comparing `tidyms-0.6.3/src/tidyms/_plot_bokeh.py` & `tidyms-0.7.0/src/tidyms/_plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/assay.py` & `tidyms-0.7.0/src/tidyms/assay.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import pickle
 import numpy as np
 import pandas as pd
 from functools import wraps
 from inspect import getfullargspec
 from joblib import Parallel, delayed
 from pathlib import Path
-from typing import Callable, List, Optional, Union
+import os
+from uuid import uuid4
+from typing import Callable, List, Optional, Tuple, Union
 from . import _constants as c
 from . import validation as val
 from . import raw_data_utils
 from .container import DataContainer
 from .correspondence import match_features
 from .fileio import MSData, read_pickle
-from .lcms import Roi, LCRoi
+from .lcms import Feature, Roi, LCTrace
 from .utils import get_progress_bar
 from ._plot_bokeh import _LCAssayPlotter
 from .fill_missing import fill_missing_lc
 from ._build_data_matrix import build_data_matrix
 import json
-from .annotation import create_annotator, annotate
+from .annotation import annotate, create_annotation_table, create_annotation_tools
 import copy
+import tempfile
 
 # TODO: add id_ column to sample metadata
 # TODO: add make_roi params to each column in sample metadata for cases where
 #   more than one sample are obtained from the same file.
 # TODO: test verbose false describe_features, extract_features
 
 
@@ -37,24 +40,25 @@
 
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         # Get function parameters
         func_arg_spec = getfullargspec(func)
-        func_arg_names = func_arg_spec.args[1:]    # exclude self
+        func_arg_names = func_arg_spec.args[1:]  # exclude self
         params = dict(zip(func_arg_names, args[1:]))
         params.update(kwargs)
-        assay = args[0]     # type: Assay
+        assay = args[0]  # type: Assay
 
         step = func.__name__
         assay.manager.manage_step_before(step, params)
         results = func(assay, **params)
         assay.manager.manage_step_after(step, params)
         return results
+
     return wrapper
 
 
 class Assay:
     """
     Manages data preprocessing workflows from raw data to data matrix.
 
@@ -103,39 +107,69 @@
         The separation method used. Used to set several defaults during data
         preprocessing.
 
     """
 
     def __init__(
         self,
-        assay_path: Union[str, Path],
-        data_path: Optional[Union[str, List[str], Path]],
+        assay_path: Union[str, Path] = None,
+        data_path: Optional[Union[str, List[str], Path]] = None,
         sample_metadata: Optional[Union[pd.DataFrame, str, Path]] = None,
         ms_mode: str = "centroid",
         instrument: str = "qtof",
         separation: str = "uplc",
+        data_import_mode: str = None,
+        n_jobs: int = 1,
+        cache_MSData_objects: bool = False,
     ):
+        if data_import_mode is None:
+            data_import_mode = c.DEFAULT_DATA_LOAD_MODE
+
         if isinstance(assay_path, str):
             assay_path = Path(assay_path)
+        if assay_path is None:
+            assay_path = tempfile.mkdtemp()
 
-        self.manager = _create_assay_manager(
-            assay_path,
-            data_path,
-            sample_metadata,
-            ms_mode,
-            instrument,
-            separation
-        )
+        self._manager = _create_assay_manager(assay_path, data_path, sample_metadata, ms_mode, instrument, separation, data_import_mode)
+        self.ms_mode = ms_mode
         self.separation = separation
         self.instrument = instrument
+        self.data_import_mode = c.DEFAULT_DATA_LOAD_MODE
+        if data_import_mode is not None:
+            self.data_import_mode = data_import_mode
         self.plot = _create_assay_plotter(self)
-        self.feature_table = None   # type: Optional[pd.DataFrame]
+        self.feature_table = None  # type: Optional[pd.DataFrame]
         self.data_matrix = None  # type: Optional[DataContainer]
         self.feature_metrics = dict()
 
+        self.n_jobs = n_jobs
+        self._cache_MSData_objects = cache_MSData_objects
+        self._MSData_objects_cache = {}
+        self._virtual_samples = set()
+
+    @property
+    def manager(self):
+        return self._manager
+
+    @manager.setter
+    def manager(self, value: None):
+        raise RuntimeError("Setting the manager is not allowed")
+
+    @property
+    def ms_mode(self) -> str:
+        return self._msMode
+
+    @ms_mode.setter
+    def ms_mode(self, value: str):
+        if value in c.MS_MODES:
+            self._ms_mode = value
+        else:
+            msg = "{} is not a valid ms mode. Valid values are: {}"
+            raise ValueError(msg.format(value, c.MS_MODES))
+
     @property
     def separation(self) -> str:
         return self._separation
 
     @separation.setter
     def separation(self, value: str):
         if value in c.LC_MODES:
@@ -152,51 +186,72 @@
     def instrument(self, value: str):
         if value in c.MS_INSTRUMENTS:
             self._instrument = value
         else:
             msg = "{} is not a valid instrument. Valid values are: {}."
             raise ValueError(msg.format(value, c.MS_INSTRUMENTS))
 
+    @property
+    def n_jobs(self) -> str:
+        return self._n_jobs
+
+    @n_jobs.setter
+    def n_jobs(self, value: str):
+        if value >= 1 or value == -1:
+            self._n_jobs = value
+        else:
+            msg = "n_jobs must be set to a positive, non-zero integer value to use a specific number of parallel workers. -1 indicates all processors. Provided value is {}."
+            raise ValueError(msg.format(value))
+
+    def add_samples(self, data_path: Optional[Union[str, List[str], Path]], sample_metadata: Optional[Union[str, pd.DataFrame]]):
+        self._manager.add_samples(
+            data_path=data_path,
+            sample_metadata=sample_metadata,
+        )
+
+    def add_virtual_sample(self, MSData_object: MSData, virtual_name: str, sample_metadata: Optional[Union[str, pd.DataFrame]]):
+        self._manager.add_virtual_sample(
+            MSData_object=MSData_object,
+            virtual_name=virtual_name,
+            sample_metadata=sample_metadata,
+        )
+        self._MSData_objects_cache[virtual_name] = MSData_object
+        self._virtual_samples.add(virtual_name)
+
     @staticmethod
-    def _get_feature_detection_strategy(
-        strategy: Union[str, Callable] = "default"
-    ) -> Callable:
+    def _get_feature_detection_strategy(strategy: Union[str, Callable] = "default") -> Callable:
         """
         Returns the function used for feature detection.
         """
         if callable(strategy):
             func = strategy
         elif strategy == "default":
             func = raw_data_utils.make_roi
         else:
             msg = "{} is not a valid strategy.".format(strategy)
             raise ValueError(msg)
         return func
 
     @staticmethod
-    def _get_feature_extraction_strategy(
-        strategy: Union[str, Callable] = "default"
-    ) -> Callable:
+    def _get_feature_extraction_strategy(strategy: Union[str, Callable] = "default") -> Callable:
         """
         Returns the function used for feature extraction.
 
         """
         if callable(strategy):
             func = strategy
         elif strategy == "default":
             func = _extract_features_default
         else:
             msg = "{} is not a valid strategy.".format(strategy)
             raise ValueError(msg)
         return func
 
     @staticmethod
-    def _get_feature_matching_strategy(
-            strategy: Union[str, Callable] = "default"
-    ) -> Callable:
+    def _get_feature_matching_strategy(strategy: Union[str, Callable] = "default") -> Callable:
         """
         Sets the function used for mathing_features.
 
         """
         if callable(strategy):
             func = strategy
         elif strategy == "default":
@@ -221,15 +276,49 @@
 
         Raises
         ------
         ValueError : if the sample is not found.
 
         """
         sample_path = self.manager.get_sample_path(sample)
-        return MSData(sample_path, **self.manager.params["MSData"])
+        ms_data = None
+
+        if sample in self._MSData_objects_cache:
+            ms_data = self._MSData_objects_cache[sample]
+
+        else:
+            temp = copy.deepcopy(self.manager.params["MSData"])
+            if "data_import_mode" in temp:
+                temp.pop("data_import_mode")
+            if self.data_import_mode.lower() == c.MEMORY:
+                ms_data = MSData.create_MSData_instance(data_import_mode=c.MEMORY, path=sample_path, **temp)
+            elif self.data_import_mode.lower() == c.INFILE:
+                path = Path(sample_path)
+                suffix = path.suffix
+                if suffix == "":
+                    ms_data = MSData.create_MSData_instance(data_import_mode=c.SIMULATED, path=sample_path, **temp)
+                else:
+                    ms_data = MSData.create_MSData_instance(data_import_mode=c.INFILE, path=sample_path, **temp)
+            elif self.data_import_mode.lower() == c.SIMULATED:
+                ms_data = MSData.create_MSData_instance(data_import_mode=c.SIMULATED, path=sample_path, **temp)
+
+            if ms_data is None:
+                raise RuntimeError("Error: file '%s' not found" % (sample_path))
+
+            if self._cache_MSData_objects:
+                self._MSData_objects_cache[sample_path] = ms_data
+
+        return ms_data
+
+    def set_ms_data(self, sample: str, msdata: MSData):
+        sample_path = self.manager.get_sample_path(sample)
+        self._MSData_objects_cache[sample_path] = msdata
+
+    def clear_MSData_objects_cache(self):
+        self._MSData_objects_cache = {}
 
     def get_sample_metadata(self) -> pd.DataFrame:
         """
         Creates a DataFrame with the metadata of each sample used in the assay.
 
         Returns
         -------
@@ -265,28 +354,28 @@
         detect_features : Detect ROI in the Assay samples.
         load_roi_list : Loads all ROI from a sample.
 
         """
         roi_path = self.manager.get_roi_path(sample)
 
         if self.separation in c.LC_MODES:
-            roi_class = LCRoi
+            roi_class = LCTrace
         else:
             roi_class = Roi
 
         with open(roi_path, "r", newline="\n") as fin:
             header = fin.readline()
             index_offset = int(header.split("=")[-1])
             fin.seek(index_offset)
             json_str = fin.read()
             index = json.loads(json_str)
             offset, length = index[roi_index]
             fin.seek(offset)
             s = fin.read(length)
-            roi = roi_class.from_json(s)
+            roi = roi_class.from_string(s)
         return roi
 
     def load_roi_list(self, sample: str) -> List[Roi]:
         """
         Loads all the ROIs detected in a sample.
 
         Must be called after performing feature detection.
@@ -313,29 +402,29 @@
         if not self.manager.check_step("detect_features"):
             msg = "`load_roi_list` must be called after `detect_features`."
             raise ValueError(msg)
 
         roi_path = self.manager.get_roi_path(sample)
 
         if self.separation in c.LC_MODES:
-            roi_class = LCRoi
+            roi_class = LCTrace
         else:
             roi_class = Roi
 
         with open(roi_path, "r", newline="\n") as fin:
             header = fin.readline()
             index_offset = int(header.split("=")[-1])
             fin.seek(index_offset)
             index = json.loads(fin.read())
 
             roi_list = list()
             for offset, length in index:
                 fin.seek(offset)
                 s = fin.read(length)
-                roi = roi_class.from_json(s)
+                roi = roi_class.from_string(s)
                 roi_list.append(roi)
         return roi_list
 
     def load_features(self, sample: str) -> pd.DataFrame:
         """
         Loads a table with feature descriptors for a sample.
 
@@ -368,15 +457,15 @@
 
     @_manage_preprocessing_step
     def detect_features(
         self,
         strategy: Union[str, Callable] = "default",
         n_jobs: Optional[int] = None,
         verbose: bool = True,
-        **kwargs
+        **kwargs,
     ) -> "Assay":
         """
         Builds Regions Of Interest (ROI) from raw data for each sample.
 
         ROIs are computed and saved to disk. Computed ROIs can be recovered
         using ``self.load_roi`` or ``self.load_roi_list``.
 
@@ -410,20 +499,23 @@
         lcms.LCRoi : ROI used in LC data
 
         """
         detect_features_func = self._get_feature_detection_strategy(strategy)
         process_samples = self.manager.sample_queue
         n_samples = len(process_samples)
 
+        if n_jobs is None:
+            n_jobs = self.n_jobs
+
         if n_samples:
 
             def iter_func(sample_list):
-                for x in sample_list:
-                    roi_path = self.manager.get_roi_path(x)
-                    ms_data = self.get_ms_data(x)
+                for sample in sample_list:
+                    roi_path = self.manager.get_roi_path(sample)
+                    ms_data = self.get_ms_data(sample)
                     yield roi_path, ms_data
 
             def worker(args):
                 roi_path, ms_data = args
                 roi_list = detect_features_func(ms_data, **kwargs)
                 _save_roi_list(roi_path, roi_list)
 
@@ -443,15 +535,15 @@
 
     @_manage_preprocessing_step
     def extract_features(
         self,
         strategy: Union[str, Callable] = "default",
         n_jobs: Optional[int] = None,
         verbose: bool = True,
-        **kwargs
+        **kwargs,
     ) -> "Assay":
         """
         Extract features from the ROIs detected on each sample.
 
         Features are stored in ``features`` attribute of each ROI. ROIs can be
         recovered using ``self.load_roi`` or ``self.load_roi_list``.
 
@@ -489,14 +581,18 @@
         lcms.Feature : abstract feature
         lcms.Peak : feature used in LC data
 
         """
         extract_features_func = self._get_feature_extraction_strategy(strategy)
         process_samples = self.manager.sample_queue
         n_samples = len(process_samples)
+
+        if n_jobs is None:
+            n_jobs = self.n_jobs
+
         if n_samples:
 
             def iterator():
                 for sample in self.manager.get_sample_names():
                     roi_path = self.manager.get_roi_path(sample)
                     roi_list = self.load_roi_list(sample)
                     yield roi_path, roi_list
@@ -518,55 +614,81 @@
             if verbose:
                 print("All samples are processed already.")
         return self
 
     @_manage_preprocessing_step
     def describe_features(
         self,
+        custom_descriptors: Optional[dict[str, Callable[[Feature], float]]] = None,
+        filters: Optional[dict[str, Tuple]] = None,
         n_jobs: Optional[int] = 1,
         verbose: bool = True,
-        **kwargs
     ) -> "Assay":
         """
         Compute feature descriptors for the features extracted from the data.
 
         Features descriptors from each sample are organized in a Pandas
         DataFrame and stored to disk and can be recovered using
         ``self.load_features``. Besides the descriptors, these DataFrames
         contain two additional columns: `roi_index` and `ft_index`. `roi_index`
         is used to indentify the ROI where the feature was detected, and
         recovered using the ``load_roi`` method. The `ft_index` value is used
         to identify the feature in the `feature` attribute of the ROI.
 
         Parameters
         ----------
+        custom_descriptors : dict or None, default=None
+            A dictionary of strings to callables, used to estimate custom
+            descriptors of a feature. The function must have the following
+            signature:
+
+            .. code-block:: python
+
+                "estimator_func(feature: Feature) -> float"
+
+        filters : dict or None, default=None
+            A dictionary of descriptor names to a tuple of minimum and maximum
+            acceptable values. To use only minimum/maximum values, use None
+            (e.g. (None, max_value) in the case of using only maximum). Features
+            with descriptors outside those ranges are removed. Filters for
+            custom descriptors can also be used.
         n_jobs: int or None, default=None
             Number of jobs to run in parallel. ``None`` means 1 unless in a
             :obj:`joblib.parallel_backend` context. ``-1`` means using all
             processors.
         verbose : bool, default=True
             If ``True``, displays a progress bar.
         **kwargs : dict
             Parameters to pass to :py:meth:`tidyms.lcms.Roi.describe_features`.
 
         """
         process_samples = self.manager.sample_queue
         n_samples = len(process_samples)
+
+        if n_jobs is None:
+            n_jobs = self.n_jobs
+
+        if custom_descriptors is None:
+            custom_descriptors = dict()
+        if filters is None:
+            filters = _get_default_filters(self.separation)
+        _fill_filter_boundaries(filters)
+
         if n_samples:
 
             def iterator():
                 for sample in self.manager.get_sample_names():
                     roi_path = self.manager.get_roi_path(sample)
                     ft_path = self.manager.get_feature_path(sample)
                     roi_list = self.load_roi_list(sample)
                     yield roi_path, ft_path, roi_list
 
             def worker(args):
                 roi_path, ft_path, roi_list = args
-                ft_table = _describe_features_default(roi_list, **kwargs)
+                ft_table = _describe_features_default(roi_list, custom_descriptors, filters)
                 _save_roi_list(roi_path, roi_list)
                 ft_table.to_pickle(ft_path)
 
             worker = delayed(worker)
             if verbose:
                 msg = "Computing feature descriptors in {} samples."
                 print(msg.format(n_samples))
@@ -574,15 +696,15 @@
                 iterator = bar(iterator(), total=n_samples)
             else:
                 iterator = iterator()
             Parallel(n_jobs=n_jobs)(worker(x) for x in iterator)
         else:
             if verbose:
                 print("All samples are processed already.")
-            return self
+        return self
 
     @_manage_preprocessing_step
     def build_feature_table(self):
         """
         Merges the feature descriptors from all samples into one DataFrame.
 
         The feature table is stored in ``self.feature_table``. Two additional
@@ -617,19 +739,15 @@
             feature_table[c.SAMPLE] = feature_table[c.SAMPLE]
             feature_table[c.CLASS] = feature_table[c.CLASS]
             feature_table.to_pickle(str(save_path))
         self.feature_table = feature_table
         return self
 
     @_manage_preprocessing_step
-    def match_features(
-        self,
-        strategy: Union[str, Callable] = "default",
-        **kwargs
-    ):
+    def match_features(self, strategy: Union[str, Callable] = "default", **kwargs):
         r"""
         Match features across samples. Each feature is labelled using an integer
         value to assign a common id. Features that do not belong to any group
         are labelled with ``-1``. The label is stored in the `label_` column
         of the feature table.
 
         Parameters
@@ -717,27 +835,25 @@
                 self.feature_table,
                 sample_metadata,
                 self.separation,
                 merge_close_features,
                 mz_merge,
                 rt_merge,
                 merge_threshold,
-                annotate_isotopologues
+                annotate_isotopologues,
             )
             dc = DataContainer(data_matrix, feature_metadata, sample_metadata)
             dc.save(dc_path)
             self.data_matrix = dc
         else:
             self.data_matrix = read_pickle(dc_path)
         return self.data_matrix
 
     @_manage_preprocessing_step
-    def annotate_isotopologues(
-        self, n_jobs: Optional[int] = 1, verbose: bool = True, **kwargs
-    ):
+    def annotate_isotopologues(self, n_jobs: Optional[int] = 1, verbose: bool = True, **kwargs):
         """
         Labels isotopic envelopes in each sample.
 
         Labels are stored in the `isotopologue_label` column of the feature
         table. Each envelope share the same label. Features labelled
         with ``-1`` do not belong to any group. The `isotopologue_index` column
         indexes the nominal mass of the isotopologue, relative to the minimum
@@ -776,20 +892,26 @@
             #         ft_table.to_pickle(ft_path)
             #         print(sample)
             def iterator():
                 for sample in self.manager.get_sample_names():
                     ft_path = self.manager.get_feature_path(sample)
                     roi_list = self.load_roi_list(sample)
                     ft_table = self.load_features(sample)
-                    yield ft_table, ft_path, roi_list
-
-            def worker(args):
-                ft_table, ft_path, roi_list = args
-                ann = create_annotator(**kwargs)
-                annotate(ft_table, roi_list, ann)
+                    ft_list = list()
+                    for roi in roi_list:
+                        if roi.features is not None:
+                            ft_list.extend(roi.features)
+                    yield ft_list, ft_table, ft_path
+
+            def worker(args: tuple[list[Feature], pd.DataFrame, Path]):
+                ft_list, ft_table, ft_path = args
+                tools = create_annotation_tools(**kwargs)
+                annotate(ft_list, *tools)
+                annotation_table = create_annotation_table(ft_list)
+                ft_table = pd.merge(ft_table, annotation_table, on=[c.ROI_INDEX, c.FT_INDEX])
                 ft_table.to_pickle(ft_path)
 
             worker = delayed(worker)
             if verbose:
                 msg = "Annotating Isotopologues in {} samples."
                 print(msg.format(n_samples))
                 bar = get_progress_bar()
@@ -808,15 +930,15 @@
     @_manage_preprocessing_step
     def fill_missing(
         self,
         mz_tolerance: float,
         n_deviations: float = 1.0,
         estimate_not_found: bool = True,
         n_jobs: Optional[int] = None,
-        verbose: bool = False
+        verbose: bool = False,
     ):
         """
         Fill missing values in the Data matrix by searching missing features in
         raw data, using values average values from the detected features.
 
         Parameters
         ----------
@@ -858,14 +980,18 @@
         ``False``. Otherwise, a fill value is computed as the area in the region
         where the chromatographic peak was expected to appear, defined by the
         `rt_start` and `rt_end` values in the feature table.
 
         """
         process_samples = self.manager.sample_queue
         n_samples = len(process_samples)
+
+        if n_jobs is None:
+            n_jobs = self.n_jobs
+
         if n_samples:
             samples = self.manager.get_sample_names()
             generator = ((x, self.get_ms_data(x)) for x in samples)
             has_missing = self.data_matrix.data_matrix.isna().any().any()
             if not has_missing:
                 mask = self.data_matrix.missing != 0
                 self.data_matrix._data_matrix[mask] = np.nan
@@ -874,23 +1000,24 @@
                 generator,
                 self.data_matrix.data_matrix,
                 self.data_matrix.feature_metadata,
                 mz_tolerance,
                 n_deviations,
                 estimate_not_found,
                 n_jobs,
-                verbose
+                verbose,
             )
             self.data_matrix._data_matrix = data_matrix
             # TODO: update DataContainer Status
             self.data_matrix.missing = missing
         else:
             if verbose:
                 msg = "Data matrix doesn't contain missing data."
                 print(msg)
+        return self
 
 
 class _AssayManager:
     """
     Manages sample metadata information, location of data files and checking
     the processing order of an Assay.
 
@@ -922,69 +1049,93 @@
 
     """
 
     def __init__(
         self,
         assay_path: Path,
         data_path: Union[str, List[str], Path],
-        sample_metadata: Optional[Union[str, Path, pd.DataFrame]],
-        ms_mode: str,
-        instrument: str,
-        separation: str,
+        sample_metadata: Optional[Union[str, Path, pd.DataFrame]] = None,
+        ms_mode: str = "centroid",
+        instrument: str = "qtof",
+        separation: str = "uplc",
+        data_import_mode: Optional[str] = None,
     ):
         self.assay_path = assay_path
-        self._sample_to_path = None
+        self._sample_to_path = {}
         self.sample_metadata = None
         self.sample_queue = None
-        self.add_samples(data_path, sample_metadata)
-        self.params = _build_params_dict(ms_mode, separation, instrument)
+        if data_path is not None:
+            self.add_samples(data_path, sample_metadata)
+        self.data_import_mode = c.DEFAULT_DATA_LOAD_MODE
+        if data_import_mode is not None:
+            self.data_import_mode = data_import_mode
+        self.params = _build_params_dict(ms_mode, separation, instrument, self.data_import_mode)
+
+        self._virtual_MSData_objects = {}
 
     def add_samples(
         self,
         data_path: Optional[Union[str, List[str], Path]],
-        sample_metadata: Optional[Union[str, pd.DataFrame]]
+        sample_metadata: Optional[Union[str, pd.DataFrame]],
     ):
         # set data path and related attributes
         if self._sample_to_path is None:
             self._add_samples_empty_assay(data_path, sample_metadata)
         else:
             self._add_samples_existing_assay(data_path, sample_metadata)
 
     def _add_samples_empty_assay(
         self,
         data_path: Optional[Union[str, List[str], Path]],
-        sample_metadata: Optional[Union[str, pd.DataFrame]]
+        sample_metadata: Optional[Union[str, pd.DataFrame]],
     ):
         path_list = sorted(_get_path_list(data_path))
         sample_to_path = {x.stem: x for x in path_list}
         self._sample_to_path = sample_to_path
 
         sample_names = self.get_sample_names()
         sm = _create_sample_metadata(sample_metadata, sample_names)
         sm = _normalize_sample_metadata(sm, sample_names)
         self.sample_metadata = sm
 
     def _add_samples_existing_assay(
         self,
         data_path: Optional[Union[str, List[str], Path]],
-        sample_metadata: Optional[Union[str, pd.DataFrame]]
+        sample_metadata: Optional[Union[str, pd.DataFrame]],
     ):
         new_path_list = sorted(_get_path_list(data_path))
         new_sample_to_path = dict()
         for path in new_path_list:
             stem = path.stem
             if stem not in self._sample_to_path:
                 new_sample_to_path[stem] = path
         self._sample_to_path.update(new_sample_to_path)
 
         new_sample_names = list(new_sample_to_path)
         sm = _create_sample_metadata(sample_metadata, new_sample_names)
         sm = _normalize_sample_metadata(sm, new_sample_names)
-        self.sample_metadata = pd.concat((self.sample_metadata, sm))
-        self.clear_data(c.BUILD_FEATURE_TABLE, new_sample_names)
+        if self.sample_metadata is None:
+            self.sample_metadata = sm
+        else:
+            self.sample_metadata = pd.concat((self.sample_metadata, sm))
+            self.clear_data(c.BUILD_FEATURE_TABLE, new_sample_names)
+
+    def add_virtual_sample(self, MSData_object: MSData, virtual_name: str, sample_metadata: Optional[Union[str, pd.DataFrame]]):
+        if virtual_name not in self._sample_to_path:
+            virtual_sample_path = os.path.join(self.assay_path, "%s.mzML" % ((str(uuid4()) + str(uuid4())).replace("-", "")))
+            self._sample_to_path[virtual_name] = Path(virtual_sample_path)
+            self._virtual_MSData_objects[virtual_name] = MSData_object
+            new_sample_name = [virtual_name]
+            sm = _create_sample_metadata(sample_metadata, new_sample_name)
+            sm = _normalize_sample_metadata(sm, new_sample_name)
+            if self.sample_metadata is None:
+                self.sample_metadata = sm
+            else:
+                self.sample_metadata = pd.concat((self.sample_metadata, sm))
+                self.clear_data(c.BUILD_FEATURE_TABLE, new_sample_name)
 
     def create_assay_dir(self):
         """
         Creates a directory to store the data from a new Assay.
         """
         self.assay_path.mkdir()
         # roi dir
@@ -1009,15 +1160,15 @@
         ------
         PreprocessingOrderError : If the previous steps were not executed.
 
         """
         try:
             ind = c.PREPROCESSING_STEPS.index(step)
             previous = c.PREPROCESSING_STEPS[ind - 1]
-        except ValueError:      # manage optional steps
+        except ValueError:  # manage optional steps
             if step == c.ANNOTATE_ISOTOPOLOGUES:
                 previous = c.PREPROCESSING_STEPS[2]
             elif step == c.ANNOTATE_ADDUCTS:
                 previous = c.ANNOTATE_ISOTOPOLOGUES
             else:
                 msg = "`{}` is not a valid preprocessing step".format(step)
                 raise ValueError(msg)
@@ -1048,28 +1199,29 @@
         """
         Deletes old processed data.
 
         """
         if step == c.DETECT_FEATURES:
             for sample in samples:
                 path = self.get_roi_path(sample)
-                path.unlink(missing_ok=True)
+                if sample not in self._virtual_MSData_objects:
+                    path.unlink(missing_ok=True)
         elif step == c.DESCRIBE_FEATURES:
             for sample in samples:
                 path = self.get_feature_path(sample)
-                path.unlink(missing_ok=True)
+                if sample not in self._virtual_MSData_objects:
+                    path.unlink(missing_ok=True)
         elif step == c.BUILD_FEATURE_TABLE:
             if samples:
                 file_name = c.FT_TABLE_FILENAME
                 table_path = self.assay_path.joinpath(file_name)
                 table_path.unlink(missing_ok=True)
         self.params["preprocess_steps"][step] = False
         processed_samples = self.params["processed_samples"][step]
-        self.params["processed_samples"][step] = \
-            processed_samples.difference(samples)
+        self.params["processed_samples"][step] = processed_samples.difference(samples)
 
     def flag_completed(self, step: str):
         """
         Flags a processing step as completed.
         """
         self.params["preprocess_steps"][step] = True
 
@@ -1082,29 +1234,32 @@
 
     def get_sample_path(self, name: str) -> Path:
         self._check_sample_name(name)
         return self._sample_to_path.get(name)
 
     def get_roi_path(self, name: str) -> Path:
         self._check_sample_name(name)
-        roi_path = self.assay_path.joinpath(c.ROI_DIR, name)
+        sampleNameFromPath = self.get_sample_path(name)
+        sampleNameFromPath = os.path.splitext(os.path.basename(sampleNameFromPath))[0]
+        roi_path = self.assay_path.joinpath(c.ROI_DIR, sampleNameFromPath)
         return roi_path
 
     def get_feature_path(self, name: str) -> Path:
         self._check_sample_name(name)
-        file_name = "{}.pickle".format(name)
+        sampleNameFromPath = self.get_sample_path(name)
+        sampleNameFromPath = os.path.splitext(os.path.basename(sampleNameFromPath))[0]
+        file_name = "{}.pickle".format(sampleNameFromPath)
         feature_path = self.assay_path.joinpath(c.FT_DIR, file_name)
         return feature_path
 
     def get_sample_metadata(self) -> pd.DataFrame:
         # TODO: remove this method after refactoring DataContainer
         sm = self.sample_metadata.copy()
         sm.index.name = "sample"
-        sm = sm.rename(columns={c.CLASS: "class", "id_": "id",
-                                c.ORDER: "order", c.BATCH: "batch"})
+        sm = sm.rename(columns={c.CLASS: "class", "id_": "id", c.ORDER: "order", c.BATCH: "batch"})
         return sm
 
     def send_samples_to_queue(self, step: str, kwargs: dict):
         """
         Get the list of samples to process. Checks if the samples has been
         processed already using the parameters specified by kwargs.
 
@@ -1158,28 +1313,33 @@
 
 class PreprocessingOrderError(ValueError):
     """
     Exception raised when the preprocessing methods are called in the wrong
     order.
 
     """
+
     pass
 
 
 def _extract_features_default(roi: Roi, **kwargs):
     return roi.extract_features(**kwargs)
 
 
-def _describe_features_default(roi_list: List[Roi], **kwargs) -> pd.DataFrame:
+def _describe_features_default(
+    roi_list: List[Roi],
+    custom_descriptors: dict[str, Callable[[Feature], float]],
+    filters: dict[str, Tuple],
+) -> pd.DataFrame:
     roi_index_list = list()
     ft_index = list()
     descriptors_list = list()
 
     for roi_index, roi in enumerate(roi_list):
-        descriptors = roi.describe_features(**kwargs)
+        descriptors = _process_features_roi(roi, custom_descriptors, filters)
         n_features = len(descriptors)
         descriptors_list.extend(descriptors)
         roi_index_list.append([roi_index] * n_features)
         ft_index.append(range(n_features))
 
     if roi_index_list:
         roi_index_list = np.hstack(roi_index_list)
@@ -1192,57 +1352,198 @@
         ft_table[c.ROI_INDEX] = ft_table[c.ROI_INDEX].astype(int)
         ft_table[c.FT_INDEX] = ft_table[c.FT_INDEX].astype(int)
     else:
         ft_table = pd.DataFrame()
     return ft_table
 
 
+def _process_features_roi(
+    roi: Roi,
+    custom_descriptors: dict[str, Callable[[Feature], float]],
+    filters: dict[str, Tuple],
+) -> list[dict[str, float]]:
+    filtered_features = list()
+    descriptors = list()
+    if roi.features is not None:
+        # TODO: temporary workaround to update feature index. This should be
+        #   replaced in the new implementation of Assay.
+        new_index = 0
+        for ft in roi.features:
+            d = _process_feature(ft, custom_descriptors, filters)
+            if d is not None:
+                ft.index = new_index
+                new_index += 1
+                filtered_features.append(ft)
+                descriptors.append(d)
+        roi.features = filtered_features
+    return descriptors
+
+
+def _process_feature(
+    feature: Feature,
+    custom_descriptors: dict[str, Callable[[Feature], float]],
+    filters: dict[str, Tuple],
+) -> Optional[dict[str, float]]:
+    descriptors = feature.describe()
+    is_valid_feature = _all_valid_descriptors(descriptors, filters)
+
+    if is_valid_feature:
+        custom = {k: v(feature) for k, v in custom_descriptors.items()}
+        is_valid_feature = _all_valid_descriptors(custom, filters)
+        if is_valid_feature:
+            descriptors.update(custom)
+
+    if not is_valid_feature:
+        descriptors = None
+
+    return descriptors
+
+
+def _all_valid_descriptors(descriptors: dict[str, float], filters: dict[str, Tuple[float, float]]) -> bool:
+    """
+    Check that the descriptors of a peak are in a valid range.
+
+    aux function of get_peak_descriptors.
+
+    Parameters
+    ----------
+    peak_descriptors : dict
+        mapping of descriptor names to descriptor values.
+    filters : dict
+        Dictionary from descriptors names to minimum and maximum acceptable
+        values.
+
+    Returns
+    -------
+    is_valid : bool
+        True if all descriptors are inside the valid ranges.
+
+    """
+    is_valid = True
+    for k, (lb, ub) in filters.items():
+        if k in descriptors:
+            d_value = descriptors[k]
+            is_valid = (lb <= d_value) and (ub >= d_value)
+            if not is_valid:
+                break
+    return is_valid
+
+
+def _describe_feature_list(
+    self,
+    custom_descriptors: Optional[dict] = None,
+    filters: Optional[dict[str, Tuple]] = None,
+) -> List[dict[str, float]]:
+    """
+    Computes descriptors for the features detected in the ROI.
+
+    Parameters
+    ----------
+    custom_descriptors : dict or None, default=None
+        A dictionary of strings to callables, used to estimate custom
+        descriptors of a feature. The function must have the following
+        signature:
+
+        .. code-block:: python
+
+            "estimator_func(feature: Feature) -> float"
+
+    filters : dict or None, default=None
+        A dictionary of descriptor names to a tuple of minimum and maximum
+        acceptable values. To use only minimum/maximum values, use None
+        (e.g. (None, max_value) in the case of using only maximum). Features
+        with descriptors outside those ranges are removed. Filters for
+        custom descriptors can also be used.
+
+    Returns
+    -------
+    features : List[Feature]
+        filtered list of features.
+    descriptors: List[Dict[str, float]]
+        Descriptors for each feature.
+
+    """
+
+    if custom_descriptors is None:
+        custom_descriptors = dict()
+
+    if filters is None:
+        filters = self.get_default_filters()
+    _fill_filter_boundaries(filters)
+
+    valid_features = list()
+    descriptor_list = list()  # Type: List[Dict[str, float]]
+    for f in self.features:
+        f_descriptors = f.get_descriptors(self)
+        for descriptor, func in custom_descriptors.items():
+            f_descriptors[descriptor] = func(self, f)
+
+        if _has_all_valid_descriptors(f_descriptors, filters):
+            valid_features.append(f)
+            descriptor_list.append(f_descriptors)
+    self.features = valid_features
+    return descriptor_list
+
+
+def _fill_filter_boundaries(filter_dict: dict[str, Tuple[Optional[float], Optional[float]]]):
+    """
+    Replaces None in the filter boundaries to perform comparisons.
+
+    aux function of get_peak_descriptors
+    """
+    for k in filter_dict:
+        lb, ub = filter_dict[k]
+        if lb is None:
+            lb = -np.inf
+        if ub is None:
+            ub = np.inf
+        filter_dict[k] = (lb, ub)
+
+
+def _get_default_filters(mode: str) -> dict:
+    """
+    Default filters for peaks detected in LC data.
+    """
+    if mode == c.HPLC:
+        filters = {"width": (10, 90), "snr": (5, None)}
+    else:  # mode = "uplc"
+        filters = {"width": (4, 60), "snr": (5, None)}
+    return filters
+
+
 def _match_features_default(assay: Assay, **kwargs):
     # set defaults and validate input
     params = val.match_features_defaults(assay.separation, assay.instrument)
     params.update(kwargs)
     validator = val.ValidatorWithLowerThan(val.match_features_schema())
     params = val.validate(params, validator)
 
-    class_to_n_samples = (
-        assay.manager.sample_metadata[c.CLASS]
-        .value_counts()
-        .to_dict()
-    )
-    results = match_features(
-        assay.feature_table,
-        class_to_n_samples,
-        **params
-    )
+    class_to_n_samples = assay.manager.sample_metadata[c.CLASS].value_counts().to_dict()
+    results = match_features(assay.feature_table, class_to_n_samples, **params)
     return results
 
 
-def _create_assay_manager(
-    assay_path,
-    data_path,
-    sample_metadata,
-    ms_mode,
-    instrument,
-    separation
-) -> _AssayManager:
+def _create_assay_manager(assay_path, data_path, sample_metadata, ms_mode, instrument, separation, data_import_mode) -> _AssayManager:
     assay_path = _normalize_assay_path(assay_path)
 
     status = _is_assay_dir(assay_path)
+
     if status == 1:  # valid assay dir, load assay
         metadata_path = assay_path.joinpath(c.MANAGER_FILENAME)
         with open(metadata_path, "rb") as fin:
             manager = pickle.load(fin)
     elif status == 0:  # dir does not exist, create assay
         manager = _AssayManager(
             assay_path,
             data_path,
             sample_metadata,
             ms_mode,
             instrument,
             separation,
+            data_import_mode,
         )
         manager.create_assay_dir()
         manager.save()
     else:
         msg = "The directory is not a valid Assay directory."
         raise ValueError(msg)
     return manager
@@ -1254,48 +1555,42 @@
         plotter = _LCAssayPlotter(assay)
     else:
         msg = "No valid plotter found for separation={}".format(separation)
         raise ValueError(msg)
     return plotter
 
 
-def _create_sample_metadata(
-        sample_metadata: Optional[Union[str, pd.DataFrame]],
-        sample_names: List[str]
-) -> pd.DataFrame:
+def _create_sample_metadata(sample_metadata: Optional[Union[str, pd.DataFrame]], sample_names: List[str]) -> pd.DataFrame:
     # sample metadata df
     if isinstance(sample_metadata, str) or isinstance(sample_metadata, Path):
         df = pd.read_csv(sample_metadata)
     elif sample_metadata is None:
         df = pd.DataFrame(data=sample_names, columns=["sample"])
     elif isinstance(sample_metadata, pd.DataFrame):
         df = sample_metadata
     else:
-        msg = (
-            "`sample_metadata` must be a path to a csv file, a DataFrame "
-            "or None."
-        )
+        msg = "`sample_metadata` must be a path to a csv file, a DataFrame " "or None."
         raise ValueError(msg)
     return df
 
 
 def _normalize_sample_metadata(df: pd.DataFrame, name_to_path: List[str]):
     n_rows, _ = df.shape
     df = df.copy()  # avoid modifying the original DataFrame
 
     if "sample" in df:
         df = df.set_index("sample")
         samples_in_path = set(name_to_path)
         samples_in_metadata = set(df.index)
         missing_in_metadata = samples_in_path.difference(samples_in_metadata)
         missing_in_path = samples_in_metadata.difference(samples_in_path)
-        if len(missing_in_metadata):     # missing samples in df
+        if len(missing_in_metadata):  # missing samples in df
             msg = "The following samples are missing in the sample metadata: {}"
             raise ValueError(msg.format(missing_in_metadata))
-        elif len(missing_in_path):   # missing samples in path
+        elif len(missing_in_path):  # missing samples in path
             msg = "The following samples were not found in the data path {}"
             raise ValueError(msg.format(missing_in_path))
     else:
         msg = "The `sample` column is missing in the data"
         raise ValueError(msg)
 
     if "class" not in df:
@@ -1333,15 +1628,14 @@
 
     rename_dict = {"order": c.ORDER, "batch": c.BATCH, "class": c.CLASS}
     df = df.rename(columns=rename_dict)
     return df
 
 
 def _normalize_assay_path(assay_path: Union[Path, str]):
-
     if not isinstance(assay_path, Path):
         assay_path = Path(assay_path)
 
     suffix = ".tidyms-assay"
     if assay_path.suffix != suffix:
         assay_path = Path(assay_path.parent / (assay_path.name + suffix))
     return assay_path.absolute()
@@ -1356,25 +1650,22 @@
     if isinstance(path, str):
         path = Path(path)
 
     if isinstance(path, list):
         path_list = [Path(x) for x in path]
     elif isinstance(path, Path):
         if path.is_dir():
-            path_list = list(path.glob("*.mzML"))   # all mzML files in the dir
+            path_list = list(path.glob("*.mzML"))  # all mzML files in the dir
         elif path.is_file():
             path_list = [path]
         else:
             msg = "{} doesn't exist".format(path)
             raise ValueError(msg)
     else:
-        msg = (
-            "Path must be a string, a Path object pointing to a directory with "
-            "mzML files or a list of strings with the path to mzML files."
-        )
+        msg = "Path must be a string, a Path object pointing to a directory with " "mzML files or a list of strings with the path to mzML files."
         raise ValueError(msg)
 
     for p in path_list:
         # check if all files in the list exists
         if not p.is_file() or (p.suffix != ".mzML"):
             msg = "{} is not a path to a mzML file".format(p)
             raise ValueError(msg)
@@ -1389,15 +1680,15 @@
     # value after all ROI have been serialized
     with open(roi_path, "w", newline="\n") as fin:
         dummy_header = header_template.format(1)
         fin.write(dummy_header)
         offset = len(dummy_header)
         index = list()
         for roi in roi_list:
-            serialized_roi = roi.to_json() + '\n'
+            serialized_roi = roi.to_string() + "\n"
             length = len(serialized_roi)
             index.append([offset, length])
             offset += len(serialized_roi)
             fin.write(serialized_roi)
         # write index
         fin.write(json.dumps(index))
         fin.seek(0)
@@ -1406,15 +1697,15 @@
         fin.write(header)
 
 
 def compare_dict(d1: Optional[dict], d2: Optional[dict]) -> bool:
     if (d1 is None) or (d2 is None):
         res = False
     else:
-        res = len(d1) == len(d2)    # first check of equality
+        res = len(d1) == len(d2)  # first check of equality
     if res:
         for k in d1:
             v1 = d1.get(k)
             v2 = d2.get(k)
             # check type
             res = type(v1) == type(v2)
             if not res:
@@ -1427,23 +1718,19 @@
                 res = v1 == v2
 
             if not res:
                 break
     return res
 
 
-def _build_params_dict(ms_mode: str, separation: str, instrument: str):
+def _build_params_dict(ms_mode: str, separation: str, instrument: str, data_import_mode: str):
     params_dict = {
-        "MSData": {
-            "ms_mode": ms_mode,
-            "separation": separation,
-            "instrument": instrument,
-        },
+        "MSData": {"ms_mode": ms_mode, "separation": separation, "instrument": instrument, "data_import_mode": data_import_mode},
         "processed_samples": {x: set() for x in c.PREPROCESSING_STEPS},
-        "preprocess_steps": {x: False for x in c.PREPROCESSING_STEPS}
+        "preprocess_steps": {x: False for x in c.PREPROCESSING_STEPS},
     }
     params_dict.update({x: dict() for x in c.PREPROCESSING_STEPS})
     return params_dict
 
 
 def _is_assay_dir(p: Path) -> int:
     """
@@ -1462,19 +1749,15 @@
     if p.exists():
         roi_dir = p.joinpath(c.ROI_DIR)
         ft_dir = p.joinpath(c.FT_DIR)
         metadata_path = p.joinpath(c.MANAGER_FILENAME)
         check_roi_dir = roi_dir.is_dir()
         check_ft_dir = ft_dir.is_dir()
         check_metadata = metadata_path.is_file()
-        is_valid_structure = (
-                check_roi_dir and
-                check_ft_dir and
-                check_metadata
-        )
+        is_valid_structure = check_roi_dir and check_ft_dir and check_metadata
         if is_valid_structure:
             status = 1
         else:
             status = -1
     else:
         status = 0
     return status
```

### Comparing `tidyms-0.6.3/src/tidyms/consensus_annotation.py` & `tidyms-0.7.0/src/tidyms/consensus_annotation.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/container.py` & `tidyms-0.7.0/src/tidyms/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 """
 
 from . import utils
 from . import validation
 from . import fileio
 from . import _batch_corrector
-from ._names import *
 from . import _constants as c
 import numpy as np
 import pandas as pd
 from sklearn.decomposition import PCA
 from typing import Dict, List, Optional, Iterable, Union, BinaryIO, TextIO
 import bokeh.plotting
 import pickle
@@ -73,15 +72,15 @@
     feature_metadata : DataFrame.
         Metadata associated to each feature (eg: mass to charge ratio (mz),
         retention time (rt), etc...). The index is equal to the `data_matrix`
         column. "mz" and "rt" are required columns.
     mapping : dictionary of sample types to a list of sample classes.
         Maps sample types to sample classes. valid samples types are `qc`,
         `blank`, `sample` or `suitability`. values are list of sample classes.
-        Mapping is used by Processor objects to define a default behaviour. For
+        Mapping is used by Processor objects to define a default behavior. For
         example, when using a BlankCorrector, the blank contribution to each
         feature is estimated using the sample classes that are values of the
         `blank` sample type.
     metrics : methods to compute common feature metrics.
     plot : methods to plot features.
     preprocess : methods to perform common preprocessing tasks.
     id
@@ -138,40 +137,34 @@
             columns.
         mapping : dict or None
             if dict, set each sample class to sample type.
         plot_mode : {"seaborn", "bokeh"}
             The package used to generate plots with the plot methods
 
         """
-        validation.validate_data_container(
-            data_matrix, feature_metadata, sample_metadata
-        )
+        validation.validate_data_container(data_matrix, feature_metadata, sample_metadata)
 
         # sort columns and indices of each DataFrame
         data_matrix = data_matrix.sort_index()
         data_matrix = data_matrix.reindex(sorted(data_matrix.columns), axis=1)
         sample_metadata = sample_metadata.sort_index()
-        sample_metadata = sample_metadata.reindex(
-            sorted(sample_metadata.columns), axis=1
-        )
+        sample_metadata = sample_metadata.reindex(sorted(sample_metadata.columns), axis=1)
         feature_metadata = feature_metadata.sort_index()
-        feature_metadata = feature_metadata.reindex(
-            sorted(feature_metadata.columns), axis=1
-        )
+        feature_metadata = feature_metadata.reindex(sorted(feature_metadata.columns), axis=1)
 
         # check and convert order and batch information
         try:
-            order = sample_metadata.pop(_sample_order)
+            order = sample_metadata.pop(c.ORDER)
             try:
-                batch = sample_metadata.pop(_sample_batch)
+                batch = sample_metadata.pop(c.BATCH)
             except KeyError:
                 batch = pd.Series(data=np.ones_like(order.values), index=order.index)
             order = _convert_to_interbatch_order(order, batch)
-            sample_metadata[_sample_order] = order
-            sample_metadata[_sample_batch] = batch
+            sample_metadata[c.ORDER] = order
+            sample_metadata[c.BATCH] = batch
         except KeyError:
             pass
 
         # values are copied to prevent that modifications on the original
         # objects affect the DataContainer attributes
         self.data_matrix = data_matrix.copy()
         self.feature_metadata = feature_metadata.copy()
@@ -227,74 +220,72 @@
             valid_samples = self.classes.unique()
             _validate_mapping(mapping, valid_samples)
             self._mapping.update(mapping)
 
     @property
     def id(self) -> pd.Series:
         """pd.Series[str] : name id of each sample."""
-        return self._sample_metadata.loc[self._sample_mask, _sample_id]
+        return self._sample_metadata.loc[self._sample_mask, c.ID]
 
     @id.setter
     def id(self, value: pd.Series):
-        self._sample_metadata.loc[self._sample_mask, _sample_id] = value
+        self._sample_metadata.loc[self._sample_mask, c.ID] = value
 
     @property
     def classes(self) -> pd.Series:
         """pd.Series[str] : class of each sample."""
-        return self._sample_metadata.loc[self._sample_mask, _sample_class]
+        return self._sample_metadata.loc[self._sample_mask, c.CLASS]
 
     @classes.setter
     def classes(self, value: pd.Series):
-        self._sample_metadata.loc[self._sample_mask, _sample_class] = value
+        self._sample_metadata.loc[self._sample_mask, c.CLASS] = value
 
     @property
     def batch(self) -> pd.Series:
         """pd.Series[int]. Analytical batch number"""
         try:
-            return self._sample_metadata.loc[self._sample_mask, _sample_batch]
+            return self._sample_metadata.loc[self._sample_mask, c.BATCH]
         except KeyError:
             raise BatchInformationError("No batch information available.")
 
     @batch.setter
     def batch(self, value: pd.Series):
 
-        self._sample_metadata.loc[self._sample_mask, _sample_batch] = value.astype(int)
+        self._sample_metadata.loc[self._sample_mask, c.BATCH] = value.astype(int)
 
     @property
     def order(self) -> pd.Series:
         """
         pd.Series[int] : Run order in which samples were analyzed. It must be
         an unique integer for each sample.
         """
         try:
-            return self._sample_metadata.loc[self._sample_mask, _sample_order]
+            return self._sample_metadata.loc[self._sample_mask, c.ORDER]
         except KeyError:
             raise RunOrderError("No run order information available")
 
     @order.setter
     def order(self, value: pd.Series):
         if utils.is_unique(value):
-            self._sample_metadata.loc[self._sample_mask, _sample_order] = value.astype(
-                int
-            )
+            self._sample_metadata.loc[self._sample_mask, c.ORDER] = value.astype(int)
         else:
             msg = "order values must be unique"
             raise ValueError(msg)
 
     @property
     def dilution(self) -> pd.Series:
         try:
-            return self._sample_metadata.loc[self._sample_mask, _sample_dilution]
+            return self._sample_metadata.loc[self._sample_mask, c.DILUTION]
         except KeyError:
             msg = "No dilution information available."
             raise DilutionInformationError(msg)
 
     @dilution.setter
     def dilution(self, value):
-        self._sample_metadata.loc[self._sample_mask, _sample_dilution] = value
+        self._sample_metadata.loc[self._sample_mask, c.DILUTION] = value
 
     def is_valid_class_name(self, test_class: Union[str, List[str]]) -> bool:
         """
         Check if at least one sample class is`class_name`.
 
         Parameters
         ----------
@@ -370,27 +361,27 @@
             if there is batch number information associated to the samples.
 
         """
 
         diagnostic = dict()
         diagnostic["empty"] = self.data_matrix.empty
         diagnostic["missing"] = self.data_matrix.isna().any().any()
-        diagnostic[_qc_sample_type] = bool(self.mapping[_qc_sample_type])
-        diagnostic[_blank_sample_type] = bool(self.mapping[_blank_sample_type])
-        diagnostic[_study_sample_type] = bool(self.mapping[_study_sample_type])
-        diagnostic[_dilution_qc_type] = bool(self.mapping[_dilution_qc_type])
+        diagnostic[c.QC_TYPE] = bool(self.mapping[c.QC_TYPE])
+        diagnostic[c.BLANK_TYPE] = bool(self.mapping[c.BLANK_TYPE])
+        diagnostic[c.STUDY_TYPE] = bool(self.mapping[c.STUDY_TYPE])
+        diagnostic[c.DQC_TYPE] = bool(self.mapping[c.DQC_TYPE])
         try:
-            diagnostic[_sample_order] = self.order.any()
+            diagnostic[c.ORDER] = self.order.any()
         except RunOrderError:
-            diagnostic[_sample_order] = False
+            diagnostic[c.ORDER] = False
 
         try:
-            diagnostic[_sample_batch] = self.batch.any()
+            diagnostic[c.BATCH] = self.batch.any()
         except BatchInformationError:
-            diagnostic[_sample_batch] = False
+            diagnostic[c.BATCH] = False
         return diagnostic
 
     def reset(self, reset_mapping: bool = True):
         """
         Reloads the original data matrix.
 
         Parameters
@@ -521,16 +512,16 @@
         interbatch_order : bool
             If True converts the order value to a unique value for the whole
             DataContainer. This makes plotting the data as a function of order
             easier.
 
         """
         df = pd.read_csv(path, index_col="sample")
-        order = df[_sample_order].astype(int)
-        batch = df[_sample_batch].astype(int)
+        order = df[c.ORDER].astype(int)
+        batch = df[c.BATCH].astype(int)
 
         if interbatch_order:
             order = _convert_to_interbatch_order(order, batch)
         self.order = order
         self.batch = batch
 
     def to_csv(self, filename: str) -> None:
@@ -630,17 +621,15 @@
             cv_func = utils.cv
 
         if groupby is not None:
             if isinstance(groupby, str):
                 by = self.__data.sample_metadata[groupby]
             else:
                 by = [self.__data.sample_metadata[x] for x in groupby]
-            result = self.__data.data_matrix.groupby(by).apply(
-                cv_func, fill_value=fill_value
-            )
+            result = self.__data.data_matrix.groupby(by).apply(cv_func, fill_value=fill_value)
         else:
             result = cv_func(self.__data.data_matrix, fill_value=fill_value)
         return result
 
     def dratio(self, robust=False) -> pd.Series:
         """
         Computes the ratio between the sample variation and the quality control
@@ -657,35 +646,33 @@
 
         Returns
         -------
         dr : pd.Series:
             D-Ratio for each feature
 
         """
-        if self.__data.mapping[_study_sample_type] is None:
+        if self.__data.mapping[c.STUDY_TYPE] is None:
             msg = "Study sample classes not specified in the sample mapping"
             raise ValueError(msg)
-        sample_classes = self.__data.mapping[_study_sample_type]
+        sample_classes = self.__data.mapping[c.STUDY_TYPE]
 
-        if self.__data.mapping[_qc_sample_type] is None:
+        if self.__data.mapping[c.QC_TYPE] is None:
             msg = "QC class not specified in the sample mapping"
             raise ValueError(msg)
-        qc_classes = self.__data.mapping[_qc_sample_type]
+        qc_classes = self.__data.mapping[c.QC_TYPE]
 
         is_sample_class = self.__data.classes.isin(sample_classes)
         is_qc_class = self.__data.classes.isin(qc_classes)
         sample_data = self.__data.data_matrix[is_sample_class]
         qc_data = self.__data.data_matrix[is_qc_class]
         # NaN are filled to inf to make filtration easier.
         dratio = utils.sd_ratio(qc_data, sample_data, robust=robust, fill_value=np.inf)
         return dratio
 
-    def detection_rate(
-        self, groupby: Union[str, List[str], None] = "class", threshold=0
-    ):
+    def detection_rate(self, groupby: Union[str, List[str], None] = "class", threshold=0):
         """
         Computes the fraction of samples where a feature was detected.
 
         Parameters
         ----------
         groupby : str, List[str] or None
             If groupby isa column or a list of columns of sample metadata, the
@@ -700,17 +687,15 @@
                 by = self.__data.sample_metadata[groupby]
             else:
                 by = [self.__data.sample_metadata[x] for x in groupby]
             result = self.__data.data_matrix.groupby(by).apply(
                 utils.detection_rate, threshold=threshold
             )
         else:
-            result = self.__data.data_matrix.apply(
-                utils.detection_rate, threshold=threshold
-            )
+            result = self.__data.data_matrix.apply(utils.detection_rate, threshold=threshold)
         return result
 
     def pca(
         self,
         n_components: Optional[int] = 2,
         normalization: Optional[str] = None,
         scaling: Optional[str] = None,
@@ -763,17 +748,15 @@
         loadings = pd.DataFrame(
             data=loadings, index=self.__data.data_matrix.columns, columns=pc_str
         )
         variance = pd.Series(data=variance, index=pc_str)
         total_variance = data.var().sum()
         return scores, loadings, variance, total_variance
 
-    def correlation(
-        self, field: str, mode: str = "ols", classes: Optional[List[str]] = None
-    ):
+    def correlation(self, field: str, mode: str = "ols", classes: Optional[List[str]] = None):
         """
         Correlates features with sample metadata properties.
 
         Parameters
         ----------
         field : str
             A column of `sample_metadata`. Must have a numeric dtype.
@@ -821,15 +804,15 @@
     def __init__(self, data: DataContainer):
         self._data_container = data
 
     def pca_scores(
         self,
         x_pc: int = 1,
         y_pc: int = 2,
-        hue: str = _sample_class,
+        hue: str = c.CLASS,
         ignore_classes: Optional[List[str]] = None,
         show_order: bool = False,
         scaling: Optional[str] = None,
         normalization: Optional[str] = None,
         draw: bool = True,
         fig_params: Optional[dict] = None,
         scatter_params: Optional[dict] = None,
@@ -878,38 +861,38 @@
         if scatter_params is None:
             scatter_params = default_scatter_params
         else:
             default_scatter_params.update(scatter_params)
             scatter_params = default_scatter_params
 
         tooltips = [
-            (_sample_class, "@{}".format(_sample_class)),
-            (_sample_order, "@{}".format(_sample_order)),
-            (_sample_batch, "@{}".format(_sample_batch)),
-            (_sample_id, "@{}".format(_sample_id)),
+            (c.CLASS, "@{}".format(c.CLASS)),
+            (c.ORDER, "@{}".format(c.ORDER)),
+            (c.BATCH, "@{}".format(c.BATCH)),
+            (c.ID, "@{}".format(c.ID)),
         ]
         fig = bokeh.plotting.figure(tooltips=tooltips, **fig_params)
 
         x_name = "PC" + str(x_pc)
         y_name = "PC" + str(y_pc)
         n_comps = max(x_pc, y_pc)
         score, _, variance, total_var = self._data_container.metrics.pca(
             n_components=n_comps,
             ignore_classes=ignore_classes,
             normalization=normalization,
             scaling=scaling,
         )
         score = score.join(self._data_container.sample_metadata)
 
-        if hue == _sample_type:
+        if hue == c.TYPE:
             rev_map = _reverse_mapping(self._data_container.mapping)
-            score[_sample_type] = score[_sample_class].apply(lambda x: rev_map.get(x))
-            score = score[~pd.isna(score[_sample_type])]
-        elif hue == _sample_batch:
-            score[_sample_batch] = score[_sample_batch].astype(str)
+            score[c.TYPE] = score[c.CLASS].apply(lambda x: rev_map.get(x))
+            score = score[~pd.isna(score[c.TYPE])]
+        elif hue == c.BATCH:
+            score[c.BATCH] = score[c.BATCH].astype(str)
 
         # setup the colors
         unique_values = score[hue].unique().astype(str)
         score = ColumnDataSource(score)
         cmap = Category10[10]
         palette = cmap * (int(unique_values.size / len(cmap)) + 1)
         palette = palette[: unique_values.size]
@@ -934,15 +917,15 @@
         fig.yaxis.axis_label_text_font_style = "bold"
         fig.xaxis.axis_label_text_font_style = "bold"
 
         if show_order:
             labels = LabelSet(
                 x=x_name,
                 y=y_name,
-                text=_sample_order,
+                text=c.ORDER,
                 level="glyph",
                 x_offset=3,
                 y_offset=3,
                 source=score,
                 render_mode="canvas",
                 text_font_size="8pt",
             )
@@ -1029,15 +1012,15 @@
         if draw:
             bokeh.plotting.show(fig)
         return fig
 
     def feature(
         self,
         ft: str,
-        hue: str = _sample_class,
+        hue: str = c.CLASS,
         ignore_classes: Optional[List[str]] = None,
         draw: bool = True,
         fig_params: Optional[dict] = None,
         scatter_params: Optional[dict] = None,
     ) -> bokeh.plotting.figure:
         """
         plots a feature intensity as a function of the run order.
@@ -1074,43 +1057,43 @@
         if ignore_classes is None:
             ignore_classes = list()
 
         source = self._data_container.sample_metadata.join(
             self._data_container.data_matrix[ft]
         )
 
-        ignore_samples = source[_sample_class].isin(ignore_classes)
+        ignore_samples = source[c.CLASS].isin(ignore_classes)
         source = source[~ignore_samples]
 
-        if hue == _sample_type:
+        if hue == c.TYPE:
             rev_map = _reverse_mapping(self._data_container.mapping)
-            source[_sample_type] = source[_sample_class].apply(lambda x: rev_map.get(x))
-            source = source[~source[_sample_type].isna()]
-        elif hue == _sample_batch:
-            source[_sample_batch] = source[_sample_batch].astype(str)
+            source[c.TYPE] = source[c.CLASS].apply(lambda x: rev_map.get(x))
+            source = source[~source[c.TYPE].isna()]
+        elif hue == c.BATCH:
+            source[c.BATCH] = source[c.BATCH].astype(str)
 
         # setup the colors
         unique_values = source[hue].unique().astype(str)
         cmap = Category10[10]
         palette = cmap * (int(unique_values.size / len(cmap)) + 1)
         palette = palette[: unique_values.size]
 
         source = ColumnDataSource(source)
 
         tooltips = [
-            (_sample_class, "@{}".format(_sample_class)),
-            (_sample_order, "@{}".format(_sample_order)),
-            (_sample_batch, "@{}".format(_sample_batch)),
-            (_sample_id, "@{}".format(_sample_id)),
+            (c.CLASS, "@{}".format(c.CLASS)),
+            (c.ORDER, "@{}".format(c.ORDER)),
+            (c.BATCH, "@{}".format(c.BATCH)),
+            (c.ID, "@{}".format(c.ID)),
         ]
         fig = bokeh.plotting.figure(tooltips=tooltips, **fig_params)
         cmap_factor = factor_cmap(hue, palette, unique_values)
         fig.scatter(
             source=source,
-            x=_sample_order,
+            x=c.ORDER,
             y=ft,
             color=cmap_factor,
             legend_group=hue,
             **scatter_params
         )
 
         fig.xaxis.axis_label = "Run order"
@@ -1133,15 +1116,15 @@
     def __init__(self, data: DataContainer):
         self.data = data
 
     def pca_scores(
         self,
         x_pc: int = 1,
         y_pc: int = 2,
-        hue: str = _sample_class,
+        hue: str = c.CLASS,
         ignore_classes: Optional[List[str]] = None,
         show_order: bool = False,
         scaling: Optional[str] = None,
         normalization: Optional[str] = None,
         relplot_params: Optional[dict] = None,
     ):
         """
@@ -1188,22 +1171,22 @@
 
         tmp_params = {"x": x_name, "y": y_name, "hue": hue, "kind": "scatter"}
         if relplot_params is None:
             relplot_params = tmp_params
         else:
             relplot_params.update(tmp_params)
 
-        if hue == _sample_type:
+        if hue == c.TYPE:
             rev_map = _reverse_mapping(self.data.mapping)
-            score[_sample_type] = score[_sample_class].apply(lambda s: rev_map.get(s))
-            score = score[~pd.isna(score[_sample_type])]
-        elif hue == _sample_batch:
-            score[_sample_batch] = score[_sample_batch].astype(str)
-        elif hue == _sample_class:
-            score[_sample_class] = self.data.classes
+            score[c.TYPE] = score[c.CLASS].apply(lambda s: rev_map.get(s))
+            score = score[~pd.isna(score[c.TYPE])]
+        elif hue == c.BATCH:
+            score[c.BATCH] = score[c.BATCH].astype(str)
+        elif hue == c.CLASS:
+            score[c.CLASS] = self.data.classes
 
         g = sns.relplot(data=score, **relplot_params)
 
         if show_order:
             for ind in score.index:
                 x = score.loc[ind, x_name] * 1.01
                 y = score.loc[ind, y_name] * 1.01
@@ -1278,40 +1261,40 @@
         g.ax.set_xlabel(x_label)
         g.ax.set_ylabel(y_label)
         return g
 
     def feature(
         self,
         ft: str,
-        hue: str = _sample_class,
+        hue: str = c.CLASS,
         ignore_classes: Optional[List[str]] = None,
         relplot_params: Optional[dict] = None,
     ):
 
-        tmp_params = {"x": _sample_order, "y": ft, "hue": hue, "kind": "scatter"}
+        tmp_params = {"x": c.ORDER, "y": ft, "hue": hue, "kind": "scatter"}
         if relplot_params is None:
             relplot_params = tmp_params
         else:
             relplot_params.update(tmp_params)
 
         if ignore_classes is None:
             ignore_classes = list()
 
         df = self.data.sample_metadata.join(self.data.data_matrix[ft])
-        ignore_samples = df[_sample_class].isin(ignore_classes)
+        ignore_samples = df[c.CLASS].isin(ignore_classes)
         df = df[~ignore_samples]
 
-        if hue == _sample_type:
+        if hue == c.TYPE:
             rev_map = _reverse_mapping(self.data.mapping)
-            df[_sample_type] = df[_sample_class].apply(lambda x: rev_map.get(x))
-            df = df[~df[_sample_type].isna()]
-        elif hue == _sample_batch:
-            df[_sample_batch] = df[_sample_batch].astype(str)
-        elif hue == _sample_class:
-            df[_sample_class] = df[_sample_class].astype(str)
+            df[c.TYPE] = df[c.CLASS].apply(lambda x: rev_map.get(x))
+            df = df[~df[c.TYPE].isna()]
+        elif hue == c.BATCH:
+            df[c.BATCH] = df[c.BATCH].astype(str)
+        elif hue == c.CLASS:
+            df[c.CLASS] = df[c.CLASS].astype(str)
 
         g = sns.relplot(data=df, **relplot_params)
         return g
 
     def correlation_histogram(self, class_: Optional[str] = None, **hist_params):
         """
         Plots the distribution of correlation of feature pairs for a given class.
@@ -1419,41 +1402,41 @@
             inter-batch where the mean across different batches is corrected.
 
         A detailed explanation of the correction algorithm can be found here.
 
         """
         mapping = self.__data.mapping
 
-        if mapping[_qc_sample_type] is None:
+        if mapping[c.QC_TYPE] is None:
             msg = "QC samples not defined in sample mapping"
             raise ValueError(msg)
 
-        if mapping[_study_sample_type] is None:
+        if mapping[c.STUDY_TYPE] is None:
             msg = "Study samples not defined in sample mapping"
             raise ValueError(msg)
 
         sample_metadata = self.__data.sample_metadata
 
-        if _sample_order not in sample_metadata:
+        if c.ORDER not in sample_metadata:
             msg = "Run order information not available"
             raise RunOrderError(msg)
 
-        if _sample_batch not in sample_metadata:
+        if c.BATCH not in sample_metadata:
             msg = "Batch information not available"
             raise BatchInformationError(msg)
 
-        sample_class = mapping[_study_sample_type]
-        qc_class = mapping[_qc_sample_type]
+        sample_class = mapping[c.STUDY_TYPE]
+        qc_class = mapping[c.QC_TYPE]
 
         rm_samples = _batch_corrector.find_invalid_samples(
             sample_metadata, sample_class, qc_class
         )
         self.__data.remove(rm_samples, "samples")
 
-        # TODO: this should be removed after fixing the Datacontainer
+        # TODO: this should be removed after fixing the DataContainer
         #   00implementation
         sample_metadata = self.__data.sample_metadata
         data_matrix = self.__data.data_matrix
 
         rm_features = _batch_corrector.find_invalid_features(
             data_matrix, sample_metadata, sample_class, qc_class, threshold, min_qc_dr
         )
@@ -1611,21 +1594,21 @@
     """
 
     pass
 
 
 def _validate_mapping(mapping, valid_samples):
     for sample_type, classes in mapping.items():
-        if sample_type not in SAMPLE_TYPES:
+        if sample_type not in c.SAMPLE_TYPES:
             msg = "{} is not a valid sample type".format(sample_type)
             raise ValueError(msg)
         else:
-            for c in classes:
-                if c not in valid_samples:
-                    msg = "{} is not a valid sample class".format(c)
+            for cl in classes:
+                if cl not in valid_samples:
+                    msg = "{} is not a valid sample class".format(cl)
                     raise ValueError(msg)
 
 
 def _convert_to_interbatch_order(order: pd.Series, batch: pd.Series) -> pd.Series:
     """
     Convert the order values from a per-batch order to a interbatch order.
 
@@ -1662,29 +1645,29 @@
     add_to_order = pd.Series(data=add_to_order, index=max_order.index)
     add_to_order = batch.map(add_to_order)
     interbatch_order = order + add_to_order
     return interbatch_order
 
 
 def _make_empty_mapping():
-    empty_mapping = {x: None for x in SAMPLE_TYPES}
+    empty_mapping = {x: None for x in c.SAMPLE_TYPES}
     return empty_mapping
 
 
 def _reverse_mapping(mapping):
     rev_map = dict()
     for k, v in mapping.items():
         if v is not None:
             for class_value in v:
                 rev_map[class_value] = k
     return rev_map
 
 
 def _create_annotation_report(
-        data_matrix: pd.DataFrame, feature_metadata: pd.DataFrame
+    data_matrix: pd.DataFrame, feature_metadata: pd.DataFrame
 ) -> Dict[str, str]:
     annotation_report = dict()
 
     median_abundance = data_matrix.median()
     score = feature_metadata["count"] / feature_metadata["total"]
     score[score.isna()] = 1
 
@@ -1700,16 +1683,10 @@
             gmz = gmz[sorted_index]
             g_score = score[features].to_numpy()
             g_score = g_score[sorted_index]
             charge = gdf.at[features[0], c.CHARGE]
             gmz = list(gmz.round(4))
             gp = list(gp.round(4))
             g_score = list(g_score.round(2))
-            d = {
-                c.CHARGE: int(charge),
-                c.MZ: gmz,
-                "abundance": gp,
-                "score": g_score
-            }
+            d = {c.CHARGE: int(charge), c.MZ: gmz, "abundance": gp, "score": g_score}
             annotation_report[main_ft] = json.dumps(d)
     return annotation_report
-
```

### Comparing `tidyms-0.6.3/src/tidyms/correspondence.py` & `tidyms-0.7.0/src/tidyms/correspondence.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/fill_missing.py` & `tidyms-0.7.0/src/tidyms/fill_missing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,38 +9,29 @@
 from .lcms import Chromatogram
 from .raw_data_utils import make_chromatograms
 from .utils import find_closest, get_progress_bar
 from sklearn.impute import KNNImputer
 
 
 missing_data_iterator_type = Generator[
-    Tuple[
-        MSData,
-        str,
-        np.ndarray,
-        np.ndarray,
-        np.ndarray,
-        np.ndarray,
-        np.ndarray,
-        pd.Index
-    ],
+    Tuple[MSData, str, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, pd.Index],
+    None,
     None,
-    None
 ]
 
 
 def fill_missing_lc(
     ms_data_generator: Generator[Tuple[str, MSData], None, None],
     data_matrix: pd.DataFrame,
     feature_metadata: pd.DataFrame,
     mz_tolerance: float,
     n_deviations: float,
     estimate_not_found: bool,
     n_jobs: Optional[int] = None,
-    verbose: bool = False
+    verbose: bool = False,
 ):
     """
     Fill missing values by searching missing peaks in the raw data.
 
     Notes
     -----
 
@@ -89,37 +80,32 @@
         Data matrix with missing values imputed
     missing_indicator : pd.DataFrame
         DataFrame with the same shape as the data matrix, with values that
         indicates if a feature was detected (0), filled (1) or estimated (2).
 
     """
     missing_iterator = _get_missing_data_iterator(
-        ms_data_generator, data_matrix, feature_metadata)
+        ms_data_generator, data_matrix, feature_metadata
+    )
     if verbose:
         progress_bar = get_progress_bar()
         total = data_matrix.shape[0]
         print("Filling missing values in {} samples".format(total))
-        missing_iterator = progress_bar(
-            missing_iterator,
-            total=total
-        )
+        missing_iterator = progress_bar(missing_iterator, total=total)
 
     func = partial(
         _get_sample_fill_values,
         mz_tolerance=mz_tolerance,
         n_deviations=n_deviations,
-        estimate_not_found=estimate_not_found
+        estimate_not_found=estimate_not_found,
     )
     func = delayed(func)
     fill_results = Parallel(n_jobs=n_jobs)(func(*x) for x in missing_iterator)
     missing = pd.DataFrame(
-        data=0,
-        index=data_matrix.index,
-        columns=data_matrix.columns,
-        dtype=int
+        data=0, index=data_matrix.index, columns=data_matrix.columns, dtype=int
     )
     for res in fill_results:
         sample, found_area, found_index, not_found_area, not_found_index = res
         # TODO: fix after refactoring DataContainer
         data_matrix.loc[sample, found_index] = found_area
         data_matrix.loc[sample, not_found_index] = not_found_area
         missing.loc[sample, found_index] = 1
@@ -174,15 +160,15 @@
     X = imputer.fit_transform(df)
     return pd.DataFrame(data=X, index=df.index, columns=df.columns)
 
 
 def _get_missing_data_iterator(
     ms_data_generator: Generator[Tuple[str, MSData], None, None],
     data_matrix: pd.DataFrame,
-    feature_metadata: pd.DataFrame
+    feature_metadata: pd.DataFrame,
 ) -> missing_data_iterator_type:
     mz = feature_metadata[c.MZ]
     rt = feature_metadata[c.RT]
     rt_std = feature_metadata[c.RT_STD]
     rt_start = feature_metadata[c.RT_START]
     rt_end = feature_metadata[c.RT_END]
     for sample, ms_data in ms_data_generator:
@@ -191,15 +177,15 @@
             ms_data,
             sample,
             mz[missing_mask].to_numpy(),
             rt[missing_mask].to_numpy(),
             rt_std[missing_mask].to_numpy(),
             rt_start[missing_mask].to_numpy(),
             rt_end[missing_mask].to_numpy(),
-            missing_mask[missing_mask].index
+            missing_mask[missing_mask].index,
         )
         yield missing_data
 
 
 def _get_sample_fill_values(
     ms_data: MSData,
     sample: str,
@@ -207,15 +193,15 @@
     rt: np.ndarray,
     rt_std: np.ndarray,
     rt_start: np.ndarray,
     rt_end: np.ndarray,
     features: pd.Index,
     mz_tolerance: float,
     n_deviations: float,
-    estimate_not_found: bool
+    estimate_not_found: bool,
 ) -> Tuple[str, np.ndarray, pd.Index, np.ndarray, pd.Index]:
     """
     Finds fill values for features not detected during feature extraction in a
     sample.
 
     Parameters
     ----------
@@ -254,15 +240,15 @@
         chrom.fill_nan(fill_value=0.0, bounds_error=False)
         area = _get_fill_area(chrom, c_rt, c_rt_std, n_deviations)
         if area is None:
             not_found_index.append(c_ft)
             if estimate_not_found:
                 area = trapz(
                     chrom.spint[c_start_index:c_end_index],
-                    chrom.time[c_start_index:c_end_index]
+                    chrom.time[c_start_index:c_end_index],
                 )
 
             else:
                 area = 0.0
             not_found_area.append(area)
         else:
             found_index.append(c_ft)
@@ -273,18 +259,15 @@
     found_index = pd.Index(found_index)
     not_found_index = pd.Index(not_found_index)
 
     return sample, found_area, found_index, not_found_area, not_found_index
 
 
 def _get_fill_area(
-    chromatogram: Chromatogram,
-    rt: float,
-    rt_std: float,
-    n_deviations: float
+    chromatogram: Chromatogram, rt: float, rt_std: float, n_deviations: float
 ) -> Optional[float]:
     """
     Search a peak in a region defined between ``rt - rt_std`` and
     ``rt + rt_std``. If a peak is found, the corresponding area is found.
     Otherwise, return None.
 
     Parameters
@@ -300,20 +283,20 @@
 
     Returns
     -------
     area : float or None
 
     """
     chromatogram.extract_features(store_smoothed=True)
-    rt_ft = np.array([p.get_rt(chromatogram) for p in chromatogram.features])
+    rt_ft = np.array([p.get_rt() for p in chromatogram.features])
     if rt_ft.size:
         closest_feature = find_closest(rt_ft, rt)
         is_valid_peak = abs(rt_ft[closest_feature] - rt) < rt_std * n_deviations
         if is_valid_peak:
-            area = chromatogram.features[closest_feature].get_area(chromatogram)
+            area = chromatogram.features[closest_feature].get_area()
             chromatogram.features = [chromatogram.features[closest_feature]]
         else:
             area = None
             chromatogram.features = []
     else:
         area = None
     return area
```

### Comparing `tidyms-0.6.3/src/tidyms/filter.py` & `tidyms-0.7.0/src/tidyms/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tools to filter and correct DataContainers.
 
 A Filter removes features or samples from a DataContainer according to some
 criteria. Correctors perform transformations on the data matrix. Each filter and
-corrector has a default behaviour based on recommendations by widely accepted by
+corrector has a default behavior based on recommendations by widely accepted by
 the metabolomics community. Operations on DataContainers are made in place. To
 generate corrections and filters, the default corrections are generated using
 information in the DataContainer mapping.
 
 For example, The BlankCorrector generates and estimation of the blank
 contribution to the signal using sample classes that are mapped from
 the "blank" sample type. See each Processor object for detailed information.
@@ -35,21 +35,21 @@
 MissingValueError : Error raised when the data matrix has missing values.
 
 """
 
 
 from .container import DataContainer
 from . import container
-from ._names import *
-from ._filter_functions import *
-from ._batch_corrector import *
+from . import _filter_functions as ff
 from . import validation
+from . import _constants as c
 import os.path
 from warnings import warn
 from typing import Optional, List, Union, Callable
+
 Number = Union[float, int]
 
 # TODO: replace Processor with Filter and Corrector objects.
 # TODO : refactor Processor using the following func prototype:
 #   func(dc, **self.params)
 
 
@@ -60,14 +60,15 @@
     Attributes
     ----------
     metrics: dict
         stores number of features, number of samples and mean coefficient of
         variation before and after processing.
     name: str
     """
+
     def __init__(self, name: Optional[str] = None):
         self.metrics = dict()
         self.name = name
         self.results = None
 
     def _record_metrics(self, dc: DataContainer, status: str):
         """
@@ -75,50 +76,55 @@
 
         Parameters
         ----------
         dc: DataContainer
         status: {"before", "after"}
         """
         metrics = dict()
-        metrics["cv"] = (dc.metrics.cv(groupby="class", fill_value=0)
-                         .median()
-                         .median())
+        metrics["cv"] = dc.metrics.cv(groupby="class", fill_value=0).median().median()
         n_samples, n_features = dc.data_matrix.shape
         metrics["features"] = n_features
         metrics["samples"] = n_samples
         if status in ["before", "after"]:
             self.metrics[status] = metrics
         else:
             msg = "status must be before or after."
             raise ValueError(msg)
 
     def _make_results(self):
         """
         Computes variation in the number of features, samples and CV.
         """
         if ("before" in self.metrics) and ("after" in self.metrics):
-            removed_features = (self.metrics["before"]["features"]
-                                - self.metrics["after"]["features"])
-            removed_samples = (self.metrics["before"]["samples"]
-                               - self.metrics["after"]["samples"])
-            cv_reduction = (self.metrics["before"]["cv"]
-                            - self.metrics["after"]["cv"]) * 100
+            removed_features = (
+                self.metrics["before"]["features"] - self.metrics["after"]["features"]
+            )
+            removed_samples = (
+                self.metrics["before"]["samples"] - self.metrics["after"]["samples"]
+            )
+            cv_reduction = (self.metrics["before"]["cv"] - self.metrics["after"]["cv"]) * 100
             results = dict()
             results["features"] = removed_features
             results["samples"] = removed_samples
             results["cv"] = cv_reduction
             self.results = results
 
     def report(self):
         if self.results:
-            msg = "Applying {}: {} features removed, " \
-                  "{} samples removed, " \
-                  "Mean CV reduced by {:.2f} %."
-            msg = msg.format(self.name, self.results["features"],
-                             self.results["samples"], self.results["cv"])
+            msg = (
+                "Applying {}: {} features removed, "
+                "{} samples removed, "
+                "Mean CV reduced by {:.2f} %."
+            )
+            msg = msg.format(
+                self.name,
+                self.results["features"],
+                self.results["samples"],
+                self.results["cv"],
+            )
             print(msg)
 
 
 class Processor(Reporter):
     """
     Abstract class to process DataContainer Objects. This class is intended to
     be subclassed to generate specific filters. Filter implementation is done
@@ -144,18 +150,24 @@
         from a DataContainer. If any value is different compared to the values
         from diagnose an error is raised.
 
     Methods
     -------
     process(data) : Applies a filter/correction to a DataContainer
     """
-    def __init__(self, mode: str, axis: Optional[str] = None,
-                 verbose: bool = False, default_process: Optional[str] = None,
-                 default_correct: Optional[str] = None,
-                 requirements: Optional[dict] = None):
+
+    def __init__(
+        self,
+        mode: str,
+        axis: Optional[str] = None,
+        verbose: bool = False,
+        default_process: Optional[str] = None,
+        default_correct: Optional[str] = None,
+        requirements: Optional[dict] = None,
+    ):
         super(Processor, self).__init__()
         self.mode = mode
         self.axis = axis
         self.verbose = verbose
         self.remove = list()
         self.params = dict()
         self._default_process = default_process
@@ -179,21 +191,22 @@
                 class_list = self.params[class_type]
                 if class_type == "process_classes":
                     default = self._default_process
                 else:
                     default = self._default_correct
                 has_mapping = dc_status[default]
                 if (class_list is None) and (not has_mapping):
-                    msg = "no classes where assigned to {} sample type in " \
+                    msg = (
+                        "no classes where assigned to {} sample type in "
                         "the sampling mapping"
+                    )
                     msg = msg.format(default)
                     raise MissingMappingInformation(msg)
                 elif not dc.is_valid_class_name(class_list):
-                    msg = "classes listed in {} aren't present " \
-                          "in the DataContainer"
+                    msg = "classes listed in {} aren't present " "in the DataContainer"
                     msg = msg.format(class_type)
                     raise container.ClassNameError(msg)
 
         for requirement in self._requirements:
             if self._requirements[requirement] != dc_status[requirement]:
                 raise _requirements_error[requirement]
 
@@ -240,14 +253,15 @@
     Attributes
     ----------
     processors: list[Processors]
         A list of processors to apply. Can also contain another Pipeline.
     verbose: bool
         If True prints a message each time a Processor is applied.
     """
+
     def __init__(self, processors: list, verbose: bool = False):
         _validate_pipeline(processors)
         super(Pipeline, self).__init__()
         self.processors = list(processors)
         self.verbose = verbose
 
     def process(self, dc):
@@ -284,43 +298,46 @@
 
 
 @register
 class DuplicateMerger(Processor):
     """
     Merge sample replicates.
     """
+
     # TODO: add merger parameter, classes to merge.
     def __init__(self, process_classes: Optional[List[str]] = None):
         super(DuplicateMerger, self).__init__(axis=None, mode="transform")
         self.params["process_classes"] = process_classes
 
     def func(self, dc: DataContainer):
         if self.params["process_classes"] is None:
-            self.params["process_classes"] = dc.mapping[_study_sample_type]
-        dc.data_matrix = average_replicates(dc.data_matrix, dc.id,
-                                            dc.classes, **self.params)
-        dc.sample_metadata = (dc.sample_metadata
-                              .loc[dc.data_matrix.index, :])
+            self.params["process_classes"] = dc.mapping[c.STUDY_TYPE]
+        dc.data_matrix = ff.average_replicates(
+            dc.data_matrix, dc.id, dc.classes, **self.params
+        )
+        dc.sample_metadata = dc.sample_metadata.loc[dc.data_matrix.index, :]
 
 
 @register
 class ClassRemover(Processor):
     """
     Remove samples from the specified classes.
 
     Parameters
     ----------
     classes: list
         List of classes to remove.
 
     """
+
     def __init__(self, classes: List[str]):
         requirements = {"empty": False, "missing": False}
-        super(ClassRemover, self).__init__(axis="samples", mode="filter",
-                                           requirements=requirements)
+        super(ClassRemover, self).__init__(
+            axis="samples", mode="filter", requirements=requirements
+        )
         self.name = "Class Remover"
         if classes is None:
             self.params["classes"] = list()
         else:
             self.params["classes"] = classes
 
     def func(self, dc):
@@ -376,42 +393,46 @@
 
     .. math::
 
         X_{corrected} = 0 \textrm{ if } X < factor * mode(X_{blank}) \\
         X_{corrected} = X - mode(X_{blank}) \textrm{ else}
 
     """
-    def __init__(self, corrector_classes: Optional[List[str]] = None,
-                 process_classes: Optional[List[str]] = None,
-                 mode: Union[str, Callable] = "lod", factor: float = 1,
-                 robust: bool = True,
-                 process_blanks: bool = True, verbose=False):
+
+    def __init__(
+        self,
+        corrector_classes: Optional[List[str]] = None,
+        process_classes: Optional[List[str]] = None,
+        mode: Union[str, Callable] = "lod",
+        factor: float = 1,
+        robust: bool = True,
+        process_blanks: bool = True,
+        verbose=False,
+    ):
         """
         Constructor for the BlankCorrector.
 
         """
-        requirements = {"empty": False, "missing": False,
-                        _blank_sample_type: True}
-        super(BlankCorrector, self).__init__(axis=None, mode="transform",
-                                             verbose=verbose,
-                                             requirements=requirements)
+        requirements = {"empty": False, "missing": False, c.BLANK_TYPE: True}
+        super(BlankCorrector, self).__init__(
+            axis=None, mode="transform", verbose=verbose, requirements=requirements
+        )
         self.name = "Blank Corrector"
         self.params["corrector_classes"] = corrector_classes
         self.params["process_classes"] = process_classes
         self.params["mode"] = mode
         self.params["factor"] = factor
         self.params["process_blanks"] = process_blanks
         self.params["robust"] = robust
-        self._default_process = _study_sample_type
-        self._default_correct = _blank_sample_type
+        self._default_process = c.STUDY_TYPE
+        self._default_correct = c.BLANK_TYPE
         validation.validate_blank_corrector_params(self.params)
 
     def func(self, dc):
-        dc.data_matrix = \
-            correct_blanks(dc.data_matrix, dc.classes, **self.params)
+        dc.data_matrix = ff.correct_blanks(dc.data_matrix, dc.classes, **self.params)
 
 
 @register
 class PrevalenceFilter(Processor):
     """
     Remove Features detected in a low number of samples.
 
@@ -440,46 +461,51 @@
     -----
     The prevalence is computed using the detection rate, that is, the fraction
     of samples where a feature was detected. A feature is considered detected
     if its value is above a threshold. The `mode` parameter controls how the
     prevalence is computed.
 
     """
-    def __init__(self, process_classes: Optional[List[str]] = None,
-                 lb: Number = 0.5, ub: Number = 1,
-                 intraclass: bool = True, verbose: bool = False,
-                 threshold: Number = 0):
+
+    def __init__(
+        self,
+        process_classes: Optional[List[str]] = None,
+        lb: Number = 0.5,
+        ub: Number = 1,
+        intraclass: bool = True,
+        verbose: bool = False,
+        threshold: Number = 0,
+    ):
         """
         Constructor of the PrevalenceFilter.
         """
         requirements = {"empty": False, "missing": False}
-        super(PrevalenceFilter, self).__init__(axis="features", mode="filter",
-                                               verbose=verbose,
-                                               requirements=requirements)
+        super(PrevalenceFilter, self).__init__(
+            axis="features", mode="filter", verbose=verbose, requirements=requirements
+        )
         self.name = "Prevalence Filter"
         self.params["process_classes"] = process_classes
         self.params["lb"] = lb
         self.params["ub"] = ub
         self.params["intraclass"] = intraclass
         self.params["threshold"] = threshold
-        self._default_correct = _study_sample_type
-        self._default_process = _study_sample_type
+        self._default_correct = c.STUDY_TYPE
+        self._default_process = c.STUDY_TYPE
         validation.validate_prevalence_filter_params(self.params)
 
     def func(self, dc):
         if self.params["intraclass"]:
             groupby = "class"
         else:
             groupby = None
-        dr = dc.metrics.detection_rate(groupby=groupby,
-                                       threshold=self.params["threshold"])
+        dr = dc.metrics.detection_rate(groupby=groupby, threshold=self.params["threshold"])
         dr = dr.loc[self.params["process_classes"], :]
         lb = self.params["lb"]
         ub = self.params["ub"]
-        return get_outside_bounds_index(dr, lb, ub)
+        return ff.get_outside_bounds_index(dr, lb, ub)
 
 
 @register
 class DRatioFilter(Processor):
     r"""
     Remove Features with low biological information.
 
@@ -519,35 +545,38 @@
     .. [1] D.Broadhurst *et al*, "Guidelines and considerations for the use
         of system suitability and quality control samples in mass spectrometry
         assays applied in untargeted clinical metabolomic studies",
         Metabolomics (2018) 14:72.
 
     """
 
-    def __init__(self, lb=0, ub=0.5, robust=False,
-                 verbose=False):
+    def __init__(self, lb=0, ub=0.5, robust=False, verbose=False):
         """
         Constructor of the DRatioFilter.
         """
-        requirements = {"empty": False, "missing": False, _qc_sample_type: True,
-                        _study_sample_type: True}
-        super(DRatioFilter, self).__init__(axis="features", mode="filter",
-                                           verbose=verbose,
-                                           requirements=requirements)
+        requirements = {
+            "empty": False,
+            "missing": False,
+            c.QC_TYPE: True,
+            c.STUDY_TYPE: True,
+        }
+        super(DRatioFilter, self).__init__(
+            axis="features", mode="filter", verbose=verbose, requirements=requirements
+        )
         self.name = "D-Ratio Filter"
         self.params["lb"] = lb
         self.params["ub"] = ub
         self.params["robust"] = robust
         validation.validate_dratio_filter_params(self.params)
 
     def func(self, dc: DataContainer):
         lb = self.params["lb"]
         ub = self.params["ub"]
         dratio = dc.metrics.dratio(robust=self.params["robust"])
-        return get_outside_bounds_index(dratio, lb, ub)
+        return ff.get_outside_bounds_index(dratio, lb, ub)
 
 
 @register
 class VariationFilter(Processor):
     """
     Remove features with low reproducibility.
 
@@ -573,44 +602,46 @@
         If True, the cv is computed for each class in `process_classes` and
         then the maximum value is compared against `lb` and `ub`. Else
         a global cv is computed for all classes in `process_classes`.
     verbose: bool
         If True, prints a message
 
     """
-    def __init__(self, lb=0, ub=0.25, process_classes=None, robust=False,
-                 intraclass=True, verbose=False):
+
+    def __init__(
+        self, lb=0, ub=0.25, process_classes=None, robust=False, intraclass=True, verbose=False
+    ):
         """
         Constructor of the VariationFilter.
         """
         requirements = {"empty": False, "missing": False}
-        super(VariationFilter, self).__init__(axis="features", mode="filter",
-                                              verbose=verbose,
-                                              requirements=requirements)
+        super(VariationFilter, self).__init__(
+            axis="features", mode="filter", verbose=verbose, requirements=requirements
+        )
         self.name = "Variation Filter"
         self.params["lb"] = lb
         self.params["ub"] = ub
         self.params["process_classes"] = process_classes
         self.params["robust"] = robust
         self.params["intraclass"] = intraclass
-        self._default_process = _qc_sample_type
+        self._default_process = c.QC_TYPE
         validation.validate_variation_filter_params(self.params)
 
     def func(self, dc: DataContainer):
         lb = self.params["lb"]
         ub = self.params["ub"]
         if self.params["intraclass"]:
             groupby = "class"
         else:
             groupby = None
         variation = dc.metrics.cv(groupby=groupby, robust=self.params["robust"])
         if self.params["intraclass"]:
             variation = variation.loc[self.params["process_classes"], :]
 
-        return get_outside_bounds_index(variation, lb, ub)
+        return ff.get_outside_bounds_index(variation, lb, ub)
 
 
 @register
 class DilutionFilter(Processor):
     """
     Filter features based on the correlation with a dilution factor.
 
@@ -643,41 +674,47 @@
     ----------
     ..  [2] Lewis MR, *et al*, Development and Application of Ultra-Performance
         Liquid Chromatography-TOF MS for Precision Large Scale Urinary Metabolic
         Phenotyping. Anal Chem. (2016), 88(18):9004-13.
         doi: 10.1021/acs.analchem.6b01481
 
     """
-    def __init__(self, min_corr: float = 0.8, plim: float = 0.1,
-                 mode: str = "ols", verbose: bool = False):
+
+    def __init__(
+        self,
+        min_corr: float = 0.8,
+        plim: float = 0.1,
+        mode: str = "ols",
+        verbose: bool = False,
+    ):
         """
         Constructor of the DilutionFilter.
         """
-        requirements = {"empty": False, "missing": False, _dilution_qc_type: True}
+        requirements = {"empty": False, "missing": False, c.DQC_TYPE: True}
         super(DilutionFilter, self).__init__(
-            axis="features", mode="filter", verbose=verbose, requirements=requirements)
+            axis="features", mode="filter", verbose=verbose, requirements=requirements
+        )
         self.name = "Dilution Filter"
         self.params["min_corr"] = min_corr
         self.params["plim"] = plim
         self.params["mode"] = mode
-        self._default_process = _qc_sample_type
+        self._default_process = c.QC_TYPE
         validation.validate_dilution_filter_params(self.params)
 
     def func(self, dc: DataContainer):
         mode = self.params["mode"]
         min_corr = self.params["min_corr"]
         plim = self.params["plim"]
-        corr = dc.metrics.correlation(
-            "dilution", mode=mode, classes=dc.mapping[_dilution_qc_type])
+        corr = dc.metrics.correlation("dilution", mode=mode, classes=dc.mapping[c.DQC_TYPE])
         if mode == "ols":
-            r2_ind = get_outside_bounds_index(corr.loc["r2", :], min_corr, 1)
-            jb_ind = get_outside_bounds_index(corr.loc["JB", :], plim, 1)
+            r2_ind = ff.get_outside_bounds_index(corr.loc["r2", :], min_corr, 1)
+            jb_ind = ff.get_outside_bounds_index(corr.loc["JB", :], plim, 1)
             rm_ind = r2_ind.union(jb_ind)
         else:
-            rm_ind = get_outside_bounds_index(corr, min_corr, 1)
+            rm_ind = ff.get_outside_bounds_index(corr, min_corr, 1)
         return rm_ind
 
 
 class _TemplateValidationFilter(Processor):
     """
     Checks that process samples in each batch are surrounded by corrector
     samples. Samples that do not meet te requirements are removed.
@@ -691,58 +728,69 @@
     process_classes: list[str], optional
         list of classes used as corrector samples
     corrector_classes: list[str], optional
         list of classes used as process samples
     verbose: bool
 
     """
-    def __init__(self, process_classes: Optional[List[str]] = None,
-                 corrector_classes: Optional[List[str]] = None,
-                 verbose: bool = False):
-
-        requirements = {"empty": False, "missing": False, _sample_order: True,
-                        _sample_batch: True}
-        (super(_TemplateValidationFilter, self)
-         .__init__(axis="samples", mode="filter", verbose=verbose,
-                   requirements=requirements))
+
+    def __init__(
+        self,
+        process_classes: Optional[List[str]] = None,
+        corrector_classes: Optional[List[str]] = None,
+        verbose: bool = False,
+    ):
+
+        requirements = {
+            "empty": False,
+            "missing": False,
+            c.ORDER: True,
+            c.BATCH: True,
+        }
+        (
+            super(_TemplateValidationFilter, self).__init__(
+                axis="samples", mode="filter", verbose=verbose, requirements=requirements
+            )
+        )
         self.name = "Batch Template Check"
         self.params["corrector_classes"] = corrector_classes
         self.params["process_classes"] = process_classes
-        self._default_process = _study_sample_type
-        self._default_correct = _qc_sample_type
+        self._default_process = c.STUDY_TYPE
+        self._default_correct = c.QC_TYPE
         validation.validate_batch_corrector_params(self.params)
 
     def func(self, dc: DataContainer):
         # TODO: create a function in _filter_functions with this code
 
-        dc.sort(_sample_order, "samples")
+        dc.sort(c.ORDER, "samples")
 
-        block_type, block_number = \
-            make_sample_blocks(dc.classes, self.params["corrector_classes"],
-                               self.params["process_classes"])
+        block_type, block_number = ff.make_sample_blocks(
+            dc.classes, self.params["corrector_classes"], self.params["process_classes"]
+        )
         qc_block_mask = block_type == 0
         sample_block_mask = block_type == 1
         sample_names = block_number[sample_block_mask].index
 
         # check the minimum number of qc samples in a batch
         n_qc = dc.classes[qc_block_mask].groupby(dc.batch).count()
-        min_n_qc = 4    # the minimum number of QC samples to use LOESS
+        min_n_qc = 4  # the minimum number of QC samples to use LOESS
         valid_batch = n_qc >= min_n_qc
         valid_batch = valid_batch[valid_batch].index
         invalid_samples = ~dc.batch.isin(valid_batch)
         invalid_samples = invalid_samples[invalid_samples].index
 
         # min and max run order per batch
         min_qc_order = dc.order[qc_block_mask].groupby(dc.batch).min()
         max_qc_order = dc.order[qc_block_mask].groupby(dc.batch).max()
 
         sample_order = dc.order.loc[sample_names].groupby(dc.batch)
         for batch_number, batch_order in sample_order:
-            rm_mask = ((batch_order < min_qc_order[batch_number]) |
-                       (batch_order > max_qc_order[batch_number]))
+            rm_mask = (batch_order < min_qc_order[batch_number]) | (
+                batch_order > max_qc_order[batch_number]
+            )
             rm_sample = rm_mask[rm_mask].index
             invalid_samples = invalid_samples.union(rm_sample)
         return invalid_samples
 
 
 class _BatchCorrectorPrevalenceFilter(Processor):
     """
@@ -778,81 +826,101 @@
     process_classes: list[str], optional
         list of classes used as corrector samples
     corrector_classes: list[str], optional
         list of classes used as process samples
     verbose: bool
     """
 
-    def __init__(self, min_qc_dr: float = 0.9, verbose: bool = False,
-                 process_classes: Optional[List[str]] = None,
-                 corrector_classes: Optional[List[str]] = None,
-                 threshold: float = 0.0):
-
-        requirements = {"empty": False, "missing": False, _sample_order: True,
-                        _sample_batch: True}
-        (super(_BatchCorrectorPrevalenceFilter, self)
-         .__init__(axis="features", mode="filter", verbose=verbose,
-                   requirements=requirements))
+    def __init__(
+        self,
+        min_qc_dr: float = 0.9,
+        verbose: bool = False,
+        process_classes: Optional[List[str]] = None,
+        corrector_classes: Optional[List[str]] = None,
+        threshold: float = 0.0,
+    ):
+
+        requirements = {
+            "empty": False,
+            "missing": False,
+            c.ORDER: True,
+            c.BATCH: True,
+        }
+        (
+            super(_BatchCorrectorPrevalenceFilter, self).__init__(
+                axis="features", mode="filter", verbose=verbose, requirements=requirements
+            )
+        )
         self.name = "Batch Prevalence Checker"
         self.params["corrector_classes"] = corrector_classes
         self.params["process_classes"] = process_classes
         self.params["min_qc_dr"] = min_qc_dr
         self.params["threshold"] = threshold
-        self._default_process = _study_sample_type
-        self._default_correct = _qc_sample_type
+        self._default_process = c.STUDY_TYPE
+        self._default_correct = c.QC_TYPE
         validation.validate_batch_corrector_params(self.params)
 
     def func(self, dc: DataContainer):
         ps = self.params["process_classes"]
         ps = [x for x in ps if x not in self.params["corrector_classes"]]
         self.params["process_classes"] = ps
-        res = check_qc_prevalence(dc.data_matrix, dc.batch,
-                                  dc.classes, self.params["corrector_classes"],
-                                  self.params["process_classes"],
-                                  threshold=self.params["threshold"],
-                                  min_qc_dr=self.params["min_qc_dr"])
+        res = ff.check_qc_prevalence(
+            dc.data_matrix,
+            dc.batch,
+            dc.classes,
+            self.params["corrector_classes"],
+            self.params["process_classes"],
+            threshold=self.params["threshold"],
+            min_qc_dr=self.params["min_qc_dr"],
+        )
         return res
 
 
 class _BatchCorrectorProcessor(Processor):
     """
     Corrects instrumental drift between in a batch. Part of the batch
     corrector pipeline
     """
-    def __init__(self, corrector_classes: Optional[List[str]] = None,
-                 process_classes: Optional[List[str]] = None,
-                 frac: Optional[float] = None,
-                 interpolator: str = "splines",
-                 n_qc: Optional[int] = None,
-                 method: str = "multiplicative",
-                 process_qc: bool = True,
-                 verbose: bool = False):
-        requirements = {"empty": False, "missing": False, _sample_order: True,
-                        _sample_batch: True}
-        super(_BatchCorrectorProcessor, self).__init__(axis=None,
-                                                       mode="transform",
-                                                       verbose=verbose,
-                                                       requirements=requirements
-                                                       )
+
+    def __init__(
+        self,
+        corrector_classes: Optional[List[str]] = None,
+        process_classes: Optional[List[str]] = None,
+        frac: Optional[float] = None,
+        interpolator: str = "splines",
+        n_qc: Optional[int] = None,
+        method: str = "multiplicative",
+        process_qc: bool = True,
+        verbose: bool = False,
+    ):
+        requirements = {
+            "empty": False,
+            "missing": False,
+            c.ORDER: True,
+            c.BATCH: True,
+        }
+        super(_BatchCorrectorProcessor, self).__init__(
+            axis=None, mode="transform", verbose=verbose, requirements=requirements
+        )
         self.name = "Batch Corrector"
         self.params["corrector_classes"] = corrector_classes
         self.params["process_classes"] = process_classes
         self.params["interpolator"] = interpolator
         self.params["n_qc"] = n_qc
         self.params["frac"] = frac
         self.params["method"] = method
         self.params["process_qc"] = process_qc
-        self._default_process = _study_sample_type
-        self._default_correct = _qc_sample_type
+        self._default_process = c.STUDY_TYPE
+        self._default_correct = c.QC_TYPE
         validation.validate_batch_corrector_params(self.params)
 
     def func(self, dc: DataContainer):
-        dc.data_matrix = interbatch_correction(dc.data_matrix, dc.order,
-                                               dc.batch, dc.classes,
-                                               **self.params)
+        dc.data_matrix = ff.interbatch_correction(
+            dc.data_matrix, dc.order, dc.batch, dc.classes, **self.params
+        )
 
 
 @register
 class BatchCorrector(Pipeline):
     r"""
     Correct time dependant systematic bias along samples due to variation in
     instrumental response.
@@ -893,16 +961,16 @@
     value :math:`m_{jk}`, a systematic bias :math:`f_{k}` and error term
     :math:`\epsilon`:
 
     .. math::
        m_{jk} = \bar{m_{k}} + f_{k}(t_{j}) + \epsilon
 
     Where :math:`m_{jk}` is the element in the j-th row and k-th column of the
-    data matrix. 
-    
+    data matrix.
+
     First, :math:`\bar{m_{k}}` is subtracted to the detected values and then
     :math:`f_{k}` is estimated using Locally weighted scatter plot smoothing
     (LOESS). The optimal fraction of samples for each feature is obtained using
     Leave One Out Cross Validation (LOOCV).
 
     In order to apply this correction, several checks needs to be made. First,
     the QC template is checked and samples that cannot be corrected are removed.
@@ -963,91 +1031,107 @@
     ----------
     .. [1] D Broadhurst *et al*, "Guidelines and considerations for the use of
         system suitability and quality control samples in mass spectrometry
         assays applied in untargeted clinical metabolomic studies.",
         Metabolomics, 2018;14(6):72. doi: 10.1007/s11306-018-1367-3
 
     """
-    def __init__(self,
-                 min_qc_dr: float = 0.9,
-                 first_n_qc: Optional[int] = None,
-                 threshold: float = 0, frac: Optional[float] = None,
-                 interpolator: str = "splines",
-                 method: str = "multiplicative",
-                 corrector_classes: Optional[List[str]] = None,
-                 process_classes: Optional[List[str]] = None,
-                 verbose: bool = False):
-
-        deprecation_msg = \
-            "{} is deprecated and is going to be removed in a future release. " \
-            "To perform batch correction use the method " \
+
+    def __init__(
+        self,
+        min_qc_dr: float = 0.9,
+        first_n_qc: Optional[int] = None,
+        threshold: float = 0,
+        frac: Optional[float] = None,
+        interpolator: str = "splines",
+        method: str = "multiplicative",
+        corrector_classes: Optional[List[str]] = None,
+        process_classes: Optional[List[str]] = None,
+        verbose: bool = False,
+    ):
+
+        deprecation_msg = (
+            "{} is deprecated and is going to be removed in a future release. "
+            "To perform batch correction use the method "
             " `preprocess.correct_batches` from DataContainer"
-        warn(deprecation_msg.format(self.__class__), DeprecationWarning,
-             stacklevel=2)
+        )
+        warn(deprecation_msg.format(self.__class__), DeprecationWarning, stacklevel=2)
 
-        checker = \
-            _TemplateValidationFilter(process_classes=process_classes,
-                                      corrector_classes=corrector_classes,
-                                      verbose=verbose)
-        prevalence = \
-            _BatchCorrectorPrevalenceFilter(min_qc_dr=min_qc_dr,
-                                            verbose=verbose,
-                                            process_classes=process_classes,
-                                            corrector_classes=corrector_classes,
-                                            threshold=threshold)
-        corrector = \
-            _BatchCorrectorProcessor(corrector_classes=corrector_classes,
-                                     process_classes=process_classes, frac=frac,
-                                     interpolator=interpolator, verbose=verbose,
-                                     n_qc=first_n_qc, method=method)
+        checker = _TemplateValidationFilter(
+            process_classes=process_classes,
+            corrector_classes=corrector_classes,
+            verbose=verbose,
+        )
+        prevalence = _BatchCorrectorPrevalenceFilter(
+            min_qc_dr=min_qc_dr,
+            verbose=verbose,
+            process_classes=process_classes,
+            corrector_classes=corrector_classes,
+            threshold=threshold,
+        )
+        corrector = _BatchCorrectorProcessor(
+            corrector_classes=corrector_classes,
+            process_classes=process_classes,
+            frac=frac,
+            interpolator=interpolator,
+            verbose=verbose,
+            n_qc=first_n_qc,
+            method=method,
+        )
         pipeline = [checker, prevalence, corrector]
         super(BatchCorrector, self).__init__(pipeline, verbose=verbose)
         self.name = "Batch Corrector"
 
 
 def pipeline_from_list(param_list: list, verbose=False):
     processors = list()
     for d in param_list:
         processors.append(filter_from_dictionary(d))
     pipeline = Pipeline(processors, verbose)
     return pipeline
 
 
 def filter_from_dictionary(d):
-    filt = None
+    filter = None
     for name, params in d.items():
-        filt = FILTERS[name](**params)
-    return filt
+        filter = FILTERS[name](**params)
+    return filter
 
 
 def sample_name_from_path(path):
     file_name = os.path.split(path)[1]
     sample_name = os.path.splitext(file_name)[0]
     return sample_name
 
 
 def _validate_pipeline(t):
     if not isinstance(t, (list, tuple)):
         t = [t]
-    for filt in t:
-        if not isinstance(filt, (Processor, Pipeline)):
-            msg = ("elements of the Pipeline must be",
-                   "instances of Filter, DataCorrector or another Pipeline.")
+    for filter in t:
+        if not isinstance(filter, (Processor, Pipeline)):
+            msg = (
+                "elements of the Pipeline must be",
+                "instances of Filter, DataCorrector or another Pipeline.",
+            )
             raise TypeError(msg)
 
 
 class MissingMappingInformation(ValueError):
     """error raised when an empty sample type is used from a mapping"""
+
     pass
 
 
 class MissingValueError(ValueError):
     """error raise when a DataContainer's data matrix has missing values"""
+
     pass
 
 
-_requirements_error = {"empty": container.EmptyDataContainerError,
-                       "missing": MissingValueError,
-                       _qc_sample_type: MissingMappingInformation,
-                       _blank_sample_type: MissingMappingInformation,
-                       _sample_batch: container.BatchInformationError,
-                       _sample_order: container.RunOrderError}
+_requirements_error = {
+    "empty": container.EmptyDataContainerError,
+    "missing": MissingValueError,
+    c.QC_TYPE: MissingMappingInformation,
+    c.BLANK_TYPE: MissingMappingInformation,
+    c.BATCH: container.BatchInformationError,
+    c.ORDER: container.RunOrderError,
+}
```

### Comparing `tidyms-0.6.3/src/tidyms/peaks.py` & `tidyms-0.7.0/src/tidyms/peaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
     start, end = _find_peak_extension(peaks, baseline_index)
     start, end = _fix_peak_overlap(spint, start, peaks, end)
     start, peaks, end = _normalize_peaks(spint, start, peaks, end)
 
     # peak centroid and total intensity computation
     # if m[0], ...,  m[n] is the m/z array and i[0], ..., i[n] is the
-    # intensity array, for a peak with start and indices k and l respectively,
+    # intensity array, for a peak with start and end indices k and l respectively,
     # the total intensity A is A = \sum_{j=k}^{l} i[j] and the centroid C,
     # computed as the weighted mean of the m/z is
     # C = \sum_{j=k}^{l} m[j] * i[j] / A
     # If we define the cumulative intensity I_{k} = \sum_{j=0}^{k} i[j]
     # It is easy to see that A = I[l - 1] - I[k - 1]. The same can be done
     # for the centroids defining the weights W[k] = \sum_{j=0}^{k} m[j] * i[j]
     # C = (W[l - 1] - W[k - 1]) / A
@@ -243,15 +243,15 @@
             # prevents using the last value from cumulative_spint
             start_cumulative_spint[0] = 0
         total_spint = cumulative_spint[end - 1] - start_cumulative_spint
 
         start_weight = weights[start - 1]
         if start[0] == 0:
             start_weight[0] = 0
-        centroid = (weights[end] - start_weight) / total_spint
+        centroid = (weights[end - 1] - start_weight) / total_spint
     else:
         centroid = np.array([])
         total_spint = np.array([])
 
     if centroid.size:
         _merge_close_peaks(centroid, total_spint, min_distance)
     return centroid, total_spint
@@ -623,14 +623,16 @@
     else:
         baseline_index = np.array([0, x.size - 1], dtype=int)
     return baseline_index
 
 
 def _merge_close_peaks(mz: np.ndarray, spint: np.ndarray,
                        min_distance: float) -> Tuple[np.ndarray, np.ndarray]:
+    if mz.shape[0] < 2:
+        return mz, spint
     dmz = np.diff(mz)
     is_close_mask = (dmz < min_distance) & (np.roll(dmz, -1) > min_distance)
     is_close_mask[-1] = (mz[-1] - mz[-2]) < min_distance    # boundary case
     close_index = np.where(is_close_mask)[0]
     while close_index.size > 0:
         # merge close centroids
         new_spint = spint[close_index] + spint[close_index + 1]
```

### Comparing `tidyms-0.6.3/src/tidyms/raw_data_utils.py` & `tidyms-0.7.0/src/tidyms/raw_data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Functions used to extract information from raw data.
 
 """
 
 import numpy as np
-from .lcms import Chromatogram, LCRoi, MSSpectrum, Roi
-from .fileio import MSData
+import os
+import pandas as pd
+from .lcms import Chromatogram, LCTrace, MSSpectrum, Roi
+from .fileio import MSData, MSData_subset_spectra
 from .utils import find_closest
 from . import _constants as c
 from . import validation as val
 from collections import deque
 from copy import deepcopy
 from scipy.interpolate import interp1d
 from typing import Callable, List, Optional, Tuple, Union
@@ -57,19 +59,15 @@
     rt = np.zeros(n_scan)
     tic = np.zeros(n_scan)
     valid_index = list()
     # it is not possible to know a priori how many scans of each level are
     # available in a given file without iterating over it. valid_index holds
     # the index related to the selected level and is used to remove scans
     # from other levels.
-    sp_iterator = ms_data.get_spectra_iterator(
-        ms_level=ms_level,
-        start_time=start_time,
-        end_time=end_time
-    )
+    sp_iterator = ms_data.get_spectra_iterator(ms_level=ms_level, start_time=start_time, end_time=end_time)
     for scan, sp in sp_iterator:
         valid_index.append(scan)
         rt[scan] = sp.time
         if sp.spint.size:
             tic[scan] = reduce(sp.spint)
         else:
             tic[scan] = 0
@@ -121,28 +119,23 @@
     -------
     chromatograms : List of Chromatograms
 
     """
     n_sp = ms_data.get_n_spectra()
 
     # mz_intervals has this shape to be compatible with reduce at
-    mz_intervals = (np.vstack((mz - window, mz + window))
-                    .T.reshape(mz.size * 2))
+    mz_intervals = np.vstack((mz - window, mz + window)).T.reshape(mz.size * 2)
 
     eic = np.zeros((mz.size, n_sp))
     if not fill_missing:
         eic[:] = np.nan
 
     rt = np.zeros(n_sp)
     valid_index = list()
-    sp_iterator = ms_data.get_spectra_iterator(
-        ms_level=ms_level,
-        start_time=start_time,
-        end_time=end_time
-    )
+    sp_iterator = ms_data.get_spectra_iterator(ms_level=ms_level, start_time=start_time, end_time=end_time)
     for scan, sp in sp_iterator:
         valid_index.append(scan)
         rt[scan] = sp.time
         sp_size = sp.mz.size
 
         # prevents error when working with empty spectra
         if sp_size == 0:
@@ -150,16 +143,15 @@
 
         # values for each eic in the current scan
         ind_sp = np.searchsorted(sp.mz, mz_intervals)  # slices for each eic
         has_mz = (ind_sp[1::2] - ind_sp[::2]) > 0  # find non-empty slices
         # elements added at the end of mz_sp raise IndexError
         ind_sp[ind_sp >= sp_size] = sp_size - 1
         # this adds the values between two consecutive indices
-        tmp_eic = np.where(
-            has_mz, np.add.reduceat(sp.spint, ind_sp)[::2], 0)
+        tmp_eic = np.where(has_mz, np.add.reduceat(sp.spint, ind_sp)[::2], 0)
         if accumulator == "mean":
             norm = ind_sp[1::2] - ind_sp[::2]
             norm[norm == 0] = 1
             tmp_eic = tmp_eic / norm
         eic[:, scan] = tmp_eic
     valid_index = np.array(valid_index)
     rt = rt[valid_index]
@@ -185,15 +177,15 @@
     sp_reduce: Union[str, Callable] = "sum",
     targeted_mz: Optional[np.ndarray] = None,
     pad: Optional[int] = None,
     ms_level: int = 1,
     start_time: float = 0.0,
     end_time: Optional[float] = None,
     min_snr: float = 10,
-    min_distance: Optional[float] = None
+    min_distance: Optional[float] = None,
 ) -> List[Roi]:
     """
     Builds regions of interest (ROI) from raw data.
 
     ROI are created by connecting values across scans based on the closeness in
     m/z. See the :ref:`user guide <roi-creation>` for a description of the
     algorithm used.
@@ -274,16 +266,15 @@
 
     """
 
     if targeted_mz is None:
         if min_intensity is None:
             mz_filter = None
         else:
-            mz_filter = _make_mz_filter(
-                ms_data, min_intensity, ms_level, start_time, end_time)
+            mz_filter = _make_mz_filter(ms_data, min_intensity, ms_level, start_time, end_time)
         targeted = False
     else:
         mz_filter = np.sort(targeted_mz)
         targeted = True
 
     if mz_reduce == "mean":
         mz_reduce = np.mean
@@ -297,47 +288,48 @@
         max_missing=max_missing,
         min_length=min_length,
         min_intensity=min_intensity,
         tolerance=tolerance,
         multiple_match=multiple_match,
         mz_reduce=mz_reduce,
         sp_reduce=sp_reduce,
-        targeted=targeted
+        targeted=targeted,
     )
 
     scans = list()
-    sp_iterator = ms_data.get_spectra_iterator(
-        ms_level=ms_level,
-        start_time=start_time,
-        end_time=end_time
-    )
+    sp_iterator = ms_data.get_spectra_iterator(ms_level=ms_level, start_time=start_time, end_time=end_time)
     for scan, spectrum in sp_iterator:
         rt[scan] = spectrum.time
         scans.append(scan)
         mz, sp = spectrum.find_centroids(min_snr, min_distance)
         processor.feed_spectrum(mz, sp, scan)
         processor.clear_completed_roi()
 
     # add roi not completed during the last scan
     processor.flag_as_completed()
     processor.clear_completed_roi()
     scans = np.array(scans)
     roi_list = processor.tmp_roi_to_roi(scans, rt, pad, ms_data.separation)
+
+    # TODO: workaround, move code to _RoiMaker
+    for k, roi in enumerate(roi_list):
+        roi.index = k
+
     return roi_list
 
 
 @val.validate_raw_data_utils(val.accumulate_spectra_schema)
 def accumulate_spectra(
     ms_data: MSData,
     *,
     start_time: float,
     end_time: float,
     subtract_left_time: Optional[float] = None,
     subtract_right_time: Optional[float] = None,
-    ms_level: int = 1
+    ms_level: int = 1,
 ) -> MSSpectrum:
     """
     accumulates a series of consecutive spectra into a single spectrum.
 
     Parameters
     ----------
     ms_data : MSData
@@ -362,35 +354,35 @@
     if ms_data.ms_mode == "centroid":
         sp = _accumulate_spectra_centroid(
             ms_data,
             start_time,
             end_time,
             subtract_left_time,
             subtract_right_time,
-            ms_level
+            ms_level,
         )
-    else:   # profile
+    else:  # profile
         sp = _accumulate_spectra_profile(
             ms_data,
             start_time,
             end_time,
             subtract_left_time,
             subtract_right_time,
-            ms_level
+            ms_level,
         )
     return sp
 
 
 def _accumulate_spectra_centroid(
     ms_data: MSData,
     start_time: float,
     end_time: float,
     subtract_left_time: float,
     subtract_right_time: float,
-    ms_level: int
+    ms_level: int,
 ) -> MSSpectrum:
     """
     accumulates a series of consecutive spectra into a single spectrum.
 
     auxiliary function for accumulate_spectra.
 
     """
@@ -399,23 +391,23 @@
 
     roi = make_roi(
         ms_data,
         max_missing=max_missing,
         min_length=1,
         start_time=subtract_left_time,
         end_time=subtract_right_time,
-        ms_level=ms_level
+        ms_level=ms_level,
     )
 
     mz = np.zeros(len(roi))
     spint = mz.copy()
 
     # set subtract values to negative
     for k, r in enumerate(roi):
-        sign = - np.ones(r.time.size)
+        sign = -np.ones(r.time.size)
         start_index, end_index = np.searchsorted(r.time, [start_time, end_time])
         sign[start_index:end_index] = 1
         mz[k] = np.nanmean(r.mz)
         spint[k] = np.nansum(r.spint * sign)
 
     # remove negative values
     pos_values = spint > 0
@@ -433,15 +425,15 @@
 
 def _accumulate_spectra_profile(
     ms_data: MSData,
     start_time: float,
     end_time: float,
     subtract_left_time: float,
     subtract_right_time: float,
-    ms_level: int
+    ms_level: int,
 ) -> MSSpectrum:
     """
     aux function for accumulate_spectra.
 
     """
     # The spectra are accumulated in two steps:
     #
@@ -452,35 +444,27 @@
     #
     #  This process is done in two steps to avoid storing the intensity
     #  values from each scan until the grid is built.
 
     accumulated_mz = None
     # m/z tol. A small value is used to prevent distortions in the results
     tol = 0.00005
-    sp_iter = ms_data.get_spectra_iterator(
-        ms_level,
-        start_time=subtract_left_time,
-        end_time=subtract_right_time
-    )
+    sp_iter = ms_data.get_spectra_iterator(ms_level, start_time=subtract_left_time, end_time=subtract_right_time)
     # first iteration. Builds a grid of m/z values for the accumulated
     # spectrum. The grid is extended using new m/z values that appear
     # in each new scan
     for scan, sp in sp_iter:
         if accumulated_mz is None:
             accumulated_mz = sp.mz
         ind = find_closest(accumulated_mz, sp.mz)
         no_match = np.abs(accumulated_mz[ind] - sp.mz) > tol
         accumulated_mz = np.sort(np.hstack((accumulated_mz, sp.mz[no_match])))
 
     accumulated_sp = np.zeros_like(accumulated_mz)
-    sp_iter = ms_data.get_spectra_iterator(
-        ms_level,
-        start_time=subtract_left_time,
-        end_time=subtract_right_time
-    )
+    sp_iter = ms_data.get_spectra_iterator(ms_level, start_time=subtract_left_time, end_time=subtract_right_time)
 
     for _, sp in sp_iter:
         interpolator = interp1d(sp.mz, sp.spint, fill_value=0.0)
         if (sp.time < start_time) or (sp.time > end_time):
             sign = -1
         else:
             sign = 1
@@ -492,15 +476,15 @@
     accumulated_sp = accumulated_sp[is_positive_sp]
 
     res = MSSpectrum(
         accumulated_mz,
         accumulated_sp,
         instrument=ms_data.instrument,
         ms_level=ms_level,
-        is_centroid=False
+        is_centroid=False,
     )
     return res
 
 
 class _RoiMaker:
     """
     Creates and extends ROIs using spectrum data.
@@ -555,15 +539,15 @@
         max_missing: int,
         min_length: Optional[int],
         min_intensity: Optional[float],
         tolerance: float,
         multiple_match: str,
         mz_reduce: Optional[Callable],
         sp_reduce: Optional[Callable],
-        targeted: bool = False
+        targeted: bool = False,
     ):
         self.tmp_roi_list = _TempRoiList(update_mean=not targeted)
         self.valid_roi = deque()
         self.mz_filter = mz_filter
         self.max_missing = max_missing
         self.min_intensity = min_intensity
         self.min_length = min_length
@@ -596,15 +580,15 @@
             match_ind, match_mz, match_sp, no_match_mz, no_match_sp = _match_mz(
                 self.tmp_roi_list.mz_mean,
                 mz,
                 sp,
                 self.tolerance,
                 self.multiple_match,
                 self.mz_reduce,
-                self.sp_reduce
+                self.sp_reduce,
             )
             self.tmp_roi_list.extend(match_mz, match_sp, scan, match_ind)
             if not self.targeted:
                 self.tmp_roi_list.insert(no_match_mz, no_match_sp, scan)
         else:
             if not self.targeted:
                 self.tmp_roi_list.insert(mz, sp, scan)
@@ -614,18 +598,15 @@
         Flags ROI as completed. Completed valid ROIs are stored  in the `roi`
         attribute. Invalid ROIs are cleared.
 
         """
         finished_mask = self.tmp_roi_list.missing_count > self.max_missing
         finished_roi_index = np.where(finished_mask)[0]
         if self.min_intensity is not None:
-            valid_mask = (
-                finished_mask &
-                (self.tmp_roi_list.max_int >= self.min_intensity)
-            )
+            valid_mask = finished_mask & (self.tmp_roi_list.max_int >= self.min_intensity)
         else:
             valid_mask = finished_mask
 
         if self.min_length is not None:
             valid_mask &= self.tmp_roi_list.length >= self.min_length
 
         valid_index = np.where(valid_mask)[0]
@@ -639,35 +620,29 @@
     def flag_as_completed(self):
         """
         Mark all ROis as completed.
 
         """
         self.tmp_roi_list.missing_count[:] = self.max_missing + 1
 
-    def tmp_roi_to_roi(
-        self,
-        valid_scan: np.ndarray,
-        time: np.ndarray,
-        pad: int,
-        separation: str
-    ) -> List[Roi]:
+    def tmp_roi_to_roi(self, valid_scan: np.ndarray, time: np.ndarray, pad: int, separation: str) -> List[Roi]:
         """
         Converts completed valid _TempRoi objects into Roi.
 
         Parameters
         ----------
         valid_scan : array
             scan values used to build the ROIs.
         time : array
             acquisition time of each scan.
         pad : int
             Number of dummy values to pad each ROI.
         separation : str
             Separation method of the ms file. Used to create LCRoi objects or
-            Roi objects. 
+            Roi objects.
 
         Returns
         -------
         valid_roi: List[Roi]
         """
         valid_roi = list()
         while self.valid_roi:
@@ -702,16 +677,16 @@
     update_mean : bool
         If ``True``, the mean of each ROI is updated after a new element is
         appended. Else, the mean when the ROI was created is used.
 
     """
 
     def __init__(self, update_mean: bool = True):
-        self.roi = list()     # type: List[_TempRoi]
-        self.mz_mean = np.array([])   # type: np.ndarray
+        self.roi = list()  # type: List[_TempRoi]
+        self.mz_mean = np.array([])  # type: np.ndarray
         self.mz_sum = np.array([])
         self.max_int = np.array([])
         self.missing_count = np.array([], dtype=int)
         self.length = np.array([], dtype=int)
         self.update_mean = update_mean
 
     def insert(self, mz: np.ndarray, sp: np.ndarray, scan: int):
@@ -729,33 +704,25 @@
 
         """
         index = np.searchsorted(self.mz_mean, mz)
         # update roi tracking values
         self.mz_mean = np.insert(self.mz_mean, index, mz)
         self.mz_sum = np.insert(self.mz_sum, index, mz)
         self.max_int = np.insert(self.max_int, index, sp)
-        self.missing_count = np.insert(
-            self.missing_count, index, np.zeros_like(index)
-        )
+        self.missing_count = np.insert(self.missing_count, index, np.zeros_like(index))
         self.length = np.insert(self.length, index, np.ones_like(index))
 
         # insert new roi
         new_roi = _create_roi_list(mz, sp, scan)
         offset = 0
         for i, roi in zip(index, new_roi):
             self.roi.insert(i + offset, roi)
             offset += 1
 
-    def extend(
-        self,
-        mz: np.ndarray,
-        sp: np.ndarray,
-        scan: int,
-        index: np.ndarray
-    ):
+    def extend(self, mz: np.ndarray, sp: np.ndarray, scan: int, index: np.ndarray):
         """
         Extends existing ROI.
 
         Parameters
         ----------
         mz : array
             m/z values used to extend the ROI
@@ -885,20 +852,15 @@
         self.scan.extendleft(valid_scan[left_pad_index:start][::-1])
 
         # right pad
         self.mz.extend([np.nan] * n_right)
         self.spint.extend([np.nan] * n_right)
         self.scan.extend(valid_scan[end:right_pad_index])
 
-    def convert_to_roi(
-        self,
-        rt: np.ndarray,
-        scans: np.ndarray,
-        separation: str
-    ) -> Roi:
+    def convert_to_roi(self, rt: np.ndarray, scans: np.ndarray, separation: str) -> Roi:
         """
         Converts a TemporaryRoi into a ROI object
 
         Parameters
         ----------
         rt: array
             Acquisition times of each scan
@@ -922,37 +884,36 @@
         # copy values from the ROI to the new arrays
         scan_index = np.array(self.scan) - self.scan[0]
         mz_tmp[scan_index] = self.mz
         spint_tmp[scan_index] = self.spint
 
         # remove scan numbers from other ms levels (i.e. scan numbers that are
         # not in the scans array)
-        start_ind, end_ind = np.searchsorted(
-            scans, [first_scan, last_scan + 1]
-        )
+        start_ind, end_ind = np.searchsorted(scans, [first_scan, last_scan + 1])
         scan_tmp = scans[start_ind:end_ind].copy()
         valid_index = scan_tmp - first_scan
         mz_tmp = mz_tmp[valid_index]
         spint_tmp = spint_tmp[valid_index]
         rt_tmp = rt[scan_tmp].copy()
 
         # Create ROI objects
         if separation in c.LC_MODES:
-            roi = LCRoi(spint_tmp, mz_tmp, rt_tmp, scan_tmp, mode=separation)
+            roi = LCTrace(rt_tmp, spint_tmp, mz_tmp, scan_tmp, mode=separation)
         else:
-            roi = Roi(spint_tmp, mz_tmp, rt_tmp, scan_tmp, mode=separation)
+            raise NotImplementedError
+            # roi = Roi(spint_tmp, mz_tmp, rt_tmp, scan_tmp, mode=separation)
         return roi
 
 
 def _make_mz_filter(
     ms_data: MSData,
     min_intensity: float,
     ms_level: int,
     start_time: float,
-    end_time: float
+    end_time: float,
 ):
     """
     Creates a list of m/z values to initialize ROI for untargeted feature
     detection based on the intensity observed for each m/z value across scans.
 
     Auxiliary function to make_roi.
 
@@ -968,41 +929,32 @@
     end_time : float or None, default=None
         Ignore scans with acquisition times higher than this value.
 
     Returns
     -------
 
     """
-    iterator = ms_data.get_spectra_iterator(
-        ms_level=ms_level,
-        start_time=start_time,
-        end_time=end_time
-    )
+    iterator = ms_data.get_spectra_iterator(ms_level=ms_level, start_time=start_time, end_time=end_time)
     mz_seed = [sp.mz[sp.spint > min_intensity] for _, sp in iterator]
     return np.unique(np.hstack(mz_seed))
 
 
-def _filter_invalid_mz(
-    valid_mz: np.ndarray,
-    mz: np.ndarray,
-    sp: np.ndarray,
-    tolerance: float
-) -> Tuple[np.ndarray, np.ndarray]:
+def _filter_invalid_mz(valid_mz: np.ndarray, mz: np.ndarray, sp: np.ndarray, tolerance: float) -> Tuple[np.ndarray, np.ndarray]:
     """
     Find values in the spectrum that are within tolerance with the m/z values
     in the seed.
 
     Auxiliary function to _RoiProcessor.extend
 
     Parameters
     ----------
     valid_mz : np.ndarray
         sorted array of m/z values.
     mz: array
-        m/z values to filter
+        m/z values to filter.
     sp : array
         intensity values associated to each m/z.
     tolerance : float
 
     Returns
     -------
     mz : np.ndarray
@@ -1010,23 +962,69 @@
     spint : np.ndarray
         Filtered intensity values in the spectrum
 
     """
 
     closest_index = find_closest(valid_mz, mz)
     dmz = np.abs(valid_mz[closest_index] - mz)
-    match_mask = (dmz <= tolerance)  # type: np.ndarray
+    match_mask = dmz <= tolerance  # type: np.ndarray
     return mz[match_mask], sp[match_mask]
 
 
-def _create_roi_list(
-    mz: np.ndarray,
-    sp: np.ndarray,
-    scan: int
-) -> List[_TempRoi]:
+def _filter_zero_intensity_signals(mz: np.ndarray, sp: np.ndarray, minimum_intensity: float = 0) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Removes any peak with an intensity below or equal to the set threshold (default 0).
+
+    Parameters
+    ----------
+    mz : np.ndarray
+        array of m/z values.
+    sp : array
+        intensity values associated to each m/z.
+    minimum_intensity : float
+        any peak with an intensity equal or below this value will be removed
+
+    Returns
+    -------
+    mz : np.ndarray
+        Filtered m/z values in the spectrum.
+    sp : np.ndarray
+        Filtered intensity values in the spectrum.
+    """
+
+    match_mask = sp > minimum_intensity
+    return mz[match_mask], sp[match_mask]
+
+
+def _get_profile_mode_mz_deltas(mz: np.ndarray, convert_to_ppm: bool = True) -> np.ndarray:
+    """_get_profile_mode_mz_deltas
+
+    Args:
+        mz (np.ndarray): sorted array of m/z values.
+
+    Returns:
+        np.ndarray:
+    """
+    diffs = np.diff(mz)
+    if convert_to_ppm:
+        diffs = diffs / mz[0 : (mz.shape[0] - 1)] * 1e6
+    return (
+        np.mean(diffs),
+        np.std(diffs),
+        np.quantile(diffs, 0.01),
+        np.quantile(diffs, 0.10),
+        np.quantile(diffs, 0.25),
+        np.quantile(diffs, 0.50),
+        np.quantile(diffs, 0.75),
+        np.quantile(diffs, 0.90),
+        np.quantile(diffs, 0.99),
+    )
+
+
+def _create_roi_list(mz: np.ndarray, sp: np.ndarray, scan: int) -> List[_TempRoi]:
     roi_list = list()
     for m, s in zip(mz, sp):
         roi = _TempRoi()
         roi.append(m, s, scan)
         roi_list.append(roi)
     return roi_list
 
@@ -1034,15 +1032,15 @@
 def _match_mz(
     mz1: np.ndarray,
     mz2: np.ndarray,
     sp2: np.ndarray,
     tolerance: float,
     mode: str,
     mz_reduce: Callable,
-    sp_reduce: Callable
+    sp_reduce: Callable,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
     """
     aux function to add method in _RoiProcessor. Find matched values.
 
     Parameters
     ----------
     mz1: numpy.ndarray
@@ -1069,24 +1067,20 @@
     sp_match: numpy.ndarray
         values of sp2 that matches with mz1
     mz_no_match: numpy.ndarray
     sp_no_match: numpy.ndarray
     """
     closest_index = find_closest(mz1, mz2)
     dmz = np.abs(mz1[closest_index] - mz2)
-    match_mask = (dmz <= tolerance)     # type: np.ndarray
+    match_mask = dmz <= tolerance  # type: np.ndarray
     no_match_mask = ~match_mask
     match_index = closest_index[match_mask]
 
     # check multiple_matches
-    match_unique, match_first, match_count = np.unique(
-        match_index,
-        return_counts=True,
-        return_index=True
-    )
+    match_unique, match_first, match_count = np.unique(match_index, return_counts=True, return_index=True)
 
     # set match values
     match_index = match_unique
     sp_match = sp2[match_mask]
     mz_match = mz2[match_mask]
 
     # solve multiple matches
@@ -1094,30 +1088,26 @@
     multiple_match_first = match_first[multiple_match_mask]
     if match_first.size > 0:
         multiple_match_count = match_count[multiple_match_mask]
         if mode == "reduce":
             for first, count in zip(multiple_match_first, multiple_match_count):
                 # mz1 and mz2 are both sorted, the multiple matches are
                 # consecutive
-                mz_multiple_match = mz_match[first:(first + count)]
-                sp_multiple_match = sp_match[first:(first + count)]
+                mz_multiple_match = mz_match[first : (first + count)]
+                sp_multiple_match = sp_match[first : (first + count)]
                 mz_match[first] = mz_reduce(mz_multiple_match)
                 sp_match[first] = sp_reduce(sp_multiple_match)
         elif mode == "closest":
             match_index_mz = np.where(match_mask)[0][match_first]
             multiple_match_index_mz = match_index_mz[multiple_match_mask]
-            iterator = zip(
-                multiple_match_index_mz,
-                multiple_match_first,
-                multiple_match_count
-            )
+            iterator = zip(multiple_match_index_mz, multiple_match_first, multiple_match_count)
             for mz2_index, first, count in iterator:
-                closest = np.argmin(dmz[mz2_index: mz2_index + count])
+                closest = np.argmin(dmz[mz2_index : mz2_index + count])
                 # flag all multiple matches as no match except the closest one
-                no_match_mask[mz2_index: mz2_index + count] = True
+                no_match_mask[mz2_index : mz2_index + count] = True
                 no_match_mask[mz2_index + closest] = False
                 mz_match[first] = mz_match[first + closest]
                 sp_match[first] = sp_match[first + closest]
         else:
             msg = "mode must be `closest` or `merge`"
             raise ValueError(msg)
```

### Comparing `tidyms-0.6.3/src/tidyms/simulation.py` & `tidyms-0.7.0/src/tidyms/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import numpy as np
 import pandas as pd
-from typing import List, Optional
+from . import _constants as c
+from typing import Optional
 from .container import DataContainer
 
 
-def simulate_dataset(population: dict, mean_dict: dict, cov_dict: dict,
-                     feature_mz: np.ndarray, feature_rt: np.ndarray,
-                     blank_contribution: Optional[np.ndarray] = None,
-                     noise_dict: Optional[dict] = None,
-                     qc_template: bool = True, qc_bracket_size: int = 5,
-                     triple_qc: bool = True, prepend_blank: int = 0,
-                     append_blank: int = 0, batch_size: int = 25
-                     ) -> DataContainer:
+def simulate_dataset(
+    population: dict,
+    mean_dict: dict,
+    cov_dict: dict,
+    feature_mz: np.ndarray,
+    feature_rt: np.ndarray,
+    blank_contribution: Optional[np.ndarray] = None,
+    noise_dict: Optional[dict] = None,
+    qc_template: bool = True,
+    qc_bracket_size: int = 5,
+    triple_qc: bool = True,
+    prepend_blank: int = 0,
+    append_blank: int = 0,
+    batch_size: int = 25,
+) -> DataContainer:
     """
     Creates DataContainer with simulated data
 
     Parameters
     ----------
     population: dict[str, int]
         A dictionary where the keys are the available classes in
@@ -54,34 +62,45 @@
 
     Returns
     -------
     DataContainer
 
     """
 
-    sm = _make_sample_list(population, qc_template, qc_bracket_size,
-                           triple_qc, prepend_blank, append_blank, batch_size)
-    dm = _make_data_matrix(population, sm, mean_dict, cov_dict,
-                           blank_contribution, noise_dict)
+    sm = _make_sample_list(
+        population,
+        qc_template,
+        qc_bracket_size,
+        triple_qc,
+        prepend_blank,
+        append_blank,
+        batch_size,
+    )
+    dm = _make_data_matrix(population, sm, mean_dict, cov_dict, blank_contribution, noise_dict)
     fm = np.vstack((feature_mz, feature_rt)).T
     fm = pd.DataFrame(data=fm, columns=["mz", "rt"], index=dm.columns)
     mapping = {"sample": list(population)}
     if qc_template:
         mapping["qc"] = ["QC"]
     if max(prepend_blank, append_blank) > 0:
         mapping["blank"] = ["blank"]
     return DataContainer(dm, fm, sm, mapping)
 
 
-def _make_sample_list(population: dict, qc_template: bool = True,
-                      qc_bracket_size: int = 5, triple_qc: bool = True,
-                      prepend_blank: int = 0, append_blank: int = 0,
-                      batch_size: int = 25):
+def _make_sample_list(
+    population: dict,
+    qc_template: bool = True,
+    qc_bracket_size: int = 5,
+    triple_qc: bool = True,
+    prepend_blank: int = 0,
+    append_blank: int = 0,
+    batch_size: int = 25,
+):
     """
-    creates a simulated sample list for an untargeted metabolomic assay.
+    creates a simulated sample list for an untargeted metabolomics assay.
 
     Parameters
     ----------
     population: dict[str, int]
         A dictionary where the keys are the available classes in
         the experiment and the values are the number of samples
         from each class.
@@ -114,33 +133,38 @@
         prepend_blank = prepend_blank + ["QC"] * n_append
         append_blank = ["QC"] * n_append + append_blank
     else:
         # setting this bracket size will avoid including QC samples
         qc_bracket_size = n_study_samples + 1
 
     # randomize classes and make QC brackets
-    classes = _make_sample_classes(population, batch_size,
-                                   qc_bracket_size, prepend_blank, append_blank)
+    classes = _make_sample_classes(
+        population, batch_size, qc_bracket_size, prepend_blank, append_blank
+    )
     n_prepend = len(prepend_blank)
     n_append = len(append_blank)
-    batch_number = _make_batch_number(batch_size, n_study_samples, n_prepend,
-                                      n_append, qc_bracket_size)
+    batch_number = _make_batch_number(
+        batch_size, n_study_samples, n_prepend, n_append, qc_bracket_size
+    )
     order = list(range(1, len(batch_number) + 1))
     sample_name = _make_sample_name(len(batch_number))
-    sample_list = {"id": sample_name, "class": classes, "order": order,
-                   "batch": batch_number}
+    sample_list = {c.ID: sample_name, c.CLASS: classes, c.ORDER: order, c.BATCH: batch_number}
     sample_list = pd.DataFrame(data=sample_list, index=sample_name)
-    sample_list.index.name = "samples"
+    sample_list.index.name = c.SAMPLE
     return sample_list
 
 
-def _make_data_matrix(population: dict, sample_list: pd.DataFrame,
-                      mean_dict: dict, cov_dict: dict,
-                      blank_contribution: Optional[np.ndarray] = None,
-                      noise_dict: Optional[dict] = None):
+def _make_data_matrix(
+    population: dict,
+    sample_list: pd.DataFrame,
+    mean_dict: dict,
+    cov_dict: dict,
+    blank_contribution: Optional[np.ndarray] = None,
+    noise_dict: Optional[dict] = None,
+):
     """
     Creates a simulated data matrix
 
     Parameters
     ----------
     population: dict
         A dictionary where each key is a sample class and the value is the
@@ -171,86 +195,78 @@
         cov = cov_dict[k_class]
         mat = generate_correlated_data(k_obs, mean, cov)
         data_mats[k_class] = mat
 
     if (sample_list["class"] == "blank").any():
         if blank_contribution is None:
             blank_contribution = np.zeros_like(mean)
-        data_mats["blank"] = \
-            _generate_blank_data(sample_list, blank_contribution)
+        data_mats["blank"] = _generate_blank_data(sample_list, blank_contribution)
 
     if (sample_list["class"] == "QC").any():
-        data_mats["QC"] = _generate_qc_data(population, sample_list,
-                                            mean_dict)
+        data_mats["QC"] = _generate_qc_data(population, sample_list, mean_dict)
 
     if noise_dict is not None:
-        for c, x in data_mats.items():
-            data_mats[c] = _add_noise(x, noise_dict[c])
+        for cl, x in data_mats.items():
+            data_mats[cl] = _add_noise(x, noise_dict[cl])
 
     data = _concat_data(data_mats, sample_list)
     ft_names = _generate_feature_names(data.shape[1])
-    data_matrix = pd.DataFrame(data=data, index=sample_list.index,
-                               columns=ft_names)
+    data_matrix = pd.DataFrame(data=data, index=sample_list.index, columns=ft_names)
     return data_matrix
 
 
-def _make_sample_classes(sample_distribution, batch_size, qc_bracket_size,
-                         prepend, append):
+def _make_sample_classes(sample_distribution, batch_size, qc_bracket_size, prepend, append):
     n_study_samples = sum(sample_distribution.values())
     # randomize classes and make QC brackets
     classes = list()
     for k, v in sample_distribution.items():
         classes.extend([k] * v)
 
     permutation_index = np.random.permutation(n_study_samples)
     qb, rb = divmod(n_study_samples, batch_size)
     n_batches = qb + bool(rb)
     res = list()
     start = 0
     end = min(batch_size, n_study_samples)
     for k_batches in range(n_batches):
         res += prepend
-        res += _make_batch_sample_block(classes,
-                                        permutation_index[start:end],
-                                        qc_bracket_size)
+        res += _make_batch_sample_block(classes, permutation_index[start:end], qc_bracket_size)
         res += append
         start = end
         end = min(start + batch_size, n_study_samples)
     return res
 
 
-def _make_batch_number(batch_size, n_study_samples, n_prepend, n_append,
-                       qc_bracket_size):
+def _make_batch_number(batch_size, n_study_samples, n_prepend, n_append, qc_bracket_size):
     n_batch, n_study_samples_last_batch = divmod(n_study_samples, batch_size)
     # adds an extra batch for the last batch
     n_batch += int(n_study_samples_last_batch > 0)
     n_qc_batch = _n_qc_per_batch(batch_size, qc_bracket_size)
     n_samples_per_batch = batch_size + n_prepend + n_append + n_qc_batch
     batch_number = list()
     for k_batch in range(1, n_batch):
         batch_number.extend([k_batch] * n_samples_per_batch)
     if n_study_samples_last_batch:
 
-        n_qc_last_batch = _n_qc_per_batch(n_study_samples_last_batch,
-                                          qc_bracket_size)
-        n_samples_last_batch = (n_study_samples_last_batch + n_prepend +
-                                n_append + n_qc_last_batch)
+        n_qc_last_batch = _n_qc_per_batch(n_study_samples_last_batch, qc_bracket_size)
+        n_samples_last_batch = (
+            n_study_samples_last_batch + n_prepend + n_append + n_qc_last_batch
+        )
         batch_number.extend([n_batch] * n_samples_last_batch)
     return batch_number
 
 
 def _make_sample_name(n_samples: int):
     pad_length = len(str(n_samples))
     template_str = "Sample-{{:0{}n}}".format(pad_length)
     sample_name = [template_str.format(x) for x in range(1, n_samples + 1)]
     return sample_name
 
 
-def generate_correlated_data(n_obs: int, mean: np.array,
-                             cov: np.array) -> np.array:
+def generate_correlated_data(n_obs: int, mean: np.array, cov: np.array) -> np.array:
     """
     Generates a data matrix with normal correlated columns
 
     Parameters
     ----------
     n_obs : int
         number of observations in the data matrix
@@ -289,15 +305,15 @@
     blank_data = np.tile(blank_contribution, [n_blank, 1])
     return blank_data
 
 
 def _generate_qc_data(sample_population, sample_list, mean_dict):
     n_qc = (sample_list["class"] == "QC").sum()
     n_samples = sum(sample_population.values())
-    mean = sum([n * mean_dict[c] for c, n in sample_population.items()])
+    mean = sum([n * mean_dict[cl] for cl, n in sample_population.items()])
     mean = np.array(mean) / n_samples
     qc_data = np.tile(mean, [n_qc, 1])
     return qc_data
 
 
 def _is_valid_covariance_matrix(cov: np.array):
     """Checks if a matrix is symmetric and positive definite"""
@@ -314,16 +330,15 @@
 def _generate_random_covariance_matrix(n: int) -> np.array:
     """Creates a random symmetric, positive definite matrix"""
     x = np.random.normal(size=(n, n))
     x = (x + x.T) / 2 + np.diag(np.abs(x).sum(axis=1)) * 2
     return x
 
 
-def _make_batch_sample_block(classes, batch_perm_index,
-                             qc_bracket_size):
+def _make_batch_sample_block(classes, batch_perm_index, qc_bracket_size):
     classes_rand = list()
     for k, ind in enumerate(batch_perm_index):
 
         if ((k % qc_bracket_size) == 0) and k > 0:
             classes_rand.append("QC")
         classes_rand.append(classes[ind])
     return classes_rand
```

### Comparing `tidyms-0.6.3/src/tidyms/utils.py` & `tidyms-0.7.0/src/tidyms/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 from tqdm.notebook import tqdm as notebook_bar
 from IPython.core.getipython import get_ipython
 
 data_type = Union[pd.DataFrame, pd.Series]
 reduced_type = Union[pd.Series, float]
 
 
-def gauss(x: np.ndarray, mu: float, sigma: float,
-          amp: float):
+def gauss(x: np.ndarray, mu: float, sigma: float, amp: float):
     """
     gaussian curve.
 
     Parameters
     ----------
     x : np.array
     mu : float
@@ -34,20 +33,19 @@
     amp : float
 
     Returns
     -------
     gaussian : np.array
 
     """
-    gaussian = amp * np.power(np.e, - 0.5 * ((x - mu) / sigma) ** 2)
+    gaussian = amp * np.power(np.e, -0.5 * ((x - mu) / sigma) ** 2)
     return gaussian
 
 
-def gaussian_mixture(x: np.ndarray, params: np.ndarray
-                     ) -> np.ndarray:
+def gaussian_mixture(x: np.ndarray, params: np.ndarray) -> np.ndarray:
     """
     Mixture of gaussian curves.
 
     Parameters
     ----------
     x : array
     params: np.ndarray
@@ -62,16 +60,15 @@
     """
     mixture = np.zeros((params.shape[0], x.size))
     for k_row, param in enumerate(params):
         mixture[k_row] = gauss(x, *param)
     return mixture
 
 
-def normalize(df: pd.DataFrame, method: str,
-              feature: Optional[str] = None) -> pd.DataFrame:
+def normalize(df: pd.DataFrame, method: str, feature: Optional[str] = None) -> pd.DataFrame:
     """
     Normalize samples using different methods.
 
     Parameters
     ----------
     df: pandas.DataFrame
     method: {"sum", "max", "euclidean", "feature"}
@@ -182,29 +179,28 @@
     full_path = [os.path.join(path, x) for x in available_files]
     d = dict()
     for k, name in enumerate(filenames):
         if name in samples:
             d[name] = full_path[k]
     return d
 
-    
+
 def cv(df: data_type, fill_value: Optional[float] = None) -> reduced_type:
     """
     Computes the Coefficient of variation for each column.
 
     Used by DataContainer objects to compute metrics.
 
     """
     res = df.std() / df.mean()
     res = _fill_na(res, fill_value)
     return res
 
 
-def robust_cv(df: data_type, fill_value: Optional[float] = None
-              ) -> reduced_type:
+def robust_cv(df: data_type, fill_value: Optional[float] = None) -> reduced_type:
     """
     Estimation of the coefficient of variation using the MAD and median.
     Assumes a normal distribution.
     """
 
     # 1.4826 is used to estimate sigma in an unbiased way assuming a normal
     # distribution for each feature.
@@ -226,16 +222,20 @@
         else:
             res = df.apply(median_abs_deviation, scale="normal")
     else:
         res = median_abs_deviation(df, scale="normal")
     return res
 
 
-def sd_ratio(df1: pd.DataFrame, df2: pd.DataFrame, robust: bool = False,
-             fill_value: Optional[float] = None) -> pd.Series:
+def sd_ratio(
+    df1: pd.DataFrame,
+    df2: pd.DataFrame,
+    robust: bool = False,
+    fill_value: Optional[float] = None,
+) -> pd.Series:
     """
     Computes the ratio between the standard deviation of the columns of
     DataFrame1 and DataFrame2.
 
     Used to compute the D-Ratio metric.
 
     Parameters
@@ -301,15 +301,15 @@
     dict
 
     """
     if mode == "ols":
         ols = OLS(y, add_constant(x)).fit()
         r2 = ols.rsquared
         jb = jarque_bera(ols.resid)[1]  # Jarque Bera test p-value
-        dw = durbin_watson(ols.resid)   # Durwin Watson statistic
+        dw = durbin_watson(ols.resid)  # Durwin Watson statistic
         res = {"r2": r2, "DW": dw, "JB": jb}
     elif mode == "pearson":
         res = pearsonr(y, x)[0]
     else:
         res = spearmanr(y, x)[0]
     return res
 
@@ -322,18 +322,15 @@
     elif pd.isna(s):
         res = fill_value
     else:
         res = s
     return res
 
 
-def _find_closest_sorted(
-        x: np.ndarray,
-        xq: Union[np.ndarray, float, int]
-) -> np.ndarray:
+def _find_closest_sorted(x: np.ndarray, xq: Union[np.ndarray, float, int]) -> np.ndarray:
     """
     Find the index in x closest to each xq element. Assumes that x is sorted.
 
     Parameters
     ----------
     x: numpy.ndarray
         Sorted vector
@@ -375,16 +372,17 @@
         mask = (ind > 0) & (ind < x.size)
         ind[mask] -= (xq[mask] - x[ind[mask] - 1]) < (x[ind[mask]] - xq[mask])
         # when the index is x.size, then the closest index is x.size -1
         ind[ind == x.size] = x.size - 1
         return ind
 
 
-def find_closest(x: np.ndarray, xq: Union[np.ndarray, float, int],
-                 is_sorted: bool = True) -> np.ndarray:
+def find_closest(
+    x: np.ndarray, xq: Union[np.ndarray, float, int], is_sorted: bool = True
+) -> np.ndarray:
     """
     Search the closest value between two arrays.
 
     Parameters
     ----------
     x : array
         Array used to search
@@ -473,27 +471,27 @@
                     "aspect_ratio": 1.5,
                 },
                 "xaxis": {
                     "axis_label": "Rt [s]",
                 },
                 "yaxis": {
                     "axis_label": "Intensity [au]",
-                }
+                },
             },
             "spectrum": {
                 "figure": {
                     "aspect_ratio": 1.5,
                 },
                 "xaxis": {
                     "axis_label": "m/z",
                 },
                 "yaxis": {
                     "axis_label": "intensity [au]",
-                }
-            }
+                },
+            },
         }
     }
     return settings
 
 
 def get_settings() -> dict:
     """
@@ -527,22 +525,22 @@
     Returns
     -------
     bool
 
     """
     try:
         shell = get_ipython().__class__.__name__
-        if shell == 'ZMQInteractiveShell':
-            return True   # Jupyter notebook or qtconsole
-        elif shell == 'TerminalInteractiveShell':
+        if shell == "ZMQInteractiveShell":
+            return True  # Jupyter notebook or qtconsole
+        elif shell == "TerminalInteractiveShell":
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
     except NameError:
-        return False      # Probably standard Python interpreter
+        return False  # Probably standard Python interpreter
 
 
 def get_progress_bar():
     if is_notebook():
         progress_bar = notebook_bar
     else:
         progress_bar = cli_bar
@@ -578,9 +576,9 @@
     Returns
     -------
     numpy.ndarray
 
     """
     sep_index = s.index(",")
     dtype = s[:sep_index]
-    data = base64.b64decode(bytes(s[sep_index + 1:], "utf8"))
+    data = base64.b64decode(bytes(s[sep_index + 1 :], "utf8"))
     return np.frombuffer(data, dtype=dtype).copy()
```

### Comparing `tidyms-0.6.3/src/tidyms/validation.py` & `tidyms-0.7.0/src/tidyms/validation.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/__init__.py` & `tidyms-0.7.0/src/tidyms/chem/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,10 +21,8 @@
 - EM : electron mass
 
 """
 
 from ._formula_generator import FormulaGenerator, get_chnops_bounds
 from .envelope_tools import EnvelopeScorer, EnvelopeValidator
 from .formula import Formula
-from .envelope_finder import EnvelopeFinder
-from .mmi_finder import MMIFinder
 from .atoms import EM, PeriodicTable
```

### Comparing `tidyms-0.6.3/src/tidyms/chem/_envelope_utils.py` & `tidyms-0.7.0/src/tidyms/chem/_envelope_utils.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/_formula_generator.py` & `tidyms-0.7.0/src/tidyms/chem/_formula_generator.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/atoms.py` & `tidyms-0.7.0/src/tidyms/chem/atoms.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/elements.json` & `tidyms-0.7.0/src/tidyms/chem/elements.json`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/envelope_tools.py` & `tidyms-0.7.0/src/tidyms/chem/envelope_tools.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/formula.py` & `tidyms-0.7.0/src/tidyms/chem/formula.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/formula_generator_utils.pyx` & `tidyms-0.7.0/src/tidyms/chem/formula_generator_utils.pyx`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/isotope_distribution_utils.pyx` & `tidyms-0.7.0/src/tidyms/chem/isotope_distribution_utils.pyx`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/isotopes.json` & `tidyms-0.7.0/src/tidyms/chem/isotopes.json`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/src/tidyms/chem/mmi_finder.py` & `tidyms-0.7.0/src/tidyms/annotation/mmi_finder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,170 +1,189 @@
 import numpy as np
 import bisect
-from typing import Dict, List, Optional, Tuple
-from .atoms import Element, PeriodicTable, EM
-from ._formula_generator import FormulaCoefficientBounds
-from .envelope_tools import make_formula_coefficients_envelopes
+from typing import Optional
+from .annotation_data import AnnotationData
+from ..chem.atoms import Element, PeriodicTable, EM
+from ..chem._formula_generator import FormulaCoefficientBounds
+from ..chem.envelope_tools import make_formula_coefficients_envelopes
+from ..lcms import Feature
 
 
 class MMIFinder:
     """
     Finds Minimum Mass Isotopologue (MMI) candidates using an array of feature
     m/z and an array of feature area.
 
     """
+
     def __init__(
         self,
-        bounds: Dict[str, Tuple[int, int]],
+        bounds: dict[str, tuple[int, int]],
         max_mass: float,
         max_charge: int,
         length: int,
         bin_size: int,
         mz_tol: float,
         p_tol: float,
-        custom_abundances: Optional[Dict[str, np.ndarray]] = None
+        min_similarity: float,
+        custom_abundances: Optional[dict[str, np.ndarray]] = None,
     ):
         """
         Constructor method.
 
         Parameters
         ----------
-        bounds : Dict
+        bounds : dict
             Mapping from an element symbol str to the minimum and maximum
             allowed values in formulas.
         max_mass : float
             Maximum mass to build rules.
         length : int
             length of the theoretical envelopes used to compute the search
             rules.
         bin_size : int
             Mass interval used to build the rules.
         mz_tol : float
             m/z tolerance to search candidates.
         p_tol : float
             abundance tolerance used to search candidates.
+        min_similarity : float, default=0.9
+            Minimum similarity to create candidates.
         custom_abundances : dict, optional
             Provides custom elemental abundances. A mapping from element
             symbols str to an abundance array. The abundance array must have
             the same size that the natural abundance and its sum must be equal
             to one. For example, for "C", an alternative abundance can be
             array([0.15, 0.85]) for isotopes with nominal mass 12 and 13.
 
         """
         self.rules = _create_rules_dict(
-            bounds, max_mass, length, bin_size, p_tol, custom_abundances)
+            bounds, max_mass, length, bin_size, p_tol, custom_abundances
+        )
         self.bin_size = bin_size
         self.max_charge = abs(max_charge)
         self.polarity = 1 if max_charge >= 0 else -1
         self.max_mass = max_mass
         self.mz_tol = mz_tol
         self.p_tol = p_tol
+        self.min_similarity = min_similarity
 
-    def find(
-        self,
-        mz: np.ndarray,
-        sp: np.ndarray,
-        mono_index: int
-    ) -> List[Tuple[int, int]]:
-
+    def find(self, data: AnnotationData) -> list[tuple[Feature, int]]:
         """
         Search MMI candidates using m/z and area information from a feature
         list.
 
         Parameters
         ----------
-        mz : array
-            Sorted array of m/z values of features
-        sp : array
-            Area array of features.
-        mono_index : int
-            Index of the most intense value in mz
+        features : list[Features]
+            list of features sorted by m/z.
+        mono: Feature
+            Candidate to monoisotopic feature.
 
         Returns
         -------
-        mmi_candidates: List[Tuple[int, int]]
-            List of candidates assuming that the monoisotopic index is part of
+        mmi_candidates: list[tuple[int, int]]
+            list of candidates assuming that the monoisotopic index is part of
             the envelope but not the MMI.
 
         """
-        mono_sp = sp[mono_index]
-        mono_mz = mz[mono_index]
-        # monoisotopic m/z to possible mass values
-        # charge sign and electron mass can be ignored as computations are done
-        # using mass differences
-        mono_M_list, charge_list = _get_valid_mono_mass(
-            mono_mz, self.max_charge, self.polarity, self.max_mass
-        )
-        candidates = [(mono_index, q) for q in charge_list]
-        for M, charge in zip(mono_M_list, charge_list):
-            M_bin = int(M // self.bin_size)
+        mono = data.get_monoisotopologue()
+        candidates = list()
+
+        if mono is None:
+            return candidates
+
+        for charge in range(1, self.max_charge + 1):
+            M_mono = mono.mz * charge - self.polarity * charge * EM
+            if M_mono < self.max_mass:
+                candidates.append((mono, charge))
+            M_bin = int(M_mono // self.bin_size)
             mmi_rules = self.rules.get(M_bin)
             if mmi_rules is not None:
                 for i_rules in mmi_rules:
                     i_candidates = _find_candidate(
-                        mz, sp, M, charge, mono_sp, i_rules, self.mz_tol,
-                        self.p_tol
+                        data,
+                        mono,
+                        charge,
+                        i_rules,
+                        self.mz_tol,
+                        self.p_tol,
+                        self.max_mass,
+                        self.min_similarity,
                     )
                     candidates.extend(i_candidates)
         return candidates
 
 
-def _get_valid_mono_mass(
-    mz_mono: float,
-    max_charge: int,
-    polarity: int,
-    max_mass: float
-) -> Tuple[List[float], List[int]]:
-    charge_list = list()
-    mono_M_list = list()
-    for q in range(1, max_charge + 1):
-        M = q * mz_mono - polarity * q * EM
-        if M <= max_mass:
-            charge_list.append(q)
-            mono_M_list.append(M)
-    return mono_M_list, charge_list
-
-
 def _find_candidate(
-    mz: np.ndarray,
-    sp: np.ndarray,
-    mono_M: float,
+    data: AnnotationData,
+    mono: Feature,
     charge: int,
-    mono_sp: float,
-    i_rules: Dict,
+    i_rules: dict,
     mz_tol: float,
-    p_tol: float
-) -> List[Tuple[int, int]]:
+    p_tol: float,
+    max_mass: float,
+    min_similarity: float,
+) -> list[tuple[int, int]]:
     # search valid m/z values
     min_dM, max_dM = i_rules["dM"]
-    min_mz = (mono_M - max_dM) / charge - mz_tol
-    max_mz = (mono_M - min_dM) / charge + mz_tol
-    min_qp = i_rules["qp"][0]
+    min_mz = mono.mz - max_dM / charge - mz_tol
+    max_mz = mono.mz - min_dM / charge + mz_tol
+    min_qp = i_rules["qp"][0] - p_tol
     max_qp = i_rules["qp"][1] + p_tol
-    start = bisect.bisect(mz, min_mz)
-    end = bisect.bisect(mz, max_mz)
+
+    if (mono.mz * charge) < max_mass:
+        start = bisect.bisect(data.features, min_mz)
+        end = bisect.bisect(data.features, max_mz)
+    else:
+        start, end = 0, 0  # dummy values
+
     # if valid m/z where found, check if the abundance quotient qp is valid
+    candidates = list()
     if start < end:
-        candidates = np.arange(start, end)
-        qp_ind = mono_sp / sp[candidates]
-        valid_mask = (qp_ind >= min_qp) & (qp_ind <= max_qp)
-        candidates = [(x, charge) for x in candidates[valid_mask]]
-    else:
-        candidates = list()
+        for k in range(start, end):
+            candidate = data.features[k]
+            is_valid = _check_candidate(data, mono, candidate, min_similarity, min_qp, max_qp)
+            if is_valid:
+                candidates.append((candidate, charge))
     return candidates
 
 
+def _check_candidate(
+    data: AnnotationData,
+    mono: Feature,
+    candidate: Feature,
+    min_similarity: float,
+    min_qp: float,
+    max_qp: float,
+) -> bool:
+    if candidate not in data.non_annotated:
+        return False
+
+    similarity = data.similarity_cache.get_similarity(mono, candidate)
+
+    if similarity < min_similarity:
+        return False
+
+    mmi_mono_pair = [candidate, mono]
+    _, p = mono.compute_isotopic_envelope(mmi_mono_pair)
+    qp = p[1] / p[0]
+    is_valid_qp = (qp >= min_qp) & (qp <= max_qp)
+
+    return is_valid_qp
+
+
 def _create_rules_dict(
-    bounds: Dict[str, Tuple[int, int]],
+    bounds: dict[str, tuple[int, int]],
     max_mass: float,
     length: int,
     bin_size: int,
     p_tol: float,
-    custom_abundances: Optional[Dict[str, np.ndarray]]
-) -> Dict[int, List[Dict[str, Tuple[float, float]]]]:
+    custom_abundances: Optional[dict[str, np.ndarray]],
+) -> dict[int, list[dict[str, tuple[float, float]]]]:
     Ma, pa = _create_envelope_arrays(bounds, max_mass, length, custom_abundances)
     # find the monoisotopic index, its Mass difference with the MMI (dM) and
     # its abundance quotient with the MMI (qp)
     bins = (Ma[:, 0] // bin_size).astype(int)
 
     # find unique values for bins and monoisotopic index that will be used
     # as key for the rule dictionary
@@ -189,34 +208,34 @@
                 b_rules.append(mi_rules)
         if b_rules:
             rules[b] = b_rules
     return rules
 
 
 def _create_envelope_arrays(
-    bounds: Dict[str, Tuple[int, int]],
+    bounds: dict[str, tuple[int, int]],
     M_max: float,
     max_length: int,
-    custom_abundances: Optional[Dict[str, np.ndarray]]
-) -> Tuple[np.ndarray, np.ndarray]:
+    custom_abundances: Optional[dict[str, np.ndarray]],
+) -> tuple[np.ndarray, np.ndarray]:
     elements = _select_elements(list(bounds), custom_abundances)
     isotopes = [x.get_mmi() for x in elements]
     f_bounds = FormulaCoefficientBounds({x: bounds[x.get_symbol()] for x in isotopes})
     coeff = f_bounds.make_coefficients(M_max)
-    envelope = make_formula_coefficients_envelopes(bounds, coeff, max_length, custom_abundances)
+    envelope = make_formula_coefficients_envelopes(
+        bounds, coeff, max_length, custom_abundances
+    )
     M = envelope.M
     p = envelope.p
     return M, p
 
 
 def _select_two_isotope_element(
-    e_list: List[str],
-    dm: int,
-    custom_abundances: Dict[str, np.ndarray]
-) -> List[str]:
+    e_list: list[str], dm: int, custom_abundances: dict[str, np.ndarray]
+) -> list[str]:
     selected = list()
     p_dm_max = 0
     best_p0_greater_than_pi = None
     for s in e_list:
         e = PeriodicTable().get_element(s)
         n_isotopes = len(e.isotopes)
         m, _, p = e.get_abundances()
@@ -230,27 +249,27 @@
                     p_dm_max = pi
                     best_p0_greater_than_pi = s
     if best_p0_greater_than_pi is not None:
         selected.append(best_p0_greater_than_pi)
     return selected
 
 
-def _select_multiple_isotope_elements(e_list: List[str]) -> List[str]:
+def _select_multiple_isotope_elements(e_list: list[str]) -> list[str]:
     selected = list()
     for s in e_list:
         e = PeriodicTable().get_element(s)
         n_isotopes = len(e.isotopes)
         if n_isotopes > 2:
             selected.append(s)
     return selected
 
 
 def _select_elements(
-        e_list: List[str], custom_abundances: Optional[Dict[str, np.ndarray]] = None
-) -> List[Element]:
+    e_list: list[str], custom_abundances: Optional[dict[str, np.ndarray]] = None
+) -> list[Element]:
     if custom_abundances is None:
         custom_abundances = dict()
     two_isotope_dm1 = _select_two_isotope_element(e_list, 1, custom_abundances)
     two_isotope_dm2 = _select_two_isotope_element(e_list, 2, custom_abundances)
     selected = _select_multiple_isotope_elements(e_list)
     if two_isotope_dm1 is not None:
         selected.extend(two_isotope_dm1)
```

### Comparing `tidyms-0.6.3/src/tidyms/chem/utils.py` & `tidyms-0.7.0/src/tidyms/chem/utils.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/conftest.py` & `tidyms-0.7.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,63 +14,44 @@
     for dataset in fileio.list_available_datasets(False):
         fileio.download_dataset(dataset)
 
 
 @pytest.fixture
 def data_container_with_order():
     population = {"healthy": 20, "disease": 35}
-    mean = {"healthy": np.array([50, 100, 150]),
-            "disease": np.array([150, 200, 300])}
-    cov = {"healthy": np.array([1, 1, 1]),
-           "disease": np.array([2, 2, 2])}
+    mean = {"healthy": np.array([50, 100, 150]), "disease": np.array([150, 200, 300])}
+    cov = {"healthy": np.array([1, 1, 1]), "disease": np.array([2, 2, 2])}
     blank_contribution = np.array([3, 5, 10])
     mz = np.array([100, 200, 300])
     rt = np.array([50, 60, 70])
-    dc = simulate_dataset(population, mean, cov, mz, rt, blank_contribution,
-                          prepend_blank=1, append_blank=1)
+    dc = simulate_dataset(
+        population, mean, cov, mz, rt, blank_contribution, prepend_blank=1, append_blank=1
+    )
     return dc
 
 
 @pytest.fixture
 def data_container_with_order_single_qc():
     population = {"healthy": 20, "disease": 35}
-    mean = {"healthy": np.array([50, 100, 150]),
-            "disease": np.array([150, 200, 300])}
-    cov = {"healthy": np.array([1, 1, 1]),
-           "disease": np.array([2, 2, 2])}
+    mean = {"healthy": np.array([50, 100, 150]), "disease": np.array([150, 200, 300])}
+    cov = {"healthy": np.array([1, 1, 1]), "disease": np.array([2, 2, 2])}
     blank_contribution = np.array([3, 5, 10])
     mz = np.array([100, 200, 300])
     rt = np.array([50, 60, 70])
-    dc = simulate_dataset(population, mean, cov, mz, rt, blank_contribution,
-                          prepend_blank=1, append_blank=1, triple_qc=False)
-    return dc
-
-
-@pytest.fixture
-def data_container_with_batch_effect():
-    population = {"healthy": 24, "disease": 24}
-    mean = {"healthy": np.array([50, 100, 150]),
-            "disease": np.array([150, 200, 300])}
-    cov = {"healthy": np.array([1, 1, 1]),
-           "disease": np.array([2, 2, 2])}
-    blank_contribution = np.array([3, 5, 10])
-    mz = np.array([100, 200, 300])
-    rt = np.array([50, 60, 70])
-    dc = simulate_dataset(population, mean, cov, mz, rt, blank_contribution,
-                          prepend_blank=1, append_blank=1)
-
-    def add_batch_effect(x):
-        n_samples = x.shape[0]
-        batch_effect = pd.Series(data=np.linspace(1, 0.8, n_samples),
-                                 index=x.index)
-        return x.multiply(batch_effect, axis=0)
-    dc._data_matrix = (dc.data_matrix.groupby(dc.batch)
-                       .apply(add_batch_effect))
-    mapping = {"sample": list(population), "qc": ["QC"]}
-    dc.mapping = mapping
+    dc = simulate_dataset(
+        population,
+        mean,
+        cov,
+        mz,
+        rt,
+        blank_contribution,
+        prepend_blank=1,
+        append_blank=1,
+        triple_qc=False,
+    )
     return dc
 
 
 @pytest.fixture
 def data_container_without_order(data_container_with_order):
     dc = data_container_with_order
     dm = dc.data_matrix.copy()
@@ -84,18 +65,18 @@
 
 @pytest.fixture
 def centroid_mzml():
     cache_path = get_tidyms_path()
     dataset_name = "test-raw-data"
     filename = "centroid-data-zlib-indexed-compressed.mzML"
     data_path = os.path.join(cache_path, dataset_name, filename)
-    ms_data = fileio.MSData(data_path, ms_mode="profile")
+    ms_data = fileio.MSData.create_MSData_instance(data_path, ms_mode="profile")
     return ms_data
 
 
 @pytest.fixture
 def profile_mzml():
     cache_path = get_tidyms_path()
     filename = "profile-data-zlib-indexed-compressed.mzML"
     data_path = os.path.join(cache_path, "test-raw-data", filename)
-    ms_data = fileio.MSData(data_path, ms_mode="profile")
+    ms_data = fileio.MSData.create_MSData_instance(data_path, ms_mode="profile")
     return ms_data
```

### Comparing `tidyms-0.6.3/tests/integration/test_assay_real_data.py` & `tidyms-0.7.0/tests/integration/test_assay_real_data.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/integration/test_real_raw_data.py` & `tidyms-0.7.0/tests/integration/test_real_raw_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 @pytest.fixture
 def ms_data_centroid() -> ms.MSData:
     tidyms_path = ms.fileio.get_tidyms_path()
     filename = "centroid-data-zlib-indexed-compressed.mzML"
     data_path = os.path.join(tidyms_path, "test-raw-data", filename)
-    return ms.MSData(data_path)
+    return ms.MSData.create_MSData_instance(data_path)
 
 
 def test_ms_data_invalid_ms_mode_setter(ms_data_centroid):
     with pytest.raises(ValueError):
         ms_data_centroid.ms_mode = "invalid-mode"
```

### Comparing `tidyms-0.6.3/tests/unit/test_assay.py` & `tidyms-0.7.0/tests/unit/test_assay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from tidyms import assay
-from tidyms.lcms import LCRoi, Peak
+from tidyms import _constants as c
+from tidyms.lcms import LCTrace, Peak
+from tidyms import _constants as c
 import pytest
 from pathlib import Path
 import os
 import numpy as np
 import pandas as pd
 
 
@@ -22,59 +24,54 @@
 
 
 def create_sample_names(n: int, start: int = 1):
     template = "Sample{}.mzML"
     return [template.format(k) for k in range(start, n + start)]
 
 
-def create_assay_dir(
-    path,
-    n,
-    start=1,
-    data_dir_name: str = "data-dir",
-    assay_dir_name: str = "assay-dir"
-):
+def create_assay_dir(path, n, start=1, data_dir_name: str = "data-dir", assay_dir_name: str = "assay-dir"):
     tmpdir = Path(str(path))
     assay_path = tmpdir.joinpath(assay_dir_name)
     data_path = tmpdir.joinpath(data_dir_name)
     # assay_path.mkdir()
     data_path.mkdir(exist_ok=True)
     sample_names = create_sample_names(n, start=start)
     fill_dummy_data_dir(data_path, sample_names)
     return assay_path, data_path
 
 
-def create_dummy_assay_manager(
-        assay_path, data_path, metadata) -> assay._AssayManager:
+def create_dummy_assay_manager(assay_path, data_path, metadata) -> assay._AssayManager:
     return assay._AssayManager(
         assay_path=assay_path,
         data_path=data_path,
         sample_metadata=metadata,
-        ms_mode="centroid",
-        instrument="qtof",
-        separation="uplc"
+        ms_mode=c.CENTROID,
+        instrument=c.QTOF,
+        separation=c.UPLC,
+        data_import_mode=c.SIMULATED,
     )
 
 
 def create_dummy_data_frame(n: int, classes: list, start: int = 1):
     sample_names = create_sample_names(n, start=start)
     sample_names = [x.split(".")[0] for x in sample_names]
-    df = pd.DataFrame(data=sample_names, columns=["sample"])
-    df["class"] = np.random.choice(classes, n)
+    df = pd.DataFrame(data=sample_names, columns=[c.SAMPLE])
+    df[c.CLASS] = np.random.choice(classes, n)
     return df
 
 
 def test_assay_metadata_creation(tmpdir):
     assay_path, data_path = create_assay_dir(tmpdir, 20)
     create_dummy_assay_manager(assay_path, data_path, None)
     assert True
 
 
 # get_path_list
 
+
 def test_get_path_list_single_file_str(tmpdir):
     file_path = str(tmpdir) + os.path.sep + "sample.mzML"
     path = Path(file_path)
     path.touch()
     path_list = assay._get_path_list(file_path)
     assert len(path_list) == 1
 
@@ -160,171 +157,168 @@
 
 def test_assay_manager_invalid_sample_metadata_extra_samples(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
     sample_metadata2 = sample_metadata.copy()
-    sample_metadata2["sample"] = sample_metadata2["sample"] + "asdf"
+    sample_metadata2[c.SAMPLE] = sample_metadata2[c.SAMPLE] + "asdf"
     sample_metadata = pd.concat([sample_metadata, sample_metadata2])
     sample_metadata = sample_metadata.reset_index()
     with pytest.raises(ValueError):
         create_dummy_assay_manager(assay_path, data_path, sample_metadata)
 
 
 def test_assay_manager_sample_metadata_without_sample_column(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    sample_metadata = sample_metadata.drop(columns=["sample"])
+    sample_metadata = sample_metadata.drop(columns=[c.SAMPLE])
     with pytest.raises(ValueError):
         create_dummy_assay_manager(assay_path, data_path, sample_metadata)
 
 
 def test_assay_manager_sample_metadata_without_class_column(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    sample_metadata = sample_metadata.drop(columns=["class"])
-    metadata = create_dummy_assay_manager(
-        assay_path, data_path, sample_metadata)
-    assert (metadata.sample_metadata.class_ == 0).all()
+    sample_metadata = sample_metadata.drop(columns=[c.CLASS])
+    metadata = create_dummy_assay_manager(assay_path, data_path, sample_metadata)
+    assert (metadata.sample_metadata[c.CLASS] == 0).all()
 
 
 def test_assay_manager_sample_metadata_without_order_column(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    sample_metadata = sample_metadata.drop(columns=["class"])
-    metadata = create_dummy_assay_manager(
-        assay_path, data_path, sample_metadata)
-    assert (metadata.sample_metadata.order_ == np.arange(n) + 1).all()
+    sample_metadata = sample_metadata.drop(columns=[c.CLASS])
+    metadata = create_dummy_assay_manager(assay_path, data_path, sample_metadata)
+    assert (metadata.sample_metadata[c.ORDER] == np.arange(n) + 1).all()
 
 
 def test_assay_manager_sample_metadata_with_order_column(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    sample_metadata["order"] = np.arange(n) + 1
+    sample_metadata[c.ORDER] = np.arange(n) + 1
     create_dummy_assay_manager(assay_path, data_path, sample_metadata)
     assert True
 
 
 def test_assay_manager_sample_metadata_invalid_order_type(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    sample_metadata["order"] = np.arange(n) + 1
-    sample_metadata["order"] = sample_metadata["order"].astype(str)
+    sample_metadata[c.ORDER] = np.arange(n) + 1
+    sample_metadata[c.ORDER] = sample_metadata[c.ORDER].astype(str)
     with pytest.raises(TypeError):
         create_dummy_assay_manager(assay_path, data_path, sample_metadata)
 
 
 def test_assay_manager_sample_metadata_invalid_order_non_pos_values(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    sample_metadata["order"] = np.arange(n) + 1
-    sample_metadata.at[2, "order"] = -1
+    sample_metadata[c.ORDER] = np.arange(n) + 1
+    sample_metadata.at[2, c.ORDER] = -1
     with pytest.raises(ValueError):
         create_dummy_assay_manager(assay_path, data_path, sample_metadata)
 
 
 def test_assay_manager_sample_metadata_invalid_order_repeated_values(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    sample_metadata["order"] = np.arange(n) + 1
-    sample_metadata.at[2, "order"] = 1
+    sample_metadata[c.ORDER] = np.arange(n) + 1
+    sample_metadata.at[2, c.ORDER] = 1
     with pytest.raises(ValueError):
         create_dummy_assay_manager(assay_path, data_path, sample_metadata)
 
 
 def test_assay_manager_sample_metadata_with_batch_column(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
     n1 = n // 2
     n2 = n - n1
-    sample_metadata["batch"] = [1] * n1 + [2] * n2
+    sample_metadata[c.BATCH] = [1] * n1 + [2] * n2
     create_dummy_assay_manager(assay_path, data_path, sample_metadata)
     assert True
 
 
 def test_assay_manager_sample_metadata_invalid_batch_type(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
     n1 = n // 2
     n2 = n - n1
-    sample_metadata["batch"] = [0] * n1 + [2] * n2
-    sample_metadata["batch"] = sample_metadata["batch"].astype(str)
+    sample_metadata[c.BATCH] = [0] * n1 + [2] * n2
+    sample_metadata[c.BATCH] = sample_metadata[c.BATCH].astype(str)
     with pytest.raises(TypeError):
         create_dummy_assay_manager(assay_path, data_path, sample_metadata)
 
 
 def test_assay_manager_sample_metadata_invalid_batch_values(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
     n1 = n // 2
     n2 = n - n1
-    sample_metadata["batch"] = [0] * n1 + [2] * n2
+    sample_metadata[c.BATCH] = [0] * n1 + [2] * n2
     with pytest.raises(ValueError):
         create_dummy_assay_manager(assay_path, data_path, sample_metadata)
 
 
 def test_assay_manager_create_assay_dir(tmpdir):
     n = 20
     classes = ["a", "b", "c"]
     assay_path, data_path = create_assay_dir(tmpdir, n)
     sample_metadata = create_dummy_data_frame(n, classes)
-    metadata = create_dummy_assay_manager(
-        assay_path, data_path, sample_metadata)
+    metadata = create_dummy_assay_manager(assay_path, data_path, sample_metadata)
     metadata.create_assay_dir()
 
     # check dir
     roi_path = metadata.assay_path.joinpath("roi")
     assert roi_path.is_dir()
     ft_path = metadata.assay_path.joinpath("feature")
     assert ft_path.is_dir()
 
 
 def test_assay_manager_check_previous_step_first_step(tmpdir):
     assay_path, data_path = create_assay_dir(tmpdir, 20)
     metadata = create_dummy_assay_manager(assay_path, data_path, None)
-    step = "detect_features"
+    step = c.DETECT_FEATURES
     metadata.check_step(step)
     assert True
 
 
 def test_assay_manager_check_previous_middle_step(tmpdir):
     assay_path, data_path = create_assay_dir(tmpdir, 20)
     metadata = create_dummy_assay_manager(assay_path, data_path, None)
-    previous = "detect_features"
+    previous = c.DETECT_FEATURES
     metadata.flag_completed(previous)
-    step = "extract_features"
+    step = c.EXTRACT_FEATURES
     metadata.check_step(step)
     assert True
 
 
 def test_assay_manager_check_invalid_order(tmpdir):
     assay_path, data_path = create_assay_dir(tmpdir, 20)
     metadata = create_dummy_assay_manager(assay_path, data_path, None)
-    step = "extract_features"
+    step = c.EXTRACT_FEATURES
     with pytest.raises(assay.PreprocessingOrderError):
         metadata.check_step(step)
 
 
 def test_assay_manager_get_sample_path_using_sample_name(tmpdir):
     assay_path, data_path = create_assay_dir(tmpdir, 20)
     metadata = create_dummy_assay_manager(assay_path, data_path, None)
@@ -366,53 +360,55 @@
 
 def test_assay_manager_add_samples(tmpdir):
     n1 = 20
     n2 = 20
     assay_path, data_path = create_assay_dir(tmpdir, n1)
     metadata = create_dummy_assay_manager(assay_path, data_path, None)
     metadata.create_assay_dir()
-    _, new_data_path = create_assay_dir(
-        tmpdir, n2, start=n1 + 1, data_dir_name="new-data-path")
+    _, new_data_path = create_assay_dir(tmpdir, n2, start=n1 + 1, data_dir_name="new-data-path")
     metadata.add_samples(new_data_path, None)
 
     assert metadata.sample_metadata.shape[0] == n1 + n2
 
     # check new sample names
     for sample_path in new_data_path.glob("*"):
         filename = sample_path.stem
         assert filename in metadata.sample_metadata.index
 
 
 # Test AssayTemplate
 
 # create a subclass with dummy methods
 
-class DummyAssay(assay.Assay):
 
+class DummyAssay(assay.Assay):
     n_roi = 5
     roi_length = 20
     n_ft = 5
 
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs, data_import_mode=c.SIMULATED)
+
     def get_ms_data(self, sample: str):
         return sample
 
 
 def detect_features_dummy(ms_data: str, **kwargs):
     results = list()
     for k in range(DummyAssay.n_roi):
         x = np.arange(DummyAssay.roi_length)
-        roi = LCRoi(x, x, x, x, "uplc")
+        roi = LCTrace(x, x, x, x, "uplc")
         results.append(roi)
     return results
 
 
 def extract_features_dummy(roi, **kwargs):
     roi.noise = np.zeros_like(roi.spint) + 1e-8
     roi.baseline = np.zeros_like(roi.spint) + 1e-8
-    roi.features = [Peak(0, 5, 10) for _ in range(DummyAssay.n_ft)]
+    roi.features = [Peak(0, 5, 10, roi) for _ in range(DummyAssay.n_ft)]
 
 
 def test_assay_creation(tmpdir):
     assay_path, data_path = create_assay_dir(tmpdir, 20)
     create_dummy_assay_manager(assay_path, data_path, None)
     DummyAssay(assay_path, data_path)
     assert True
@@ -569,15 +565,15 @@
 
 
 def test_assay_load_features(tmpdir):
     assay_path, data_path = create_assay_dir(tmpdir, 20)
     test_assay = DummyAssay(assay_path, data_path)
     test_assay.detect_features(strategy=detect_features_dummy)
     test_assay.extract_features(strategy=extract_features_dummy)
-    filters = {"width": (0, None), "snr": (0, None)}
+    filters = {c.WIDTH: (0, None), c.SNR: (0, None)}
     test_assay.describe_features(filters=filters)
     sample_list = test_assay.manager.get_sample_names()
     for sample in sample_list:
         features = test_assay.load_features(sample)
         n_features = DummyAssay.n_ft * DummyAssay.n_roi
         # descriptors = area, width, height, snr, mz, mz_std, rt, rt start,
         # rt end, roi index, ft index == 11
@@ -589,14 +585,41 @@
 
 def test_assay_build_feature_table(tmpdir):
     n_samples = 20
     assay_path, data_path = create_assay_dir(tmpdir, n_samples)
     test_assay = DummyAssay(assay_path, data_path)
     test_assay.detect_features(strategy=detect_features_dummy)
     test_assay.extract_features(strategy=extract_features_dummy)
-    filters = {"width": (0, None), "snr": (0, None)}
+    filters = {c.WIDTH: (0, None), c.SNR: (0, None)}
     test_assay.describe_features(filters=filters)
     test_assay.build_feature_table()
     n_features = DummyAssay.n_ft * DummyAssay.n_roi * n_samples
     n_descriptors = 13
     expected_shape = (n_features, n_descriptors)
     assert test_assay.feature_table.shape == expected_shape
+
+
+# test peak descriptors
+
+
+def test_fill_filter_boundaries_fill_upper_bound():
+    filters = {"loc": (50, None), "snr": (5, 10)}
+    assay._fill_filter_boundaries(filters)
+    assert np.isclose(filters["loc"][1], np.inf)
+
+
+def test_fill_filter_boundaries_fill_lower_bound():
+    filters = {"loc": (None, 50), "snr": (5, 10)}
+    assay._fill_filter_boundaries(filters)
+    assert np.isclose(filters["loc"][0], -np.inf)
+
+
+def test_has_all_valid_descriptors():
+    descriptors = {"loc": 50, "height": 10, "snr": 5}
+    filters = {"snr": (3, 10)}
+    assert assay._all_valid_descriptors(descriptors, filters)
+
+
+def test_has_all_valid_descriptors_descriptors_outside_valid_ranges():
+    descriptors = {"loc": 50, "height": 10, "snr": 5}
+    filters = {"snr": (10, 20)}
+    assert not assay._all_valid_descriptors(descriptors, filters)
```

### Comparing `tidyms-0.6.3/tests/unit/test_batch_corrector.py` & `tidyms-0.7.0/tests/unit/test_batch_corrector.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_build_data_matrix.py` & `tidyms-0.7.0/tests/unit/test_build_data_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 from tidyms import _constants as c
 import pytest
 
 
 def create_dummy_sample_metadata(n_samples):
     samples = ["Sample{}".format(x + 1) for x in range(n_samples)]
     # dummy sample metadata, we only care about the index
-    return pd.DataFrame(
-        data=1,
-        index=samples,
-        columns=["class", "id"]
-    )
+    return pd.DataFrame(data=1, index=samples, columns=["class", "id"])
 
 
 def create_dummy_feature_table(n_ft, n_samples):
     n_rows = 1000
     columns = [c.AREA, c.HEIGHT, c.MZ, c.RT, c.RT_START, c.RT_END]
     n_cols = len(columns)
     samples = ["Sample{}".format(x + 1) for x in range(n_samples)]
@@ -25,25 +21,24 @@
 
     # assign unique cluster/sample pairs to each feature
     def assign_cluster(df):
         size = df.shape[0]
         clusters = np.arange(n_ft)
         if size > n_ft:
             # excess values are set to -1
-            label = - np.ones(size, dtype=int)
+            label = -np.ones(size, dtype=int)
             label[:n_ft] = np.random.choice(clusters, replace=False, size=n_ft)
 
         else:
             label = np.random.choice(clusters, replace=False, size=size)
         df[c.LABEL] = label
         return df
 
-    feature_table[c.SAMPLE] = np.random.choice(
-        samples, replace=True, size=n_rows)
-    feature_table = feature_table.groupby(c.SAMPLE).apply(assign_cluster)
+    feature_table[c.SAMPLE] = np.random.choice(samples, replace=True, size=n_rows)
+    feature_table = feature_table.groupby(c.SAMPLE, group_keys=False).apply(assign_cluster)
     feature_table = feature_table[feature_table[c.LABEL] > -1]
 
     return feature_table
 
 
 @pytest.mark.parametrize("n_ft", [5, 50, 200])
 def test_cluster_to_feature_name(n_ft):
@@ -68,104 +63,100 @@
     n_samples = 20
     n_ft = 10
     sample_metadata = create_dummy_sample_metadata(n_samples)
     feature_table = create_dummy_feature_table(n_ft, n_samples)
     labels = feature_table[c.LABEL]
     cluster_to_ft = _build_data_matrix._cluster_to_feature_name(labels)
     data_matrix = _build_data_matrix._build_data_matrix(
-        feature_table, sample_metadata, cluster_to_ft)
+        feature_table, sample_metadata, cluster_to_ft
+    )
     assert data_matrix.index.name == c.SAMPLE
     assert data_matrix.columns.name == c.FEATURE
     assert data_matrix.shape == (n_samples, n_ft)
     assert data_matrix.index.equals(sample_metadata.index)
 
 
 def test__build_data_matrix_all_features_missing_in_a_sample():
     n_samples = 20
     n_ft = 10
     sample_metadata = create_dummy_sample_metadata(n_samples + 1)
     feature_table = create_dummy_feature_table(n_ft, n_samples)
     labels = feature_table[c.LABEL]
     cluster_to_ft = _build_data_matrix._cluster_to_feature_name(labels)
     data_matrix = _build_data_matrix._build_data_matrix(
-        feature_table, sample_metadata, cluster_to_ft)
+        feature_table, sample_metadata, cluster_to_ft
+    )
     assert data_matrix.index.name == c.SAMPLE
     assert data_matrix.columns.name == c.FEATURE
     assert data_matrix.shape == (n_samples + 1, n_ft)
     assert data_matrix.index.equals(sample_metadata.index)
 
 
 def test__merge_features_not_merge():
     # features detected in all samples should not be merged
     merge_threshold = 0.8
     n_ft = 4
     n_samples = 20
     feature_names = ["FT1", "FT2", "FT3", "FT4"]
     feature_set = set(feature_names)
     merged_dict = dict()
-    data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=feature_names
-    )
+    data_matrix = pd.DataFrame(data=np.ones((n_samples, n_ft)), columns=feature_names)
     ft1 = feature_names[1]
     ft2 = feature_names[2]
     results = _build_data_matrix._merge_features(
-        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold)
+        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold
+    )
     assert results is None
 
 
 def test__merge_features_merge_main_ft1():
     # features detected in all samples should not be merged
     merge_threshold = 0.8
     n_ft = 4
     n_samples = 20
     feature_names = ["FT1", "FT2", "FT3", "FT4"]
     feature_set = set(feature_names)
     merged_dict = dict()
-    data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=feature_names
-    )
+    data_matrix = pd.DataFrame(data=np.ones((n_samples, n_ft)), columns=feature_names)
     ft1 = feature_names[1]
     ft2 = feature_names[2]
 
     nan_index = data_matrix.index[:10]
     not_nan_index = data_matrix.index[10:]
     data_matrix.loc[nan_index, ft2] = np.nan
 
     merged_ft = _build_data_matrix._merge_features(
-        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold)
+        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold
+    )
     assert merged_ft == ft2
     assert ft1 in merged_dict
     assert ft2 not in feature_set
     assert (data_matrix.loc[nan_index, ft1] == 1).all()
     assert (data_matrix.loc[not_nan_index, ft1] == 2).all()
 
 
 def test__merge_features_merge_main_ft1_ft1_in_merged_dict():
     # features detected in all samples should not be merged
     merge_threshold = 0.8
     n_ft = 4
     n_samples = 20
     feature_names = ["FT1", "FT2", "FT3", "FT4"]
     feature_set = set(feature_names)
-    data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=feature_names
-    )
+    data_matrix = pd.DataFrame(data=np.ones((n_samples, n_ft)), columns=feature_names)
     ft1 = feature_names[1]
     ft2 = feature_names[2]
     merged_dict = {ft1: ["FT5"]}
 
     nan_index = data_matrix.index[:10]
     not_nan_index = data_matrix.index[10:]
     data_matrix.loc[nan_index, ft2] = np.nan
 
     merged_ft = _build_data_matrix._merge_features(
-        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold)
+        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold
+    )
     assert merged_ft == ft2
     assert ft1 in merged_dict
     assert merged_dict[ft1] == ["FT5", ft2]
     assert ft2 not in feature_set
     assert (data_matrix.loc[nan_index, ft1] == 1).all()
     assert (data_matrix.loc[not_nan_index, ft1] == 2).all()
 
@@ -173,28 +164,26 @@
 def test__merge_features_merge_main_ft1_ft2_in_merged_dict():
     # features detected in all samples should not be merged
     merge_threshold = 0.8
     n_ft = 4
     n_samples = 20
     feature_names = ["FT1", "FT2", "FT3", "FT4"]
     feature_set = set(feature_names)
-    data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=feature_names
-    )
+    data_matrix = pd.DataFrame(data=np.ones((n_samples, n_ft)), columns=feature_names)
     ft1 = feature_names[1]
     ft2 = feature_names[2]
     merged_dict = {ft2: ["FT5"]}
 
     nan_index = data_matrix.index[:10]
     not_nan_index = data_matrix.index[10:]
     data_matrix.loc[nan_index, ft2] = np.nan
 
     merged_ft = _build_data_matrix._merge_features(
-        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold)
+        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold
+    )
     assert merged_ft == ft2
     assert ft1 in merged_dict
     assert set(merged_dict[ft1]) == {"FT5", ft2}
     assert ft2 not in feature_set
     assert (data_matrix.loc[nan_index, ft1] == 1).all()
     assert (data_matrix.loc[not_nan_index, ft1] == 2).all()
 
@@ -203,27 +192,25 @@
     # features detected in all samples should not be merged
     merge_threshold = 0.8
     n_ft = 4
     n_samples = 20
     feature_names = ["FT1", "FT2", "FT3", "FT4"]
     feature_set = set(feature_names)
     merged_dict = dict()
-    data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=feature_names
-    )
+    data_matrix = pd.DataFrame(data=np.ones((n_samples, n_ft)), columns=feature_names)
     ft1 = feature_names[1]
     ft2 = feature_names[2]
 
     nan_index = data_matrix.index[:10]
     not_nan_index = data_matrix.index[10:]
     data_matrix.loc[nan_index, ft1] = np.nan
 
     merged_ft = _build_data_matrix._merge_features(
-        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold)
+        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold
+    )
     assert ft1 not in merged_dict
     assert merged_ft == ft1
     assert ft1 in merged_dict[ft2]
     assert ft2 in feature_set
     assert (data_matrix.loc[nan_index, ft2] == 1).all()
     assert (data_matrix.loc[not_nan_index, ft2] == 2).all()
 
@@ -231,28 +218,26 @@
 def test__merge_features_merge_main_ft2_ft1_in_merged_dict():
     # features detected in all samples should not be merged
     merge_threshold = 0.8
     n_ft = 4
     n_samples = 20
     feature_names = ["FT1", "FT2", "FT3", "FT4"]
     feature_set = set(feature_names)
-    data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=feature_names
-    )
+    data_matrix = pd.DataFrame(data=np.ones((n_samples, n_ft)), columns=feature_names)
     ft1 = feature_names[1]
     ft2 = feature_names[2]
     merged_dict = {ft1: ["FT5"]}
 
     nan_index = data_matrix.index[:10]
     not_nan_index = data_matrix.index[10:]
     data_matrix.loc[nan_index, ft1] = np.nan
 
     merged_ft = _build_data_matrix._merge_features(
-        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold)
+        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold
+    )
     assert ft1 not in merged_dict
     assert merged_ft == ft1
     assert {"FT5", ft1} == set(merged_dict[ft2])
     assert ft2 in feature_set
     assert (data_matrix.loc[nan_index, ft2] == 1).all()
     assert (data_matrix.loc[not_nan_index, ft2] == 2).all()
 
@@ -260,28 +245,26 @@
 def test__merge_features_merge_main_ft2_ft2_in_merged_dict():
     # features detected in all samples should not be merged
     merge_threshold = 0.8
     n_ft = 4
     n_samples = 20
     feature_names = ["FT1", "FT2", "FT3", "FT4"]
     feature_set = set(feature_names)
-    data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=feature_names
-    )
+    data_matrix = pd.DataFrame(data=np.ones((n_samples, n_ft)), columns=feature_names)
     ft1 = feature_names[1]
     ft2 = feature_names[2]
     merged_dict = {ft2: ["FT5"]}
 
     nan_index = data_matrix.index[:10]
     not_nan_index = data_matrix.index[10:]
     data_matrix.loc[nan_index, ft1] = np.nan
 
     merged_ft = _build_data_matrix._merge_features(
-        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold)
+        data_matrix, merged_dict, feature_set, ft1, ft2, merge_threshold
+    )
     assert ft1 not in merged_dict
     assert merged_ft == ft1
     assert {"FT5", ft1} == set(merged_dict[ft2])
     assert ft2 in feature_set
     assert (data_matrix.loc[nan_index, ft2] == 1).all()
     assert (data_matrix.loc[not_nan_index, ft2] == 2).all()
 
@@ -360,121 +343,96 @@
 
 def test__lc_merge_close_features_none_close():
     n_samples = 10
     n_ft = 4
     ft_names = ["FT-{}".format(x) for x in range(n_ft)]
     samples = ["sample{}".format(x) for x in range(n_samples)]
     data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=ft_names,
-        index=samples
+        data=np.ones((n_samples, n_ft)), columns=ft_names, index=samples
     )
     ft_descriptors = [c.MZ, c.RT]
     feature_metadata = pd.DataFrame(
-        data=[[1, 1], [2, 2], [3, 3], [4, 4]],
-        columns=ft_descriptors,
-        index=ft_names
+        data=[[1, 1], [2, 2], [3, 3], [4, 4]], columns=ft_descriptors, index=ft_names
     )
 
     mz_merge = 0.01
     rt_merge = 0.01
     merge_threshold = 1.0
 
     expected_data_matrix = data_matrix.copy()
     expected_feature_metadata = feature_metadata.copy()
     _build_data_matrix._lc_merge_close_features(
-        data_matrix,
-        feature_metadata,
-        mz_merge,
-        rt_merge,
-        merge_threshold
+        data_matrix, feature_metadata, mz_merge, rt_merge, merge_threshold
     )
     assert expected_data_matrix.equals(data_matrix)
     merged = feature_metadata.pop(c.MERGED)
     assert expected_feature_metadata.equals(feature_metadata)
     assert (merged == "").all()
 
 
 def test__lc_merge_close_features_all_features_above_merge_threshold():
     n_samples = 10
     n_ft = 4
     ft_names = ["FT-{}".format(x) for x in range(n_ft)]
     samples = ["sample{}".format(x) for x in range(n_samples)]
     data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=ft_names,
-        index=samples
+        data=np.ones((n_samples, n_ft)), columns=ft_names, index=samples
     )
     ft_descriptors = [c.MZ, c.RT]
     feature_metadata = pd.DataFrame(
-        data=[[1, 1], [1.005, 1.005], [3, 3], [4, 4]],
-        columns=ft_descriptors,
-        index=ft_names
+        data=[[1, 1], [1.005, 1.005], [3, 3], [4, 4]], columns=ft_descriptors, index=ft_names
     )
 
     mz_merge = 0.01
     rt_merge = 0.01
     merge_threshold = 1.0
 
     expected_data_matrix = data_matrix.copy()
     expected_feature_metadata = feature_metadata.copy()
     _build_data_matrix._lc_merge_close_features(
-        data_matrix,
-        feature_metadata,
-        mz_merge,
-        rt_merge,
-        merge_threshold
+        data_matrix, feature_metadata, mz_merge, rt_merge, merge_threshold
     )
     assert expected_data_matrix.equals(data_matrix)
     merged = feature_metadata.pop(c.MERGED)
     assert expected_feature_metadata.equals(feature_metadata)
     assert (merged == "").all()
 
 
 def test__lc_merge_close_features_merge_one_feature():
     n_samples = 10
     n_ft = 4
     ft_names = ["FT-{}".format(x) for x in range(n_ft)]
     samples = ["sample{}".format(x) for x in range(n_samples)]
     data_matrix = pd.DataFrame(
-        data=np.ones((n_samples, n_ft)),
-        columns=ft_names,
-        index=samples
+        data=np.ones((n_samples, n_ft)), columns=ft_names, index=samples
     )
     ft_descriptors = [c.MZ, c.RT]
     feature_metadata = pd.DataFrame(
-        data=[[1, 1], [1.005, 1.005], [3, 3], [4, 4]],
-        columns=ft_descriptors,
-        index=ft_names
+        data=[[1, 1], [1.005, 1.005], [3, 3], [4, 4]], columns=ft_descriptors, index=ft_names
     )
 
     # set values in FT2 to nan
     main_ft = ft_names[0]
     merge_ft = ft_names[1]
     data_matrix.loc[samples[5:], merge_ft] = np.nan
 
     mz_merge = 0.01
     rt_merge = 0.01
     merge_threshold = 1.0
 
     expected_data_matrix = data_matrix.copy()
-    expected_data_matrix[main_ft] = (
-        expected_data_matrix[main_ft] +
-        expected_data_matrix[merge_ft].fillna(0)
-    )
+    expected_data_matrix[main_ft] = expected_data_matrix[main_ft] + expected_data_matrix[
+        merge_ft
+    ].fillna(0)
     expected_data_matrix.drop(columns=[merge_ft], inplace=True)
     expected_feature_metadata = feature_metadata.copy()
     expected_feature_metadata.drop(index=[merge_ft], inplace=True)
 
     _build_data_matrix._lc_merge_close_features(
-        data_matrix,
-        feature_metadata,
-        mz_merge,
-        rt_merge,
-        merge_threshold
+        data_matrix, feature_metadata, mz_merge, rt_merge, merge_threshold
     )
     assert expected_data_matrix.equals(data_matrix)
     merged = feature_metadata.pop(c.MERGED)
     expected_merged = pd.Series("", index=ft_names)
     expected_merged[main_ft] = merge_ft
     expected_merged.pop(merge_ft)
     assert expected_feature_metadata.equals(feature_metadata)
```

### Comparing `tidyms-0.6.3/tests/unit/test_consensus_annotation.py` & `tidyms-0.7.0/tests/unit/test_consensus_annotation.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_correspondence.py` & `tidyms-0.7.0/tests/unit/test_correspondence.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_data_container.py` & `tidyms-0.7.0/tests/unit/test_data_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from tidyms import container
-from tidyms._names import *
+from tidyms.container import DataContainer
+from tidyms import _constants as c
 import numpy as np
 import pandas as pd
 import pytest
 import os
 
 
 def test_class_getter(data_container_with_order):
@@ -11,15 +12,15 @@
     class_series = pd.Series(data=data.classes, index=data.classes.index)
     assert data.classes.equals(class_series)
 
 
 def test_class_setter(data_container_with_order):
     data = data_container_with_order
     class_series = pd.Series(data=data.classes, index=data.classes.index)
-    #set classes to an arbitrary value
+    # set classes to an arbitrary value
     data.classes = 4
     data.classes = class_series
     assert data.classes.equals(class_series)
 
 
 def test_batch_getter(data_container_with_order):
     data = data_container_with_order
@@ -29,19 +30,19 @@
 
 def test_batch_getter_no_batch_information(data_container_without_order):
     data = data_container_without_order
     with pytest.raises(container.BatchInformationError):
         data.batch
 
 
-def test_batch_setter(data_container_with_order):
+def test_batch_setter(data_container_with_order: DataContainer):
     data = data_container_with_order
     b = np.arange(data.data_matrix.shape[0])
-    batch_series = pd.Series(data=b, index=data.batch.index)
-    data.batch = b
+    batch_series = pd.Series(data=b, index=data.batch.index, dtype=data.batch.dtype)
+    data.batch = batch_series
     assert data.batch.equals(batch_series)
 
 
 def test_order_getter(data_container_with_order):
     data = data_container_with_order
     order_series = pd.Series(data=data.order, index=data.order.index)
     assert data.order.equals(order_series)
@@ -53,25 +54,23 @@
         data.order
 
 
 def test_order_setter(data_container_with_order):
     data = data_container_with_order
     # new order value
     order_series = pd.Series(
-        data=data.order + 1,
-        index=data.order.index,
-        dtype=data.order.dtype
+        data=data.order + 1, index=data.order.index, dtype=data.order.dtype
     )
     data.order = order_series
     assert (data.order == order_series).all()
 
 
 def test_id_getter(data_container_with_order):
     data = data_container_with_order
-    assert  np.equal(data.data_matrix.index.values, data.id.values).all()
+    assert np.equal(data.data_matrix.index.values, data.id.values).all()
 
 
 def test_is_valid_class_name_with_valid_names(data_container_with_order):
     data = data_container_with_order
     assert data.is_valid_class_name("healthy")
 
 
@@ -84,35 +83,39 @@
     data = data_container_with_order
     classes = ["bad_class_name_1", "bad_class_name_2"]
     assert not data.is_valid_class_name(classes)
 
 
 def test_mapping_setter(data_container_with_order):
     data = data_container_with_order
-    mapping = {"sample": ["healthy", "disease"],
-               "blank": ["blank"]}
-    expected_mapping = {"sample": ["healthy", "disease"],
-                        "blank": ["blank"], "qc": None, "zero": None,
-                        "suitability": None, "dqc": None}
+    mapping = {c.STUDY_TYPE: ["healthy", "disease"], c.BLANK_TYPE: ["blank"]}
+    expected_mapping = {
+        c.STUDY_TYPE: ["healthy", "disease"],
+        c.BLANK_TYPE: ["blank"],
+        c.QC_TYPE: None,
+        c.DQC_TYPE: None,
+    }
     data.mapping = mapping
     assert data.mapping == expected_mapping
 
 
 def test_mapping_setter_bad_sample_type(data_container_with_order):
     data = data_container_with_order
-    mapping = {"sample": ["healthy", "disease"],
-               "blank": ["SV"], "bad_sample_type": ["healthy"]}
+    mapping = {
+        "sample": ["healthy", "disease"],
+        "blank": ["SV"],
+        "bad_sample_type": ["healthy"],
+    }
     with pytest.raises(ValueError):
         data.mapping = mapping
 
 
 def test_mapping_setter_bad_sample_class(data_container_with_order):
     data = data_container_with_order
-    mapping = {"sample": ["healthy", "disease"],
-               "blank": ["SV", "bad_sample_class"]}
+    mapping = {"sample": ["healthy", "disease"], "blank": ["SV", "bad_sample_class"]}
     with pytest.raises(ValueError):
         data.mapping = mapping
 
 
 def test_remove_invalid_axis(data_container_with_order):
     data = data_container_with_order
     with pytest.raises(ValueError):
@@ -143,15 +146,15 @@
 
 def test_remove_correct_features(data_container_with_order):
     data = data_container_with_order
     features = data.data_matrix.columns.copy()
     rm_features = data.data_matrix.columns[[1, 2]]
     data.remove(rm_features, "features")
     assert data.data_matrix.columns.equals(features.difference(rm_features))
-    
+
 
 def test_equal_feature_index(data_container_with_order):
     data = data_container_with_order
     assert data.feature_metadata.index.equals(data.data_matrix.columns)
 
 
 def test_equal_sample_index(data_container_with_order):
@@ -196,44 +199,44 @@
     # remove all features
     data.remove(data.data_matrix.columns, "features")
     assert data.diagnose()["empty"]
 
 
 def test_diagnose_missing(data_container_with_order):
     data = data_container_with_order
-    assert  not data.diagnose()["missing"]
-    # set one column to nans
+    assert not data.diagnose()["missing"]
+    # set one column to nan
     data._data_matrix[data.data_matrix.columns[0]] = np.nan
     assert data.diagnose()["missing"]
     # reset data values
     data.reset()
 
 
 def test_diagnose_qc(data_container_with_order):
     data = data_container_with_order
-    assert data.diagnose()[_qc_sample_type]
+    assert data.diagnose()[c.QC_TYPE]
     # remove mapping info
     data.mapping = None
-    assert not data.diagnose()[_qc_sample_type]
+    assert not data.diagnose()[c.QC_TYPE]
 
 
 def test_diagnose_blank(data_container_with_order):
     data = data_container_with_order
-    assert data.diagnose()[_blank_sample_type]
+    assert data.diagnose()[c.BLANK_TYPE]
     # remove mapping info
     data.mapping = None
-    assert  not data.diagnose()[_blank_sample_type]
+    assert not data.diagnose()[c.BLANK_TYPE]
 
 
 def test_diagnose_sample(data_container_with_order):
     data = data_container_with_order
-    assert data.diagnose()[_study_sample_type]
+    assert data.diagnose()[c.STUDY_TYPE]
     # remove mapping info
     data.mapping = None
-    assert not data.diagnose()[_study_sample_type]
+    assert not data.diagnose()[c.STUDY_TYPE]
 
 
 def test_diagnose_run_order(data_container_with_order):
     data = data_container_with_order
     assert data.diagnose()["order"]
 
 
@@ -271,24 +274,24 @@
     data.reset()
 
     assert data.data_matrix.equals(original_dm)
     assert data.feature_metadata.equals(original_fm)
     assert data.sample_metadata.equals(original_sm)
 
 
-def test_select_featurest(data_container_with_order):
+def test_select_features(data_container_with_order):
     data = data_container_with_order
     # manually selected features
     mz_tol = 0.1
     mz_mask = np.abs(data.feature_metadata["mz"] - 200) < mz_tol
     rt_tol = 2
-    rt_mask = np.abs(data.feature_metadata["rt"] - 200)  < rt_tol
+    rt_mask = np.abs(data.feature_metadata["rt"] - 200) < rt_tol
     ft_mask = mz_mask & rt_mask
     ft_name = ft_mask[ft_mask].index
-    assert data.select_features(200, 200, 0.1 ,2).equals(ft_name)
+    assert data.select_features(200, 200, 0.1, 2).equals(ft_name)
 
 
 def test_set_default_order(data_container_without_order):
     data = data_container_without_order
     data.set_default_order()
     # this should not raise any exception
     data.order
@@ -340,26 +343,26 @@
     # test invalid mode
     with pytest.raises(ValueError):
         data.set_plot_mode("bad-plot-mode")
 
 
 def test_add_run_order_from_csv(tmpdir, data_container_without_order):
     data = data_container_without_order
-    order_data = pd.DataFrame(data=np.arange(data.data_matrix.shape[0]),
-                              columns=["order"])
+    order_data = pd.DataFrame(data=np.arange(data.data_matrix.shape[0]), columns=["order"])
     order_data["sample"] = data.data_matrix.index
     order_data["batch"] = 1
     save_path = os.path.join(tmpdir, "order.csv")
     order_data.to_csv(save_path)
     data.add_order_from_csv(save_path)
     assert True
 
 
 # test metrics
 
+
 def test_metrics_cv_no_groupby(data_container_with_order):
     data = data_container_with_order
     cv = data.metrics.cv(groupby=None)
     assert cv.size == data.data_matrix.shape[1]
 
 
 def test_metrics_cv_groupby_class(data_container_with_order):
@@ -434,81 +437,82 @@
     n_ft = data.data_matrix.shape[1]
     dr = data.metrics.detection_rate(groupby=["class", "batch"])
     assert dr.shape == (n_class * n_batch, n_ft)
 
 
 def test_metrics_pca(data_container_with_order):
     data = data_container_with_order
-    scores, loadings, pc_variance, total_variance = \
-        data.metrics.pca(n_components=None)
+    scores, loadings, pc_variance, total_variance = data.metrics.pca(n_components=None)
     # shape check for scores and loadings
     assert scores.shape[0] == data.data_matrix.shape[0]
     assert loadings.shape[0] == data.data_matrix.shape[1]
     # check variance calculation
     assert np.isclose(pc_variance.sum(), total_variance)
 
 
 def test_metrics_pca_n_components(data_container_with_order):
     n_comp = 3
     data = data_container_with_order
-    scores, loadings, pc_variance, total_variance = \
-        data.metrics.pca(n_components=n_comp)
+    scores, loadings, pc_variance, total_variance = data.metrics.pca(n_components=n_comp)
     # shape check for scores and loadings
     assert scores.shape[1] == n_comp
     assert scores.shape[0] == data.data_matrix.shape[0]
     assert loadings.shape[0] == data.data_matrix.shape[1]
 
 
 def test_metrics_pca_normalization(data_container_with_order):
     n_comp = 2
     data = data_container_with_order
-    scores, loadings, pc_variance, total_variance = \
-        data.metrics.pca(n_components=n_comp, normalization="sum")
+    scores, loadings, pc_variance, total_variance = data.metrics.pca(
+        n_components=n_comp, normalization="sum"
+    )
     # shape check for scores and loadings
     assert scores.shape[1] == n_comp
     assert scores.shape[0] == data.data_matrix.shape[0]
     assert loadings.shape[0] == data.data_matrix.shape[1]
 
 
 def test_metrics_pca_scaling(data_container_with_order):
     n_comp = 2
     data = data_container_with_order
-    scores, loadings, pc_variance, total_variance = \
-        data.metrics.pca(n_components=n_comp, scaling="autoscaling")
+    scores, loadings, pc_variance, total_variance = data.metrics.pca(
+        n_components=n_comp, scaling="autoscaling"
+    )
     # shape check for scores and loadings
     assert scores.shape[1] == n_comp
     assert scores.shape[0] == data.data_matrix.shape[0]
     assert loadings.shape[0] == data.data_matrix.shape[1]
 
 
 def test_metrics_pca_ignore_classes(data_container_with_order):
     n_comp = 2
     data = data_container_with_order
-    scores, loadings, pc_variance, total_variance = \
-        data.metrics.pca(n_components=n_comp, ignore_classes=["blank"])
+    scores, loadings, pc_variance, total_variance = data.metrics.pca(
+        n_components=n_comp, ignore_classes=["blank"]
+    )
     # shape check for scores and loadings
     assert scores.shape[1] == n_comp
     assert loadings.shape[0] == data.data_matrix.shape[1]
 
+
 def test_metrics_correlation_spearman(data_container_with_order):
     data = data_container_with_order
     r = data.metrics.correlation("order", mode="spearman")
     assert r.size == data.data_matrix.shape[1]
 
 
 def test_metrics_correlation_ols(data_container_with_order):
     data = data_container_with_order
     r = data.metrics.correlation("order", mode="ols")
     assert r.shape[1] == data.data_matrix.shape[1]
 
 
 def test_metrics_correlation_class(data_container_with_order):
     data = data_container_with_order
-    r = data.metrics.correlation("order", mode="ols",
-                                 classes=["healthy", "disease"])
+    r = data.metrics.correlation("order", mode="ols", classes=["healthy", "disease"])
     assert r.shape[1] == data.data_matrix.shape[1]
 
 
 def test_metrics_correlation_invalid_mode(data_container_with_order):
     data = data_container_with_order
     with pytest.raises(ValueError):
-        data.metrics.correlation("order", mode="invalid-mode")
+        data.metrics.correlation("order", mode="invalid-mode")
```

### Comparing `tidyms-0.6.3/tests/unit/test_fileio.py` & `tidyms-0.7.0/tests/unit/test_fileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     assert True
 
 
 def test_read_uncompressed_indexed_mzml():
     cache_path = get_tidyms_path()
     filename = "centroid-data-indexed-uncompressed.mzML"
     data_path = os.path.join(cache_path, "test-raw-data", filename)
-    ms_data = fileio.MSData(data_path)
+    ms_data = fileio.MSData.create_MSData_instance(data_path)
     n_spectra = ms_data.get_n_spectra()
     n_chromatogram = ms_data.get_n_chromatograms()
 
     # test spectra
     for k in range(n_spectra):
         ms_data.get_spectrum(k)
 
@@ -83,15 +83,15 @@
     assert True
 
 
 def test_read_compressed_no_index_mzml():
     cache_path = get_tidyms_path()
     filename = "centroid-data-zlib-no-index-compressed.mzML"
     data_path = os.path.join(cache_path, "test-raw-data", filename)
-    ms_data = fileio.MSData(data_path)
+    ms_data = fileio.MSData.create_MSData_instance(data_path)
     n_spectra = ms_data.get_n_spectra()
     n_chromatogram = ms_data.get_n_chromatograms()
 
     # test spectra
     for k in range(n_spectra):
         ms_data.get_spectrum(k)
```

### Comparing `tidyms-0.6.3/tests/unit/test_fill_missing.py` & `tidyms-0.7.0/tests/unit/test_fill_missing.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,85 +9,69 @@
     rt = 50
     rt_std = 10
     n_dev = 1
 
     def mock_extract_features(self, **kwargs):
         self.features = list()
 
-    monkeypatch.setattr(
-        ms.Chromatogram,
-        "extract_features",
-        mock_extract_features
-    )
+    monkeypatch.setattr(ms.Chromatogram, "extract_features", mock_extract_features)
 
     area = ms.fill_missing._get_fill_area(chromatogram, rt, rt_std, n_dev)
     assert area is None
 
 
 def test_get_fill_area_peak_detected_outside_valid_range(monkeypatch):
     time = np.arange(100)
     spint = np.ones_like(time)
     chromatogram = ms.Chromatogram(time, spint)
     rt = 50
     rt_std = 10
     n_dev = 1
 
     def mock_extract_features(self, **kwargs):
-        self.features = [ms.lcms.Peak(70, 75, 80)]
+        self.features = [ms.lcms.Peak(70, 75, 80, self)]
 
-    monkeypatch.setattr(
-        ms.Chromatogram,
-        "extract_features",
-        mock_extract_features
-    )
+    monkeypatch.setattr(ms.Chromatogram, "extract_features", mock_extract_features)
 
     area = ms.fill_missing._get_fill_area(chromatogram, rt, rt_std, n_dev)
     assert area is None
 
 
 def test_get_fill_area_peak_detected_inside_valid_range(monkeypatch):
     time = np.arange(100)
     spint = np.ones_like(time)
     chromatogram = ms.Chromatogram(time, spint)
     chromatogram.baseline = np.zeros_like(time)
     rt = 50
     rt_std = 10
     n_dev = 1
-    test_peak = ms.lcms.Peak(50, 55, 60)
-    expected_area = test_peak.get_area(chromatogram)
+    test_peak = ms.lcms.Peak(50, 55, 60, chromatogram)
+    expected_area = test_peak.get_area()
 
     def mock_extract_features(self, **kwargs):
         self.features = [test_peak]
 
-    monkeypatch.setattr(
-        ms.Chromatogram,
-        "extract_features",
-        mock_extract_features
-    )
+    monkeypatch.setattr(ms.Chromatogram, "extract_features", mock_extract_features)
 
     area = ms.fill_missing._get_fill_area(chromatogram, rt, rt_std, n_dev)
     assert np.isclose(area, expected_area)
 
 
 def test_get_fill_area_multiple_valid_peaks_choose_closest(monkeypatch):
     time = np.arange(100)
     spint = np.ones_like(time)
     chromatogram = ms.Chromatogram(time, spint)
     chromatogram.baseline = np.zeros_like(time)
     rt = 50
     rt_std = 10
     n_dev = 1
-    valid_peak = ms.lcms.Peak(45, 50, 52)
-    detected_peaks = [valid_peak, ms.lcms.Peak(55, 60, 65)]
-    expected_area = valid_peak.get_area(chromatogram)
+    valid_peak = ms.lcms.Peak(45, 50, 52, chromatogram)
+    detected_peaks = [valid_peak, ms.lcms.Peak(55, 60, 65, chromatogram)]
+    expected_area = valid_peak.get_area()
 
     def mock_extract_features(self, **kwargs):
         self.features = detected_peaks
 
-    monkeypatch.setattr(
-        ms.Chromatogram,
-        "extract_features",
-        mock_extract_features
-    )
+    monkeypatch.setattr(ms.Chromatogram, "extract_features", mock_extract_features)
 
     area = ms.fill_missing._get_fill_area(chromatogram, rt, rt_std, n_dev)
-    assert np.isclose(area, expected_area)
+    assert np.isclose(area, expected_area)
```

### Comparing `tidyms-0.6.3/tests/unit/test_peaks.py` & `tidyms-0.7.0/tests/unit/test_peaks.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_raw_data_utils.py` & `tidyms-0.7.0/tests/unit/test_raw_data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tidyms.fileio import SimulatedMSData
+from tidyms.fileio import MSData_simulated
 from tidyms.lcms import Chromatogram
 from tidyms.raw_data_utils import _match_mz
 import pytest
 import numpy as np
 import tidyms as ms
 
 
@@ -13,44 +13,38 @@
 def sim_ms_data():
     mz = np.array(mz_list)
     rt = np.linspace(0, 100, 100)
 
     # simulated features params
     mz_params = np.array([mz_list, [3, 10, 5, 31, 22]])
     mz_params = mz_params.T
-    rt_params = np.array(
-        [[30, 40, 60, 80, 80], [1, 2, 2, 3, 3], [1, 1, 1, 1, 1]]
-    )
+    rt_params = np.array([[30, 40, 60, 80, 80], [1, 2, 2, 3, 3], [1, 1, 1, 1, 1]])
     rt_params = rt_params.T
 
     noise_level = 0.1
-    sim_exp = SimulatedMSData(mz, rt, mz_params, rt_params, noise=noise_level)
+    sim_exp = MSData_simulated(mz, rt, mz_params, rt_params, noise=noise_level)
     return sim_exp
 
 
 def test_make_roi(sim_ms_data):
-    roi_list = ms.make_roi(
-        sim_ms_data,
-        tolerance=0.005,
-        max_missing=0,
-        min_length=1
-    )
+    roi_list = ms.make_roi(sim_ms_data, tolerance=0.005, max_missing=0, min_length=1)
     assert len(roi_list) == sim_ms_data._reader.mz_params.shape[0]
 
 
 def test_make_roi_targeted_mz(sim_ms_data):
     # the first three m/z values generated by simulated experiment are used
     targeted_mz = sim_ms_data._reader.mz_params[:, 0][:3]
     roi_list = ms.make_roi(
         sim_ms_data,
         tolerance=0.005,
         max_missing=0,
         min_length=1,
         min_intensity=0,
-        targeted_mz=targeted_mz)
+        targeted_mz=targeted_mz,
+    )
     assert len(roi_list) == targeted_mz.size
 
 
 def test_make_roi_min_intensity(sim_ms_data):
     min_intensity = 15
     roi_list = ms.make_roi(
         sim_ms_data,
@@ -61,97 +55,84 @@
     )
     # only two roi should have intensities greater than 15
     assert len(roi_list) == 2
 
 
 def test_make_roi_multiple_match_closest(sim_ms_data):
     roi_list = ms.make_roi(
-        sim_ms_data,
-        tolerance=0.005,
-        max_missing=0,
-        min_length=1,
-        multiple_match="closest")
+        sim_ms_data, tolerance=0.005, max_missing=0, min_length=1, multiple_match="closest"
+    )
     assert len(roi_list) == sim_ms_data._reader.mz_params.shape[0]
 
 
 def test_make_roi_multiple_match_reduce_merge(sim_ms_data):
     # set a tolerance such that two mz values are merged
     # test is done in targeted mode to force a multiple match by removing
     # one of the mz values
     targeted_mz = sim_ms_data._reader.mz_params[:, 0]
     targeted_mz = np.delete(targeted_mz, 3)
     tolerance = 31
     roi_list = ms.make_roi(
-        sim_ms_data,
-        tolerance=tolerance,
-        max_missing=0,
-        min_length=1,
-        targeted_mz=targeted_mz)
+        sim_ms_data, tolerance=tolerance, max_missing=0, min_length=1, targeted_mz=targeted_mz
+    )
     assert len(roi_list) == (sim_ms_data._reader.mz_params.shape[0] - 1)
 
 
 def test_make_roi_multiple_match_reduce_custom_mz_reduce(sim_ms_data):
     roi_list = ms.make_roi(
-        sim_ms_data,
-        tolerance=0.005,
-        max_missing=0,
-        min_length=1,
-        mz_reduce=np.median
+        sim_ms_data, tolerance=0.005, max_missing=0, min_length=1, mz_reduce=np.median
     )
     assert len(roi_list) == sim_ms_data._reader.mz_params.shape[0]
 
 
 def test_make_roi_multiple_match_reduce_custom_sp_reduce(sim_ms_data):
     roi_list = ms.make_roi(
-        sim_ms_data,
-        tolerance=0.005,
-        max_missing=0,
-        min_length=1,
-        sp_reduce=lambda x: 1
+        sim_ms_data, tolerance=0.005, max_missing=0, min_length=1, sp_reduce=lambda x: 1
     )
     assert len(roi_list) == sim_ms_data._reader.mz_params.shape[0]
 
 
 def test_make_roi_invalid_multiple_match(sim_ms_data):
     with pytest.raises(ValueError):
         ms.make_roi(
             sim_ms_data,
             tolerance=0.005,
             max_missing=0,
             min_length=0,
-            multiple_match="invalid-value"
+            multiple_match="invalid-value",
         )
 
 
 # # test accumulate spectra
 
+
 def test_accumulate_spectra_centroid(sim_ms_data):
     start_time = sim_ms_data._reader.rt.min()
     end_time = sim_ms_data._reader.rt.max()
-    sp = ms.accumulate_spectra(
-        sim_ms_data, start_time=start_time, end_time=end_time)
+    sp = ms.accumulate_spectra(sim_ms_data, start_time=start_time, end_time=end_time)
     assert sp.mz.size == sim_ms_data._reader.mz_params.shape[0]
 
 
 def test_accumulate_spectra_centroid_subtract_left(sim_ms_data):
     start_time = sim_ms_data._reader.rt[70]
     end_time = sim_ms_data._reader.rt[90]
     subtract_left_time = sim_ms_data._reader.rt[20]
     sp = ms.accumulate_spectra(
         sim_ms_data,
         start_time=start_time,
         end_time=end_time,
-        subtract_left_time=subtract_left_time
+        subtract_left_time=subtract_left_time,
     )
     # only two peaks at rt 80 should be present
     assert sp.mz.size == 2
 
 
 # test make_chromatogram
 
+
 def test_make_chromatograms(sim_ms_data):
     # test that the chromatograms generated are valid
 
     # create chromatograms
     n_sp = sim_ms_data.get_n_spectra()
     n_mz = sim_ms_data._reader.mz_params.shape[0]
     rt = np.zeros(n_sp)
@@ -182,14 +163,15 @@
 def test_make_tic_bpi(sim_ms_data):
     ms.make_tic(sim_ms_data, kind="bpi")
     assert True
 
 
 # Test _RoiMaker
 
+
 def test_TempRoi_creation():
     troi = ms.raw_data_utils._TempRoi()
     assert len(troi.mz) == 0
     assert len(troi.spint) == 0
     assert len(troi.scan) == 0
 
 
@@ -294,20 +276,17 @@
 def test_TempRoi_convert_to_roi_di_roi():
     troi = ms.raw_data_utils._TempRoi()
     troi.append(1, 1, 2)
     troi.append(1, 1, 4)
     troi.append(1, 1, 5)
     scans = np.arange(6)
     time = np.arange(6)
-    roi = troi.convert_to_roi(time, scans, "di")
-
-    assert np.array_equal(roi.scan, [2, 3, 4, 5])
-    assert np.allclose(roi.time, [2, 3, 4, 5])
-    assert np.allclose(roi.mz, [1, np.nan, 1, 1], equal_nan=True)
-    assert np.allclose(roi.spint, [1, np.nan, 1, 1], equal_nan=True)
+    with pytest.raises(NotImplementedError):
+        # TODO: FIX after implementing DI ROI creation
+        troi.convert_to_roi(time, scans, "di")
 
 
 def test_RoiList_creation():
     roi_list = ms.raw_data_utils._TempRoiList()
     assert True
 
 
@@ -335,15 +314,15 @@
         assert r.scan[-1] == scan
 
 
 def test_RoiList_two_consecutive_insert():
     roi_list = ms.raw_data_utils._TempRoiList()
     # first insert
     scan1 = 1
-    mz1 = np.array([0, 1, 2, 3, 4, 6, 7, 9])     # 5 and 8 are missing
+    mz1 = np.array([0, 1, 2, 3, 4, 6, 7, 9])  # 5 and 8 are missing
     spint1 = mz1.copy()
     roi_list.insert(mz1, spint1, scan1)
 
     # second insert
     scan2 = 2
     mz2 = np.array([5, 8])
     spint2 = mz2.copy()
@@ -354,15 +333,15 @@
     expected_missing_count = np.zeros_like(roi_list.missing_count)
     expected_missing_count[mz1] = 1
     assert np.allclose(roi_list.mz_mean, expected_mz)
     assert np.allclose(roi_list.mz_sum, expected_mz)
     assert np.allclose(roi_list.max_int, expected_mz)
     assert (roi_list.length == 1).all()
     assert (roi_list.missing_count == 0).all()
-    assert (np.diff(roi_list.mz_mean) >= 0).all()   # check is sorted
+    assert (np.diff(roi_list.mz_mean) >= 0).all()  # check is sorted
 
     # check roi values
     # values for mz and spint should be 0, 1, 2, 3, ...
     for expected, r in enumerate(roi_list.roi):
         assert r.mz[-1] == expected
         assert r.spint[-1] == expected
         if expected in [5, 8]:
@@ -563,15 +542,15 @@
         mz_seed,
         max_missing,
         min_length,
         min_intensity,
         tolerance,
         multiple_match,
         mz_reduce,
-        sp_reduce
+        sp_reduce,
     )
     assert np.array_equal(processor.mz_filter, mz_seed)
     assert processor.max_missing == max_missing
     assert processor.min_length == min_length
     assert processor.min_intensity == min_intensity
     assert processor.tolerance == tolerance
     assert processor.multiple_match == multiple_match
@@ -593,29 +572,31 @@
         mz_seed,
         max_missing,
         min_length,
         min_intensity,
         tolerance,
         multiple_match,
         mz_reduce,
-        sp_reduce
+        sp_reduce,
     )
 
+
 def test_RoiProcessor_feed_spectrum_empty_processor_no_mz_filter(roi_processor):
     n = 5
     mz = np.arange(n)
     sp = np.arange(n)
     scan = 1
     roi_processor.feed_spectrum(mz, sp, scan)
 
     assert np.allclose(roi_processor.tmp_roi_list.mz_mean, mz)
     assert np.allclose(roi_processor.tmp_roi_list.max_int, sp)
     assert (roi_processor.tmp_roi_list.length == 1).all()
     assert (roi_processor.tmp_roi_list.missing_count == 0).all()
 
+
 def test_RoiProcessor_feed_spectrum_empty_processor_mz_filter(roi_processor):
 
     mz_filter = np.array([0, 1, 2, 3])
     roi_processor.mz_filter = mz_filter
     n = 5
     mz = np.arange(n)
     sp = np.arange(n)
@@ -644,17 +625,15 @@
     expected_max_int = expected_mz_mean
     expected_missing_count = np.array([1, 1, 1, 0, 0, 0, 0])
     expected_length = np.array([1, 1, 1, 2, 2, 1, 1])
 
     assert np.allclose(roi_processor.tmp_roi_list.mz_mean, expected_mz_mean)
     assert np.allclose(roi_processor.tmp_roi_list.max_int, expected_max_int)
     assert np.array_equal(roi_processor.tmp_roi_list.length, expected_length)
-    assert np.array_equal(
-        roi_processor.tmp_roi_list.missing_count, expected_missing_count
-    )
+    assert np.array_equal(roi_processor.tmp_roi_list.missing_count, expected_missing_count)
 
 
 def test_RoiProcessor_feed_spectrum_mz_filter(roi_processor):
 
     mz_filter = np.array([1, 2, 3, 4])
     roi_processor.mz_filter = mz_filter
 
@@ -673,22 +652,18 @@
     expected_max_int = expected_mz_mean
     expected_missing_count = np.array([1, 1, 0, 0])
     expected_length = np.array([1, 1, 2, 2])
 
     assert np.allclose(roi_processor.tmp_roi_list.mz_mean, expected_mz_mean)
     assert np.allclose(roi_processor.tmp_roi_list.max_int, expected_max_int)
     assert np.array_equal(roi_processor.tmp_roi_list.length, expected_length)
-    assert np.array_equal(
-        roi_processor.tmp_roi_list.missing_count, expected_missing_count
-    )
+    assert np.array_equal(roi_processor.tmp_roi_list.missing_count, expected_missing_count)
 
 
-def test_RoiProcessor_clear_completed_roi_min_intensity_None_min_length_None(
-    roi_processor
-):
+def test_RoiProcessor_clear_completed_roi_min_intensity_None_min_length_None(roi_processor):
     n = 5
     mz1 = np.arange(n)
     sp1 = np.arange(n)
     scan1 = 1
     roi_processor.feed_spectrum(mz1, sp1, scan1)
 
     mz2 = np.array([3, 4, 5, 6])
@@ -702,23 +677,19 @@
     expected_mz_mean = np.arange(7)
     expected_max_int = np.array([0, 0, 0, 3, 4, 5, 6])
     expected_missing_count = np.array([0, 0, 0, 0, 0, 0, 0])
     expected_length = np.array([0, 0, 0, 3, 3, 2, 2])
     assert np.allclose(roi_processor.tmp_roi_list.mz_mean, expected_mz_mean)
     assert np.allclose(roi_processor.tmp_roi_list.max_int, expected_max_int)
     assert np.array_equal(roi_processor.tmp_roi_list.length, expected_length)
-    assert np.array_equal(
-        roi_processor.tmp_roi_list.missing_count, expected_missing_count
-    )
+    assert np.array_equal(roi_processor.tmp_roi_list.missing_count, expected_missing_count)
     assert len(roi_processor.valid_roi) == 3
 
 
-def test_RoiProcessor_clear_completed_roi_min_intensity_int_min_length_None(
-    roi_processor
-):
+def test_RoiProcessor_clear_completed_roi_min_intensity_int_min_length_None(roi_processor):
     roi_processor.min_intensity = 2
     n = 5
     mz1 = np.arange(n)
     sp1 = np.arange(n)
     scan1 = 1
     roi_processor.feed_spectrum(mz1, sp1, scan1)
 
@@ -733,29 +704,25 @@
     expected_mz_mean = np.arange(7)
     expected_max_int = np.array([0, 0, 0, 3, 4, 5, 6])
     expected_missing_count = np.array([0, 0, 0, 0, 0, 0, 0])
     expected_length = np.array([0, 0, 0, 3, 3, 2, 2])
     assert np.allclose(roi_processor.tmp_roi_list.mz_mean, expected_mz_mean)
     assert np.allclose(roi_processor.tmp_roi_list.max_int, expected_max_int)
     assert np.array_equal(roi_processor.tmp_roi_list.length, expected_length)
-    assert np.array_equal(
-        roi_processor.tmp_roi_list.missing_count, expected_missing_count
-    )
+    assert np.array_equal(roi_processor.tmp_roi_list.missing_count, expected_missing_count)
     # using a min intensity filter of 2, only the ROI generated from mz1 = 2,
     # sp2 = 2 should be valid
     assert len(roi_processor.valid_roi) == 1
     roi = roi_processor.valid_roi[0]
     assert np.allclose(roi.mz[0], 2.0)
     assert np.allclose(roi.spint[0], 2.0)
     assert np.allclose(roi.scan[0], 1)
 
 
-def test_RoiProcessor_clear_completed_roi_min_intensity_int_min_length_int(
-    roi_processor
-):
+def test_RoiProcessor_clear_completed_roi_min_intensity_int_min_length_int(roi_processor):
     roi_processor.min_intensity = 2
     roi_processor.min_length = 2
     n = 5
     mz1 = np.arange(n)
     sp1 = np.arange(n)
     scan1 = 1
     roi_processor.feed_spectrum(mz1, sp1, scan1)
@@ -771,17 +738,15 @@
     expected_mz_mean = np.arange(7)
     expected_max_int = np.array([0, 0, 0, 3, 4, 5, 6])
     expected_missing_count = np.array([0, 0, 0, 0, 0, 0, 0])
     expected_length = np.array([0, 0, 0, 3, 3, 2, 2])
     assert np.allclose(roi_processor.tmp_roi_list.mz_mean, expected_mz_mean)
     assert np.allclose(roi_processor.tmp_roi_list.max_int, expected_max_int)
     assert np.array_equal(roi_processor.tmp_roi_list.length, expected_length)
-    assert np.array_equal(
-        roi_processor.tmp_roi_list.missing_count, expected_missing_count
-    )
+    assert np.array_equal(roi_processor.tmp_roi_list.missing_count, expected_missing_count)
     # using a min length filter of 2, all cleared ROI are invalid
     assert len(roi_processor.valid_roi) == 0
 
 
 def test_RoiProcessor_flag_as_completed(roi_processor):
     n = 5
     mz1 = np.arange(n)
@@ -826,16 +791,17 @@
     mz2 = np.array([40, 51, 78, 91, 99, 130, 150])
     sp2 = np.array([100] * mz2.size)
     # expected values for match/no match indices
     mz1_match_index = np.array([0, 2, 4], dtype=int)
     mz2_match_index = np.array([1, 4, 6], dtype=int)
     mz2_no_match_index = np.array([0, 2, 3, 5], dtype=int)
     mode = "closest"
-    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = \
-        _match_mz(mz1, mz2, sp2, tolerance, mode, np.mean, np.mean)
+    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = _match_mz(
+        mz1, mz2, sp2, tolerance, mode, np.mean, np.mean
+    )
     # test match index
     assert np.array_equal(mz1_match_index, test_mz1_index)
     # test match mz and sp values
     assert np.array_equal(mz2[mz2_match_index], mz2_match)
     assert np.array_equal(sp2[mz2_match_index], sp2_match)
     # test no match mz and sp values
     assert np.array_equal(mz2[mz2_no_match_index], mz2_no_match)
@@ -848,16 +814,17 @@
     mz2 = np.array([40, 53, 78, 91, 97, 130, 154])
     sp2 = np.array([100] * mz2.size)
     # expected values for match/no match indices
     mz1_match_index = np.array([], dtype=int)
     mz2_match_index = np.array([], dtype=int)
     mz2_no_match_index = np.array([0, 1, 2, 3, 4, 5, 6], dtype=int)
     mode = "closest"
-    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = \
-        _match_mz(mz1, mz2, sp2, tolerance, mode, np.mean, np.mean)
+    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = _match_mz(
+        mz1, mz2, sp2, tolerance, mode, np.mean, np.mean
+    )
     # test match index
     assert np.array_equal(mz1_match_index, test_mz1_index)
     # test match mz and sp values
     assert np.array_equal(mz2[mz2_match_index], mz2_match)
     assert np.array_equal(sp2[mz2_match_index], sp2_match)
     # test no match mz and sp values
     assert np.array_equal(mz2[mz2_no_match_index], mz2_no_match)
@@ -870,16 +837,17 @@
     mz2 = np.array([51, 77, 99, 126, 150])
     sp2 = np.array([100] * mz2.size)
     # expected values for match/no match indices
     mz1_match_index = np.array([0, 1, 2, 3, 4], dtype=int)
     mz2_match_index = np.array([0, 1, 2, 3, 4], dtype=int)
     mz2_no_match_index = np.array([], dtype=int)
     mode = "closest"
-    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = \
-        _match_mz(mz1, mz2, sp2, tolerance, mode, np.mean, np.mean)
+    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = _match_mz(
+        mz1, mz2, sp2, tolerance, mode, np.mean, np.mean
+    )
     # test match index
     assert np.array_equal(mz1_match_index, test_mz1_index)
     # test match mz and sp values
     assert np.array_equal(mz2[mz2_match_index], mz2_match)
     assert np.array_equal(sp2[mz2_match_index], sp2_match)
     # test no match mz and sp values
     assert np.array_equal(mz2[mz2_no_match_index], mz2_no_match)
@@ -895,16 +863,17 @@
     # in `closest` mode, argmin is used to select the closest value. If more
     # than one value has the same difference, the first one in the array is
     # going to be selected.
     mz1_match_index = np.array([0, 2, 3, 4], dtype=int)
     mz2_match_index = np.array([0, 4, 6, 7], dtype=int)
     mz2_no_match_index = np.array([1, 2, 3, 5, 8], dtype=int)
     mode = "closest"
-    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = \
-        _match_mz(mz1, mz2, sp2, tolerance, mode, np.mean, np.mean)
+    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = _match_mz(
+        mz1, mz2, sp2, tolerance, mode, np.mean, np.mean
+    )
     # test match index
     assert np.array_equal(mz1_match_index, test_mz1_index)
     # test match mz and sp values
     assert np.array_equal(mz2[mz2_match_index], mz2_match)
     assert np.array_equal(sp2[mz2_match_index], sp2_match)
     # test no match mz and sp values
     assert np.array_equal(mz2[mz2_no_match_index], mz2_no_match)
@@ -922,16 +891,17 @@
     # going to be selected.
     mz1_match_index = np.array([0, 2, 3, 4], dtype=int)
     mz2_match_index = np.array([0, 1, 3, 4, 5, 6, 7, 8], dtype=int)
     mz2_no_match_index = np.array([2], dtype=int)
     expected_mz2_match = [50.0, 100.0, 126.0, 150.5]
     expected_sp2_match = [200, 300, 100, 200]
     mode = "reduce"
-    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = \
-        _match_mz(mz1, mz2, sp2, tolerance, mode, np.mean, np.sum)
+    test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = _match_mz(
+        mz1, mz2, sp2, tolerance, mode, np.mean, np.sum
+    )
     # test match index
     assert np.array_equal(mz1_match_index, test_mz1_index)
     # test match mz and sp values
     assert np.allclose(mz2_match, expected_mz2_match)
     assert np.allclose(sp2_match, expected_sp2_match)
     # test no match mz and sp values
     assert np.array_equal(mz2[mz2_no_match_index], mz2_no_match)
@@ -948,13 +918,15 @@
     # than one value has the same difference, the first one in the array is
     # going to be selected.
     mz1_match_index = np.array([0, 2, 3, 4], dtype=int)
     mz2_match_index = np.array([0, 4, 6, 7], dtype=int)
     mz2_no_match_index = np.array([1, 2, 3, 5, 8], dtype=int)
     mode = "invalid-mode"
     with pytest.raises(ValueError):
-        test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = \
-            _match_mz(mz1, mz2, sp2, tolerance, mode, np.mean, np.mean)
+        test_mz1_index, mz2_match, sp2_match, mz2_no_match, sp2_no_match = _match_mz(
+            mz1, mz2, sp2, tolerance, mode, np.mean, np.mean
+        )
+
 
 # def test_accumulate_spectra_profile(profile_mzml):
 #     sp = ms.accumulate_spectra(profile_mzml, start_time=5, end_time=10)
 #     assert sp.mz.size == sp.spint.size
```

### Comparing `tidyms-0.6.3/tests/unit/test_utils.py` & `tidyms-0.7.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_validation.py` & `tidyms-0.7.0/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_chem/test_atoms.py` & `tidyms-0.7.0/tests/unit/test_chem/test_atoms.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_chem/test_formula.py` & `tidyms-0.7.0/tests/unit/test_chem/test_formula.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_chem/test_formula_generator.py` & `tidyms-0.7.0/tests/unit/test_chem/test_formula_generator.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_chem/test_isotope_distributions.py` & `tidyms-0.7.0/tests/unit/test_chem/test_isotope_distributions.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_chem/test_isotope_scorer.py` & `tidyms-0.7.0/tests/unit/test_chem/test_isotope_scorer.py`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/tests/unit/test_chem/test_mmi_finder.py` & `tidyms-0.7.0/tests/unit/annotation/test_mmi_finder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from tidyms.chem import mmi_finder
+from tidyms.annotation import mmi_finder
+from tidyms.annotation.annotation_data import AnnotationData
 from tidyms.chem import PeriodicTable
+from tidyms.lcms import LCTrace, Peak
 import pytest
 import numpy as np
+from typing import Sequence
 
 
 def test__select_two_isotope_elements_dm_1_p0_greater_than_pi():
     elements = ["C", "H", "N", "O", "P", "S"]
     expected = ["C"]
     custom_abundances = dict()
     dm = 1
@@ -112,231 +115,168 @@
 def test__select_multiple_isotope_elements_no_elements():
     elements = ["Cl", "H", "N", "P"]
     expected = []
     res = mmi_finder._select_multiple_isotope_elements(elements)
     assert len(res) == len(expected)
     assert set(res) == set(expected)
 
+
 @pytest.mark.parametrize(
     "elements,expected",
     [
-        [
-            ["C", "H", "N", "O", "P", "S"],
-            ["C", "O", "S"]
-        ],
-        [
-            ["C", "H", "N", "O", "P", "S", "Cl", "Li", "Na"],
-            ["C", "O", "S", "Li", "Cl"]
-        ]
-
-     ]
+        [["C", "H", "N", "O", "P", "S"], ["C", "O", "S"]],
+        [["C", "H", "N", "O", "P", "S", "Cl", "Li", "Na"], ["C", "O", "S", "Li", "Cl"]],
+    ],
 )
 def test__select_elements(elements, expected):
     res = mmi_finder._select_elements(elements)
     res = [x.symbol for x in res]
     assert len(res) == len(expected)
     assert set(res) == set(expected)
 
 
-# @pytest.mark.parametrize("e2", ["Na", "P"])
-# def test__is_distort_envelope_e2_monoisotope(e2):
-#     e1 = PeriodicTable().get_element("C")
-#     e2 = PeriodicTable().get_element(e2)
-#     assert not mmi_finder._is_distort_envelope(e1, e2)
-#
-#
-# @pytest.mark.parametrize("e2", ["O", "S"])
-# def test__is_distort_envelope_different_n_isotopes(e2):
-#     e1 = PeriodicTable().get_element("C")
-#     e2 = PeriodicTable().get_element(e2)
-#     assert mmi_finder._is_distort_envelope(e1, e2)
-#
-#
-# @pytest.mark.parametrize("e2", ["Cl", "Br"])
-# def test__is_distort_envelope_different_nominal_mass_increments(e2):
-#     e1 = PeriodicTable().get_element("C")
-#     e2 = PeriodicTable().get_element(e2)
-#     assert mmi_finder._is_distort_envelope(e1, e2)
-#
-#
-# @pytest.mark.parametrize("e2", ["H", "N"])
-# def test__is_distort_envelope_equal_envelopes_e2_dont_distort(e2):
-#     e1 = PeriodicTable().get_element("C")
-#     e2 = PeriodicTable().get_element(e2)
-#     assert not mmi_finder._is_distort_envelope(e1, e2)
-#
-#
-# @pytest.mark.parametrize("e2", ["B", "Li"])
-# def test__is_distort_envelope_equal_envelopes_e2_distort(e2):
-#     e1 = PeriodicTable().get_element("C")
-#     e2 = PeriodicTable().get_element(e2)
-#     assert mmi_finder._is_distort_envelope(e1, e2)
-#
-#
-# def test__get_relevant_elements():
-#     e_list = ["C", "H", "N", "O", "P", "S", "Li", "Na"]
-#     e_list = [PeriodicTable().get_element(x) for x in e_list]
-#     expected = ["C", "O", "S", "Li"]
-#     expected = [PeriodicTable().get_element(x) for x in expected]
-#     res = mmi_finder._get_relevant_elements(e_list)
-#     assert set(res) == set(expected)
-
-
-@pytest.mark.parametrize("max_charge", [1, 2, 3, 4])
-def test__get_monoisotopic_mass_candidates_positive_max_charge(max_charge):
-    max_mass = 2000.0
-    mono_M = 250.0
-    polarity = 1
-    # all possible values should be lower than max_mass
-    expected_charge = np.arange(1, abs(max_charge) + 1)
-    expected_M = expected_charge * mono_M
-    test_M, test_charge = mmi_finder._get_valid_mono_mass(
-        mono_M, max_charge, polarity, max_mass)
-    assert np.allclose(expected_M, test_M)
-    assert np.array_equal(expected_charge, test_charge)
-
-
-@pytest.mark.parametrize("max_charge", [1, 2, 3, 4])
-def test__get_monoisotopic_mass_candidates_negative_max_charge(max_charge):
-    max_mass = 2000.0
-    mono_M = 250.0
-    polarity = -1
-    # all possible values should be lower than max_mass
-    expected_charge = np.arange(1, abs(max_charge) + 1)
-    expected_M = np.abs(expected_charge) * mono_M
-    test_M, test_charge = mmi_finder._get_valid_mono_mass(
-        mono_M, max_charge, polarity, max_mass)
-    assert np.allclose(expected_M, test_M)
-    assert np.array_equal(expected_charge, test_charge)
-
-
-def test__get_monoisotopic_mass_candidates_mono_mass_greater_than_max_mass():
-    max_mass = 2000.0
-    mono_M = 900.0
-    # valid charges should be 1 and 2.
-    max_charge = 3
-    expected_charge = np.arange(1, 3)
-    polarity = 1
-    expected_M = expected_charge * mono_M
-    test_M, test_charge = mmi_finder._get_valid_mono_mass(
-        mono_M, max_charge, polarity, max_mass)
-    assert np.allclose(expected_M, test_M)
-    assert np.array_equal(expected_charge, test_charge)
-
-
 @pytest.fixture
 def rules():
-    bounds = {
-        "C": (0, 108),
-        "H": (0, 100),
-        "S": (0, 8),
-        "Cl": (0, 2)
-    }
+    bounds = {"C": (0, 108), "H": (0, 100), "S": (0, 8), "Cl": (0, 2)}
     max_mass = 2000.0
     length = 5
     bin_size = 100
     p_tol = 0.05
     r = mmi_finder._create_rules_dict(bounds, max_mass, length, bin_size, p_tol, None)
     return r, max_mass, length, bin_size
 
 
+def create_peak_list(mz: list[float], sp: list[float]) -> Sequence[Peak]:
+    peak_list = list()
+    size = 30
+    time = np.linspace(0, size, size)
+    scan = np.arange(size)
+    spint = np.ones(size)
+    for k_mz, k_sp in zip(mz, sp):
+        roi = LCTrace(time.copy(), spint * k_sp, spint * k_mz, scan)
+        peak = Peak(10, 15, 20, roi)
+        peak_list.append(peak)
+    return peak_list
+
+
 def test__find_candidates(rules):
     rules, max_mass, length, bin_size = rules
     # create an m/z and sp list where the monoisotopic m/z is the M1 in the
     # isotopic envelope.
+
     _, M_cl, _ = PeriodicTable().get_element("Cl").get_abundances()
     dm_cl = M_cl[1] - M_cl[0]
     mono_mz = 400.0
     charge = 1
     mono_index = 3
-    mz = np.array([100.0, 300.0, mono_mz - dm_cl, mono_mz, 456.0])
-    sp = np.array([100.0, 200.0, 500.0, 501.0, 34.0])
-    mono_sp = sp[mono_index]
+    mz = [100.0, 300.0, mono_mz - dm_cl, mono_mz, 456.0]
+    sp = [100.0, 200.0, 500.0, 501.0, 34.0]
+    peak_list = create_peak_list(mz, sp)
+    monoisotopologue = peak_list[mono_index]
 
     # find the rule to search the mmi candidate
     m_bin = int(mono_mz // bin_size)
     i_rules = rules.get(m_bin)[0]
     mz_tol = 0.005
     p_tol = 0.05
+    min_similarity = 0.9
+
+    data = AnnotationData(peak_list)
 
     test_candidates = mmi_finder._find_candidate(
-        mz, sp, mono_mz, charge, mono_sp, i_rules, mz_tol, p_tol)
-    expected_candidates = [(2, 1)]
+        data, monoisotopologue, charge, i_rules, mz_tol, p_tol, max_mass, min_similarity
+    )
+    mmi = peak_list[2]
+    expected_candidates = [(mmi, 1)]
     assert test_candidates == expected_candidates
 
 
 def test__find_candidates_multiple_candidates(rules):
     rules, max_mass, length, bin_size = rules
     # create an m/z and sp list where the monoisotopic m/z is the M1 in the
     # isotopic envelope.
     _, M_cl, _ = PeriodicTable().get_element("Cl").get_abundances()
     dm_cl = M_cl[1] - M_cl[0]
     mono_mz = 400.0
     charge = 1
     mono_index = 4
     M01 = mono_mz - dm_cl
     M02 = M01 + 0.00001
-    mz = np.array([100.0, 300.0, M01, M02, mono_mz, 456.0])
-    sp = np.array([100.0, 200.0, 500.0, 500.5, 501.0, 34.0])
-    mono_sp = sp[mono_index]
+    mz = [100.0, 300.0, M01, M02, mono_mz, 456.0]
+    sp = [100.0, 200.0, 500.0, 500.5, 501.0, 34.0]
+    peak_list = create_peak_list(mz, sp)
+    monoisotopologue = peak_list[mono_index]
 
     # find the rule to search the mmi candidate
     m_bin = int(mono_mz // bin_size)
     i_rules = rules.get(m_bin)[0]
     mz_tol = 0.005
     p_tol = 0.05
+    min_similarity = 0.9
+
+    data = AnnotationData(peak_list)
 
     test_candidates = mmi_finder._find_candidate(
-        mz, sp, mono_mz, charge, mono_sp, i_rules, mz_tol, p_tol)
-    expected_candidates = [(2, 1), (3, 1)]
+        data, monoisotopologue, charge, i_rules, mz_tol, p_tol, max_mass, min_similarity
+    )
+    expected_candidates = [(peak_list[2], 1), (peak_list[3], 1)]
     assert test_candidates == expected_candidates
 
 
 def test__find_candidates_no_candidates(rules):
     rules, max_mass, length, bin_size = rules
     # create an m/z and sp list where the monoisotopic m/z is the M1 in the
     # isotopic envelope.
     _, M_cl, _ = PeriodicTable().get_element("Cl").get_abundances()
-    dm_cl = M_cl[1] - M_cl[0]
     mono_mz = 400.0
     charge = 1
     mono_index = 2
-    mz = np.array([100.0, 300.0, mono_mz, 456.0])
-    sp = np.array([100.0, 200.0, 501.0, 34.0])
-    mono_sp = sp[mono_index]
+    mz = [100.0, 300.0, mono_mz, 456.0]
+    sp = [100.0, 200.0, 501.0, 34.0]
+    peak_list = create_peak_list(mz, sp)
+    monoisotopologue = peak_list[mono_index]
 
     # find the rule to search the mmi candidate
     m_bin = int(mono_mz // bin_size)
     i_rules = rules.get(m_bin)[0]
     mz_tol = 0.005
     p_tol = 0.05
+    min_similarity = 0.9
+
+    data = AnnotationData(peak_list)
 
     test_candidates = mmi_finder._find_candidate(
-        mz, sp, mono_mz, charge, mono_sp, i_rules, mz_tol, p_tol)
+        data, monoisotopologue, charge, i_rules, mz_tol, p_tol, max_mass, min_similarity
+    )
     assert len(test_candidates) == 0
 
 
 def test_MMIFinder():
-    bounds = {
-        "C": (0, 108),
-        "H": (0, 100),
-        "S": (0, 8),
-        "Cl": (0, 2)
-    }
+    bounds = {"C": (0, 108), "H": (0, 100), "S": (0, 8), "Cl": (0, 2)}
     max_mass = 2000.0
     length = 5
     bin_size = 100
     max_charge = 3
     mz_tol = 0.005
     p_tol = 0.05
+    min_similarity = 0.9
     finder = mmi_finder.MMIFinder(
-        bounds, max_mass, max_charge, length, bin_size, mz_tol, p_tol)
+        bounds, max_mass, max_charge, length, bin_size, mz_tol, p_tol, min_similarity
+    )
 
     _, M_cl, _ = PeriodicTable().get_element("Cl").get_abundances()
     dm_cl = M_cl[1] - M_cl[0]
     mono_mz = 400.0
-    mono_index = 3
-    mz = np.array([100.0, 300.0, mono_mz - dm_cl, mono_mz, 456.0])
-    sp = np.array([100.0, 200.0, 500.0, 501.0, 34.0])
-    test_mmi_index = finder.find(mz, sp, mono_index)
-    expected_mmi_index = [(3, 1), (3, 2), (3, 3), (2, 1)]
-    assert test_mmi_index == expected_mmi_index
+    mz = [100.0, 300.0, mono_mz - dm_cl, mono_mz, 456.0]
+    sp = [100.0, 200.0, 500.0, 501.0, 34.0]
+    peak_list = create_peak_list(mz, sp)
+    data = AnnotationData(peak_list)
+    monoisotopologue = data.get_monoisotopologue()
+    test_mmi_index = finder.find(data)
+    expected_mmi_index = [
+        (monoisotopologue, 1),
+        (monoisotopologue, 2),
+        (monoisotopologue, 3),
+        (peak_list[2], 1),
+    ]
+    # check with set because features may be in a different order
+    assert set(test_mmi_index) == set(expected_mmi_index)
```

### Comparing `tidyms-0.6.3/.gitignore` & `tidyms-0.7.0/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -125,7 +125,15 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # Pycharm
 .idea/
+
+# VS code
+.vscode/
+*.featureML
+*.dill
+docs/examples/exportedDataMatrix.tsv
+docs/examples/defined_spots_rtShifted.tsv
+docs/examples/defined_spots.tsv
```

### Comparing `tidyms-0.6.3/LICENSE` & `tidyms-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tidyms-0.6.3/README.md` & `tidyms-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,23 @@
 
 Examples
 --------
 
 Jupyter notebooks with examples are available
 [here](https://github.com/griquelme/tidyms-notebooks).
 
+Tests
+-----
+
+TidyMS uses unit tests for most of its functionality. 
+The tests can be executed with 
+```
+    python setup.py test
+```
+
 Documentation
 -------------
 
 The official documentation is available at 
 [readthedocs](https://tidyms.readthedocs.io/en/latest/).
```

### Comparing `tidyms-0.6.3/pyproject.toml` & `tidyms-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tidyms"
-version = "0.6.3"
+version = "0.7.0"
 description = "Tools for working with MS data in metabolomics"
 authors = [
     { name = "Gabriel Riquelme" },
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
@@ -16,32 +16,42 @@
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: BSD License",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Medical Science Apps."
 ]
 dependencies = [
+    "beautifulsoup4>=4.11.2",
     "bokeh>=3.0",
     "Cerberus>=1.3",
+    "dill>=0.3.6",
     "ipython>=8.1",
     "joblib>=1.1",
     "matplotlib>=3.5.1",
+    "natsort>=8.2.0",
     "networkx>=3.0",
     "numpy>=1.22",
     "openpyxl>=3.0",
-    "pandas>=1.4.1",
+    "pandas>=1.5.3",
+    "plotnine>=0.10.1",
     "requests",
     "scikit-learn>=1.0.2",
     "scipy>=1.8",
     "seaborn>=0.11",
     "statsmodels>=0.13",
     "tqdm>=4.0",
+    "umap-learn>=0.5.3",
     "xlrd>=2.0"
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/griquelme/tidyms"
 
 [tool.mypy]
 python_version = "3.9"
-files = ["src/tidyms"]
+files = ["src/tidyms"]
+
+[tool.pytest.ini_options]
+pythonpath = [
+  ".", "./src"
+]
```

### Comparing `tidyms-0.6.3/PKG-INFO` & `tidyms-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyms
-Version: 0.6.3
+Version: 0.7.0
 Summary: Tools for working with MS data in metabolomics
 Project-URL: Homepage, https://github.com/griquelme/tidyms
 Author: Gabriel Riquelme
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Bioanalytical mass spectrometry group at CIBION-CONICET
         All rights reserved.
@@ -37,29 +37,34 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.9
+Requires-Dist: beautifulsoup4>=4.11.2
 Requires-Dist: bokeh>=3.0
 Requires-Dist: cerberus>=1.3
+Requires-Dist: dill>=0.3.6
 Requires-Dist: ipython>=8.1
 Requires-Dist: joblib>=1.1
 Requires-Dist: matplotlib>=3.5.1
+Requires-Dist: natsort>=8.2.0
 Requires-Dist: networkx>=3.0
 Requires-Dist: numpy>=1.22
 Requires-Dist: openpyxl>=3.0
-Requires-Dist: pandas>=1.4.1
+Requires-Dist: pandas>=1.5.3
+Requires-Dist: plotnine>=0.10.1
 Requires-Dist: requests
 Requires-Dist: scikit-learn>=1.0.2
 Requires-Dist: scipy>=1.8
 Requires-Dist: seaborn>=0.11
 Requires-Dist: statsmodels>=0.13
 Requires-Dist: tqdm>=4.0
+Requires-Dist: umap-learn>=0.5.3
 Requires-Dist: xlrd>=2.0
 Description-Content-Type: text/markdown
 
 TidyMS: Tools for working with MS data in metabolomics
 ======================================================
 
 TidyMS is a python library for processing Mass Spectrometry data. It aims to
@@ -93,14 +98,23 @@
 
 Examples
 --------
 
 Jupyter notebooks with examples are available
 [here](https://github.com/griquelme/tidyms-notebooks).
 
+Tests
+-----
+
+TidyMS uses unit tests for most of its functionality. 
+The tests can be executed with 
+```
+    python setup.py test
+```
+
 Documentation
 -------------
 
 The official documentation is available at 
 [readthedocs](https://tidyms.readthedocs.io/en/latest/).
```

