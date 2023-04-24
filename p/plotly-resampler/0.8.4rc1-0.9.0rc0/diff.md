# Comparing `tmp/plotly_resampler-0.8.4rc1.tar.gz` & `tmp/plotly_resampler-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_resampler-0.8.4rc1.tar", max compression
+gzip compressed data, was "plotly_resampler-0.9.0rc0.tar", max compression
```

## Comparing `plotly_resampler-0.8.4rc1.tar` & `plotly_resampler-0.9.0rc0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
--rw-r--r--   0        0        0     1115 2022-11-08 12:19:01.827472 plotly_resampler-0.8.4rc1/LICENSE
--rw-r--r--   0        0        0     9948 2022-12-01 14:29:16.346994 plotly_resampler-0.8.4rc1/README.md
--rw-r--r--   0        0        0     2509 2022-11-08 12:19:01.827472 plotly_resampler-0.8.4rc1/build.py
--rw-r--r--   0        0        0      838 2022-12-21 11:46:52.679862 plotly_resampler-0.8.4rc1/plotly_resampler/__init__.py
--rw-r--r--   0        0        0      540 2022-12-02 12:24:11.819301 plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/__init__.py
--rw-r--r--   0        0        0     6592 2022-12-20 16:33:03.364294 plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/aggregation_interface.py
--rw-r--r--   0        0        0    16270 2022-12-20 16:33:03.364294 plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/aggregators.py
--rw-r--r--   0        0        0        0 2022-11-08 12:19:01.907470 plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/algorithms/__init__.py
--rw-r--r--   0        0        0     1276 2022-12-20 16:33:03.364294 plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/algorithms/lttb_c.py
--rw-r--r--   0        0        0     3279 2022-12-21 10:23:53.062098 plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/algorithms/lttb_py.py
--rw-r--r--   0        0        0    20021 2022-11-08 12:19:01.911470 plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/algorithms/lttbc.c
--rw-r--r--   0        0        0      473 2022-12-20 16:33:03.368294 plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/__init__.py
--rw-r--r--   0        0        0    21931 2022-12-20 16:33:03.368294 plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/figure_resampler.py
--rw-r--r--   0        0        0    58669 2022-12-20 16:33:03.368294 plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/figure_resampler_interface.py
--rw-r--r--   0        0        0    13466 2022-12-20 16:33:03.368294 plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/figurewidget_resampler.py
--rw-r--r--   0        0        0     4536 2022-12-20 16:33:03.368294 plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/utils.py
--rw-r--r--   0        0        0     4911 2022-12-20 16:33:03.368294 plotly_resampler-0.8.4rc1/plotly_resampler/registering.py
--rw-r--r--   0        0        0     2463 2022-12-21 11:46:30.492273 plotly_resampler-0.8.4rc1/pyproject.toml
--rw-r--r--   0        0        0    11317 1970-01-01 00:00:00.000000 plotly_resampler-0.8.4rc1/setup.py
--rw-r--r--   0        0        0    11178 1970-01-01 00:00:00.000000 plotly_resampler-0.8.4rc1/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-04-24 11:55:40.176114 plotly_resampler-0.9.0rc0/LICENSE
+-rw-r--r--   0        0        0     9540 2023-04-24 11:55:40.176114 plotly_resampler-0.9.0rc0/README.md
+-rw-r--r--   0        0        0      853 2023-04-24 11:56:28.830431 plotly_resampler-0.9.0rc0/plotly_resampler/__init__.py
+-rw-r--r--   0        0        0      796 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/__init__.py
+-rw-r--r--   0        0        0     7281 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/aggregation_interface.py
+-rw-r--r--   0        0        0    14446 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/aggregators.py
+-rw-r--r--   0        0        0     3048 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/gap_handler_interface.py
+-rw-r--r--   0        0        0     3116 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/gap_handlers.py
+-rw-r--r--   0        0        0     7889 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/plotly_aggregator_parser.py
+-rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/__init__.py
+-rw-r--r--   0        0        0    23717 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler.py
+-rw-r--r--   0        0        0    58683 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler_interface.py
+-rw-r--r--   0        0        0    13669 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figurewidget_resampler.py
+-rw-r--r--   0        0        0     5376 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/utils.py
+-rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc0/plotly_resampler/registering.py
+-rw-r--r--   0        0        0     3035 2023-04-24 11:56:14.754918 plotly_resampler-0.9.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    11486 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc0/PKG-INFO
```

### Comparing `plotly_resampler-0.8.4rc1/LICENSE` & `plotly_resampler-0.9.0rc0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost.
+Copyright (c) 2023 Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `plotly_resampler-0.8.4rc1/README.md` & `plotly_resampler-0.9.0rc0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
         <img alt="Plotly-Resampler logo" src="https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/logo.svg" width=65%>
     </a>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)](https://pypi.org/project/plotly-resampler/)
 [![support-version](https://img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/pyversions/plotly-resampler)
 [![codecov](https://img.shields.io/codecov/c/github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/predict-idlab/plotly-resampler)
-[![Code quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/plotly-resampler?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-idlab/plotly-resampler/context:python)
 [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
 [![Documentation](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml)
 [![Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml)
 
 
 <!-- [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler) -->
@@ -36,15 +35,26 @@
 
 ### Installation
 
 | [**pip**](https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
 | ---| ----|
 <!-- | [**conda**](https://anaconda.org/conda-forge/plotly_resampler/) | `conda install -c conda-forge plotly_resampler` | -->
 
-<br>
+### Features :tada:
+
+  * **Convenient** to use:
+    * just add either
+      * `register_plotly_resampler` function to your notebook with the best suited `mode` argument.
+      * `FigureResampler` decorator around a plotly Figure and call `.show_dash()`
+      * `FigureWidgetResampler` decorator around a plotly Figure and output the instance in a cell
+    * allows all other plotly figure construction flexibility to be used!
+  * **Environment-independent**
+    * can be used in Jupyter, vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as application (on a server)
+  * Interface for **various aggregation algorithms**:
+    * ability to develop or select your preferred sequence aggregation method
 
 ## Usage
 
 **Add dynamic aggregation** to your plotly Figure _(unfold your fitting use case)_
 * 🤖 <b>Automatically</b> _(minimal code overhead)_:
   <details><summary>Use the <code>register_plotly_resampler</code> function</summary>
     <br>
@@ -75,118 +85,85 @@
     > **Note**: This wraps **all** plotly graph object figures with a 
     > `FigureResampler` | `FigureWidgetResampler`. This can thus also be 
     > used for the `plotly.express` interface. 🎉
 
   </details>
 
 * 👷 <b>Manually</b> _(higher data aggregation configurability, more speedup possibilities)_:
-  <details>
-    <summary>Within a <b><i>jupyter</i></b> environment without creating a <i>web application</i></summary>
-    <br>
-
+  * Within a <b><i>jupyter</i></b> environment without creating a <i>web application</i>
     1. wrap the plotly Figure with `FigureWidgetResampler`
     2. output the `FigureWidgetResampler` instance in a cell
-
-    * **code example**:
       ```python
       import plotly.graph_objects as go; import numpy as np
       from plotly_resampler import FigureResampler, FigureWidgetResampler
 
       x = np.arange(1_000_000)
       noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000
 
       # OPTION 1 - FigureWidgetResampler: dynamic aggregation via `FigureWidget.layout.on_change`
       fig = FigureWidgetResampler(go.Figure())
       fig.add_trace(go.Scattergl(name='noisy sine', showlegend=True), hf_x=x, hf_y=noisy_sin)
 
       fig
       ```
-  </details>
-  <details>
-    <summary>Using a <b><i>web-application</i></b> with <b><a href="https://github.com/plotly/dash">dash</a></b> callbacks</summary>
-    <br>
-
+  * Using a <b><i>web-application</i></b> with <b><a href="https://github.com/plotly/dash">dash</a></b> callbacks
     1. wrap the plotly Figure with `FigureResampler`
     2. call `.show_dash()` on the `Figure`
-
-    * **code example**:
       ```python
       import plotly.graph_objects as go; import numpy as np
       from plotly_resampler import FigureResampler, FigureWidgetResampler
 
       x = np.arange(1_000_000)
       noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000
 
       # OPTION 2 - FigureResampler: dynamic aggregation via a Dash web-app
       fig = FigureResampler(go.Figure())
       fig.add_trace(go.Scattergl(name='noisy sine', showlegend=True), hf_x=x, hf_y=noisy_sin)
 
       fig.show_dash(mode='inline')
       ```
-
-  </details>
-  <br>
-
   > **Tip** 💡:
    > For significant faster initial loading of the Figure, we advise to wrap the 
    > constructor of the plotly Figure and add the trace data as `hf_x` and `hf_y`
 
 <br>
 
 > **Note**:
 > Any plotly Figure can be wrapped with `FigureResampler` and `FigureWidgetResampler`! 🎉
 > But, (obviously) only the scatter traces will be resampled.
 
-
-
-
-<br>
-<details><summary>👉 <b>Features</b></summary>
-
-  * **Convenient** to use:
-    * just add either
-      * `register_plotly_resampler` function to your notebook with the best suited `mode` argument.
-      * `FigureResampler` decorator around a plotly Figure and call `.show_dash()`
-      * `FigureWidgetResampler` decorator around a plotly Figure and output the instance in a cell
-    * allows all other plotly figure construction flexibility to be used!
-  * **Environment-independent**
-    * can be used in Jupyter, vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as application (on a server)
-  * Interface for **various aggregation algorithms**:
-    * ability to develop or select your preferred sequence aggregation method
-</details>
-
-### Important considerations & tips
+## Important considerations & tips
 
 * When running the code on a server, you should forward the port of the `FigureResampler.show_dash()` method to your local machine.<br>
   **Note** that you can add dynamic aggregation to plotly figures with the `FigureWidgetResampler` wrapper without needing to forward a port!
 * The `FigureWidgetResampler` *uses the IPython main thread* for its data aggregation functionality, so when this main thread is occupied, no resampling logic can be executed. For example; if you perform long computations within your notebook, the kernel will be occupied during these computations, and will only execute the resampling operations that take place during these computations after finishing that computation.
 * In general, when using downsampling one should be aware of (possible) [aliasing](https://en.wikipedia.org/wiki/Aliasing) effects.
   The <b style="color:orange">[R]</b> in the legend indicates when the corresponding trace is being resampled (and thus possibly distorted) or not. Additionally, the `~<range>` suffix represent the mean aggregation bin size in terms of the sequence index.
 * The plotly **autoscale** event (triggered by the autoscale button or a double-click within the graph), **does not reset the axes but autoscales the current graph-view** of plotly-resampler figures. This design choice was made as it seemed more intuitive for the developers to support this behavior with double-click than the default axes-reset behavior. The graph axes can ofcourse be resetted by using the `reset_axis` button.  If you want to give feedback and discuss this further with the developers, see issue [#49](https://github.com/predict-idlab/plotly-resampler/issues/49).
 
 ## Cite
 
 Paper (preprint): https://arxiv.org/abs/2206.08703
 
-```latex
-@misc{https://doi.org/10.48550/arxiv.2206.08703,
-  author = {Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
-  title = {Plotly-Resampler: Effective Visual Analytics for Large Time Series},
-  year = {2022},
-  doi = {10.48550/ARXIV.2206.08703},
-  url = {https://arxiv.org/abs/2206.08703},
-  publisher = {arXiv},
+```bibtex
+@inproceedings{van2022plotly,
+  title={Plotly-resampler: Effective visual analytics for large time series},
+  author={Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
+  booktitle={2022 IEEE Visualization and Visual Analytics (VIS)},
+  pages={21--25},
+  year={2022},
+  organization={IEEE}
 }
 ```
 
 ## Future work 🔨
 
 - [x] Support `.add_traces()` (currently only `.add_trace` is supported)
-- [ ] Support `hf_color` and `hf_markersize`, see [#50](https://github.com/predict-idlab/plotly-resampler/pull/50)
-- [ ] Create C bindings for our EfficientLTTB algorithm.
+- [ ] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
+- [x] Integrate with [tsdownsample](https://github.com/predict-idlab/tsdownsample) :racehorse:
 
 <br>
 
 ---
 
 <p align="center">
 👤 <i>Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost</i>
```

#### html2text {}

```diff
@@ -1,19 +1,16 @@
                             [Plotly-Resampler_logo]
 [![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)]
 (https://pypi.org/project/plotly-resampler/) [![support-version](https://
 img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/
 pyversions/plotly-resampler) [![codecov](https://img.shields.io/codecov/c/
 github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/
-predict-idlab/plotly-resampler) [![Code quality](https://img.shields.io/lgtm/
-grade/python/github/predict-idlab/plotly-
-resampler?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-
-idlab/plotly-resampler/context:python) [![Downloads](https://pepy.tech/badge/
-plotly-resampler)](https://pepy.tech/project/plotly-resampler) [![PRs Welcome]
-(https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
+predict-idlab/plotly-resampler) [![Downloads](https://pepy.tech/badge/plotly-
+resampler)](https://pepy.tech/project/plotly-resampler) [![PRs Welcome](https:/
+/img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
 makeapullrequest.com) [![Documentation](https://github.com/predict-idlab/
 plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://
 github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml) [!
 [Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/
 test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/
 workflows/test.yml)  > `plotly_resampler`: visualize large sequential data by
 **adding resampling functionality to Plotly figures** [Plotly](https://
@@ -24,68 +21,63 @@
 interact with the plot (panning, zooming, ...), callbacks are used to aggregate
 data and update the figure. ![basic example gif](https://
 raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/
 _static/basic_example.gif) In [this Plotly-Resampler demo](https://github.com/
 predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
 `110,000,000` data points are visualized!       ### Installation | [**pip**]
 (https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
-| ---| ----|
-## Usage **Add dynamic aggregation** to your plotly Figure _(unfold your
-fitting use case)_ * ð¤ Automatically _(minimal code overhead)_: Use the
+| ---| ----|  ### Features :tada: * **Convenient** to use: * just add either *
+`register_plotly_resampler` function to your notebook with the best suited
+`mode` argument. * `FigureResampler` decorator around a plotly Figure and call
+`.show_dash()` * `FigureWidgetResampler` decorator around a plotly Figure and
+output the instance in a cell * allows all other plotly figure construction
+flexibility to be used! * **Environment-independent** * can be used in Jupyter,
+vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as
+application (on a server) * Interface for **various aggregation algorithms**: *
+ability to develop or select your preferred sequence aggregation method ##
+Usage **Add dynamic aggregation** to your plotly Figure _(unfold your fitting
+use case)_ * ð¤ Automatically _(minimal code overhead)_: Use the
 register_plotly_resampler function
 1. Import and call the `register_plotly_resampler` method 2. Just use your
 regular graph construction code * **code example**: ```python import
 plotly.graph_objects as go; import numpy as np from plotly_resampler import
 register_plotly_resampler # Call the register function once and all Figures/
 FigureWidgets will be wrapped # according to the register_plotly_resampler its
 `mode` argument register_plotly_resampler(mode='auto') x = np.arange(1_000_000)
 noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000 #
 auto mode: when working in an IPython environment, this will automatically be a
 # FigureWidgetResampler else, this will be an FigureResampler f = go.Figure()
 f.add_trace({"y": noisy_sin + 2, "name": "yp2"}) f ``` > **Note**: This wraps
 **all** plotly graph object figures with a > `FigureResampler` |
 `FigureWidgetResampler`. This can thus also be > used for the `plotly.express`
 interface. ð  * ð· Manually _(higher data aggregation configurability,
-more speedup possibilities)_:  Within a jupyter environment without creating a
-web application
-1. wrap the plotly Figure with `FigureWidgetResampler` 2. output the
-`FigureWidgetResampler` instance in a cell * **code example**: ```python import
+more speedup possibilities)_: * Within a jupyter environment without creating a
+web application 1. wrap the plotly Figure with `FigureWidgetResampler` 2.
+output the `FigureWidgetResampler` instance in a cell ```python import
 plotly.graph_objects as go; import numpy as np from plotly_resampler import
 FigureResampler, FigureWidgetResampler x = np.arange(1_000_000) noisy_sin = (3
 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000 # OPTION 1 -
 FigureWidgetResampler: dynamic aggregation via `FigureWidget.layout.on_change`
 fig = FigureWidgetResampler(go.Figure()) fig.add_trace(go.Scattergl(name='noisy
-sine', showlegend=True), hf_x=x, hf_y=noisy_sin) fig ```   Using a web-
-application with dash callbacks
-1. wrap the plotly Figure with `FigureResampler` 2. call `.show_dash()` on the
-`Figure` * **code example**: ```python import plotly.graph_objects as go;
-import numpy as np from plotly_resampler import FigureResampler,
-FigureWidgetResampler x = np.arange(1_000_000) noisy_sin = (3 + np.sin(x / 200)
-+ np.random.randn(len(x)) / 10) * x / 1_000 # OPTION 2 - FigureResampler:
-dynamic aggregation via a Dash web-app fig = FigureResampler(go.Figure())
-fig.add_trace(go.Scattergl(name='noisy sine', showlegend=True), hf_x=x,
-hf_y=noisy_sin) fig.show_dash(mode='inline') ```
-> **Tip** ð¡: > For significant faster initial loading of the Figure, we
-advise to wrap the > constructor of the plotly Figure and add the trace data as
-`hf_x` and `hf_y`
+sine', showlegend=True), hf_x=x, hf_y=noisy_sin) fig ``` * Using a web-
+application with dash callbacks 1. wrap the plotly Figure with
+`FigureResampler` 2. call `.show_dash()` on the `Figure` ```python import
+plotly.graph_objects as go; import numpy as np from plotly_resampler import
+FigureResampler, FigureWidgetResampler x = np.arange(1_000_000) noisy_sin = (3
++ np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000 # OPTION 2 -
+FigureResampler: dynamic aggregation via a Dash web-app fig = FigureResampler
+(go.Figure()) fig.add_trace(go.Scattergl(name='noisy sine', showlegend=True),
+hf_x=x, hf_y=noisy_sin) fig.show_dash(mode='inline') ``` > **Tip** ð¡: > For
+significant faster initial loading of the Figure, we advise to wrap the >
+constructor of the plotly Figure and add the trace data as `hf_x` and `hf_y`
 > **Note**: > Any plotly Figure can be wrapped with `FigureResampler` and
 `FigureWidgetResampler`! ð > But, (obviously) only the scatter traces will
-be resampled.
-ð Features * **Convenient** to use: * just add either *
-`register_plotly_resampler` function to your notebook with the best suited
-`mode` argument. * `FigureResampler` decorator around a plotly Figure and call
-`.show_dash()` * `FigureWidgetResampler` decorator around a plotly Figure and
-output the instance in a cell * allows all other plotly figure construction
-flexibility to be used! * **Environment-independent** * can be used in Jupyter,
-vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as
-application (on a server) * Interface for **various aggregation algorithms**: *
-ability to develop or select your preferred sequence aggregation method  ###
-Important considerations & tips * When running the code on a server, you should
-forward the port of the `FigureResampler.show_dash()` method to your local
-machine.
+be resampled. ## Important considerations & tips * When running the code on a
+server, you should forward the port of the `FigureResampler.show_dash()` method
+to your local machine.
 **Note** that you can add dynamic aggregation to plotly figures with the
 `FigureWidgetResampler` wrapper without needing to forward a port! * The
 `FigureWidgetResampler` *uses the IPython main thread* for its data aggregation
 functionality, so when this main thread is occupied, no resampling logic can be
 executed. For example; if you perform long computations within your notebook,
 the kernel will be occupied during these computations, and will only execute
 the resampling operations that take place during these computations after
@@ -98,18 +90,18 @@
 the graph), **does not reset the axes but autoscales the current graph-view**
 of plotly-resampler figures. This design choice was made as it seemed more
 intuitive for the developers to support this behavior with double-click than
 the default axes-reset behavior. The graph axes can ofcourse be resetted by
 using the `reset_axis` button. If you want to give feedback and discuss this
 further with the developers, see issue [#49](https://github.com/predict-idlab/
 plotly-resampler/issues/49). ## Cite Paper (preprint): https://arxiv.org/abs/
-2206.08703 ```latex @misc{https://doi.org/10.48550/arxiv.2206.08703, author =
-{Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van
-Hoecke, Sofie}, title = {Plotly-Resampler: Effective Visual Analytics for Large
-Time Series}, year = {2022}, doi = {10.48550/ARXIV.2206.08703}, url = {https://
-arxiv.org/abs/2206.08703}, publisher = {arXiv}, } ``` ## Future work ð¨ - [x]
-Support `.add_traces()` (currently only `.add_trace` is supported) - [ ]
-Support `hf_color` and `hf_markersize`, see [#50](https://github.com/predict-
-idlab/plotly-resampler/pull/50) - [ ] Create C bindings for our EfficientLTTB
-algorithm.
+2206.08703 ```bibtex @inproceedings{van2022plotly, title={Plotly-resampler:
+Effective visual analytics for large time series}, author={Van Der Donckt,
+Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
+booktitle={2022 IEEE Visualization and Visual Analytics (VIS)}, pages={21--25},
+year={2022}, organization={IEEE} } ``` ## Future work ð¨ - [x] Support
+`.add_traces()` (currently only `.add_trace` is supported) - [ ] Support
+`hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/
+plotly-resampler/pull/148) - [x] Integrate with [tsdownsample](https://
+github.com/predict-idlab/tsdownsample) :racehorse:
 ---
         ð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
```

### Comparing `plotly_resampler-0.8.4rc1/plotly_resampler/__init__.py` & `plotly_resampler-0.9.0rc0/plotly_resampler/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """**plotly\_resampler**: visualizing large sequences."""
 
-from .aggregation import LTTB, EfficientLTTB, EveryNthPoint
+import contextlib
+
+from .aggregation import LTTB, EveryNthPoint, MinMaxLTTB
 from .figure_resampler import FigureResampler, FigureWidgetResampler
 from .registering import register_plotly_resampler, unregister_plotly_resampler
 
 __docformat__ = "numpy"
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
-__version__ = "0.8.4rc1"
+__version__ = "0.9.0rc0"
 
 __all__ = [
     "__version__",
     "FigureResampler",
     "FigureWidgetResampler",
-    "EfficientLTTB",
+    "MinMaxLTTB",
     "LTTB",
     "EveryNthPoint",
     "register_plotly_resampler",
     "unregister_plotly_resampler",
 ]
 
 
-try:  # Enable ipywidgets on google colab!
+# Enable ipywidgets on google colab!
+with contextlib.suppress(ImportError, ModuleNotFoundError):
     import sys
 
     if "google.colab" in sys.modules:
         from google.colab import output
 
         output.enable_custom_widget_manager()
-except (ImportError, ModuleNotFoundError):
-    pass
```

### Comparing `plotly_resampler-0.8.4rc1/plotly_resampler/aggregation/__init__.py` & `plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,26 +3,33 @@
 other downsample methods.
 
 """
 
 __author__ = "Jonas Van Der Donckt"
 
 
-from .aggregation_interface import AbstractSeriesAggregator
+from .aggregation_interface import AbstractAggregator
 from .aggregators import (
     LTTB,
-    EfficientLTTB,
     EveryNthPoint,
     FuncAggregator,
     MinMaxAggregator,
+    MinMaxLTTB,
     MinMaxOverlapAggregator,
 )
+from .gap_handler_interface import AbstractGapHandler
+from .gap_handlers import MedDiffGapHandler, NoGapHandler
+from .plotly_aggregator_parser import PlotlyAggregatorParser
 
 __all__ = [
-    "AbstractSeriesAggregator",
+    "AbstractAggregator",
+    "AbstractGapHandler",
+    "PlotlyAggregatorParser",
     "LTTB",
-    "EfficientLTTB",
+    "MinMaxLTTB",
     "EveryNthPoint",
     "FuncAggregator",
+    "MedDiffGapHandler",
     "MinMaxAggregator",
     "MinMaxOverlapAggregator",
+    "NoGapHandler",
 ]
```

### Comparing `plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/figure_resampler.py` & `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 """
 
 from __future__ import annotations
 
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
 
 import base64
+import contextlib
 import uuid
 import warnings
 from typing import List, Tuple
 
 import dash
 import plotly.graph_objects as go
-from flask_cors import cross_origin
 from jupyter_dash import JupyterDash
 from plotly.basedatatypes import BaseFigure
 from trace_updater import TraceUpdater
 
-from ..aggregation import AbstractSeriesAggregator, EfficientLTTB
+from ..aggregation import (
+    AbstractAggregator,
+    AbstractGapHandler,
+    MedDiffGapHandler,
+    MinMaxLTTB,
+)
 from .figure_resampler_interface import AbstractFigureAggregator
 from .utils import is_figure, is_fr
 
 
 class JupyterDashPersistentInlineOutput(JupyterDash):
     """Extension of the JupyterDash class to support the custom inline output for
     ``FigureResampler`` figures.
@@ -44,37 +49,53 @@
     Hence, this extension enables to maintain always an output in the notebook.
 
     .. Note::
         This subclass is only used when the mode is set to ``"inline_persistent"`` in
         the :func:`FigureResampler.show_dash <plotly_resampler.figure_resampler.FigureResampler.show_dash>`
         method. However, the mode should be passed as ``"inline"`` since this subclass
         overwrites the inline behavior.
+
+    .. Note::
+        This subclass utilizes the optional ``flask_cors`` package to detect whether the
+        server is alive or not.
+
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._uid = str(uuid.uuid4())  # A new unique id for each app
 
-        # Mimic the _alive_{token} endpoint but with cors
-        @self.server.route(f"/_is_alive_{self._uid}", methods=["GET"])
-        @cross_origin(origin=["*"], allow_headers=["Content-Type"])
-        def broadcast_alive():
-            return "Alive"
+        with contextlib.suppress(ImportWarning, ModuleNotFoundError):
+            from flask_cors import cross_origin
+
+            # Mimic the _alive_{token} endpoint but with cors
+            @self.server.route(f"/_is_alive_{self._uid}", methods=["GET"])
+            @cross_origin(origin=["*"], allow_headers=["Content-Type"])
+            def broadcast_alive():
+                return "Alive"
 
     def _display_inline_output(self, dashboard_url, width, height):
         """Display the dash app persistent inline in the notebook.
 
         The figure is displayed as an iframe in the notebook if the server is reachable,
         otherwise as an image.
         """
         # TODO: check whether an error gets logged in case of crash
         # TODO: add option to opt out of this
         from IPython.display import display
 
+        try:
+            import flask_cors  # noqa: F401
+        except (ImportError, ModuleNotFoundError):
+            warnings.warn(
+                "'flask_cors' is not installed. The persistent inline output will "
+                + " not be able to detect whether the server is alive or not."
+            )
+
         # Get the image from the dashboard and encode it as base64
         fig = self.layout.children[0].figure  # is stored there in the show_dash method
         f_width = 1000 if fig.layout.width is None else fig.layout.width
         fig_base64 = base64.b64encode(
             fig.to_image(format="png", width=f_width, scale=1, height=fig.layout.height)
         ).decode("utf8")
 
@@ -184,15 +205,16 @@
     """Data aggregation functionality for ``go.Figures``."""
 
     def __init__(
         self,
         figure: BaseFigure | dict = None,
         convert_existing_traces: bool = True,
         default_n_shown_samples: int = 1000,
-        default_downsampler: AbstractSeriesAggregator = EfficientLTTB(),
+        default_downsampler: AbstractAggregator = MinMaxLTTB(),
+        default_gap_handler: AbstractGapHandler = MedDiffGapHandler(),
         resampled_trace_prefix_suffix: Tuple[str, str] = (
             '<b style="color:sandybrown">[R]</b> ',
             "",
         ),
         show_mean_aggregation_size: bool = True,
         convert_traces_kwargs: dict | None = None,
         verbose: bool = False,
@@ -213,18 +235,29 @@
         default_n_shown_samples: int, optional
             The default number of samples that will be shown for each trace,
             by default 1000.\n
             .. note::
                 * This can be overridden within the :func:`add_trace` method.
                 * If a trace withholds fewer datapoints than this parameter,
                   the data will *not* be aggregated.
-        default_downsampler: AbstractSeriesDownsampler
-            An instance which implements the AbstractSeriesDownsampler interface and
-            will be used as default downsampler, by default ``EfficientLTTB`` with
-            _interleave_gaps_ set to True. \n
+        default_downsampler: AbstractAggregator, optional
+            An instance which implements the AbstractAggregator interface and
+            will be used as default downsampler, by default ``MinMaxLTTB`` with
+            _interleave_gaps_ set to True. ``MinMaxLTTB`` is a heuristic to the LTTB
+            algorithm that uses pre-selection of min-max values (default 4 per bin) to
+            speed up LTTB (as now only 4 values per bin should be compared). This
+            min-max ratio of 4 can be changed by initializing ``MinMaxLTTB`` with a
+            different value for the ``minmax_ratio`` parameter. \n
+            .. note:: This can be overridden within the :func:`add_trace` method.
+        default_gap_handler: AbstractGapHandler, optional
+            An instance which implements the AbstractGapHandler interface and
+            will be used as default gap handler, by default ``MedDiffGapHandler``.
+            ``MedDiffGapHandler`` will determine gaps by first calculating the median
+            aggregated x difference and then thresholding the aggregated x delta on a
+            multiple of this median difference.  \n
             .. note:: This can be overridden within the :func:`add_trace` method.
         resampled_trace_prefix_suffix: str, optional
             A tuple which contains the ``prefix`` and ``suffix``, respectively, which
             will be added to the trace its legend-name when a resampled version of the
             trace is shown. By default a bold, orange ``[R]`` is shown as prefix
             (no suffix is shown).
         show_mean_aggregation_size: bool, optional
@@ -291,14 +324,15 @@
         )
 
         super().__init__(
             f,
             convert_existing_traces,
             default_n_shown_samples,
             default_downsampler,
+            default_gap_handler,
             resampled_trace_prefix_suffix,
             show_mean_aggregation_size,
             convert_traces_kwargs,
             verbose,
         )
 
         if isinstance(figure, AbstractFigureAggregator):
@@ -344,15 +378,17 @@
               * ``"inline_persistent"``: The app will be displayed inline in the
                 notebook output cell in an iframe, if the app is not reachable a static
                 image of the figure is shown. Hence this is a persistent version of the
                 ``"inline"`` mode, allowing users to see a static figure in other
                 environments, browsers, etc.
 
                 .. note::
-                    This mode requires the ``kaleido`` package.
+                    This mode requires the ``kaleido`` and ``flask_cors`` package.
+                    Install them : ``pip install plotly_resampler[inline_persistent]``
+                    or ``pip install kaleido flask_cors``.
 
               * ``"jupyterlab"``: The app will be displayed in a dedicated tab in the
                 JupyterLab interface. Requires JupyterLab and the ``jupyterlab-dash``
                 extension.
             By default None, which will result in the same behavior as ``"external"``.
         config: dict, optional
             The configuration options for displaying this figure, by default None.
@@ -373,32 +409,32 @@
 
         """
         available_modes = ["external", "inline", "inline_persistent", "jupyterlab"]
         assert (
             mode is None or mode in available_modes
         ), f"mode must be one of {available_modes}"
         graph_properties = {} if graph_properties is None else graph_properties
-        assert "config" not in graph_properties.keys()  # There is a param for config
+        assert "config" not in graph_properties  # There is a param for config
 
         # 0. Check if the traces need to be updated when there is a xrange set
         # This will be the case when the users has set a xrange (via the `update_layout`
         # or `update_xaxes` methods`)
         relayout_dict = {}
         for xaxis_str in self._xaxis_list:
             x_range = self.layout[xaxis_str].range
             if x_range:  # when not None
                 relayout_dict[f"{xaxis_str}.range[0]"] = x_range[0]
                 relayout_dict[f"{xaxis_str}.range[1]"] = x_range[1]
-        if len(relayout_dict):
+        if relayout_dict:  # when not empty
             update_data = self.construct_update_data(relayout_dict)
 
             if not self._is_no_update(update_data):  # when there is an update
                 with self.batch_update():
                     # First update the layout (first item of update_data)
-                    self.layout.update(update_data[0])
+                    self.layout.update(self._parse_relayout(update_data[0]))
 
                     # Then update the data
                     for updated_trace in update_data[1:]:
                         trace_idx = updated_trace.pop("index")
                         self.data[trace_idx].update(updated_trace)
 
         # 1. Construct the Dash app layout
@@ -448,15 +484,14 @@
         warn: bool
             Whether a warning message will be shown or  not, by default True.
 
         .. attention::
             This only works if the dash-app was started with :func:`show_dash`.
         """
         if self._app is not None:
-
             old_server = self._app._server_threads.get((self._host, self._port))
             if old_server:
                 old_server.kill()
                 old_server.join()
                 del self._app._server_threads[(self._host, self._port)]
         elif warn:
             warnings.warn(
```

### Comparing `plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/figure_resampler_interface.py` & `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 
 import dash
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 from plotly.basedatatypes import BaseFigure, BaseTraceType
 
-from ..aggregation import AbstractSeriesAggregator, EfficientLTTB
+from ..aggregation import AbstractAggregator, MedDiffGapHandler, MinMaxLTTB
+from ..aggregation.aggregation_interface import DataPointSelector
+from ..aggregation.gap_handler_interface import AbstractGapHandler
+from ..aggregation.plotly_aggregator_parser import PlotlyAggregatorParser
 from .utils import round_number_str, round_td_str
 
 _hf_data_container = namedtuple("DataContainer", ["x", "y", "text", "hovertext"])
 
 
 class AbstractFigureAggregator(BaseFigure, ABC):
     """Abstract interface for data aggregation functionality for plotly figures."""
@@ -37,15 +40,16 @@
     _high_frequency_traces = ["scatter", "scattergl"]
 
     def __init__(
         self,
         figure: BaseFigure,
         convert_existing_traces: bool = True,
         default_n_shown_samples: int = 1000,
-        default_downsampler: AbstractSeriesAggregator = EfficientLTTB(),
+        default_downsampler: AbstractAggregator = MinMaxLTTB(),
+        default_gap_handler: AbstractGapHandler = MedDiffGapHandler(),
         resampled_trace_prefix_suffix: Tuple[str, str] = (
             '<b style="color:sandybrown">[R]</b> ',
             "",
         ),
         show_mean_aggregation_size: bool = True,
         convert_traces_kwargs: dict | None = None,
         verbose: bool = False,
@@ -65,23 +69,27 @@
         default_n_shown_samples: int, optional
             The default number of samples that will be shown for each trace,
             by default 1000.\n
             .. note::
                 * This can be overridden within the :func:`add_trace` method.
                 * If a trace withholds fewer datapoints than this parameter,
                   the data will *not* be aggregated.
-        default_downsampler: AbstractSeriesDownsampler
+        default_downsampler: AbstractAggregator
             An instance which implements the AbstractSeriesDownsampler interface and
             will be used as default downsampler, by default ``EfficientLTTB`` with
             _interleave_gaps_ set to True. \n
             .. note:: This can be overridden within the :func:`add_trace` method.
+        default_gap_handler: GapHandler
+            An instance which implements the AbstractGapHandler interface and will be
+            used as default gap handler, by default ``MedDiffGapHandler``. \n
+            .. note:: This can be overridden within the :func:`add_trace` method.
         resampled_trace_prefix_suffix: str, optional
             A tuple which contains the ``prefix`` and ``suffix``, respectively, which
             will be added to the trace its legend-name when a resampled version of the
-            trace is shown. By default a bold, orange ``[R]`` is shown as prefix
+            trace is shown. By default, a bold, orange ``[R]`` is shown as prefix
             (no suffix is shown).
         show_mean_aggregation_size: bool, optional
             Whether the mean aggregation bin size will be added as a suffix to the trace
             its legend-name, by default True.
         convert_traces_kwargs: dict, optional
             A dict of kwargs that will be passed to the :func:`add_traces` method and
             will be used to convert the existing traces. \n
@@ -97,14 +105,15 @@
         self._print_verbose = verbose
         self._show_mean_aggregation_size = show_mean_aggregation_size
 
         assert len(resampled_trace_prefix_suffix) == 2
         self._prefix, self._suffix = resampled_trace_prefix_suffix
 
         self._global_downsampler = default_downsampler
+        self._global_gap_handler = default_gap_handler
 
         # Given figure should always be a BaseFigure that is not wrapped by
         # a plotly-resampler class
         assert isinstance(figure, BaseFigure)
         assert not issubclass(type(figure), AbstractFigureAggregator)
         self._figure_class = figure.__class__
 
@@ -195,21 +204,66 @@
         --------
         https://github.com/plotly/plotly.py/blob/2e7f322c5ea4096ce6efe3b4b9a34d9647a8be9c/packages/python/plotly/plotly/basedatatypes.py#L3278
         """
         return {
             "data": [
                 {
                     k: copy(trace[k])
+                    # TODO: why not "text" as well? -> we can use _hf_data_container.fields then
                     for k in set(trace.keys()).difference({"x", "y", "hovertext"})
                 }
                 for trace in self._data
             ],
             "layout": copy(self._layout),
         }
 
+    def _parse_trace_name(
+        self, hf_trace_data: dict, slice_len: int, agg_x: np.ndarray
+    ) -> str:
+        """Parse the trace name.
+
+        Parameters
+        ----------
+        hf_trace_data : dict
+            The high-frequency trace data dict.
+        slice_len : int
+            The length of the slice.
+        agg_x : np.ndarray
+            The x-axis values of the aggregated trace.
+
+        Returns
+        -------
+        str
+            The parsed trace name.
+            When no downsampling is needed, the original trace name is returned.
+            When downsampling is needed, the average bin size (expressed in x-units) is
+            added in orange color with a `~` to the trace name.
+
+        """
+        if slice_len <= hf_trace_data["max_n_samples"]:  # When no downsampling needed
+            return hf_trace_data["name"]
+
+        # The data is downsampled, so we add the downsampling information to the name
+        agg_prefix, agg_suffix = ' <i style="color:#fc9944">~', "</i>"
+        name = self._prefix + hf_trace_data["name"] + self._suffix
+
+        # Add the mean aggregation bin size to the trace name
+        if self._show_mean_aggregation_size:
+            # Base case ...
+            if len(agg_x) < 2:
+                return name
+
+            mean_bin_size = (agg_x[-1] - agg_x[0]) / agg_x.shape[0]  # mean bin size
+            if isinstance(mean_bin_size, (np.timedelta64, pd.Timedelta)):
+                mean_bin_size = round_td_str(pd.Timedelta(mean_bin_size))
+            else:
+                mean_bin_size = round_number_str(mean_bin_size)
+            name += f"{agg_prefix}{mean_bin_size}{agg_suffix}"
+        return name
+
     def _check_update_trace_data(
         self,
         trace: dict,
         start: Optional[Union[str, float]] = None,
         end: Optional[Union[str, float]] = None,
     ) -> Optional[Union[dict, BaseTraceType]]:
         """Check and update the passed ``trace`` its data properties based on the
@@ -250,102 +304,75 @@
         ----
         * If ``start`` and ``stop`` are strings, they most likely represent time-strings
         * ``start`` and ``stop`` will always be of the same type (float / time-string)
            because their underlying axis is the same.
 
         """
         hf_trace_data = self._query_hf_data(trace)
-        if hf_trace_data is not None:
-            axis_type = hf_trace_data["axis_type"]
-            if axis_type == "date":
-                start, end = pd.to_datetime(start), pd.to_datetime(end)
-                hf_series = self._slice_time(
-                    self._to_hf_series(hf_trace_data["x"], hf_trace_data["y"]),
-                    start,
-                    end,
-                )
-            else:
-                hf_series = self._to_hf_series(hf_trace_data["x"], hf_trace_data["y"])
-                if len(hf_series) and (start is not None or end is not None):
-                    start = hf_series.index[0] if start is None else start
-                    end = hf_series.index[-1] if end is None else end
-                    if hf_series.index.is_integer():
-                        start = round(start)
-                        end = round(end)
-
-                    # Search the index-positions
-                    start_idx, end_idx = np.searchsorted(hf_series.index, [start, end])
-                    hf_series = hf_series.iloc[start_idx:end_idx]
-
-            # Return an invisible, single-point, trace when the sliced hf_series doesn't
-            # contain any data in the current view
-            if len(hf_series) == 0:
-                trace["x"] = [start]
-                trace["y"] = [None]
-                trace["text"] = ""
-                trace["hovertext"] = ""
-                return trace
-
-            # Downsample the data and store it in the trace-fields
-            downsampler: AbstractSeriesAggregator = hf_trace_data["downsampler"]
-            s_res: pd.Series = downsampler.aggregate(
-                hf_series, hf_trace_data["max_n_samples"]
-            )
-            # Also parse the data types to an orjson compatible format
-            # Note this can be removed once orjson supports f16
-            trace["x"] = self._parse_dtype_orjson(s_res.index)
-            trace["y"] = self._parse_dtype_orjson(s_res.values)
-            # todo -> first draft & not MP safe
-
-            agg_prefix, agg_suffix = ' <i style="color:#fc9944">~', "</i>"
-            name: str = trace["name"].split(agg_prefix)[0]
-
-            if len(hf_series) > hf_trace_data["max_n_samples"]:
-                name = ("" if name.startswith(self._prefix) else self._prefix) + name
-                name += self._suffix if not name.endswith(self._suffix) else ""
-                # Add the mean aggregation bin size to the trace name
-                if self._show_mean_aggregation_size:
-                    agg_mean = np.mean(np.diff(s_res.index.values))
-                    if isinstance(agg_mean, np.timedelta64):
-                        agg_mean = round_td_str(pd.Timedelta(agg_mean))
-                    else:
-                        agg_mean = round_number_str(agg_mean)
-                    name += f"{agg_prefix}{agg_mean}{agg_suffix}"
-            else:
-                # When not resampled: trim prefix and/or suffix if necessary
-                if len(self._prefix) and name.startswith(self._prefix):
-                    name = name[len(self._prefix) :]
-                if len(self._suffix) and trace["name"].endswith(self._suffix):
-                    name = name[: -len(self._suffix)]
-            trace["name"] = name
-
-            # Check if text also needs to be resampled
-            text = hf_trace_data.get("text")
-            if isinstance(text, (np.ndarray, pd.Series)):
-                # TODO -> extra logic is necessary for the detection and processing of
-                # non data-point selection downsamplers
-                trace["text"] = self._to_hf_series(x=hf_trace_data["x"], y=text).loc[
-                    s_res.index
-                ]
-            else:
-                trace["text"] = text
 
-            # Check if hovertext also needs to be resampled
-            hovertext = hf_trace_data.get("hovertext")
-            if isinstance(hovertext, (np.ndarray, pd.Series)):
-                trace["hovertext"] = self._to_hf_series(
-                    x=hf_trace_data["x"], y=hovertext
-                ).loc[s_res.index]
-            else:
-                trace["hovertext"] = hovertext
-            return trace
-        else:
+        if hf_trace_data is None:
             self._print("hf_data not found")
             return None
 
+        # Parse trace data (necessary when updating the trace data)
+        for k in _hf_data_container._fields:
+            if isinstance(
+                hf_trace_data[k], (np.ndarray, pd.RangeIndex, pd.DatetimeIndex)
+            ):
+                # is faster to escape the loop here than check inside the hasattr if
+                continue
+            if hasattr(hf_trace_data[k], "values"):
+                # when not a range index or datetime index
+                hf_trace_data[k] = hf_trace_data[k].values
+
+        # Also check if the y-data is empty, if so, return an empty trace
+        if len(hf_trace_data["y"]) == 0:
+            trace["x"] = []
+            trace["y"] = []
+            trace["name"] = hf_trace_data["name"]
+            return trace
+
+        start_idx, end_idx = PlotlyAggregatorParser.get_start_end_indices(
+            hf_trace_data, start, end
+        )
+
+        # Return an invisible, single-point, trace when the sliced hf_series doesn't
+        # contain any data in the current view
+        if end_idx == start_idx:
+            trace["x"] = [hf_trace_data["x"][0]]
+            trace["y"] = [None]
+            trace["name"] = hf_trace_data["name"]
+            return trace
+
+        agg_x, agg_y, indices = PlotlyAggregatorParser.aggregate(
+            hf_trace_data, start_idx, end_idx
+        )
+
+        # -------------------- Set the hf_trace_data_props -------------------
+        # Parse the data types to an orjson compatible format
+        # NOTE: this can be removed once orjson supports f16
+        trace["x"] = self._parse_dtype_orjson(agg_x)
+        trace["y"] = self._parse_dtype_orjson(agg_y)
+        trace["name"] = self._parse_trace_name(
+            hf_trace_data, end_idx - start_idx, agg_x
+        )
+
+        # Check if (hover)text also needs to be downsampled
+        for k in ["text", "hovertext"]:
+            k_val = hf_trace_data.get(k)
+            if isinstance(k_val, (np.ndarray, pd.Series)):
+                assert isinstance(
+                    hf_trace_data["downsampler"], DataPointSelector
+                ), "Only DataPointSelector can downsample non-data trace array props."
+                trace[k] = k_val[start_idx + indices]
+            elif k_val is not None:
+                trace[k] = k_val
+
+        return trace
+
     def _check_update_figure_dict(
         self,
         figure: dict,
         start: Optional[Union[float, str]] = None,
         stop: Optional[Union[float, str]] = None,
         xaxis_filter: str = None,
         updated_trace_indices: Optional[List[int]] = None,
@@ -429,20 +456,20 @@
                 #   -> why None: traces without row/col argument and stand on first row
                 #      and do not have the anchor property (hence the DICT.get() method)
                 # * x_axis_filter_short not in [x_anchor or xaxis matches] for
                 #   NON first rows
                 if (
                     xaxis_filter_short == "x"
                     and (
-                        x_anchor_trace not in [None, "x"]
+                        x_anchor_trace not in (None, "x")
                         and xaxis_matches != xaxis_filter_short
                     )
                 ) or (
                     xaxis_filter_short != "x"
-                    and (xaxis_filter_short not in [x_anchor_trace, xaxis_matches])
+                    and (xaxis_filter_short not in (x_anchor_trace, xaxis_matches))
                 ):
                     continue
 
             # If we managed to find and update the trace, it will return the trace
             # and thus not None.
             updated_trace = self._check_update_trace_data(trace, start=start, end=stop)
             if updated_trace is not None:
@@ -469,77 +496,28 @@
             The plotly figure class (constructor) of the given `constr`.
 
         """
         from ..registering import _get_plotly_constr  # To avoid ImportError
 
         return _get_plotly_constr(constr)
 
-    @staticmethod
-    def _slice_time(
-        hf_series: pd.Series,
-        t_start: Optional[pd.Timestamp] = None,
-        t_stop: Optional[pd.Timestamp] = None,
-    ) -> pd.Series:
-        """Slice the time-indexed ``hf_series`` for the passed pd.Timestamps.
-
-        Note
-        ----
-        This returns a **view** of ``hf_series``!
-
-        Parameters
-        ----------
-        hf_series: pd.Series
-            The **datetime-indexed** series, which will be sliced.
-        t_start: pd.Timestamp, optional
-            The lower-time-bound of the slice, if set to None, no lower-bound threshold
-            will be applied, by default None.
-        t_stop:  pd.Timestamp, optional
-            The upper time-bound of the slice, if set to None, no upper-bound threshold
-            will be applied, by default None.
-
-        Returns
-        -------
-        pd.Series
-            The sliced **view** of the series.
-
-        """
-
-        def to_same_tz(
-            ts: Union[pd.Timestamp, None], reference_tz=hf_series.index.tz
-        ) -> Union[pd.Timestamp, None]:
-            """Adjust `ts` its timezone to the `reference_tz`."""
-            if ts is None:
-                return None
-            elif reference_tz is not None:
-                if ts.tz is not None:
-                    assert ts.tz.zone == reference_tz.zone
-                    return ts
-                else:  # localize -> time remains the same
-                    return ts.tz_localize(reference_tz)
-            elif reference_tz is None and ts.tz is not None:
-                return ts.tz_localize(None)
-            return ts
-
-        if t_start is not None and t_stop is not None:
-            assert t_start.tz == t_stop.tz
-
-        return hf_series[to_same_tz(t_start) : to_same_tz(t_stop)]
-
     @property
     def hf_data(self):
         """Property to adjust the `data` component of the current graph
 
         .. note::
             The user has full responsibility to adjust ``hf_data`` properly.
 
 
         Example:
+            >>> from plotly_resampler import FigureResampler
             >>> fig = FigureResampler(go.Figure())
             >>> fig.add_trace(...)
-            >>> fig.hf_data[-1]["y"] = - s ** 2  # adjust the y-property of the trace added above
+            >>> # Adjust the y property of the above added trace
+            >>> fig.hf_data[-1]["y"] = - s ** 2
             >>> fig.hf_data
             [
                 {
                     'max_n_samples': 1000,
                     'x': RangeIndex(start=0, stop=11000000, step=1),
                     'y': array([-0.01339909,  0.01390696,, ...,  0.25051913, 0.55876513]),
                     'axis_type': 'linear',
@@ -547,50 +525,14 @@
                     'text': None,
                     'hovertext': None
                 },
             ]
         """
         return list(self._hf_data.values())
 
-    @staticmethod
-    def _to_hf_series(x: np.ndarray, y: np.ndarray) -> pd.Series:
-        """Construct the hf-series.
-
-        By constructing the hf-series this way, users can dynamically adjust the hf
-        series argument.
-
-        Parameters
-        ----------
-        x : np.ndarray
-            The hf_series index
-        y : np.ndarray
-            The hf_series values
-
-        Returns
-        -------
-        pd.Series
-            The constructed hf_series
-        """
-        # Note this is the same behavior as plotly support
-        # i.e. it also used the `values` property of the `x` and `y` parameters when
-        # these are pd.Series
-        if isinstance(x, pd.Series):
-            x = x.values
-
-        if isinstance(y, pd.Series):
-            y = y.values
-
-        return pd.Series(
-            data=y,
-            index=x,
-            copy=False,
-            name="data",
-            dtype="category" if y.dtype.type == np.str_ else y.dtype,
-        )
-
     def _parse_get_trace_props(
         self,
         trace: BaseTraceType,
         hf_x: Iterable = None,
         hf_y: Iterable = None,
         hf_text: Iterable = None,
         hf_hovertext: Iterable = None,
@@ -636,15 +578,17 @@
         hf_y = (
             trace["y"]
             if hasattr(trace, "y") and hf_y is None
             else hf_y.values
             if isinstance(hf_y, (pd.Series, pd.Index))
             else hf_y
         )
-        hf_y: np.ndarray = np.asarray(hf_y)
+        # NOTE: the if will not be triggered for a categorical series its values
+        if not hasattr(hf_y, "dtype"):
+            hf_y: np.ndarray = np.asarray(hf_y)
 
         hf_text = (
             hf_text
             if hf_text is not None
             else trace["text"]
             if hasattr(trace, "text") and trace["text"] is not None
             else None
@@ -715,24 +659,23 @@
                             "datetime-like \nMore details in the stacktrace above."
                         )
 
             # If the categorical or string-like hf_y data is of type object (happens
             # when y argument is used for the trace constructor instead of hf_y), we
             # transform it to type string as such it will be sent as categorical data
             # to the downsampling algorithm
-            if hf_y.dtype == "object":
+            if hf_y.dtype == "object" or hf_y.dtype.type == np.str_:
                 # But first, we try to parse to a numeric dtype (as this is the
                 # behavior that plotly supports)
                 # Note that a bool array of type object will remain a bool array (and
                 # not will be transformed to an array of ints (0, 1))
                 try:
                     hf_y = pd.to_numeric(hf_y, errors="raise")
                 except ValueError:
-                    hf_y = hf_y.astype("str")
-
+                    hf_y = pd.Categorical(hf_y)  # TODO: ordered=True?
             assert len(hf_x) == len(hf_y), "x and y have different length!"
         else:
             self._print(f"trace {trace['type']} is not a high-frequency trace")
 
             # hf_x and hf_y have priority over the traces' data
             if hasattr(trace, "x"):
                 trace["x"] = hf_x
@@ -748,43 +691,49 @@
 
         return _hf_data_container(hf_x, hf_y, hf_text, hf_hovertext)
 
     def _construct_hf_data_dict(
         self,
         dc: _hf_data_container,
         trace: BaseTraceType,
-        downsampler: AbstractSeriesAggregator | None,
+        downsampler: AbstractAggregator | None,
+        gap_handler: AbstractGapHandler | None,
         max_n_samples: int | None,
         offset=0,
     ) -> dict:
         """Create the `hf_data` dict which will be put in the `_hf_data` property.
 
         Parameters
         ----------
         dc : _hf_data_container
             The hf_data container, withholding the parsed hf-data.
         trace : BaseTraceType
             The trace.
-        downsampler : AbstractSeriesAggregator | None
+        downsampler : AbstractAggregator | None
             The downsampler which will be used.
+        gap_handler : AbstractGapHandler | None
+            The gap handler which will be used.
         max_n_samples : int | None
             The max number of output samples.
 
         Returns
         -------
         dict
             The hf_data dict.
         """
-        # We will re-create this each time as hf_x and hf_y withholds
-        # high-frequency data and can be adjusted on the fly with the public hf_data
-        # property.
-        hf_series = self._to_hf_series(x=dc.x, y=dc.y)
-
         # Checking this now avoids less interpretable `KeyError` when resampling
-        assert hf_series.index.is_monotonic_increasing
+        assert_text = (
+            "In order to perform time series aggregation, the data must be "
+            "sorted in time; i.e., the x-data must be (non-strictly) "
+            "monotonically increasing."
+        )
+        if isinstance(dc.x, pd.Index):
+            assert dc.x.is_monotonic_increasing, assert_text
+        else:
+            assert pd.Series(dc.x).is_monotonic_increasing, assert_text
 
         # As we support prefix-suffixing of downsampled data, we assure that
         # each trace has a name
         # https://github.com/plotly/plotly.py/blob/ce0ed07d872c487698bde9d52e1f1aadf17aa65f/packages/python/plotly/plotly/basedatatypes.py#L539
         # The link above indicates that the trace index is derived from `data`
         if trace.name is None:
             trace.name = f"trace {len(self.data) + offset}"
@@ -800,27 +749,32 @@
             max_n_samples = self._global_n_shown_samples
 
         default_downsampler = False
         if downsampler is None:
             default_downsampler = True
             downsampler = self._global_downsampler
 
+        default_gap_handler = False
+        if gap_handler is None:
+            default_gap_handler = True
+            gap_handler = self._global_gap_handler
+
         # TODO -> can't we just store the DC here (might be less duplication of
         #  code knowledge, because now, you need to know all the eligible hf_keys in
         #  dc
         return {
             "max_n_samples": max_n_samples,
             "default_n_samples": default_n_samples,
-            "x": dc.x,
-            "y": dc.y,
+            "name": trace.name,
             "axis_type": axis_type,
             "downsampler": downsampler,
             "default_downsampler": default_downsampler,
-            "text": dc.text,
-            "hovertext": dc.hovertext,
+            "gap_handler": gap_handler,
+            "default_gap_handler": default_gap_handler,
+            **dc._asdict(),
         }
 
     @staticmethod
     def _add_trace_to_add_traces_kwargs(kwargs: dict) -> dict:
         """Convert the `add_trace` kwargs to the `add_traces` kwargs."""
         # The keywords that need to be converted to a list
         convert_keywords = ["row", "col", "secondary_y"]
@@ -835,15 +789,16 @@
 
         return {**kwargs, **updated_kwargs}
 
     def add_trace(
         self,
         trace: Union[BaseTraceType, dict],
         max_n_samples: int = None,
-        downsampler: AbstractSeriesAggregator = None,
+        downsampler: AbstractAggregator = None,
+        gap_handler: AbstractGapHandler = None,
         limit_to_view: bool = False,
         # Use these if you want some speedups (and are working with really large data)
         hf_x: Iterable = None,
         hf_y: Iterable = None,
         hf_text: Union[str, Iterable] = None,
         hf_hovertext: Union[str, Iterable] = None,
         check_nans: bool = True,
@@ -865,18 +820,22 @@
                   assumed.
                 - All remaining properties are passed to the constructor
                   of the specified trace type.
         max_n_samples : int, optional
             The maximum number of samples that will be shown by the trace.\n
             .. note::
                 If this variable is not set; ``_global_n_shown_samples`` will be used.
-        downsampler: AbstractSeriesDownsampler, optional
+        downsampler: AbstractAggregator, optional
             The abstract series downsampler method.\n
             .. note::
                 If this variable is not set, ``_global_downsampler`` will be used.
+        gap_handler: AbstractGapHandler, optional
+            The abstract series gap handler method.\n
+            .. note::
+                If this variable is not set, ``_global_gap_handler`` will be used.
         limit_to_view: boolean, optional
             If set to True, the trace's datapoints will be cut to the corresponding
             front-end view, even if the total number of samples is lower than
             ``max_n_samples``, By default False.\n
             Remark that setting this parameter to True ensures that low frequency traces
             are added to the ``hf_data`` property.
         hf_x: Iterable, optional
@@ -983,14 +942,15 @@
                     f"\t[i] DOWNSAMPLE {trace['name']}\t{n_samples}->{max_out_s}"
                 )
 
                 self._hf_data[uuid_str] = self._construct_hf_data_dict(
                     dc,
                     trace=trace,
                     downsampler=downsampler,
+                    gap_handler=gap_handler,
                     max_n_samples=max_n_samples,
                 )
 
                 # Before we update the trace, we create a new pointer to that trace in
                 # which the downsampled data will be stored. This way, the original
                 # data of the trace to this `add_trace` method will not be altered.
                 # We copy (by reference) all the non-data properties of the trace in
@@ -1007,33 +967,29 @@
                 trace = self._check_update_trace_data(trace)
                 assert trace is not None
                 return super(AbstractFigureAggregator, self).add_traces(
                     [trace], **self._add_trace_to_add_traces_kwargs(trace_kwargs)
                 )
             else:
                 self._print(f"[i] NOT resampling {trace['name']} - len={n_samples}")
-                # TODO: can be made more generic
-                trace.x = dc.x
-                trace.y = dc.y
-                trace.text = dc.text
-                trace.hovertext = dc.hovertext
+                for k in dc._fields:
+                    setattr(trace, k, getattr(dc, k))
                 return super(AbstractFigureAggregator, self).add_traces(
                     [trace], **self._add_trace_to_add_traces_kwargs(trace_kwargs)
                 )
         return super(AbstractFigureAggregator, self).add_traces(
             [trace], **self._add_trace_to_add_traces_kwargs(trace_kwargs)
         )
 
     def add_traces(
         self,
         data: List[BaseTraceType | dict] | BaseTraceType | Dict,
         max_n_samples: None | List[int] | int = None,
-        downsamplers: None
-        | List[AbstractSeriesAggregator]
-        | AbstractFigureAggregator = None,
+        downsamplers: None | List[AbstractAggregator] | AbstractAggregator = None,
+        gap_handlers: None | List[AbstractGapHandler] | AbstractGapHandler = None,
         limit_to_views: List[bool] | bool = False,
         check_nans: List[bool] | bool = True,
         **traces_kwargs,
     ):
         """Add traces to the figure.
 
         .. note::
@@ -1057,18 +1013,22 @@
                   - All remaining properties are passed to the constructor
                     of the specified trace type.
 
         max_n_samples : None | List[int] | int, optional
               The maximum number of samples that will be shown for each trace.
               If a single integer is passed, all traces will use this number. If this
               variable is not set; ``_global_n_shown_samples`` will be used.
-        downsamplers : None | List[AbstractSeriesAggregator] | AbstractFigureAggregator, optional
+        downsamplers : None | List[AbstractAggregator] | AbstractAggregator, optional
             The downsampler that will be used to aggregate the traces. If a single
             aggregator is passed, all traces will use this aggregator.
             If this variable is not set, ``_global_downsampler`` will be used.
+        gap_handlers : None | List[AbstractGapHandler] | AbstractGapHandler, optional
+            The gap handler that will be used to aggregate the traces. If a single
+            gap handler is passed, all traces will use this gap handler.
+            If this variable is not set, ``_global_gap_handler`` will be used.
         limit_to_views : None | List[bool] | bool, optional
             List of limit_to_view booleans for the added traces. If set to True the
             trace's datapoints will be cut to the corresponding front-end view, even if
             the total number of samples is lower than ``max_n_samples``.
             If a single boolean is passed, all to be added traces will use this value,
             by default False.\n
             Remark that setting this parameter to True ensures that low frequency traces
@@ -1113,24 +1073,30 @@
         for trace in data:
             uuid_str = str(uuid4()) if trace.uid is None else trace.uid
             trace.uid = uuid_str
 
         # Convert the data properties
         if isinstance(max_n_samples, (int, np.integer)) or max_n_samples is None:
             max_n_samples = [max_n_samples] * len(data)
-        if isinstance(downsamplers, AbstractSeriesAggregator) or downsamplers is None:
+        if isinstance(downsamplers, AbstractAggregator) or downsamplers is None:
             downsamplers = [downsamplers] * len(data)
+        if isinstance(gap_handlers, AbstractGapHandler) or gap_handlers is None:
+            gap_handlers = [gap_handlers] * len(data)
         if isinstance(limit_to_views, bool):
             limit_to_views = [limit_to_views] * len(data)
         if isinstance(check_nans, bool):
             check_nans = [check_nans] * len(data)
 
-        for i, (trace, max_out, downsampler, limit_to_view, check_nan) in enumerate(
-            zip(data, max_n_samples, downsamplers, limit_to_views, check_nans)
-        ):
+        zipped = zip(
+            data, max_n_samples, downsamplers, gap_handlers, limit_to_views, check_nans
+        )
+        for (
+            i,
+            (trace, max_out, downsampler, gap_handler, limit_to_view, check_nan),
+        ) in enumerate(zipped):
             if (
                 trace.type.lower() not in self._high_frequency_traces
                 or self._hf_data.get(trace.uid) is not None
             ):
                 continue
 
             max_out_s = self._global_n_shown_samples if max_out is None else max_out
@@ -1138,14 +1104,15 @@
                 continue
 
             dc = self._parse_get_trace_props(trace, check_nans=check_nan)
             self._hf_data[trace.uid] = self._construct_hf_data_dict(
                 dc,
                 trace=trace,
                 downsampler=downsampler,
+                gap_handler=gap_handler,
                 max_n_samples=max_out,
                 offset=i,
             )
 
             # convert the trace into a dict, and only withholds the non-hf props
             trace = trace._props
             trace = {k: trace[k] for k in set(trace.keys()).difference(set(dc._fields))}
@@ -1154,15 +1121,15 @@
             trace = self._check_update_trace_data(trace)
             assert trace is not None
             data[i] = trace
 
         return super(self._figure_class, self).add_traces(data, **traces_kwargs)
 
     def _clear_figure(self):
-        """Clear the current figure object it's data and layout."""
+        """Clear the current figure object its data and layout."""
         self._hf_data = {}
         self.data = []
         self._data = []
         self._layout = {}
         self.layout = {}
 
     def _copy_hf_data(self, hf_data: dict, adjust_default_values: bool = False) -> dict:
@@ -1189,14 +1156,16 @@
         }
 
         # Adjust the default arguments to the current argument values
         if adjust_default_values:
             for hf_props in hf_data_cp.values():
                 if hf_props.get("default_downsampler", False):
                     hf_props["downsampler"] = self._global_downsampler
+                if hf_props.get("default_gap_handler", False):
+                    hf_props["gap_handler"] = self._global_gap_handler
                 if hf_props.get("default_n_samples", False):
                     hf_props["max_n_samples"] = self._global_n_shown_samples
 
         return hf_data_cp
 
     def replace(self, figure: go.Figure, convert_existing_traces: bool = True):
         """Replace the current figure layout with the passed figure object.
@@ -1215,14 +1184,35 @@
             figure=figure,
             convert_existing_traces=convert_existing_traces,
             default_n_shown_samples=self._global_n_shown_samples,
             default_downsampler=self._global_downsampler,
             resampled_trace_prefix_suffix=(self._prefix, self._suffix),
         )
 
+    def _parse_relayout(self, relayout_dict: dict) -> dict:
+        """Update the relayout object so that the autorange will be set to None when
+        there are xy-matches.
+
+        Parameters
+        ----------
+        relayout_dict : dict
+            The relayout dictionary.
+        """
+        # 1. Create a new dict with additional layout updates for the front-end
+        extra_layout_updates = {}
+
+        # 1.1. Set autorange to False for each layout item with a specified x-range
+        xy_matches = self._re_matches(
+            re.compile(r"[xy]axis\d*.range\[\d+]"), relayout_dict.keys()
+        )
+        for range_change_axis in xy_matches:
+            axis = range_change_axis.split(".")[0]
+            extra_layout_updates[f"{axis}.autorange"] = None
+        return extra_layout_updates
+
     def construct_update_data(
         self,
         relayout_data: dict,
     ) -> Union[List[dict], dash.no_update]:
         """Construct the to-be-updated front-end data, based on the layout change.
 
         Attention
@@ -1250,21 +1240,21 @@
 
         """
         current_graph = self._get_current_graph()
         updated_trace_indices, cl_k = [], []
         if relayout_data:
             self._print("-" * 100 + "\n", "changed layout", relayout_data)
 
-            cl_k = relayout_data.keys()
+            cl_k = list(relayout_data.keys())
 
             # ------------------ HF DATA aggregation ---------------------
             # 1. Base case - there is an x-range specified in the front-end
             start_matches = self._re_matches(re.compile(r"xaxis\d*.range\[0]"), cl_k)
             stop_matches = self._re_matches(re.compile(r"xaxis\d*.range\[1]"), cl_k)
-            if len(start_matches) and len(stop_matches):
+            if start_matches and stop_matches:  # when both are not empty
                 for t_start_key, t_stop_key in zip(start_matches, stop_matches):
                     # Check if the xaxis<NUMB> part of xaxis<NUMB>.[0-1] matches
                     xaxis = t_start_key.split(".")[0]
                     assert xaxis == t_stop_key.split(".")[0]
                     # -> we want to copy the layout on the back-end
                     updated_trace_indices = self._check_update_figure_dict(
                         current_graph,
@@ -1276,55 +1266,49 @@
 
             # 2. The user clicked on either autorange | reset axes
             autorange_matches = self._re_matches(
                 re.compile(r"xaxis\d*.autorange"), cl_k
             )
             spike_matches = self._re_matches(re.compile(r"xaxis\d*.showspikes"), cl_k)
             # 2.1 Reset-axes -> autorange & reset to the global data view
-            if len(autorange_matches) and len(spike_matches):
+            if autorange_matches and spike_matches:  # when both are not empty
                 for autorange_key in autorange_matches:
                     if relayout_data[autorange_key]:
                         xaxis = autorange_key.split(".")[0]
                         updated_trace_indices = self._check_update_figure_dict(
                             current_graph,
                             xaxis_filter=xaxis,
                             updated_trace_indices=updated_trace_indices,
                         )
             # 2.1. Autorange -> do nothing, the autorange will be applied on the
             #      current front-end view
-            elif len(autorange_matches) and not len(spike_matches):
+            elif (
+                autorange_matches and not spike_matches
+            ):  # when only autorange is not empty
                 # PreventUpdate returns a 204 status code response on the
                 # relayout post request
                 return dash.no_update
 
         # If we do not have any traces to be updated, we will return an empty
         # request response
-        if len(updated_trace_indices) == 0:
+        if not updated_trace_indices:  # when updated_trace_indices is empty
             # PreventUpdate returns a 204 status-code response on the relayout post
             # request
             return dash.no_update
 
         # -------------------- construct callback data --------------------------
-        layout_traces_list: List[dict] = []  # the data
-
-        # 1. Create a new dict with additional layout updates for the front-end
-        extra_layout_updates = {}
-
-        # 1.1. Set autorange to False for each layout item with a specified x-range
-        xy_matches = self._re_matches(re.compile(r"[xy]axis\d*.range\[\d+]"), cl_k)
-        for range_change_axis in xy_matches:
-            axis = range_change_axis.split(".")[0]
-            extra_layout_updates[f"{axis}.autorange"] = None
-        layout_traces_list.append(extra_layout_updates)
+        # 1. Create the layout data for the front-end
+        layout_traces_list: List[dict] = [relayout_data]
 
         # 2. Create the additional trace data for the frond-end
-        relevant_keys = ["x", "y", "text", "hovertext", "name"]  # TODO - marker color
+        relevant_keys = list(_hf_data_container._fields) + ["name"]
         # Note that only updated trace-data will be sent to the client
         for idx in updated_trace_indices:
             trace = current_graph["data"][idx]
+            # TODO: check if we can reduce even more
             trace_reduced = {k: trace[k] for k in relevant_keys if k in trace}
 
             # Store the index into the corresponding to-be-sent trace-data so
             # the client front-end can know which trace needs to be updated
             trace_reduced.update({"index": idx})
             layout_traces_list.append(trace_reduced)
         return layout_traces_list
@@ -1332,15 +1316,15 @@
     @staticmethod
     def _parse_dtype_orjson(series: np.ndarray) -> np.ndarray:
         """Verify the orjson compatibility of the series and convert it if needed."""
         # NOTE:
         #    * float16 and float128 aren't supported with latest orjson versions (3.8.1)
         #    * this method assumes that the it will not get a float128 series
         # -> this method can be removed if orjson supports float16
-        if series.dtype in [np.float16]:
+        if series.dtype == np.float16:
             return series.astype(np.float32)
         return series
 
     @staticmethod
     def _re_matches(regex: re.Pattern, strings: Iterable[str]) -> List[str]:
         """Returns all the items in ``strings`` which regex.match(es) ``regex``."""
         matches = []
@@ -1350,15 +1334,15 @@
                 matches.append(m.string)
         return sorted(matches)
 
     @staticmethod
     def _is_no_update(update_data: Union[List[dict], dash.no_update]) -> bool:
         return update_data is dash.no_update
 
-    ## Magic methods (to use plotly.py words :grin:)
+    # ------------------------------- Magic methods ---------------------------------
 
     def _get_pr_props_keys(self) -> List[str]:
         """Returns the keys (i.e., the names) of the plotly-resampler properties.
 
         Note
         ----
         This method is used to serialize the object in the `__reduce__` method.
```

### Comparing `plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/figurewidget_resampler.py` & `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figurewidget_resampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
 
 from typing import Tuple
 
 import plotly.graph_objects as go
 from plotly.basedatatypes import BaseFigure
 
-from ..aggregation import AbstractSeriesAggregator, EfficientLTTB
+from ..aggregation import (
+    AbstractAggregator,
+    AbstractGapHandler,
+    MedDiffGapHandler,
+    MinMaxLTTB,
+)
 from .figure_resampler_interface import AbstractFigureAggregator
 
 
 class _FigureWidgetResamplerM(type(AbstractFigureAggregator), type(go.FigureWidget)):
     # MetaClass for the FigureWidgetResampler
     pass
 
@@ -39,15 +44,16 @@
     """
 
     def __init__(
         self,
         figure: BaseFigure | dict = None,
         convert_existing_traces: bool = True,
         default_n_shown_samples: int = 1000,
-        default_downsampler: AbstractSeriesAggregator = EfficientLTTB(),
+        default_downsampler: AbstractAggregator = MinMaxLTTB(),
+        default_gap_handler: AbstractGapHandler = MedDiffGapHandler(),
         resampled_trace_prefix_suffix: Tuple[str, str] = (
             '<b style="color:sandybrown">[R]</b> ',
             "",
         ),
         show_mean_aggregation_size: bool = True,
         convert_traces_kwargs: dict | None = None,
         verbose: bool = False,
@@ -88,14 +94,15 @@
             f.add_traces(figure)
 
         super().__init__(
             f,
             convert_existing_traces,
             default_n_shown_samples,
             default_downsampler,
+            default_gap_handler,
             resampled_trace_prefix_suffix,
             show_mean_aggregation_size,
             convert_traces_kwargs,
             verbose,
         )
 
         if isinstance(figure, AbstractFigureAggregator):
@@ -164,15 +171,15 @@
                 relayout_dict[f"{xaxis_str}.range[0]"] = x_range[0]
                 relayout_dict[f"{xaxis_str}.range[1]"] = x_range[1]
 
                 # An update will take place for that trace
                 # -> save current xaxis range to _prev_layout
                 self._prev_layout[xaxis_str]["range"] = x_range
 
-        if len(relayout_dict):
+        if relayout_dict:  # when not empty
             # Construct the update data
             update_data = self.construct_update_data(relayout_dict)
 
             if self._is_no_update(update_data):
                 # Return when no data update
                 return
 
@@ -180,15 +187,15 @@
                 self._relayout_hist.append(dict(zip(self._xaxis_list, x_ranges)))
                 self._relayout_hist.append(layout)
                 self._relayout_hist.append(["xaxis-range-update", len(update_data) - 1])
                 self._relayout_hist.append("-" * 30)
 
             with self.batch_update():
                 # First update the layout (first item of update_data)
-                self.layout.update(update_data[0])
+                self.layout.update(self._parse_relayout(update_data[0]))
 
                 for xaxis_str in self._xaxis_list:
                     if "showspikes" in layout[xaxis_str]:
                         self.layout[xaxis_str].pop("showspikes")
 
                 # Then update the data
                 for updated_trace in update_data[1:]:
@@ -251,15 +258,15 @@
                 self._relayout_hist.append(layout)
                 self._relayout_hist.append(["showspikes-update", len(update_data) - 1])
                 self._relayout_hist.append("-" * 30)
 
             with self.batch_update():
                 # First update the layout (first item of update_data)
                 if not force_update:
-                    self.layout.update(update_data[0])
+                    self.layout.update(self._parse_relayout(update_data[0]))
 
                 # Also:  Remove the showspikes from the layout, otherwise the autorange
                 # will not work as intended (it will not be triggered again)
                 # Note: this removal causes a second trigger of this method
                 # which will go in the "else" part below.
                 for xaxis_str in self._xaxis_list:
                     self.layout[xaxis_str].pop("showspikes")
```

### Comparing `plotly_resampler-0.8.4rc1/plotly_resampler/figure_resampler/utils.py` & `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -110,62 +110,97 @@
     td: pd.Timedelta
         The timedelta for which the string representation is constructed
 
     Returns
     -------
     str:
         The tight string bounds of format '$d-$h$m$s.$ms'.
+        If the timedelta is negative, the string starts with 'NEG'.
 
     """
     out_str = ""
 
     # Edge case if we deal with negative
     if td < pd.Timedelta(seconds=0):
         td *= -1
         out_str += "NEG"
 
     # Note: this must happen after the *= -1
     c = td.components
     if c.days > 0:
         out_str += f"{c.days}D"
     if c.hours > 0 or c.minutes > 0 or c.seconds > 0 or c.milliseconds > 0:
-        out_str += "_" if len(out_str) else ""
+        out_str += "_" if out_str else ""  # add seperator if non-empty
 
     if c.hours > 0:
         out_str += f"{c.hours}h"
     if c.minutes > 0:
         out_str += f"{c.minutes}m"
     if c.seconds > 0:
         if c.milliseconds:
             out_str += (
                 f"{c.seconds}.{str(c.milliseconds / 1000).split('.')[-1].rstrip('0')}s"
             )
         else:
             out_str += f"{c.seconds}s"
     elif c.milliseconds > 0:
-        out_str += f"{str(c.milliseconds)}ms"
+        out_str += f"{c.milliseconds}ms"
     if c.microseconds > 0:
-        out_str += f"{str(c.microseconds)}us"
+        out_str += f"{c.microseconds}us"
     if c.nanoseconds > 0:
-        out_str += f"{str(c.nanoseconds)}ns"
+        out_str += f"{c.nanoseconds}ns"
     return out_str
 
 
 def round_td_str(td: pd.Timedelta) -> str:
     """Round a timedelta to the nearest unit and convert to a string.
 
+    Parameters
+    ----------
+    td : pd.Timedelta
+        The timedelta to round.
+
+    Returns
+    -------
+    str
+        The rounded timedelta as a string.
+        If the timedelta is == 0, None is returned.
+
     .. seealso::
         :func:`timedelta_to_str`
+
     """
-    for t_s in ["D", "H", "min", "s", "ms", "us", "ns"]:
+    for t_s in ("D", "H", "min", "s", "ms", "us", "ns"):
         if td > 0.95 * pd.Timedelta(f"1{t_s}"):
             return timedelta_to_str(td.round(t_s))
 
 
 def round_number_str(number: float) -> str:
+    """Round a number to the nearest unit and convert to a string.
+
+    Parameters
+    ----------
+    number : float
+        The number to round.
+
+    Returns
+    -------
+    str
+        The rounded number as a string.
+        If the number is == 0, None is returned.
+
+    """
+    sign = "-" if number < 0 else ""
+    number = abs(number)
     if number > 0.95:
-        for unit, scaling in [("M", int(1e6)), ("k", int(1e3))]:
+        for unit, scaling in [
+            ("T", int(1e12)),  # Trillion
+            ("B", int(1e9)),  # Billion
+            ("M", int(1e6)),  # Million
+            ("k", int(1e3)),  # Thousand
+        ]:
             if number / scaling > 0.95:
                 return f"{round(number / scaling)}{unit}"
-        return str(round(number))
-    # we have a number < 1 --> round till nearest non-zero digit
-    return str(round(number, 1 + abs(int(math.log10(number)))))
+        return sign + str(round(number))
+    if number > 0:  # avoid log10(0)
+        # we have a number between 0-0.95 -> round till nearest non-zero digit
+        return sign + str(round(number, 1 + abs(int(math.log10(number)))))
```

### Comparing `plotly_resampler-0.8.4rc1/plotly_resampler/registering.py` & `plotly_resampler-0.9.0rc0/plotly_resampler/registering.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.8.4rc1/pyproject.toml` & `plotly_resampler-0.9.0rc0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plotly-resampler"  # Do not forget to update the __init__.py __version__ variable
-version = "0.8.4rc1"
+version = "0.9.0rc0"
 description = "Visualizing large time series with plotly"
 authors = ["Jonas Van Der Donckt", "Jeroen Van Der Donckt", "Emiel Deprost"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/predict-idlab/plotly-resampler"
 documentation = "https://predict-idlab.github.io/plotly-resampler"
 keywords = ["time-series", "visualization", "resampling", "plotly", "plotly-dash"]
@@ -12,77 +12,89 @@
     { include = "plotly_resampler" }
 ]
 include = [
     # C extensions must be included in the wheel distributions
     {path = "plotly_resampler/aggregation/algorithms/*.so", format = "wheel"},
     {path = "plotly_resampler/aggregation/algorithms/*.pyd", format = "wheel"}
 ]
-build = "build.py"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 jupyter-dash = ">=0.4.2"
 plotly = "^5.5.0"
 dash = "^2.2.0"
-pandas = "^1.3.5"
+pandas = ">=1"
 trace-updater = ">=0.0.8"
 numpy = [
     { version = ">=1.14", python = "<3.11" },
     { version = ">=1.24", python = ">=3.11" }
 ]
-Flask-Cors = "^3.0.10"
 orjson = "^3.8.0"  # Faster json serialization
-# TODO -> check other werkzeug versions: 2.1.2 and 2.1.1 seem to work.
-# https://github.com/predict-idlab/plotly-resampler/issues/123
-Werkzeug = "<=2.1.2"
+# Optional dependencies
+Flask-Cors = { version = "^3.0.10", optional = true }
+# Lock kaleido dependency until https://github.com/plotly/Kaleido/issues/156 is resolved
+kaleido = {version = "0.2.1", optional = true}
+tsdownsample = "0.1.2"
+
+[tool.poetry.extras]
+# Optional dependencies
+inline_persistent = ["kaleido", "Flask-Cors"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 selenium = "4.2.0"
 pytest-selenium = "^2.0.1"
 webdriver-manager = "^3.5.2"
 selenium-wire = "^5.0"
 pyarrow = "^10.0"
 Sphinx = "^4.4.0"
-pydata-sphinx-theme = "^0.9.0"
+pydata-sphinx-theme = "^0.13.3"
 sphinx-autodoc-typehints = "^1.17.0"
 ipywidgets = "^7.7.1"
 memory-profiler = "^0.60.0"
 line-profiler = "^4.0"
-kaleido = "0.2.1"
 ruff = "^0.0.173"
 black = "^22.6.0"
 isort = "^5.10.1"
+pytest-lazy-fixture = "^0.6.3"
 # yep = "^0.4"  # c code profiling
 
 # Linting
 [tool.ruff]
 line-length = 88
 ignore = ["E501"] # Never enforce `E501` (line length violations).
 [tool.ruff.per-file-ignores]
 "tests/test_registering.py" = ["F401", "F811"]
 "tests/test_serialization.py" = ["F401", "F811"]
 
 # Formatting
 [tool.black]
-color = true
 line-length = 88
 
 # Sort imports
 [tool.isort]
 line_length = 88
 known_first_party = ["plotly_resampler"]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 combine_as_imports = true
 
 [build-system]
-requires = [
-    "setuptools",
-    "poetry-core>=1.1.0a6",
-    "wheel",
-    # https://github.com/scipy/oldest-supported-numpy
-    "oldest-supported-numpy; python_version>='3.7'",
-]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `plotly_resampler-0.8.4rc1/setup.py` & `plotly_resampler-0.9.0rc0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,214 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['plotly_resampler',
- 'plotly_resampler.aggregation',
- 'plotly_resampler.aggregation.algorithms',
- 'plotly_resampler.figure_resampler']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Flask-Cors>=3.0.10,<4.0.0',
- 'Werkzeug<=2.1.2',
- 'dash>=2.2.0,<3.0.0',
- 'jupyter-dash>=0.4.2',
- 'orjson>=3.8.0,<4.0.0',
- 'pandas>=1.3.5,<2.0.0',
- 'plotly>=5.5.0,<6.0.0',
- 'trace-updater>=0.0.8']
-
-extras_require = \
-{':python_version < "3.11"': ['numpy>=1.14'],
- ':python_version >= "3.11"': ['numpy>=1.24']}
-
-setup_kwargs = {
-    'name': 'plotly-resampler',
-    'version': '0.8.4rc1',
-    'description': 'Visualizing large time series with plotly',
-    'long_description': '<p align="center">\n    <a href="#readme">\n        <img alt="Plotly-Resampler logo" src="https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/logo.svg" width=65%>\n    </a>\n</p>\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)](https://pypi.org/project/plotly-resampler/)\n[![support-version](https://img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/pyversions/plotly-resampler)\n[![codecov](https://img.shields.io/codecov/c/github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/predict-idlab/plotly-resampler)\n[![Code quality](https://img.shields.io/lgtm/grade/python/github/predict-idlab/plotly-resampler?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-idlab/plotly-resampler/context:python)\n[![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)\n[![Documentation](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml)\n[![Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml)\n\n\n<!-- [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler) -->\n\n> `plotly_resampler`: visualize large sequential data by **adding resampling functionality to Plotly figures**\n\n[Plotly](https://github.com/plotly/plotly.py) is an awesome interactive visualization library, however it can get pretty slow when a lot of data points are visualized (100 000+ datapoints). This library solves this by downsampling (aggregating) the data respective to the view and then plotting the aggregated points. When you interact with the plot (panning, zooming, ...), callbacks are used to aggregate data and update the figure.\n\n![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/basic_example.gif)\n\n\nIn [this Plotly-Resampler demo](https://github.com/predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over `110,000,000` data points are visualized!\n\n<!-- These dynamic aggregation callbacks are realized with: -->\n<!-- * [Dash](https://github.com/plotly/dash) when a `go.Figure` object is wrapped with dynamic aggregation functionality, see example ⬆️. -->\n<!-- * The [FigureWidget.layout.on_change](https://plotly.com/python-api-reference/generated/plotly.html?highlight=on_change#plotly.basedatatypes.BasePlotlyType.on_change) method, when a `go.FigureWidget` is used within a `.ipynb` environment. -->\n\n<!-- #### Useful links -->\n\n<!-- - [Documentation]() work in progress 🚧  -->\n<!-- - [Example notebooks](https://github.com/predict-idlab/plotly-resampler/tree/main/examples/) -->\n\n### Installation\n\n| [**pip**](https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |\n| ---| ----|\n<!-- | [**conda**](https://anaconda.org/conda-forge/plotly_resampler/) | `conda install -c conda-forge plotly_resampler` | -->\n\n<br>\n\n## Usage\n\n**Add dynamic aggregation** to your plotly Figure _(unfold your fitting use case)_\n* 🤖 <b>Automatically</b> _(minimal code overhead)_:\n  <details><summary>Use the <code>register_plotly_resampler</code> function</summary>\n    <br>\n\n    1. Import and call the `register_plotly_resampler` method\n    2. Just use your regular graph construction code\n\n    * **code example**:\n      ```python\n      import plotly.graph_objects as go; import numpy as np\n      from plotly_resampler import register_plotly_resampler\n\n      # Call the register function once and all Figures/FigureWidgets will be wrapped\n      # according to the register_plotly_resampler its `mode` argument\n      register_plotly_resampler(mode=\'auto\')\n\n      x = np.arange(1_000_000)\n      noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000\n\n\n      # auto mode: when working in an IPython environment, this will automatically be a \n      # FigureWidgetResampler else, this will be an FigureResampler\n      f = go.Figure()\n      f.add_trace({"y": noisy_sin + 2, "name": "yp2"})\n      f\n      ```\n\n    > **Note**: This wraps **all** plotly graph object figures with a \n    > `FigureResampler` | `FigureWidgetResampler`. This can thus also be \n    > used for the `plotly.express` interface. 🎉\n\n  </details>\n\n* 👷 <b>Manually</b> _(higher data aggregation configurability, more speedup possibilities)_:\n  <details>\n    <summary>Within a <b><i>jupyter</i></b> environment without creating a <i>web application</i></summary>\n    <br>\n\n    1. wrap the plotly Figure with `FigureWidgetResampler`\n    2. output the `FigureWidgetResampler` instance in a cell\n\n    * **code example**:\n      ```python\n      import plotly.graph_objects as go; import numpy as np\n      from plotly_resampler import FigureResampler, FigureWidgetResampler\n\n      x = np.arange(1_000_000)\n      noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000\n\n      # OPTION 1 - FigureWidgetResampler: dynamic aggregation via `FigureWidget.layout.on_change`\n      fig = FigureWidgetResampler(go.Figure())\n      fig.add_trace(go.Scattergl(name=\'noisy sine\', showlegend=True), hf_x=x, hf_y=noisy_sin)\n\n      fig\n      ```\n  </details>\n  <details>\n    <summary>Using a <b><i>web-application</i></b> with <b><a href="https://github.com/plotly/dash">dash</a></b> callbacks</summary>\n    <br>\n\n    1. wrap the plotly Figure with `FigureResampler`\n    2. call `.show_dash()` on the `Figure`\n\n    * **code example**:\n      ```python\n      import plotly.graph_objects as go; import numpy as np\n      from plotly_resampler import FigureResampler, FigureWidgetResampler\n\n      x = np.arange(1_000_000)\n      noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000\n\n      # OPTION 2 - FigureResampler: dynamic aggregation via a Dash web-app\n      fig = FigureResampler(go.Figure())\n      fig.add_trace(go.Scattergl(name=\'noisy sine\', showlegend=True), hf_x=x, hf_y=noisy_sin)\n\n      fig.show_dash(mode=\'inline\')\n      ```\n\n  </details>\n  <br>\n\n  > **Tip** 💡:\n   > For significant faster initial loading of the Figure, we advise to wrap the \n   > constructor of the plotly Figure and add the trace data as `hf_x` and `hf_y`\n\n<br>\n\n> **Note**:\n> Any plotly Figure can be wrapped with `FigureResampler` and `FigureWidgetResampler`! 🎉\n> But, (obviously) only the scatter traces will be resampled.\n\n\n\n\n<br>\n<details><summary>👉 <b>Features</b></summary>\n\n  * **Convenient** to use:\n    * just add either\n      * `register_plotly_resampler` function to your notebook with the best suited `mode` argument.\n      * `FigureResampler` decorator around a plotly Figure and call `.show_dash()`\n      * `FigureWidgetResampler` decorator around a plotly Figure and output the instance in a cell\n    * allows all other plotly figure construction flexibility to be used!\n  * **Environment-independent**\n    * can be used in Jupyter, vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as application (on a server)\n  * Interface for **various aggregation algorithms**:\n    * ability to develop or select your preferred sequence aggregation method\n</details>\n\n### Important considerations & tips\n\n* When running the code on a server, you should forward the port of the `FigureResampler.show_dash()` method to your local machine.<br>\n  **Note** that you can add dynamic aggregation to plotly figures with the `FigureWidgetResampler` wrapper without needing to forward a port!\n* The `FigureWidgetResampler` *uses the IPython main thread* for its data aggregation functionality, so when this main thread is occupied, no resampling logic can be executed. For example; if you perform long computations within your notebook, the kernel will be occupied during these computations, and will only execute the resampling operations that take place during these computations after finishing that computation.\n* In general, when using downsampling one should be aware of (possible) [aliasing](https://en.wikipedia.org/wiki/Aliasing) effects.\n  The <b style="color:orange">[R]</b> in the legend indicates when the corresponding trace is being resampled (and thus possibly distorted) or not. Additionally, the `~<range>` suffix represent the mean aggregation bin size in terms of the sequence index.\n* The plotly **autoscale** event (triggered by the autoscale button or a double-click within the graph), **does not reset the axes but autoscales the current graph-view** of plotly-resampler figures. This design choice was made as it seemed more intuitive for the developers to support this behavior with double-click than the default axes-reset behavior. The graph axes can ofcourse be resetted by using the `reset_axis` button.  If you want to give feedback and discuss this further with the developers, see issue [#49](https://github.com/predict-idlab/plotly-resampler/issues/49).\n\n## Cite\n\nPaper (preprint): https://arxiv.org/abs/2206.08703\n\n```latex\n@misc{https://doi.org/10.48550/arxiv.2206.08703,\n  author = {Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},\n  title = {Plotly-Resampler: Effective Visual Analytics for Large Time Series},\n  year = {2022},\n  doi = {10.48550/ARXIV.2206.08703},\n  url = {https://arxiv.org/abs/2206.08703},\n  publisher = {arXiv},\n}\n```\n\n## Future work 🔨\n\n- [x] Support `.add_traces()` (currently only `.add_trace` is supported)\n- [ ] Support `hf_color` and `hf_markersize`, see [#50](https://github.com/predict-idlab/plotly-resampler/pull/50)\n- [ ] Create C bindings for our EfficientLTTB algorithm.\n\n<br>\n\n---\n\n<p align="center">\n👤 <i>Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost</i>\n</p>\n',
-    'author': 'Jonas Van Der Donckt',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/predict-idlab/plotly-resampler',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<4.0.0',
+Metadata-Version: 2.1
+Name: plotly-resampler
+Version: 0.9.0rc0
+Summary: Visualizing large time series with plotly
+Home-page: https://github.com/predict-idlab/plotly-resampler
+License: MIT
+Keywords: time-series,visualization,resampling,plotly,plotly-dash
+Author: Jonas Van Der Donckt
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: inline-persistent
+Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0) ; extra == "inline-persistent"
+Requires-Dist: dash (>=2.2.0,<3.0.0)
+Requires-Dist: jupyter-dash (>=0.4.2)
+Requires-Dist: kaleido (==0.2.1) ; extra == "inline-persistent"
+Requires-Dist: numpy (>=1.14) ; python_version < "3.11"
+Requires-Dist: numpy (>=1.24) ; python_version >= "3.11"
+Requires-Dist: orjson (>=3.8.0,<4.0.0)
+Requires-Dist: pandas (>=1)
+Requires-Dist: plotly (>=5.5.0,<6.0.0)
+Requires-Dist: trace-updater (>=0.0.8)
+Requires-Dist: tsdownsample (==0.1.2)
+Project-URL: Documentation, https://predict-idlab.github.io/plotly-resampler
+Project-URL: Repository, https://github.com/predict-idlab/plotly-resampler
+Description-Content-Type: text/markdown
+
+<p align="center">
+    <a href="#readme">
+        <img alt="Plotly-Resampler logo" src="https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/logo.svg" width=65%>
+    </a>
+</p>
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)](https://pypi.org/project/plotly-resampler/)
+[![support-version](https://img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/pyversions/plotly-resampler)
+[![codecov](https://img.shields.io/codecov/c/github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/predict-idlab/plotly-resampler)
+[![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
+[![Documentation](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml)
+[![Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml)
+
+
+<!-- [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler) -->
+
+> `plotly_resampler`: visualize large sequential data by **adding resampling functionality to Plotly figures**
+
+[Plotly](https://github.com/plotly/plotly.py) is an awesome interactive visualization library, however it can get pretty slow when a lot of data points are visualized (100 000+ datapoints). This library solves this by downsampling (aggregating) the data respective to the view and then plotting the aggregated points. When you interact with the plot (panning, zooming, ...), callbacks are used to aggregate data and update the figure.
+
+![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/basic_example.gif)
+
+
+In [this Plotly-Resampler demo](https://github.com/predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over `110,000,000` data points are visualized!
+
+<!-- These dynamic aggregation callbacks are realized with: -->
+<!-- * [Dash](https://github.com/plotly/dash) when a `go.Figure` object is wrapped with dynamic aggregation functionality, see example ⬆️. -->
+<!-- * The [FigureWidget.layout.on_change](https://plotly.com/python-api-reference/generated/plotly.html?highlight=on_change#plotly.basedatatypes.BasePlotlyType.on_change) method, when a `go.FigureWidget` is used within a `.ipynb` environment. -->
+
+<!-- #### Useful links -->
+
+<!-- - [Documentation]() work in progress 🚧  -->
+<!-- - [Example notebooks](https://github.com/predict-idlab/plotly-resampler/tree/main/examples/) -->
+
+### Installation
+
+| [**pip**](https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
+| ---| ----|
+<!-- | [**conda**](https://anaconda.org/conda-forge/plotly_resampler/) | `conda install -c conda-forge plotly_resampler` | -->
+
+### Features :tada:
+
+  * **Convenient** to use:
+    * just add either
+      * `register_plotly_resampler` function to your notebook with the best suited `mode` argument.
+      * `FigureResampler` decorator around a plotly Figure and call `.show_dash()`
+      * `FigureWidgetResampler` decorator around a plotly Figure and output the instance in a cell
+    * allows all other plotly figure construction flexibility to be used!
+  * **Environment-independent**
+    * can be used in Jupyter, vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as application (on a server)
+  * Interface for **various aggregation algorithms**:
+    * ability to develop or select your preferred sequence aggregation method
+
+## Usage
+
+**Add dynamic aggregation** to your plotly Figure _(unfold your fitting use case)_
+* 🤖 <b>Automatically</b> _(minimal code overhead)_:
+  <details><summary>Use the <code>register_plotly_resampler</code> function</summary>
+    <br>
+
+    1. Import and call the `register_plotly_resampler` method
+    2. Just use your regular graph construction code
+
+    * **code example**:
+      ```python
+      import plotly.graph_objects as go; import numpy as np
+      from plotly_resampler import register_plotly_resampler
+
+      # Call the register function once and all Figures/FigureWidgets will be wrapped
+      # according to the register_plotly_resampler its `mode` argument
+      register_plotly_resampler(mode='auto')
+
+      x = np.arange(1_000_000)
+      noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000
+
+
+      # auto mode: when working in an IPython environment, this will automatically be a 
+      # FigureWidgetResampler else, this will be an FigureResampler
+      f = go.Figure()
+      f.add_trace({"y": noisy_sin + 2, "name": "yp2"})
+      f
+      ```
+
+    > **Note**: This wraps **all** plotly graph object figures with a 
+    > `FigureResampler` | `FigureWidgetResampler`. This can thus also be 
+    > used for the `plotly.express` interface. 🎉
+
+  </details>
+
+* 👷 <b>Manually</b> _(higher data aggregation configurability, more speedup possibilities)_:
+  * Within a <b><i>jupyter</i></b> environment without creating a <i>web application</i>
+    1. wrap the plotly Figure with `FigureWidgetResampler`
+    2. output the `FigureWidgetResampler` instance in a cell
+      ```python
+      import plotly.graph_objects as go; import numpy as np
+      from plotly_resampler import FigureResampler, FigureWidgetResampler
+
+      x = np.arange(1_000_000)
+      noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000
+
+      # OPTION 1 - FigureWidgetResampler: dynamic aggregation via `FigureWidget.layout.on_change`
+      fig = FigureWidgetResampler(go.Figure())
+      fig.add_trace(go.Scattergl(name='noisy sine', showlegend=True), hf_x=x, hf_y=noisy_sin)
+
+      fig
+      ```
+  * Using a <b><i>web-application</i></b> with <b><a href="https://github.com/plotly/dash">dash</a></b> callbacks
+    1. wrap the plotly Figure with `FigureResampler`
+    2. call `.show_dash()` on the `Figure`
+      ```python
+      import plotly.graph_objects as go; import numpy as np
+      from plotly_resampler import FigureResampler, FigureWidgetResampler
+
+      x = np.arange(1_000_000)
+      noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000
+
+      # OPTION 2 - FigureResampler: dynamic aggregation via a Dash web-app
+      fig = FigureResampler(go.Figure())
+      fig.add_trace(go.Scattergl(name='noisy sine', showlegend=True), hf_x=x, hf_y=noisy_sin)
+
+      fig.show_dash(mode='inline')
+      ```
+  > **Tip** 💡:
+   > For significant faster initial loading of the Figure, we advise to wrap the 
+   > constructor of the plotly Figure and add the trace data as `hf_x` and `hf_y`
+
+<br>
+
+> **Note**:
+> Any plotly Figure can be wrapped with `FigureResampler` and `FigureWidgetResampler`! 🎉
+> But, (obviously) only the scatter traces will be resampled.
+
+## Important considerations & tips
+
+* When running the code on a server, you should forward the port of the `FigureResampler.show_dash()` method to your local machine.<br>
+  **Note** that you can add dynamic aggregation to plotly figures with the `FigureWidgetResampler` wrapper without needing to forward a port!
+* The `FigureWidgetResampler` *uses the IPython main thread* for its data aggregation functionality, so when this main thread is occupied, no resampling logic can be executed. For example; if you perform long computations within your notebook, the kernel will be occupied during these computations, and will only execute the resampling operations that take place during these computations after finishing that computation.
+* In general, when using downsampling one should be aware of (possible) [aliasing](https://en.wikipedia.org/wiki/Aliasing) effects.
+  The <b style="color:orange">[R]</b> in the legend indicates when the corresponding trace is being resampled (and thus possibly distorted) or not. Additionally, the `~<range>` suffix represent the mean aggregation bin size in terms of the sequence index.
+* The plotly **autoscale** event (triggered by the autoscale button or a double-click within the graph), **does not reset the axes but autoscales the current graph-view** of plotly-resampler figures. This design choice was made as it seemed more intuitive for the developers to support this behavior with double-click than the default axes-reset behavior. The graph axes can ofcourse be resetted by using the `reset_axis` button.  If you want to give feedback and discuss this further with the developers, see issue [#49](https://github.com/predict-idlab/plotly-resampler/issues/49).
+
+## Cite
+
+Paper (preprint): https://arxiv.org/abs/2206.08703
+
+```bibtex
+@inproceedings{van2022plotly,
+  title={Plotly-resampler: Effective visual analytics for large time series},
+  author={Van Der Donckt, Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
+  booktitle={2022 IEEE Visualization and Visual Analytics (VIS)},
+  pages={21--25},
+  year={2022},
+  organization={IEEE}
 }
-from build import *
-build(setup_kwargs)
+```
+
+## Future work 🔨
+
+- [x] Support `.add_traces()` (currently only `.add_trace` is supported)
+- [ ] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
+- [x] Integrate with [tsdownsample](https://github.com/predict-idlab/tsdownsample) :racehorse:
+
+<br>
+
+---
+
+<p align="center">
+👤 <i>Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost</i>
+</p>
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,136 +1,134 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['plotly_resampler', 'plotly_resampler.aggregation',
-'plotly_resampler.aggregation.algorithms', 'plotly_resampler.figure_resampler']
-package_data = \ {'': ['*']} install_requires = \ ['Flask-Cors>=3.0.10,<4.0.0',
-'Werkzeug<=2.1.2', 'dash>=2.2.0,<3.0.0', 'jupyter-dash>=0.4.2',
-'orjson>=3.8.0,<4.0.0', 'pandas>=1.3.5,<2.0.0', 'plotly>=5.5.0,<6.0.0', 'trace-
-updater>=0.0.8'] extras_require = \ {':python_version < "3.11"':
-['numpy>=1.14'], ':python_version >= "3.11"': ['numpy>=1.24']} setup_kwargs =
-{ 'name': 'plotly-resampler', 'version': '0.8.4rc1', 'description':
-'Visualizing large time series with plotly', 'long_description': '
-                       \n \n_[Plotly-Resampler_logo]\n\n
-\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-
-resampler.svg)](https://pypi.org/project/plotly-resampler/)\n[![support-
-version](https://img.shields.io/pypi/pyversions/plotly-resampler)](https://
-img.shields.io/pypi/pyversions/plotly-resampler)\n[![codecov](https://
-img.shields.io/codecov/c/github/predict-idlab/plotly-resampler?logo=codecov)]
-(https://codecov.io/gh/predict-idlab/plotly-resampler)\n[![Code quality](https:
-//img.shields.io/lgtm/grade/python/github/predict-idlab/plotly-
-resampler?label=code%20quality&logo=lgtm)](https://lgtm.com/projects/g/predict-
-idlab/plotly-resampler/context:python)\n[![Downloads](https://pepy.tech/badge/
-plotly-resampler)](https://pepy.tech/project/plotly-resampler)\n[![PRs Welcome]
-(https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
-makeapullrequest.com)\n[![Documentation](https://github.com/predict-idlab/
+Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc0 Summary:
+Visualizing large time series with plotly Home-page: https://github.com/
+predict-idlab/plotly-resampler License: MIT Keywords: time-
+series,visualization,resampling,plotly,plotly-dash Author: Jonas Van Der Donckt
+Requires-Python: >=3.7.1,<4.0.0 Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
+MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Provides-Extra: inline-persistent Requires-Dist:
+Flask-Cors (>=3.0.10,<4.0.0) ; extra == "inline-persistent" Requires-Dist: dash
+(>=2.2.0,<3.0.0) Requires-Dist: jupyter-dash (>=0.4.2) Requires-Dist: kaleido
+(==0.2.1) ; extra == "inline-persistent" Requires-Dist: numpy (>=1.14) ;
+python_version < "3.11" Requires-Dist: numpy (>=1.24) ; python_version >=
+"3.11" Requires-Dist: orjson (>=3.8.0,<4.0.0) Requires-Dist: pandas (>=1)
+Requires-Dist: plotly (>=5.5.0,<6.0.0) Requires-Dist: trace-updater (>=0.0.8)
+Requires-Dist: tsdownsample (==0.1.2) Project-URL: Documentation, https://
+predict-idlab.github.io/plotly-resampler Project-URL: Repository, https://
+github.com/predict-idlab/plotly-resampler Description-Content-Type: text/
+markdown
+                            [Plotly-Resampler_logo]
+[![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)]
+(https://pypi.org/project/plotly-resampler/) [![support-version](https://
+img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/
+pyversions/plotly-resampler) [![codecov](https://img.shields.io/codecov/c/
+github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/
+predict-idlab/plotly-resampler) [![Downloads](https://pepy.tech/badge/plotly-
+resampler)](https://pepy.tech/project/plotly-resampler) [![PRs Welcome](https:/
+/img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
+makeapullrequest.com) [![Documentation](https://github.com/predict-idlab/
 plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://
-github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml)\n
-[![Testing](https://github.com/predict-idlab/plotly-resampler/actions/
-workflows/test.yml/badge.svg)](https://github.com/predict-idlab/plotly-
-resampler/actions/workflows/test.yml)\n\n\n\n\n> `plotly_resampler`: visualize
-large sequential data by **adding resampling functionality to Plotly
-figures**\n\n[Plotly](https://github.com/plotly/plotly.py) is an awesome
-interactive visualization library, however it can get pretty slow when a lot of
-data points are visualized (100 000+ datapoints). This library solves this by
-downsampling (aggregating) the data respective to the view and then plotting
-the aggregated points. When you interact with the plot (panning, zooming, ...),
-callbacks are used to aggregate data and update the figure.\n\n![basic example
-gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/
-docs/sphinx/_static/basic_example.gif)\n\n\nIn [this Plotly-Resampler demo]
-(https://github.com/predict-idlab/plotly-resampler/blob/main/examples/
-basic_example.ipynb) over `110,000,000` data points are
-visualized!\n\n\n\n\n\n\n\n\n\n\n### Installation\n\n| [**pip**](https://
-pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |\n| ---
-| ----|\n\n\n
-\n\n## Usage\n\n**Add dynamic aggregation** to your plotly Figure _(unfold your
-fitting use case)_\n* ð¤ Automatically _(minimal code overhead)_:\n Use the
-register_plotly_resampler function\n
-\n\n 1. Import and call the `register_plotly_resampler` method\n 2. Just use
-your regular graph construction code\n\n * **code example**:\n ```python\n
-import plotly.graph_objects as go; import numpy as np\n from plotly_resampler
-import register_plotly_resampler\n\n # Call the register function once and all
-Figures/FigureWidgets will be wrapped\n # according to the
-register_plotly_resampler its `mode` argument\n register_plotly_resampler
-(mode=\'auto\')\n\n x = np.arange(1_000_000)\n noisy_sin = (3 + np.sin(x / 200)
-+ np.random.randn(len(x)) / 10) * x / 1_000\n\n\n # auto mode: when working in
-an IPython environment, this will automatically be a \n # FigureWidgetResampler
-else, this will be an FigureResampler\n f = go.Figure()\n f.add_trace({"y":
-noisy_sin + 2, "name": "yp2"})\n f\n ```\n\n > **Note**: This wraps **all**
-plotly graph object figures with a \n > `FigureResampler` |
-`FigureWidgetResampler`. This can thus also be \n > used for the
-`plotly.express` interface. ð\n\n \n\n* ð· Manually _(higher data
-aggregation configurability, more speedup possibilities)_:\n \n Within a
-jupyter environment without creating a web application\n
-\n\n 1. wrap the plotly Figure with `FigureWidgetResampler`\n 2. output the
-`FigureWidgetResampler` instance in a cell\n\n * **code example**:\n
-```python\n import plotly.graph_objects as go; import numpy as np\n from
-plotly_resampler import FigureResampler, FigureWidgetResampler\n\n x =
-np.arange(1_000_000)\n noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len
-(x)) / 10) * x / 1_000\n\n # OPTION 1 - FigureWidgetResampler: dynamic
-aggregation via `FigureWidget.layout.on_change`\n fig = FigureWidgetResampler
-(go.Figure())\n fig.add_trace(go.Scattergl(name=\'noisy sine\',
-showlegend=True), hf_x=x, hf_y=noisy_sin)\n\n fig\n ```\n \n \n Using a web-
-application with dash callbacks\n
-\n\n 1. wrap the plotly Figure with `FigureResampler`\n 2. call `.show_dash()`
-on the `Figure`\n\n * **code example**:\n ```python\n import
-plotly.graph_objects as go; import numpy as np\n from plotly_resampler import
-FigureResampler, FigureWidgetResampler\n\n x = np.arange(1_000_000)\n noisy_sin
-= (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000\n\n # OPTION
-2 - FigureResampler: dynamic aggregation via a Dash web-app\n fig =
-FigureResampler(go.Figure())\n fig.add_trace(go.Scattergl(name=\'noisy sine\',
-showlegend=True), hf_x=x, hf_y=noisy_sin)\n\n fig.show_dash(mode=\'inline\')\n
-```\n\n \n
-\n\n > **Tip** ð¡:\n > For significant faster initial loading of the Figure,
-we advise to wrap the \n > constructor of the plotly Figure and add the trace
-data as `hf_x` and `hf_y`\n\n
-\n\n> **Note**:\n> Any plotly Figure can be wrapped with `FigureResampler` and
-`FigureWidgetResampler`! ð\n> But, (obviously) only the scatter traces will
-be resampled.\n\n\n\n\n
-\nð Features\n\n * **Convenient** to use:\n * just add either\n *
+github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml) [!
+[Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/
+test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/
+workflows/test.yml)  > `plotly_resampler`: visualize large sequential data by
+**adding resampling functionality to Plotly figures** [Plotly](https://
+github.com/plotly/plotly.py) is an awesome interactive visualization library,
+however it can get pretty slow when a lot of data points are visualized (100
+000+ datapoints). This library solves this by downsampling (aggregating) the
+data respective to the view and then plotting the aggregated points. When you
+interact with the plot (panning, zooming, ...), callbacks are used to aggregate
+data and update the figure. ![basic example gif](https://
+raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/
+_static/basic_example.gif) In [this Plotly-Resampler demo](https://github.com/
+predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
+`110,000,000` data points are visualized!       ### Installation | [**pip**]
+(https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
+| ---| ----|  ### Features :tada: * **Convenient** to use: * just add either *
 `register_plotly_resampler` function to your notebook with the best suited
-`mode` argument.\n * `FigureResampler` decorator around a plotly Figure and
-call `.show_dash()`\n * `FigureWidgetResampler` decorator around a plotly
-Figure and output the instance in a cell\n * allows all other plotly figure
-construction flexibility to be used!\n * **Environment-independent**\n * can be
-used in Jupyter, vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell,
-and even as application (on a server)\n * Interface for **various aggregation
-algorithms**:\n * ability to develop or select your preferred sequence
-aggregation method\n\n\n### Important considerations & tips\n\n* When running
-the code on a server, you should forward the port of the
-`FigureResampler.show_dash()` method to your local machine.
-\n **Note** that you can add dynamic aggregation to plotly figures with the
-`FigureWidgetResampler` wrapper without needing to forward a port!\n* The
+`mode` argument. * `FigureResampler` decorator around a plotly Figure and call
+`.show_dash()` * `FigureWidgetResampler` decorator around a plotly Figure and
+output the instance in a cell * allows all other plotly figure construction
+flexibility to be used! * **Environment-independent** * can be used in Jupyter,
+vscode-notebooks, Pycharm-notebooks, Google Colab, DataSpell, and even as
+application (on a server) * Interface for **various aggregation algorithms**: *
+ability to develop or select your preferred sequence aggregation method ##
+Usage **Add dynamic aggregation** to your plotly Figure _(unfold your fitting
+use case)_ * ð¤ Automatically _(minimal code overhead)_: Use the
+register_plotly_resampler function
+1. Import and call the `register_plotly_resampler` method 2. Just use your
+regular graph construction code * **code example**: ```python import
+plotly.graph_objects as go; import numpy as np from plotly_resampler import
+register_plotly_resampler # Call the register function once and all Figures/
+FigureWidgets will be wrapped # according to the register_plotly_resampler its
+`mode` argument register_plotly_resampler(mode='auto') x = np.arange(1_000_000)
+noisy_sin = (3 + np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000 #
+auto mode: when working in an IPython environment, this will automatically be a
+# FigureWidgetResampler else, this will be an FigureResampler f = go.Figure()
+f.add_trace({"y": noisy_sin + 2, "name": "yp2"}) f ``` > **Note**: This wraps
+**all** plotly graph object figures with a > `FigureResampler` |
+`FigureWidgetResampler`. This can thus also be > used for the `plotly.express`
+interface. ð  * ð· Manually _(higher data aggregation configurability,
+more speedup possibilities)_: * Within a jupyter environment without creating a
+web application 1. wrap the plotly Figure with `FigureWidgetResampler` 2.
+output the `FigureWidgetResampler` instance in a cell ```python import
+plotly.graph_objects as go; import numpy as np from plotly_resampler import
+FigureResampler, FigureWidgetResampler x = np.arange(1_000_000) noisy_sin = (3
++ np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000 # OPTION 1 -
+FigureWidgetResampler: dynamic aggregation via `FigureWidget.layout.on_change`
+fig = FigureWidgetResampler(go.Figure()) fig.add_trace(go.Scattergl(name='noisy
+sine', showlegend=True), hf_x=x, hf_y=noisy_sin) fig ``` * Using a web-
+application with dash callbacks 1. wrap the plotly Figure with
+`FigureResampler` 2. call `.show_dash()` on the `Figure` ```python import
+plotly.graph_objects as go; import numpy as np from plotly_resampler import
+FigureResampler, FigureWidgetResampler x = np.arange(1_000_000) noisy_sin = (3
++ np.sin(x / 200) + np.random.randn(len(x)) / 10) * x / 1_000 # OPTION 2 -
+FigureResampler: dynamic aggregation via a Dash web-app fig = FigureResampler
+(go.Figure()) fig.add_trace(go.Scattergl(name='noisy sine', showlegend=True),
+hf_x=x, hf_y=noisy_sin) fig.show_dash(mode='inline') ``` > **Tip** ð¡: > For
+significant faster initial loading of the Figure, we advise to wrap the >
+constructor of the plotly Figure and add the trace data as `hf_x` and `hf_y`
+> **Note**: > Any plotly Figure can be wrapped with `FigureResampler` and
+`FigureWidgetResampler`! ð > But, (obviously) only the scatter traces will
+be resampled. ## Important considerations & tips * When running the code on a
+server, you should forward the port of the `FigureResampler.show_dash()` method
+to your local machine.
+**Note** that you can add dynamic aggregation to plotly figures with the
+`FigureWidgetResampler` wrapper without needing to forward a port! * The
 `FigureWidgetResampler` *uses the IPython main thread* for its data aggregation
 functionality, so when this main thread is occupied, no resampling logic can be
 executed. For example; if you perform long computations within your notebook,
 the kernel will be occupied during these computations, and will only execute
 the resampling operations that take place during these computations after
-finishing that computation.\n* In general, when using downsampling one should
-be aware of (possible) [aliasing](https://en.wikipedia.org/wiki/Aliasing)
-effects.\n The [R] in the legend indicates when the corresponding trace is
-being resampled (and thus possibly distorted) or not. Additionally, the `~`
-suffix represent the mean aggregation bin size in terms of the sequence
-index.\n* The plotly **autoscale** event (triggered by the autoscale button or
-a double-click within the graph), **does not reset the axes but autoscales the
-current graph-view** of plotly-resampler figures. This design choice was made
-as it seemed more intuitive for the developers to support this behavior with
-double-click than the default axes-reset behavior. The graph axes can ofcourse
-be resetted by using the `reset_axis` button. If you want to give feedback and
-discuss this further with the developers, see issue [#49](https://github.com/
-predict-idlab/plotly-resampler/issues/49).\n\n## Cite\n\nPaper (preprint):
-https://arxiv.org/abs/2206.08703\n\n```latex\n@misc{https://doi.org/10.48550/
-arxiv.2206.08703,\n author = {Van Der Donckt, Jonas and Van Der Donckt, Jeroen
-and Deprost, Emiel and Van Hoecke, Sofie},\n title = {Plotly-Resampler:
-Effective Visual Analytics for Large Time Series},\n year = {2022},\n doi =
-{10.48550/ARXIV.2206.08703},\n url = {https://arxiv.org/abs/2206.08703},\n
-publisher = {arXiv},\n}\n```\n\n## Future work ð¨\n\n- [x] Support
-`.add_traces()` (currently only `.add_trace` is supported)\n- [ ] Support
-`hf_color` and `hf_markersize`, see [#50](https://github.com/predict-idlab/
-plotly-resampler/pull/50)\n- [ ] Create C bindings for our EfficientLTTB
-algorithm.\n\n
-\n\n---\n\n
-      \nð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost\n
-\n', 'author': 'Jonas Van Der Donckt', 'author_email': 'None', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/predict-idlab/
-plotly-resampler', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'python_requires': '>=3.7.1,<4.0.0', } from build import * build(setup_kwargs)
-setup(**setup_kwargs)
+finishing that computation. * In general, when using downsampling one should be
+aware of (possible) [aliasing](https://en.wikipedia.org/wiki/Aliasing) effects.
+The [R] in the legend indicates when the corresponding trace is being resampled
+(and thus possibly distorted) or not. Additionally, the `~` suffix represent
+the mean aggregation bin size in terms of the sequence index. * The plotly
+**autoscale** event (triggered by the autoscale button or a double-click within
+the graph), **does not reset the axes but autoscales the current graph-view**
+of plotly-resampler figures. This design choice was made as it seemed more
+intuitive for the developers to support this behavior with double-click than
+the default axes-reset behavior. The graph axes can ofcourse be resetted by
+using the `reset_axis` button. If you want to give feedback and discuss this
+further with the developers, see issue [#49](https://github.com/predict-idlab/
+plotly-resampler/issues/49). ## Cite Paper (preprint): https://arxiv.org/abs/
+2206.08703 ```bibtex @inproceedings{van2022plotly, title={Plotly-resampler:
+Effective visual analytics for large time series}, author={Van Der Donckt,
+Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
+booktitle={2022 IEEE Visualization and Visual Analytics (VIS)}, pages={21--25},
+year={2022}, organization={IEEE} } ``` ## Future work ð¨ - [x] Support
+`.add_traces()` (currently only `.add_trace` is supported) - [ ] Support
+`hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/
+plotly-resampler/pull/148) - [x] Integrate with [tsdownsample](https://
+github.com/predict-idlab/tsdownsample) :racehorse:
+---
+        ð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
```

