# Comparing `tmp/transformer_lens-1.2.1.tar.gz` & `tmp/transformer_lens-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_lens-1.2.1.tar", max compression
+gzip compressed data, was "transformer_lens-1.2.2.tar", max compression
```

## Comparing `transformer_lens-1.2.1.tar` & `transformer_lens-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-03-19 00:40:16.611859 transformer_lens-1.2.1/LICENSE
--rw-r--r--   0        0        0     7501 2023-03-19 00:40:16.631859 transformer_lens-1.2.1/README.md
--rw-r--r--   0        0        0     1872 2023-03-19 00:42:09.448238 transformer_lens-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    35224 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/ActivationCache.py
--rw-r--r--   0        0        0     7795 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/FactoredMatrix.py
--rw-r--r--   0        0        0    76212 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/HookedTransformer.py
--rw-r--r--   0        0        0    11978 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/HookedTransformerConfig.py
--rw-r--r--   0        0        0      838 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/__init__.py
--rw-r--r--   0        0        0    33525 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/components.py
--rw-r--r--   0        0        0     5955 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/evals.py
--rw-r--r--   0        0        0    14149 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/hook_points.py
--rw-r--r--   0        0        0    41346 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/loading_from_pretrained.py
--rw-r--r--   0        0        0     2092 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/make_docs.py
--rw-r--r--   0        0        0    11177 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/model_properties_table.md
--rw-r--r--   0        0        0     2771 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/past_key_value_caching.py
--rw-r--r--   0        0        0    17098 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/patching.py
--rw-r--r--   0        0        0     5425 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/tests/test_activation_cache.py
--rw-r--r--   0        0        0     5511 2023-03-19 00:40:16.647859 transformer_lens-1.2.1/transformer_lens/train.py
--rw-r--r--   0        0        0    27319 2023-03-19 00:40:16.651859 transformer_lens-1.2.1/transformer_lens/utils.py
--rw-r--r--   0        0        0     9449 1970-01-01 00:00:00.000000 transformer_lens-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-24 07:40:25.148681 transformer_lens-1.2.2/LICENSE
+-rw-r--r--   0        0        0     8084 2023-04-24 07:40:25.148681 transformer_lens-1.2.2/README.md
+-rw-r--r--   0        0        0     1902 2023-04-24 07:41:40.743673 transformer_lens-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    36290 2023-04-24 07:40:25.240679 transformer_lens-1.2.2/transformer_lens/ActivationCache.py
+-rw-r--r--   0        0        0     7776 2023-04-24 07:40:25.240679 transformer_lens-1.2.2/transformer_lens/FactoredMatrix.py
+-rw-r--r--   0        0        0    81131 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/HookedTransformer.py
+-rw-r--r--   0        0        0    12588 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/HookedTransformerConfig.py
+-rw-r--r--   0        0        0      867 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/__init__.py
+-rw-r--r--   0        0        0    36777 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/components.py
+-rw-r--r--   0        0        0    12267 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/evals.py
+-rw-r--r--   0        0        0     8525 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/head_detector.py
+-rw-r--r--   0        0        0    19943 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/hook_points.py
+-rw-r--r--   0        0        0    50594 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/loading_from_pretrained.py
+-rw-r--r--   0        0        0     2092 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/make_docs.py
+-rw-r--r--   0        0        0    11177 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/model_properties_table.md
+-rw-r--r--   0        0        0     2865 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/past_key_value_caching.py
+-rw-r--r--   0        0        0    24180 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/patching.py
+-rw-r--r--   0        0        0     5511 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/train.py
+-rw-r--r--   0        0        0        0 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/utilities/__init__.py
+-rw-r--r--   0        0        0     1257 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/utilities/devices.py
+-rw-r--r--   0        0        0    28437 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/utils.py
+-rw-r--r--   0        0        0     9911 1970-01-01 00:00:00.000000 transformer_lens-1.2.2/PKG-INFO
```

### Comparing `transformer_lens-1.2.1/LICENSE` & `transformer_lens-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.2.1/README.md` & `transformer_lens-1.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,39 +4,42 @@
 
 (Formerly known as EasyTransformer)
 
 ## [Read the Docs Here](https://neelnanda-io.github.io/TransformerLens/)
 
 ## [Main Tutorial Here](https://neelnanda.io/transformer-lens-demo)
 
+See also this better and more in-depth, but still [work-in-progress tutorial from Callum McDougall](https://transformerlens-intro.streamlit.app/)
+
 ## A Library for Mechanistic Interpretability of Generative Language Models
 
-This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this! 
+This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this!
 
-TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make *my* experience of doing research easier and more fun, hopefully this transfers to you!
+TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make _my_ experience of doing research easier and more fun, hopefully this transfers to you!
 
-I used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to *use* or *train* models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook! 
+I used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook!
 
 The core features were heavily inspired by the interface to [Anthropic's excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson Elhage and Chris Olah for building Garcon and showing me the value of good infrastructure for enabling exploratory research!
 
 ## Getting Started
 
 **Start with the [main demo](https://neelnanda.io/transformer-lens-demo) to learn how the library works, and the basic features**.
 
-To see what using it for exploratory analysis in practice looks like, check out [my notebook analysing Indirect Objection Identification](https://neelnanda.io/exploratory-analysis-demo) or [my recording of myself doing research](https://www.youtube.com/watch?v=yo4QvDn-vsU)! 
+To see what using it for exploratory analysis in practice looks like, check out [my notebook analysing Indirect Objection Identification](https://neelnanda.io/exploratory-analysis-demo) or [my recording of myself doing research](https://www.youtube.com/watch?v=yo4QvDn-vsU)!
 
-Mechanistic interpretability is a very young and small field, and there are a *lot* of open problems - if you would like to help, please try working on one! **Check out my [list of concrete open problems](https://docs.google.com/document/d/1WONBzNqfKIxERejrrPlQMyKqg7jSFW92x5UMXNrMdPo/edit) to figure out where to start.**. It begins with advice on skilling up, and key resources to check out. 
+Mechanistic interpretability is a very young and small field, and there are a _lot_ of open problems - if you would like to help, please try working on one! **Check out my [list of concrete open problems](https://docs.google.com/document/d/1WONBzNqfKIxERejrrPlQMyKqg7jSFW92x5UMXNrMdPo/edit) to figure out where to start.**. It begins with advice on skilling up, and key resources to check out.
 
 If you're new to transformers, check out my [what is a transformer tutorial](https://neelnanda.io/transformer-tutorial) and [tutorial on coding GPT-2 from scratch](https://neelnanda.io/transformer-tutorial-2) (with [an accompanying template](https://neelnanda.io/transformer-template) to write one yourself!
 
 ## Gallery
 
 User contributed examples of the library being used in action:
-* [Induction Heads Phase Change Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb): A partial replication of [In-Context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) from Connor Kissane
-* [Decision Transformer Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of scripts for training decision transformers which uses transformer lens to view intermediate activations, perform attribution and ablations. A write up of the initial work can be found [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
+
+- [Induction Heads Phase Change Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb): A partial replication of [In-Context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) from Connor Kissane
+- [Decision Transformer Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of scripts for training decision transformers which uses transformer lens to view intermediate activations, perform attribution and ablations. A write up of the initial work can be found [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
 
 ## Advice for Reading the Code
 
 One significant design decision made was to have a single transformer implementation that could support a range of subtly different GPT-style models. This has the upside of interpretability code just working for arbitrary models when you change the model name in `HookedTransformer.from_pretrained`! But it has the significant downside that the code implementing the model (in `HookedTransformer.py` and `components.py`) can be difficult to read. I recommend starting with my [Clean Transformer Demo](https://neelnanda.io/transformer-solution), which is a clean, minimal implementation of GPT-2 with the same internal architecture and activation names as HookedTransformer, but is significantly clearer and better documented.
 
 ## Installation
 
@@ -65,26 +68,32 @@
 
 Then the library can be imported as `import transformer_lens`.
 
 ### Testing
 
 If adding a feature, please add unit tests for it to the tests folder, and check that it hasn't broken anything major using the existing tests (install pytest and run it in the root TransformerLens/ directory).
 
-To run tests, you can use the following command:
+#### Running the tests
 
-```
-poetry run pytest -v tests
-```
+- All tests via `make test`
+- Unit tests only via `make unit-test`
+- Acceptance tests only via `make acceptance-test`
+
+### Demos
+
+If adding a feature, please add it to the demo notebook in the `demos` folder, and check that it works in the demo format. This can be tested by replacing `pip install git+https://github.com/JayBaileyCS/TransformerLens.git` with `pip install git+https://github.com/<YOUR_USERNAME_HERE>/TransformerLens.git` in the demo notebook, and running it in a fresh environment.
 
 ## Citation
 
 Please cite this library as:
+
 ```
 @misc{nandatransformerlens2022,
     title  = {TransformerLens},
     author = {Nanda, Neel},
     url    = {https://github.com/neelnanda-io/TransformerLens},
     year   = {2022}
 }
 ```
+
 (This is my best guess for how citing software works, feel free to send a correction!)
 Also, if you're actually using this for your research, I'd love to chat! Reach out at neelnanda27@gmail.com
```

### Comparing `transformer_lens-1.2.1/pyproject.toml` & `transformer_lens-1.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [tool.poetry]
 name = "transformer-lens"
-version = "v1.2.1" # This is automatically set by the CD pipeline on release
+version = "v1.2.2" # This is automatically set by the CD pipeline on release
 description = "An implementation of transformers tailored for mechanistic interpretability."
 authors = ["Neel Nanda <77788841+neelnanda-io@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "transformer_lens"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-einops = "^0.6.0"
-numpy = [{ version = "^1.21", python = "<3.10" },
-         { version = "^1.23", python = ">=3.10" }]
-torch = "^1.10"
-datasets = "^2.7.1"
-transformers = "^4.25.1"
-tqdm = "^4.64.1"
-pandas = "^1.1.5"
-wandb = "^0.13.5"
-fancy-einsum = "^0.0.3"
-rich = "^12.6.0"
-jaxtyping = "^0.2.11"
+python = ">=3.7,<4.0"
+einops = ">=0.6.0"
+numpy = [{ version = ">=1.21", python = "<3.10" },
+         { version = ">=1.23", python = ">=3.10" }]
+torch = ">=1.10"
+datasets = ">=2.7.1"
+transformers = ">=4.25.1"
+tqdm = ">=4.64.1"
+pandas = ">=1.1.5"
+wandb = ">=0.13.5"
+fancy-einsum = ">=0.0.3"
+rich = ">=12.6.0"
+jaxtyping = ">=0.2.11"
 sphinx = {version = "5.2.3", optional = true, python = ">=3.8,<3.10"}
-sphinxcontrib-napoleon = {version = "^0.7", optional = true, python = ">=3.8,<3.10"}
-sphinx-autobuild = {version = "^2021.3.14", optional = true, python = ">=3.8,<3.10"}
-furo = {version = "^2022.12.7", optional = true, python = ">=3.8,<3.10"}
-myst-parser = {version = "^0.18.1", optional = true, python = ">=3.8,<3.10"}
-tabulate= {version = "^0.9.0", optional = true, python = ">=3.8,<3.10"}
+sphinxcontrib-napoleon = {version = ">=0.7", optional = true, python = ">=3.8,<3.10"}
+sphinx-autobuild = {version = ">=2021.3.14", optional = true, python = ">=3.8,<3.10"}
+furo = {version = ">=2022.12.7", optional = true, python = ">=3.8,<3.10"}
+myst-parser = {version = ">=0.18.1", optional = true, python = ">=3.8,<3.10"}
+tabulate= {version = ">=0.9.0", optional = true, python = ">=3.8,<3.10"}
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-mypy = "^0.991"
-jupyter = "^1.0.0"
-circuitsvis = "^1.38.1"
-plotly = "^5.12.0"
+pytest = ">=7.2.0"
+pytest-cov = ">=4.0.0"
+mypy = ">=0.991"
+jupyter = ">=1.0.0"
+circuitsvis = ">=1.38.1"
+plotly = ">=5.12.0"
 
 [tool.poetry.group.jupyter.dependencies]
-jupyterlab = "^3.5.0"
+jupyterlab = ">=3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-autobuild", "sphinxcontrib-napoleon", "furo", "myst_parser","tabulate"]
```

### Comparing `transformer_lens-1.2.1/transformer_lens/ActivationCache.py` & `transformer_lens-1.2.2/transformer_lens/ActivationCache.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,24 +136,26 @@
             new_cache_dict, self.model, has_batch_dim=still_has_batch_dim
         )
 
     def accumulated_resid(
         self,
         layer: Optional[int] = None,
         incl_mid: bool = False,
+        apply_ln: bool = False,
         pos_slice: Union[Slice, SliceInput] = None,
         mlp_input: bool = False,
         return_labels: bool = False,
     ) -> Float[torch.Tensor, "layers_covered *batch_and_pos_dims d_model"]:
         """Returns the accumulated residual stream up to a given layer, ie a stack of previous residual streams up to that layer's input. This can be thought of as a series of partial values of the residual stream, where the model gradually accumulates what it wants.
 
         Args:
             layer (int, *optional*): The layer to take components up to - by default includes resid_pre for that layer and excludes resid_mid and resid_post for that layer. layer==n_layers, -1 or None means to return all residual streams, including the final one (ie immediately pre logits). The indices are taken such that this gives the accumulated streams up to the input to layer l
             incl_mid (bool, optional): Whether to return resid_mid for all previous layers. Defaults to False.
             mlp_input (bool, optional): Whether to include resid_mid for the current layer - essentially giving MLP input rather than Attn input. Defaults to False.
+            apply_ln (bool, optional): Whether to apply LayerNorm to the stack. Defaults to False.
             pos_slice (Slice): A slice object to apply to the pos dimension. Defaults to None, do nothing.
             return_labels (bool, optional): Whether to return a list of labels for the residual stream components. Useful for labelling graphs. Defaults to True.
 
         Returns:
             Components: A [num_components, batch_size, pos, d_model] tensor of the accumulated residual streams.
             (labels): An optional list of labels for the components.
         """
@@ -173,14 +175,18 @@
             components.append(self[("resid_pre", l)])
             labels.append(f"{l}_pre")
             if (incl_mid and l < layer) or (mlp_input and l == layer):
                 components.append(self[("resid_mid", l)])
                 labels.append(f"{l}_mid")
         components = [pos_slice.apply(c, dim=-2) for c in components]
         components = torch.stack(components, dim=0)
+        if apply_ln:
+            components = self.apply_ln_to_stack(
+                components, layer, pos_slice=pos_slice, mlp_input=mlp_input
+            )
         if return_labels:
             return components, labels
         else:
             return components
 
     def logit_attrs(
             self,
@@ -242,14 +248,15 @@
         return logit_attrs
         
     def decompose_resid(
         self,
         layer: Optional[int] = None,
         mlp_input: bool = False,
         mode: Literal["all", "mlp", "attn"] = "all",
+        apply_ln: bool = False,
         pos_slice: Union[Slice, SliceInput] = None,
         incl_embeds: bool = True,
         return_labels: bool = False,
     ) -> Float[torch.Tensor, "layers_covered *batch_and_pos_dims d_model"]:
         """Decomposes the residual stream input to layer L into a stack of the output of previous layers. The sum of these is the input to layer L (plus embedding and pos embedding). This is useful for attributing model behaviour to different components of the residual stream
 
         Args:
@@ -257,14 +264,15 @@
                 resid_pre for that layer and excludes resid_mid and resid_post for that layer. layer==n_layers means to return all layer outputs incl in the final layer, layer==0 means just embed and pos_embed. The indices are taken such that this gives the accumulated streams up to the input to layer l
             incl_mid (bool, optional): Whether to return resid_mid for all previous
                 layers. Defaults to False.
             mlp_input (bool, optional): Whether to include attn_out for the current
                 layer - essentially decomposing the residual stream that's input to the MLP input rather than the Attn input. Defaults to False.
             mode (str): Values are "all", "mlp" or "attn". "all" returns all
                 components, "mlp" returns only the MLP components, and "attn" returns only the attention components. Defaults to "all".
+            apply_ln (bool, optional): Whether to apply LayerNorm to the stack. Defaults to False.
             pos_slice (Slice): A slice object to apply to the pos dimension.
                 Defaults to None, do nothing.
             incl_embeds (bool): Whether to include embed & pos_embed
             return_labels (bool, optional): Whether to return a list of labels for
                 the residual stream components. Useful for labelling graphs. Defaults to True.
 
         Returns:
@@ -298,14 +306,18 @@
                 components.append(self[("mlp_out", l)])
                 labels.append(f"{l}_mlp_out")
         if mlp_input and incl_attn:
             components.append(self[("attn_out", layer)])
             labels.append(f"{layer}_attn_out")
         components = [pos_slice.apply(c, dim=-2) for c in components]
         components = torch.stack(components, dim=0)
+        if apply_ln:
+            components = self.apply_ln_to_stack(
+                components, layer, pos_slice=pos_slice, mlp_input=mlp_input
+            )
         if return_labels:
             return components, labels
         else:
             return components
 
     def compute_head_results(
         self,
@@ -326,24 +338,24 @@
 
     def stack_head_results(
         self,
         layer: int = -1,
         return_labels: bool = False,
         incl_remainder: bool = False,
         pos_slice: Union[Slice, SliceInput] = None,
+        apply_ln: bool = False,
     ) -> Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"]:
         """Returns a stack of all head results (ie residual stream contribution) up to layer L. A good way to decompose the outputs of attention layers into attribution by specific heads. Note that the num_components axis has length layer x n_heads ((layer head_index) in einops notation)
 
-        Assumes that the model has been run with use_attn_results=True
-
         Args:
             layer (int): Layer index - heads at all layers strictly before this are included. layer must be in [1, n_layers-1], or any of (n_layers, -1, None), which all mean the final layer
             return_labels (bool, optional): Whether to also return a list of labels of the form "L0H0" for the heads. Defaults to False.
             incl_remainder (bool, optional): Whether to return a final term which is "the rest of the residual stream". Defaults to False.
             pos_slice (Slice): A slice object to apply to the pos dimension. Defaults to None, do nothing.
+            apply_ln (bool, optional): Whether to apply LayerNorm to the stack. Defaults to False.
         """
         if not isinstance(pos_slice, Slice):
             pos_slice = Slice(pos_slice)
         if layer is None or layer == -1:
             # Default to the residual stream immediately pre unembed
             layer = self.model.cfg.n_layers
 
@@ -379,14 +391,19 @@
             # This uses the shape of hook_embed, which is pretty janky since it assumes embed is in the cache. But it's hard to explicitly code the shape, since it depends on the pos slice, whether we have a batch dim, etc. And it's pretty messy!
             components = torch.zeros(
                 0,
                 *pos_slice.apply(self["hook_embed"], dim=-2).shape,
                 device=self.model.cfg.device,
             )
 
+        if apply_ln:
+            components = self.apply_ln_to_stack(
+                components, layer, pos_slice=pos_slice
+            )
+            
         if return_labels:
             return components, labels
         else:
             return components
     
     def stack_activation(
         self,
@@ -449,25 +466,27 @@
     def stack_neuron_results(
         self,
         layer: int,
         pos_slice: Union[Slice, SliceInput] = None,
         neuron_slice: Union[Slice, SliceInput] = None,
         return_labels: bool = False,
         incl_remainder: bool = False,
+        apply_ln: bool = False,
     ) -> Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"]:
         """Returns a stack of all neuron results (ie residual stream contribution) up to layer L - ie the amount each individual neuron contributes to the residual stream. Also returns a list of labels of the form "L0N0" for the neurons. A good way to decompose the outputs of MLP layers into attribution by specific neurons.
 
         Note that doing this for all neurons is SUPER expensive on GPU memory and only works for small models or short inputs.
 
         Args:
             layer (int): Layer index - heads at all layers strictly before this are included. layer must be in [1, n_layers]
             pos_slice (Slice, optional): Slice of the positions. Defaults to None. See utils.Slice for details.
             neuron_slice (Slice, optional): Slice of the neurons. Defaults to None. See utils.Slice for details.
             return_labels (bool, optional): Whether to also return a list of labels of the form "L0H0" for the heads. Defaults to False.
             incl_remainder (bool, optional): Whether to return a final term which is "the rest of the residual stream". Defaults to False.
+            apply_ln (bool, optional): Whether to apply LayerNorm to the stack. Defaults to False.
         """
 
         if layer is None or layer == -1:
             # Default to the residual stream immediately pre unembed
             layer = self.model.cfg.n_layers
 
         components = []
@@ -505,14 +524,20 @@
         else:
             # Returning empty, give it the right shape to stack properly
             components = torch.zeros(
                 0,
                 *pos_slice.apply(self["hook_embed"], dim=-2).shape,
                 device=self.model.cfg.device,
             )
+
+        if apply_ln:
+            components = self.apply_ln_to_stack(
+                components, layer, pos_slice=pos_slice
+            )
+
         if return_labels:
             return components, labels
         else:
             return components
 
     def apply_ln_to_stack(
         self,
@@ -595,15 +620,15 @@
     ) -> Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"]:
         """Returns the full decomposition of the residual stream into embed, pos_embed, each head result, each neuron result, and the accumulated biases. We break down the residual stream that is input into some layer.
 
         Args:
             layer (int): The layer we're inputting into. layer is in [0, n_layers], if layer==n_layers (or None) we're inputting into the unembed (the entire stream), if layer==0 then it's just embed and pos_embed
             mlp_input (bool, optional): Are we inputting to the MLP in that layer or the attn? Must be False for final layer, since that's the unembed. Defaults to False.
             expand_neurons (bool, optional): Whether to expand the MLP outputs to give every neuron's result or just return the MLP layer outputs. Defaults to True.
-            apply_ln (bool, optional): Whether to apply LayerNorm to the stack. Defaults to True.
+            apply_ln (bool, optional): Whether to apply LayerNorm to the stack. Defaults to False.
             pos_slice (Slice, optional): Slice of the positions to take. Defaults to None. See utils.Slice for details.
             return_labels (bool): Whether to return the labels. Defaults to False.
         """
         if layer is None or layer == -1:
             # Default to the residual stream immediately pre unembed
             layer = self.model.cfg.n_layers
```

### Comparing `transformer_lens-1.2.1/transformer_lens/FactoredMatrix.py` & `transformer_lens-1.2.2/transformer_lens/FactoredMatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
+
+from functools import lru_cache
+from typing import Union, Tuple
+
 import torch
-from typing import Optional, Union, Tuple, List, Dict
 from jaxtyping import Float
-from functools import lru_cache
+
 import transformer_lens.utils as utils
 
 class FactoredMatrix:
     """
     Class to represent low rank factored matrices, where the matrix is represented as a product of two matrices. Has utilities for efficient calculation of eigenvalues, norm and SVD.
     """
 
@@ -51,15 +54,15 @@
     ) -> Union[FactoredMatrix, Float[torch.Tensor, "... rdim"]]:
         if isinstance(other, torch.Tensor):
             assert (
                 other.size(-1) == self.ldim
             ), f"Left matrix must match on inner dimension, shapes were self: {self.shape}, other:{other.shape}"
             if other.ndim < 2:
                 # It's a vector, so we collapse the factorisation and just return a vector
-                return ((other.unsqueeze(-2) @ self.A) @ self.B).squeeze(-1)
+                return ((other.unsqueeze(-2) @ self.A) @ self.B).squeeze(-2)
             elif self.ldim > self.mdim:
                 return FactoredMatrix(other @ self.A, self.B)
             else:
                 return FactoredMatrix(other, self.AB)
         elif isinstance(other, FactoredMatrix):
             return other.A @ (other.B @ self)
```

### Comparing `transformer_lens-1.2.1/transformer_lens/HookedTransformer.py` & `transformer_lens-1.2.2/transformer_lens/HookedTransformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from transformer_lens.past_key_value_caching import (
     HookedTransformerKeyValueCache,
 )
 
 from transformer_lens.components import *
 import transformer_lens.loading_from_pretrained as loading
 import transformer_lens.utils as utils
+from transformer_lens.utilities import devices
 
 SingleLoss = Float[torch.Tensor, ""] # Type alias for a single element tensor
 LossPerToken = Float[torch.Tensor, "batch pos-1"]
 Loss = Union[SingleLoss, LossPerToken]
 
 # Named tuple object for if we want to output both logits and loss
 class Output(NamedTuple):
@@ -61,35 +62,45 @@
 
         cfg Union[HookedTransformerConfig, Dict]: The config to use for the
             model.
         tokenizer (*optional): The tokenizer to use for the model. If not
             provided, it is inferred from cfg.tokenizer_name or initialized to None.
             If None, then the model cannot be passed strings, and d_vocab must be explicitly set.
         move_to_device (bool): Whether to move the model to the device specified in cfg.
-            device.
+            device. Must be true if `n_devices` in the config is greater than 1, since the model's layers
+            will be split across multiple devices.
         """
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig(**cfg)
         elif isinstance(cfg, str):
             raise ValueError(
                 "Please pass in a config dictionary or HookedTransformerConfig object. If you want to load a pretrained model, use HookedTransformer.from_pretrained() instead."
             )
         self.cfg = cfg
+
+        assert (
+            self.cfg.n_devices == 1 or move_to_device
+        ), "If n_devices > 1, must move_to_device"
+
         if tokenizer is not None:
             self.tokenizer = tokenizer
         elif self.cfg.tokenizer_name is not None:
             # If we have a tokenizer name, we can load it from HuggingFace
-            self.tokenizer = AutoTokenizer.from_pretrained(self.cfg.tokenizer_name)
-            if self.tokenizer.eos_token is None:
-                self.tokenizer.eos_token = "<|endoftext|>"
-            if self.tokenizer.pad_token is None:
-                self.tokenizer.pad_token = self.tokenizer.eos_token
-            if self.tokenizer.bos_token is None:
-                self.tokenizer.bos_token = self.tokenizer.eos_token
+            if 'llama' in self.cfg.tokenizer_name: 
+                # llama tokenizer requires special handling
+                print("Warning: LLaMA tokenizer not loaded. Please load manually.")
+            else: 
+                self.tokenizer = AutoTokenizer.from_pretrained(self.cfg.tokenizer_name)
+                if self.tokenizer.eos_token is None:
+                    self.tokenizer.eos_token = "<|endoftext|>"
+                if self.tokenizer.pad_token is None:
+                    self.tokenizer.pad_token = self.tokenizer.eos_token
+                if self.tokenizer.bos_token is None:
+                    self.tokenizer.bos_token = self.tokenizer.eos_token
         else:
             # If no tokenizer name is provided, we assume we're training on an algorithmic task and will pass in tokens directly. In this case, we don't need a tokenizer.
             self.tokenizer = None
 
         if self.cfg.d_vocab == -1:
             # If we have a tokenizer, vocab size can be inferred from it.
             assert (
@@ -112,15 +123,19 @@
         self.blocks = nn.ModuleList(
             [
                 TransformerBlock(self.cfg, block_index)
                 for block_index in range(self.cfg.n_layers)
             ]
         )
 
-        if self.cfg.normalization_type == "LN":
+        if self.cfg.normalization_type == "RMS": 
+            self.ln_final = RMSNorm(self.cfg)
+        elif self.cfg.normalization_type == "RMSPre":
+            self.ln_final = RMSNormPre(self.cfg)
+        elif self.cfg.normalization_type == "LN":
             if self.cfg.final_rms:
                 self.ln_final = RMSNorm(self.cfg)
             else:
                 self.ln_final = LayerNorm(self.cfg)
         elif self.cfg.normalization_type == "LNPre":
             # We've folded in LayerNorm weights, so just need the center + scale parts
             if self.cfg.final_rms:
@@ -136,30 +151,31 @@
             )
         self.unembed = Unembed(self.cfg)
 
         if self.cfg.init_weights:
             self.init_weights()
 
         if move_to_device:
-            # Move the model to the relevant device, suppress the logging message
-            self.to(self.cfg.device, print_details=False)
-        
+            # We load the devices in a pipeline manner - the first device gets the embed and pos_embed layers and the first n_layers // n_devices blocks,
+            # the second gets the next n_layers // n_devices blocks ... the last gets the last n_layers // n_devices blocks, the final
+            # normalization layer (if it exists) and the unembed layer
+            HookedTransformer.move_model_modules_to_device(self)
+
         # Helper variable to store a small (10K-20K) dataset of training data. Empty by default, can be loaded with load_sample_training_dataset
         self.dataset = None
 
         # Gives each module a parameter with its name (relative to this root module)
         # Needed for HookPoints to work
         self.setup()
 
-    def check_and_add_hook(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False) -> None:
+    def check_hooks_to_add(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False) -> None:
         if hook_point_name.endswith("attn.hook_result"):
             assert self.cfg.use_attn_result, f"Cannot add hook {hook_point_name} if use_attn_result_hook is False"
         if hook_point_name.endswith(("hook_q_input", "hook_k_input", "hook_v_input")):
             assert self.cfg.use_split_qkv_input, f"Cannot add hook {hook_point_name} if use_split_qkv_input is False"
-        hook_point.add_hook(hook, dir=dir, is_permanent=is_permanent)
 
     @overload
     def forward(
         self, 
         input, 
         return_type: Literal["logits"], 
         loss_per_token: bool = False,
@@ -234,16 +250,16 @@
             tokens = self.to_tokens(input, prepend_bos=prepend_bos)
         else:
             tokens = input
         if len(tokens.shape) == 1:
             # If tokens are a rank 1 tensor, add a dummy batch dimension to avoid things breaking.
             tokens = tokens[None]
         if tokens.device.type != self.cfg.device:
-            tokens = tokens.to(self.cfg.device)
-        assert isinstance(tokens, torch.Tensor)
+            tokens = tokens.to(devices.get_device_for_block_index(0, self.cfg))
+
         # If we're doing caching, then we reuse keys and values from previous runs, as that's the only
         # way that past activations will affect the final logits. The cache contains those so we don't
         # need to recompute them. This is useful for generating text. As we have absolute positional
         # encodings, to implement this we have a `pos_offset` variable, defaulting to zero, which says
         # to offset which positional encodings are used (cached keys and values were calculated with
         # their own positional encodings).
         if past_kv_cache is None:
@@ -295,19 +311,26 @@
         else:
             # If we explicitly want to stop at a layer, we only iterate through the blocks up to that layer. Note that this is exclusive, eg stop_at_layer==0 means to only run the embed, stop_at_layer==-1 means to run every layer *apart* from the final one, etc.
             transformer_block_list = self.blocks[:stop_at_layer] # type: ignore
  
         for i, block in enumerate(transformer_block_list): # type: ignore
             # Note that each block includes skip connections, so we don't need
             # residual + block(residual)
+            # If we're using multiple GPUs, we need to send the residual and shortformer_pos_embed to the correct GPU
+            residual = residual.to(devices.get_device_for_block_index(i, self.cfg))
+            if shortformer_pos_embed is not None:
+                shortformer_pos_embed = shortformer_pos_embed.to(
+                    devices.get_device_for_block_index(i, self.cfg)
+                )
+
             residual = block(
                 residual,
                 past_kv_cache_entry=past_kv_cache[i]
                 if past_kv_cache is not None
-                else None,  # Cache is contains a list of HookedTransformerKeyValueCache objects, one for each block
+                else None,  # Cache contains a list of HookedTransformerKeyValueCache objects, one for each block
                 shortformer_pos_embed=shortformer_pos_embed,
             )  # [batch, pos, d_model]
         
         if stop_at_layer is not None:
             # When we stop at an early layer, we end here rather than doing further computation
             return None
 
@@ -334,14 +357,16 @@
         logits: Float[torch.Tensor, "batch pos d_vocab"],
         tokens: Int[torch.Tensor, "batch pos"],
         per_token: bool = False,
     ):
         """
         Wrapper around utils.lm_cross_entropy_loss, used in forward() with return_type=="loss" or "both".
         """
+        if tokens.device != logits.device:
+            tokens = tokens.to(logits.device)
         return utils.lm_cross_entropy_loss(logits, tokens, per_token)
 
     @overload
     def run_with_cache(
         self, *model_args, return_cache_object: Literal[True] = True, **kwargs
     ) -> Tuple[Output, ActivationCache]:
         ...
@@ -449,15 +474,20 @@
         elif len(tokens.shape) <= 1:
             return self.tokenizer.decode(tokens, clean_up_tokenization_spaces=False)
         else:
             raise ValueError(f"Invalid shape passed in: {tokens.shape}")
 
     def to_str_tokens(
         self,
-        input: Union[str, Union[Float[torch.Tensor, "pos"], Float[torch.Tensor, "1 pos"]], list],
+        input: Union[str,
+                     Int[torch.Tensor, "pos"],
+                     Int[torch.Tensor, "1 pos"],
+                     Int[np.ndarray, "pos"],
+                     Int[np.ndarray, "1 pos"],
+                     list],
         prepend_bos: bool = True,
     ) -> List[str]:
         """Method to map text, a list of text or tokens to a list of tokens as strings
 
         Gotcha: prepend_bos prepends a beginning of string token. This is a recommended default when inputting a prompt to the model as the first token is often treated weirdly, but should only be done at the START of the prompt. Make sure to turn it off if you're looking at the tokenization of part of the prompt!
         (Note: some models eg GPT-2 were not trained with a BOS token, others (OPT and my models) were)
 
@@ -477,20 +507,26 @@
                 map(lambda tokens: self.to_str_tokens(tokens, prepend_bos), input)
             )  # type: ignore
         elif isinstance(input, str):
             tokens = self.to_tokens(input, prepend_bos=prepend_bos)[0]
         elif isinstance(input, torch.Tensor):
             tokens = input
             tokens = tokens.squeeze()  # Get rid of a trivial batch dimension
+            if tokens.dim() == 0:
+                # Don't pass dimensionless tensor
+                tokens = tokens.unsqueeze(0)
             assert (
                 tokens.dim() == 1
             ), f"Invalid tokens input to to_str_tokens, has shape: {tokens.shape}"
         elif isinstance(input, np.ndarray):
             tokens = input
             tokens = tokens.squeeze()  # Get rid of a trivial batch dimension
+            if tokens.ndim == 0:
+                # Don't pass dimensionless tensor
+                tokens = np.expand_dims(tokens, axis=0)
             assert (
                 tokens.ndim == 1
             ), f"Invalid tokens input to to_str_tokens, has shape: {tokens.shape}"
         else:
             raise ValueError(f"Invalid input type to to_str_tokens: {type(input)}")
         str_tokens = self.tokenizer.batch_decode(
             tokens, clean_up_tokenization_spaces=False
@@ -502,14 +538,21 @@
 
         # We use the to_tokens method, do not append a BOS token
         token = self.to_tokens(string, prepend_bos=False).squeeze()
         # If token shape is non-empty, raise error
         assert not token.shape, f"Input string: {string} is not a single token!"
         return token.item()
 
+    def to_single_str_token(self, int_token: int) -> str:
+        # Gives the single token corresponding to an int in string form
+        assert isinstance(int_token, int)
+        token = self.to_str_tokens(torch.tensor([int_token]))
+        assert len(token) == 1
+        return token[0]
+
     def get_token_position(
         self,
         single_token: Union[str, int],
         input: Union[str, Union[Float[torch.Tensor, "pos"], Float[torch.Tensor, "1 pos"]]],
         mode="first",
         prepend_bos=True,
     ):
@@ -601,36 +644,57 @@
         elif isinstance(device_or_dtype, str):
             self.cfg.device = device_or_dtype
             if print_details: 
                 print("Moving model to device: ", self.cfg.device)
         elif isinstance(device_or_dtype, torch.dtype):
             if print_details: 
                 print("Changing model dtype to", device_or_dtype)
+            # change state_dict dtypes
+            for k, v in self.state_dict().items():
+                self.state_dict()[k] = v.to(device_or_dtype)
         return nn.Module.to(self, device_or_dtype)
 
     def cuda(self):
         # Wrapper around cuda that also changes self.cfg.device
         return self.to("cuda")
 
     def cpu(self):
         # Wrapper around cuda that also changes self.cfg.device
         return self.to("cpu")
 
     @classmethod
+    def move_model_modules_to_device(cls, model: "HookedTransformer"):
+        model.embed.to(devices.get_device_for_block_index(0, model.cfg))
+        model.hook_embed.to(devices.get_device_for_block_index(0, model.cfg))
+        if model.cfg.positional_embedding_type != "rotary":
+            model.pos_embed.to(devices.get_device_for_block_index(0, model.cfg))
+            model.hook_pos_embed.to(devices.get_device_for_block_index(0, model.cfg))
+        if hasattr(model, "ln_final"):
+            model.ln_final.to(
+                devices.get_device_for_block_index(model.cfg.n_layers - 1, model.cfg)
+            )
+        model.unembed.to(
+            devices.get_device_for_block_index(model.cfg.n_layers - 1, model.cfg)
+        )
+        for i, block in enumerate(model.blocks):
+            block.to(devices.get_device_for_block_index(i, model.cfg))
+
+    @classmethod
     def from_pretrained(
         cls,
         model_name: str,
         fold_ln=True,
         center_writing_weights=True,
         center_unembed=True,
         refactor_factored_attn_matrices=False,
         checkpoint_index=None,
         checkpoint_value=None,
         hf_model=None,
         device=None,
+        n_devices=1,
         move_state_dict_to_device=True,
         **model_kwargs,
     ):
         """Class method to load in a pretrained model weights to the HookedTransformer format and optionally to do some processing to make the model easier to interpret. Currently supports loading from most autoregressive HuggingFace models (GPT2, GPTNeo, GPTJ, OPT) and from a range of toy models and SoLU models trained by me (Neel Nanda).
 
         Also supports loading from a checkpoint for checkpointed models (currently, models trained by me (NeelNanda) and the stanford-crfm models). These can either be determined by the checkpoint index (the index of the checkpoint in the checkpoint list) or by the checkpoint value (the value of the checkpoint, eg 1000 for a checkpoint taken at step 1000 or after 1000 tokens. Each model has checkpoints labelled with exactly one of labels and steps). If neither is specified the final model is loaded. If both are specified, the checkpoint index is used.
 
@@ -658,14 +722,16 @@
                 has checkpoints labelled with exactly one of these). Defaults to
                 None.
             hf_model (AutoModelForCausalLM, optional): If you have already loaded in the
                 HuggingFace model, you can pass it in here rather than needing
                 to recreate the object. Defaults to None.
             device (str, optional): The device to load the model onto. By
                 default will load to CUDA if available, else CPU.
+            n_devices (int, optional): The number of devices to split the model
+                across. Defaults to 1. If greater than 1, `device` must be cuda.
             move_state_dict_to_device (bool): Whether to move the state dict to the
                 relevant device before processing and loading in the weights.
                 Defaults to True.
             model_kwargs (dict, optional): Any additional kwargs to pass to the
                 HookedTransformer initialization.
         """
         # Get the model name used in HuggingFace, rather than the alias.
@@ -676,14 +742,15 @@
         # checkpoint
         cfg = loading.get_pretrained_model_config(
             official_model_name,
             checkpoint_index=checkpoint_index,
             checkpoint_value=checkpoint_value,
             fold_ln=fold_ln,
             device=device,
+            n_devices=n_devices,
         )
 
         # Get the state dict of the model (ie a mapping of parameter names to tensors), processed to match the HookedTransformer parameter names.
         state_dict = loading.get_pretrained_state_dict(
             official_model_name, cfg, hf_model
         )
 
@@ -770,18 +837,50 @@
                 residual stream (ie set mean to be zero). Due to LayerNorm this doesn't change the computation. Defaults to True.
             center_unembed (bool, optional): Whether to center W_U (ie set mean to be zero).
                 Softmax is translation invariant so this doesn't affect log probs or loss, but does change logits. Defaults to True.
             fold_value_biases (bool, optional): Whether to fold the value biases into the output bias. Because attention patterns add up to 1, the value biases always have a constant effect on a layer's output, and it doesn't matter which head a bias is associated with. We can factor this all into a single output bias to the layer, and make it easier to interpret the head's output.
             refactor_factored_attn_matrices (bool, optional): Whether to convert the factored
                 matrices (W_Q & W_K, and W_O & W_V) to be "even". Defaults to False
             move_state_dict_to_device (bool, optional): Whether to move the state dict to the device of the model. Defaults to True.
+            model_name (str, optional): checks the model name for special cases of state dict loading. Only used for Redwood 2L model currently
         """
 
+        assert (
+            self.cfg.n_devices == 1 or move_state_dict_to_device
+        ), "If n_devices > 1, move_state_dict_to_device must be True"
+
+        
+        if self.cfg.positional_embedding_type == "shortformer":
+            if fold_ln:
+                logging.warning("You tried to specify fold_ln=True for a shortformer model, but this can't be done! Setting fold_ln=False instead.")
+                fold_ln = False
+
         if move_state_dict_to_device:
-            state_dict = {k: v.to(self.cfg.device) for k, v in state_dict.items()}
+            for k, v in state_dict.items():
+                if k.startswith("embed") or k.startswith("pos_embed"):
+                    state_dict[k] = v.to(
+                        devices.get_device_for_block_index(0, self.cfg)
+                    )
+                elif k.startswith("ln_final") or k.startswith("unembed"):
+                    state_dict[k] = v.to(
+                        devices.get_device_for_block_index(
+                            self.cfg.n_layers - 1, self.cfg
+                        )
+                    )
+                elif k.startswith("blocks"):
+                    state_dict[k] = v.to(
+                        devices.get_device_for_block_index(
+                            int(k.split(".")[1]), self.cfg
+                        )
+                    )
+                else:
+                    raise KeyError(
+                        f"State Dict contains a key not in the HookedTransformer format: {k}"
+                    )
+
         state_dict = self.fill_missing_keys(state_dict)
         if fold_ln:
             if self.cfg.normalization_type not in ["LN", "LNPre"]:
                 logging.warning(
                     "You are not using LayerNorm, so the layer norm weights can't be folded! Skipping"
                 )
             else:
@@ -1190,15 +1289,15 @@
             if type(input) == str:
                 return_type = "str"
             else:
                 return_type = "tensor"
 
         assert isinstance(tokens, torch.Tensor)
         batch_size, ctx_length = tokens.shape
-        tokens = tokens.to(self.cfg.device)
+        tokens = tokens.to(devices.get_device_for_block_index(0, self.cfg))
         if use_past_kv_cache:
             past_kv_cache = HookedTransformerKeyValueCache.init_cache(
                 self.cfg, self.cfg.device, batch_size
             )
         else:
             past_kv_cache = None
 
@@ -1240,15 +1339,15 @@
             sampled_tokens = utils.sample_logits(
                 final_logits,
                 top_k=top_k,
                 top_p=top_p,
                 temperature=temperature,
                 freq_penalty=freq_penalty,
                 tokens=tokens,
-            )
+            ).to(devices.get_device_for_block_index(0, self.cfg))
 
             if stop_at_eos:
                 # For all unfinished sequences, add on the next token. If a sequence finished, we throw away the generated token and instead add an EOS token to pad.
                 sampled_tokens[finished_sequences] = eos_token_id
                 finished_sequences.logical_or_(sampled_tokens == eos_token_id)
 
             tokens = torch.cat([tokens, sampled_tokens.unsqueeze(-1)], dim=-1)
```

### Comparing `transformer_lens-1.2.1/transformer_lens/HookedTransformerConfig.py` & `transformer_lens-1.2.2/transformer_lens/HookedTransformerConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,21 +69,23 @@
             initialized to 0 and weights are standard normals of range
             initializer_range.
         normalization_type (str, *optional*): the type of normalization to use.
             Options are None (no normalization), 'LN' (use LayerNorm, including weights
             & biases) and 'LNPre' (use LayerNorm, but no weights & biases).
             Defaults to LN
         device(str): The device to use for the model. Defaults to 'cuda' if
-            available, else 'cpu
+            available, else 'cpu'. Must be 'cuda' if `n_devices` > 1.
+        n_devices (int): The number of devices to use for the model. Defaults to 1. Layers are loaded
+            to support "pipeline parallelism", where each device is responsible for a subset of the layers.
         attention_dir (str): Whether to use causal (aka unidirectional aka GPT-2
             style) or bidirectional attention. Options are 'causal' and
             'bidirectional'. Defaults to 'causal'
         attn_only (bool): Whether to only use attention layers, no feedforward
             layers. Defaults to False
-        seed (int, *optional*): The seed to use for the model. 
+        seed (int, *optional*): The seed to use for the model.
             Used to set sources of randomness (Python, PyTorch and
             NumPy) and to initialize weights. Defaults to None. We recommend setting a seed, so your experiments are reproducible.
         initializer_range (float): The standard deviation of the normal used to
             initialise the weights, initialized to 0.8 / sqrt(d_model) .
         init_weights (bool): Whether to initialize the weights. Defaults to
             True. If False, does not initialize weights.
         scale_attn_by_inverse_layer_idx (bool): Whether to scale the attention
@@ -144,27 +146,29 @@
     checkpoint_value: Optional[int] = None
     tokenizer_name: Optional[str] = None
     window_size: Optional[int] = None
     attn_types: Optional[List] = None
     init_mode: str = "gpt2"
     normalization_type: Optional[str] = "LN"
     device: Optional[str] = None
+    n_devices: int = 1
     attention_dir: str = "causal"
     attn_only: bool = False
     seed: Optional[int] = None
     initializer_range: float = -1.0
     init_weights: bool = True
     scale_attn_by_inverse_layer_idx: bool = False
     positional_embedding_type: str = "standard"
     final_rms: bool = False
     d_vocab_out: int = -1
     parallel_attn_mlp: bool = False
     rotary_dim: Optional[int] = None
     n_params: Optional[int] = None
     use_hook_tokens: bool = False
+    gated_mlp: bool = False
 
     def __post_init__(self):
         if self.n_heads==-1:
             self.n_heads = self.d_model // self.d_head
 
             if not self.d_model % (self.d_head) == 0:
                 logging.warning(
@@ -209,25 +213,33 @@
         if not self.attn_only:
             # Number of parameters in MLP layers (ignoring biases and layer norm). 2 because W_in and W_out
             self.n_params += self.n_layers * self.d_model * self.d_mlp * 2
 
         if self.device is None:
             self.device = "cuda" if torch.cuda.is_available() else "cpu"
 
+        if self.n_devices > 1:
+            assert (
+                self.device == "cuda"
+            ), "n_devices > 1 is only supported on CUDA devices"
+            assert (
+                torch.cuda.device_count() >= self.n_devices
+            ), f"Not enough CUDA devices to support n_devices {self.n_devices}"
+
     @classmethod
     def from_dict(cls, config_dict: Dict[str, Any]):
         """
         Instantiates a `HookedTransformerConfig` from a Python dictionary of
         parameters.
         """
         return cls(**config_dict)
 
     def to_dict(self):
         return self.__dict__
 
     def __repr__(self):
         return "HookedTransformerConfig:\n" + pprint.pformat(self.to_dict())
-    
+
     def set_seed_everywhere(self, seed: int):
         torch.manual_seed(seed)
         random.seed(seed)
         np.random.seed(seed)
```

### Comparing `transformer_lens-1.2.1/transformer_lens/__init__.py` & `transformer_lens-1.2.2/transformer_lens/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     HookedTransformerKeyValueCacheEntry,
 )
 from . import components
 from .HookedTransformerConfig import HookedTransformerConfig
 from .FactoredMatrix import FactoredMatrix
 from .ActivationCache import ActivationCache
 from .HookedTransformer import HookedTransformer
+from . import head_detector
 from . import loading_from_pretrained as loading
 from . import patching
 from . import train
 
 from .past_key_value_caching import (
     HookedTransformerKeyValueCache as EasyTransformerKeyValueCache,
     HookedTransformerKeyValueCacheEntry as EasyTransformerKeyValueCacheEntry,
 )
 from .HookedTransformer import HookedTransformer as EasyTransformer
-from .HookedTransformerConfig import HookedTransformerConfig as EasyTransformerConfig
+from .HookedTransformerConfig import HookedTransformerConfig as EasyTransformerConfig
```

### Comparing `transformer_lens-1.2.1/transformer_lens/components.py` & `transformer_lens-1.2.2/transformer_lens/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,15 +500,15 @@
         Note: For some inexplicable reason, in GPT-J each ADJACENT pair of elements in k and q are rotated, in GPT-NeoX the pair of elements at k and k+n//2 are rotated (ie folding the full length in half, and then looking at pairs accordingly). I have absolutely no clue why, it should be completely equivalent.
         To resolve this, I've coded it to default to the GPT-J mode, but to explicitly check whether it's GPT-NeoX and then do the GPT-NeoX thing if it is.
         """
         pos = torch.arange(n_ctx, dtype=torch.float32)
         dim = torch.arange(rotary_dim // 2, dtype=torch.float32)
         # A set of frequencies evenly spaced in log space
         freq = base ** (dim / (rotary_dim / 2))
-        if self.cfg.original_architecture == "GPTNeoXForCausalLM":
+        if self.cfg.original_architecture == "GPTNeoXForCausalLM" or self.cfg.original_architecture == "LLaMAForCausalLM":
             freq = einops.repeat(freq, "d -> (2 d)")
         else:
             freq = einops.repeat(freq, "d -> (d 2)")
         # Create a n_ctx x rotary_dim tensor, where each column is an arithmetic sequence of angles in that frequency
         angles = pos[:, None] / freq[None, :]
         return torch.sin(angles), torch.cos(angles)
 
@@ -517,15 +517,15 @@
         Rotary helper function, splits x into blocks of size 2 along the final axis and maps [x0, x1] to [-x1, x0]
 
         The final axis of x must have even length.
 
         GPT-NeoX and GPT-J do rotary subtly differently, see calculate_sin_cos_rotary for details.
         """
         rot_x = x.clone()
-        if self.cfg.original_architecture == "GPTNeoXForCausalLM":
+        if self.cfg.original_architecture == "GPTNeoXForCausalLM" or self.cfg.original_architecture == "LLaMAForCausalLM":
             n = x.size(-1) // 2
             rot_x[..., :n] = -x[..., n:]
             rot_x[..., n:] = x[..., :n]
         else:
             rot_x[..., ::2] = -x[..., 1::2]
             rot_x[..., 1::2] = x[..., ::2]
 
@@ -603,14 +603,75 @@
                 "batch pos d_mlp, d_mlp d_model -> batch pos d_model",
                 post_act,
                 self.W_out,
             )
             + self.b_out
         )
 
+# TODO
+# not sure whether to fold this into MLP or not
+class GatedMLP(nn.Module):
+    def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
+        super().__init__()
+        if isinstance(cfg, Dict):
+            cfg = HookedTransformerConfig.from_dict(cfg)
+        self.cfg = cfg
+        self.W_in = nn.Parameter(torch.empty(self.cfg.d_model, self.cfg.d_mlp))
+        self.W_gate = nn.Parameter(torch.empty(self.cfg.d_model, self.cfg.d_mlp))
+        self.b_in = nn.Parameter(torch.zeros(self.cfg.d_mlp))
+        self.W_out = nn.Parameter(torch.empty(self.cfg.d_mlp, self.cfg.d_model))
+        self.b_out = nn.Parameter(torch.zeros(self.cfg.d_model))
+
+        # hook on gate output but before act_fn 
+        self.hook_pre = HookPoint() # [batch, pos, d_mlp]
+        # hook on act_fn(gate_output) * W_in(x) + b_in 
+        self.hook_post = HookPoint() # [batch, pos, d_mlp]
+
+        if self.cfg.act_fn == "relu":
+            self.act_fn = F.relu
+        elif self.cfg.act_fn == "gelu":
+            self.act_fn = F.gelu
+        elif self.cfg.act_fn == "silu":
+            self.act_fn = F.silu
+        elif self.cfg.act_fn == "gelu_new":
+            self.act_fn = gelu_new
+        elif self.cfg.act_fn == "gelu_fast":
+            self.act_fn = gelu_fast
+        elif self.cfg.act_fn == "solu_ln":
+            self.act_fn = solu
+            # Hook taken between activation and layer norm
+            self.hook_mid = HookPoint()  # [batch, pos, d_mlp]
+            if self.cfg.normalization_type == "LN":
+                self.ln = LayerNorm(self.cfg, self.cfg.d_mlp)
+            else:
+                self.ln = LayerNormPre(self.cfg)
+
+        else:
+            raise ValueError(f"Invalid activation function name: {self.cfg.act_fn}")
+
+    def forward(
+        self, x: Float[torch.Tensor, "batch pos d_model"]
+    ) -> Float[torch.Tensor, "batch pos d_model"]:
+        # Technically, all these einsums could be done with a single matmul, but this is more readable.
+        pre_act = self.hook_pre(einsum("batch pos d_model, d_model d_mlp -> batch pos d_mlp", x, self.W_gate))  # [batch, pos, d_mlp]
+        if not self.cfg.act_fn.endswith("_ln"):
+            post_act = self.hook_post(self.act_fn(pre_act) * einsum("batch pos d_model, d_model d_mlp -> batch pos d_mlp", x, self.W_in)
+            + self.b_in)  # [batch, pos, d_mlp]
+        else:
+            mid_act = self.hook_mid(self.act_fn(pre_act))  # [batch, pos, d_mlp]
+            post_act = self.hook_post(self.ln(mid_act))
+        return (
+            einsum(
+                "batch pos d_mlp, d_mlp d_model -> batch pos d_model",
+                post_act,
+                self.W_out,
+            )
+            + self.b_out
+        )
+
 
 # Transformer Block
 class TransformerBlock(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig], block_index):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
@@ -620,14 +681,22 @@
             if not self.cfg.attn_only:
                 self.ln2 = LayerNorm(cfg)
         elif self.cfg.normalization_type == "LNPre":
             # We've folded in LayerNorm weights, so just need the center + scale parts
             self.ln1 = LayerNormPre(cfg)
             if not self.cfg.attn_only:
                 self.ln2 = LayerNormPre(cfg)
+        elif self.cfg.normalization_type == "RMS": 
+            self.ln1 = RMSNorm(cfg)
+            if not self.cfg.attn_only:
+                self.ln2 = RMSNorm(cfg)
+        elif self.cfg.normalization_type == "RMSPre":
+            self.ln1 = RMSNormPre(cfg)
+            if not self.cfg.attn_only:
+                self.ln2 = RMSNormPre(cfg)
         elif self.cfg.normalization_type is None:
             self.ln1 = nn.Identity()
             if not self.cfg.attn_only:
                 self.ln2 = nn.Identity()
         else:
             logging.warning(
                 f"Invalid normalization_type passed in {self.cfg.normalization_type}"
@@ -636,15 +705,18 @@
         if not self.cfg.use_local_attn:
             self.attn = Attention(cfg, "global", block_index)
         else:
             assert self.cfg.attn_types is not None
             attn_type = self.cfg.attn_types[block_index]
             self.attn = Attention(cfg, attn_type, block_index)
         if not self.cfg.attn_only:
-            self.mlp = MLP(cfg)
+            if self.cfg.gated_mlp:
+                self.mlp = GatedMLP(cfg)
+            else: 
+                self.mlp = MLP(cfg)
 
         self.hook_q_input = HookPoint()  # [batch, pos, d_model]
         self.hook_k_input = HookPoint()  # [batch, pos, d_model]
         self.hook_v_input = HookPoint()  # [batch, pos, d_model]
 
         self.hook_attn_out = HookPoint()  # [batch, pos, d_model]
         self.hook_mlp_out = HookPoint()  # [batch, pos, d_model]
```

### Comparing `transformer_lens-1.2.1/transformer_lens/hook_points.py` & `transformer_lens-1.2.2/transformer_lens/hook_points.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,74 +2,89 @@
 import logging
 from typing import Callable, Union, Optional, Sequence, Dict, List, Tuple
 import torch
 import torch.nn as nn
 import torch.utils.hooks as hooks
 
 from functools import *
+from contextlib import contextmanager
 
 from dataclasses import dataclass
 
 @dataclass
 class LensHandle:
+    """
+    A dataclass that holds information about a PyTorch hook.
+
+    Attributes:
+        hook (hooks.RemovableHandle): Reference to the hook's RemovableHandle.
+        is_permanent (bool, optional): Indicates if the hook is permanent. Defaults to False.
+        context_level (Optional[int], optional): Context level associated with the hooks context
+            manager for the given hook. Defaults to None.
+    """
     hook: hooks.RemovableHandle
     is_permanent: bool = False
+    context_level: Optional[int] = None
     
 
 # %%
 # Define type aliases
 NamesFilter = Optional[Union[Callable[[str], bool], Sequence[str]]]
 
 # %%
-# A helper class to get access to intermediate activations (inspired by Garcon)
-# It's a dummy module that is the identity function by default
-# I can wrap any intermediate activation in a HookPoint and get a convenient
-# way to add PyTorch hooks
 class HookPoint(nn.Module):
+    """
+    A helper class to access intermediate activations in a PyTorch model (inspired by Garcon).
+
+    HookPoint is a dummy module that acts as an identity function by default. By wrapping any
+    intermediate activation in a HookPoint, it provides a convenient way to add PyTorch hooks.
+    """
     def __init__(self):
         super().__init__()
         self.fwd_hooks: List[LensHandle] = []
         self.bwd_hooks: List[LensHandle] = []
         self.ctx = {}
 
         # A variable giving the hook's name (from the perspective of the root
         # module) - this is set by the root module at setup.
         self.name = None
 
     def add_perma_hook(self, hook, dir="fwd") -> None:
         self.add_hook(hook, dir=dir, is_permanent=True)
 
-    def add_hook(self, hook, dir="fwd", is_permanent=False) -> None:
+    def add_hook(self, hook, dir="fwd", is_permanent=False, level=None) -> None:
         # Hook format is fn(activation, hook_name)
         # Change it into PyTorch hook format (this includes input and output,
         # which are the same for a HookPoint)
         if dir == "fwd":
 
             def full_hook(module, module_input, module_output):
                 return hook(module_output, hook=self)
 
             handle = self.register_forward_hook(full_hook)
-            handle = LensHandle(handle, is_permanent)
+            handle = LensHandle(handle, is_permanent, level)
             self.fwd_hooks.append(handle)
         elif dir == "bwd":
             # For a backwards hook, module_output is a tuple of (grad,) - I don't know why.
             def full_hook(module, module_input, module_output):
                 return hook(module_output[0], hook=self)
             handle = self.register_full_backward_hook(full_hook)
-            handle = LensHandle(handle, is_permanent)
+            handle = LensHandle(handle, is_permanent, level)
             self.bwd_hooks.append(handle)
         else:
             raise ValueError(f"Invalid direction {dir}")
 
-    def remove_hooks(self, dir="fwd", including_permanent=False) -> None:
+    def remove_hooks(self, dir="fwd", including_permanent=False, level=None) -> None:
 
         def _remove_hooks(handles: List[LensHandle]) -> List[LensHandle]:
             output_handles = []
             for handle in handles:
-                if not handle.is_permanent or including_permanent:
+                if including_permanent:
+                    handle.hook.remove()
+                elif (not handle.is_permanent) and (level is None or handle.context_level == level):
                     handle.hook.remove()
                 else:
                     output_handles.append(handle)
             return output_handles
 
         if dir == "fwd" or dir == "both":
             self.fwd_hooks = _remove_hooks(self.fwd_hooks)
@@ -103,129 +118,179 @@
 
     The main time this goes wrong is when you want to use backward hooks (to cache or intervene on gradients). In this case, you need to keep the hooks around as global state until you've run loss.backward() (and so need to disable the reset_hooks_end flag on run_with_hooks)
     """
 
     def __init__(self, *args):
         super().__init__()
         self.is_caching = False
+        self.context_level = 0
 
     def setup(self):
-        # Setup function - this needs to be run in __init__ AFTER defining all
-        # layers
-        # Add a parameter to each module giving its name
-        # Build a dictionary mapping a module name to the module
+        """
+        Sets up model.
+
+        This function must be called in the model's `__init__` method AFTER defining all layers. It
+        adds a parameter to each module containing its name, and builds a dictionary mapping module
+        names to the module instances. It also initializes a hook dictionary for modules of type
+        "HookPoint".
+        """
         self.mod_dict = {}
         self.hook_dict: Dict[str, HookPoint] = {}
         for name, module in self.named_modules():
             module.name = name
             self.mod_dict[name] = module
             if "HookPoint" in str(type(module)):
                 self.hook_dict[name] = module
 
     def hook_points(self):
         return self.hook_dict.values()
 
-    def remove_all_hook_fns(self, direction="both", including_permanent=False):
+    def remove_all_hook_fns(self, direction="both", including_permanent=False, level=None):
         for hp in self.hook_points():
-            hp.remove_hooks(direction, including_permanent=including_permanent)
+            hp.remove_hooks(direction, including_permanent=including_permanent, level=level)
 
     def clear_contexts(self):
         for hp in self.hook_points():
             hp.clear_context()
 
-    def reset_hooks(self, clear_contexts=True, direction="both", including_permanent=False):
+    def reset_hooks(self, clear_contexts=True, direction="both", including_permanent=False, level=None):
         if clear_contexts:
             self.clear_contexts()
-        self.remove_all_hook_fns(direction, including_permanent)
+        self.remove_all_hook_fns(direction, including_permanent, level=level)
         self.is_caching = False
 
-    def check_and_add_hook(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False) -> None:
+    def check_and_add_hook(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False, level=None) -> None:
+        """Runs checks on the hook, and then adds it to the hook point"""
+        self.check_hooks_to_add(hook_point, hook_point_name, hook, dir=dir, is_permanent=is_permanent)
+        hook_point.add_hook(hook, dir=dir, is_permanent=is_permanent, level=level)
+    
+    def check_hooks_to_add(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False) -> None:
         """Override this function to add checks on which hooks should be added"""
-        hook_point.add_hook(hook, dir=dir, is_permanent=is_permanent)
+        pass
 
-    def add_hook(self, name, hook, dir="fwd", is_permanent=False) -> None:
+    def add_hook(self, name, hook, dir="fwd", is_permanent=False, level=None) -> None:
         if type(name) == str:
-            self.check_and_add_hook(self.mod_dict[name], name, hook, dir=dir, is_permanent=is_permanent)
+            self.check_and_add_hook(self.mod_dict[name], name, hook, dir=dir, is_permanent=is_permanent, level=level)
         else:
             # Otherwise, name is a Boolean function on names
             for hook_point_name, hp in self.hook_dict.items():
                 if name(hook_point_name):
-                    self.check_and_add_hook(hp, hook_point_name, hook, dir=dir, is_permanent=is_permanent)
+                    self.check_and_add_hook(hp, hook_point_name, hook, dir=dir, is_permanent=is_permanent, level=level)
 
     def add_perma_hook(self, name, hook, dir="fwd") -> None:
         self.add_hook(name, hook, dir=dir, is_permanent=True)
-
-    def run_with_hooks(
+    
+    @contextmanager
+    def hooks(
         self,
-        *model_args,
         fwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
         bwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
-        reset_hooks_end=True,
-        clear_contexts=False,
-        **model_kwargs,
-    ):
+        reset_hooks_end: bool = True,
+        clear_contexts: bool = False,
+        ):
         """
-        fwd_hooks: A list of (name, hook), where name is either the name of
-        a hook point or a Boolean function on hook names and hook is the
-        function to add to that hook point, or the hook whose names evaluate
-        to True respectively. Ditto bwd_hooks
-        reset_hooks_end (bool): If True, all hooks are removed at the end (ie,
-        including those added in this run)
-        clear_contexts (bool): If True, clears hook contexts whenever hooks are reset
-        Note that if we want to use backward hooks, we need to set
-        reset_hooks_end to be False, so the backward hooks are still there - this function only runs a forward pass.
+        A context manager for adding temporary hooks to the model.
+
+        Args:
+            fwd_hooks: List[Tuple[name, hook]], where name is either the name of a hook point or a
+                Boolean function on hook names and hook is the function to add to that hook point.
+            bwd_hooks: Same as fwd_hooks, but for the backward pass.
+            reset_hooks_end (bool): If True, removes all hooks added by this context manager when the context manager exits.
+            clear_contexts (bool): If True, clears hook contexts whenever hooks are reset.
+        
+        Example:
+        --------
+        .. code-block:: python
+
+            >>> with model.hooks(fwd_hooks=my_hooks):
+            >>>     hooked_loss = model(text, return_type="loss")
         """
         try:
+            self.context_level += 1
+
             for name, hook in fwd_hooks:
                 if type(name) == str:
-                    self.mod_dict[name].add_hook(hook, dir="fwd")
+                    self.mod_dict[name].add_hook(hook, dir="fwd", level=self.context_level)
                 else:
                     # Otherwise, name is a Boolean function on names
                     for hook_name, hp in self.hook_dict.items():
                         if name(hook_name):
-                            hp.add_hook(hook, dir="fwd")
+                            hp.add_hook(hook, dir="fwd", level=self.context_level)
             for name, hook in bwd_hooks:
                 if type(name) == str:
-                    self.mod_dict[name].add_hook(hook, dir="bwd")
+                    self.mod_dict[name].add_hook(hook, dir="bwd", level=self.context_level)
                 else:
                     # Otherwise, name is a Boolean function on names
                     for hook_name, hp in self.hook_dict:
                         if name(hook_name):
-                            hp.add_hook(hook, dir="bwd")
-            return self.forward(*model_args, **model_kwargs)
+                            hp.add_hook(hook, dir="bwd", level=self.context_level)
+            yield self
         finally:
             if reset_hooks_end:
-                if len(bwd_hooks) > 0:
-                    logging.warning(
-                        "WARNING: Hooks were reset at the end of run_with_hooks while backward hooks were set. This removes the backward hooks before a backward pass can occur"
-                    )
-                self.reset_hooks(clear_contexts, including_permanent=False)
+                self.reset_hooks(clear_contexts, including_permanent=False, level=self.context_level)
+            self.context_level -= 1
+
+    def run_with_hooks(
+        self,
+        *model_args,
+        fwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
+        bwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
+        reset_hooks_end=True,
+        clear_contexts=False,
+        **model_kwargs,
+    ):
+        """
+        Runs the model with specified forward and backward hooks.
+
+        Args:
+            fwd_hooks (List[Tuple[Union[str, Callable], Callable]]): A list of (name, hook), where name is
+                either the name of a hook point or a boolean function on hook names, and hook is the
+                function to add to that hook point. Hooks with names that evaluate to True are added
+                respectively.
+            bwd_hooks (List[Tuple[Union[str, Callable], Callable]]): Same as fwd_hooks, but for the
+                backward pass.
+            reset_hooks_end (bool): If True, all hooks are removed at the end, including those added
+                during this run. Default is True.
+            clear_contexts (bool): If True, clears hook contexts whenever hooks are reset. Default is
+                False.
+            *model_args: Positional arguments for the model.
+            **model_kwargs: Keyword arguments for the model.
+
+        Note:
+            If you want to use backward hooks, set `reset_hooks_end` to False, so the backward hooks
+            remain active. This function only runs a forward pass.
+        """
+        if len(bwd_hooks) > 0 and reset_hooks_end:
+            logging.warning(
+                "WARNING: Hooks will be reset at the end of run_with_hooks. This removes the backward hooks before a backward pass can occur."
+            )
+
+        with self.hooks(fwd_hooks, bwd_hooks, reset_hooks_end, clear_contexts) as hooked_model:
+            return hooked_model.forward(*model_args, **model_kwargs)
 
     def add_caching_hooks(
         self,
         names_filter: NamesFilter = None,
         incl_bwd: bool = False,
         device=None,
         remove_batch_dim: bool = False,
         cache: Optional[dict] = None,
     ) -> dict:
         """Adds hooks to the model to cache activations. Note: It does NOT actually run the model to get activations, that must be done separately.
 
         Args:
             names_filter (NamesFilter, optional): Which activations to cache. Can be a list of strings (hook names) or a filter function mapping hook names to booleans. Defaults to lambda name: True.
             incl_bwd (bool, optional): Whether to also do backwards hooks. Defaults to False.
-            device (_type_, optional): The device to store on. Defaults to CUDA if available else CPU.
+            device (_type_, optional): The device to store on. Defaults to same device as model.
             remove_batch_dim (bool, optional): Whether to remove the batch dimension (only works for batch_size==1). Defaults to False.
             cache (Optional[dict], optional): The cache to store activations in, a new dict is created by default. Defaults to None.
 
         Returns:
             cache (dict): The cache where activations will be stored.
         """
-        if device is None:
-            device = "cuda" if torch.cuda.is_available() else "cpu"
         if cache is None:
             cache = {}
 
         if names_filter is None:
             names_filter = lambda name: True
         elif type(names_filter) == str:
             names_filter = lambda name: name == names_filter
@@ -261,35 +326,105 @@
         remove_batch_dim=False,
         incl_bwd=False,
         reset_hooks_end=True,
         clear_contexts=False,
         **model_kwargs,
     ):
         """
-        Runs the model and returns model output and a Cache object
+        Runs the model and returns the model output and a Cache object.
+
+        Args:
+            *model_args: Positional arguments for the model.
+            names_filter (NamesFilter, optional): A filter for which activations to cache. Accepts None, str,
+                list of str, or a function that takes a string and returns a bool. Defaults to None, which
+                means cache everything.
+            device (str or torch.Device, optional): The device to cache activations on. Defaults to the
+                model device. WARNING: Setting a different device than the one used by the model leads to
+                significant performance degradation.
+            remove_batch_dim (bool, optional): If True, removes the batch dimension when caching. Only
+                makes sense with batch_size=1 inputs. Defaults to False.
+            incl_bwd (bool, optional): If True, calls backward on the model output and caches gradients
+                as well. Assumes that the model outputs a scalar (e.g., return_type="loss"). Custom loss
+                functions are not supported. Defaults to False.
+            reset_hooks_end (bool, optional): If True, removes all hooks added by this function at the 
+                end of the run. Defaults to True.
+            clear_contexts (bool, optional): If True, clears hook contexts whenever hooks are reset.
+                Defaults to False.
+            **model_kwargs: Keyword arguments for the model.
+
+        Returns:
+            tuple: A tuple containing the model output and a Cache object.
 
-        model_args and model_kwargs - all positional arguments and keyword arguments not otherwise captured are input to the model
-        names_filter (None or str or [str] or fn:str->bool): a filter for which activations to cache. Defaults to None, which means cache everything.
-        device (str or torch.Device): The device to cache activations on, defaults to model device. Note that this must be set if the model does not have a model.cfg.device attribute. WARNING: Setting a different device than the one used by the model leads to significant performance degradation.
-        remove_batch_dim (bool): If True, will remove the batch dimension when caching. Only makes sense with batch_size=1 inputs.
-        incl_bwd (bool): If True, will call backward on the model output and also cache gradients. It is assumed that the model outputs a scalar, ie. return_type="loss", for predict the next token loss. Custom loss functions are not supported
-        reset_hooks_end (bool): If True, all hooks are removed at the end (ie, both those added in this run *and* any added before!)
-        clear_contexts (bool): If True, clears hook contexts whenever hooks are reset
         """
-        cache_dict = self.add_caching_hooks(
+        cache_dict, fwd, bwd = self.get_caching_hooks(
             names_filter, incl_bwd, device, remove_batch_dim=remove_batch_dim
         )
-        model_out = self(*model_args, **model_kwargs)
 
-        if incl_bwd:
-            model_out.backward()
+        with self.hooks(fwd_hooks=fwd, bwd_hooks=bwd, reset_hooks_end=reset_hooks_end, clear_contexts=clear_contexts):
+            model_out = self(*model_args, **model_kwargs)
+            if incl_bwd:
+                model_out.backward()
 
-        if reset_hooks_end:
-            self.reset_hooks(clear_contexts, including_permanent=False)
         return model_out, cache_dict
+    
+    def get_caching_hooks(
+        self,
+        names_filter: NamesFilter = None,
+        incl_bwd: bool = False,
+        device=None,
+        remove_batch_dim: bool = False,
+        cache: Optional[dict] = None,
+    ) -> Tuple[dict, list, list]:
+        """Creates hooks to cache activations. Note: It does not add the hooks to the model.
+
+        Args:
+            names_filter (NamesFilter, optional): Which activations to cache. Can be a list of strings (hook names) or a filter function mapping hook names to booleans. Defaults to lambda name: True.
+            incl_bwd (bool, optional): Whether to also do backwards hooks. Defaults to False.
+            device (_type_, optional): The device to store on. Keeps on the same device as the layer if None.
+            remove_batch_dim (bool, optional): Whether to remove the batch dimension (only works for batch_size==1). Defaults to False.
+            cache (Optional[dict], optional): The cache to store activations in, a new dict is created by default. Defaults to None.
+
+        Returns:
+            cache (dict): The cache where activations will be stored.
+            fwd_hooks (list): The forward hooks.
+            bwd_hooks (list): The backward hooks. Empty if incl_bwd is False.
+        """
+        if cache is None:
+            cache = {}
+
+        if names_filter is None:
+            names_filter = lambda name: True
+        elif type(names_filter) == str:
+            names_filter = lambda name: name == names_filter
+        elif type(names_filter) == list:
+            names_filter = lambda name: name in names_filter
+
+        self.is_caching = True
+
+        def save_hook(tensor, hook):
+            if remove_batch_dim:
+                cache[hook.name] = tensor.detach().to(device)[0]
+            else:
+                cache[hook.name] = tensor.detach().to(device)
+
+        def save_hook_back(tensor, hook):
+            if remove_batch_dim:
+                cache[hook.name + "_grad"] = tensor.detach().to(device)[0]
+            else:
+                cache[hook.name + "_grad"] = tensor.detach().to(device)
+        
+        fwd_hooks = []
+        bwd_hooks = []
+        for name, hp in self.hook_dict.items():
+            if names_filter(name):
+                fwd_hooks.append((name, save_hook))
+                if incl_bwd:
+                    bwd_hooks.append((name, save_hook_back))
+
+        return cache, fwd_hooks, bwd_hooks
 
     def cache_all(self, cache, incl_bwd=False, device=None, remove_batch_dim=False):
         logging.warning(
             "cache_all is deprecated and will eventually be removed, use add_caching_hooks or run_with_cache"
         )
         self.add_caching_hooks(
             names_filter=lambda name: True,
```

### Comparing `transformer_lens-1.2.1/transformer_lens/loading_from_pretrained.py` & `transformer_lens-1.2.2/transformer_lens/loading_from_pretrained.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,14 +50,30 @@
     "EleutherAI/pythia-160m-deduped",
     "EleutherAI/pythia-410m-deduped",
     "EleutherAI/pythia-1b-deduped",
     "EleutherAI/pythia-1.4b-deduped",
     "EleutherAI/pythia-2.8b-deduped",
     "EleutherAI/pythia-6.9b-deduped",
     "EleutherAI/pythia-12b-deduped",
+    "EleutherAI/pythia-70m-v0",
+    "EleutherAI/pythia-160m-v0",
+    "EleutherAI/pythia-410m-v0",
+    "EleutherAI/pythia-1b-v0",
+    "EleutherAI/pythia-1.4b-v0",
+    "EleutherAI/pythia-2.8b-v0",
+    "EleutherAI/pythia-6.9b-v0",
+    "EleutherAI/pythia-12b-v0",
+    "EleutherAI/pythia-70m-deduped-v0",
+    "EleutherAI/pythia-160m-deduped-v0",
+    "EleutherAI/pythia-410m-deduped-v0",
+    "EleutherAI/pythia-1b-deduped-v0",
+    "EleutherAI/pythia-1.4b-deduped-v0",
+    "EleutherAI/pythia-2.8b-deduped-v0",
+    "EleutherAI/pythia-6.9b-deduped-v0",
+    "EleutherAI/pythia-12b-deduped-v0",
     "NeelNanda/SoLU_1L_v9_old",
     "NeelNanda/SoLU_2L_v10_old",
     "NeelNanda/SoLU_4L_v11_old",
     "NeelNanda/SoLU_6L_v13_old",
     "NeelNanda/SoLU_8L_v21_old",
     "NeelNanda/SoLU_10L_v22_old",
     "NeelNanda/SoLU_12L_v23_old",
@@ -76,14 +92,19 @@
     "NeelNanda/Attn_Only_1L512W_C4_Code",
     "NeelNanda/Attn_Only_2L512W_C4_Code",
     "NeelNanda/Attn_Only_3L512W_C4_Code",
     "NeelNanda/Attn_Only_4L512W_C4_Code",
     "NeelNanda/Attn-Only-2L512W-Shortformer-6B-big-lr",
     "NeelNanda/SoLU_1L512W_Wiki_Finetune",
     "NeelNanda/SoLU_4L512W_Wiki_Finetune",
+    "ArthurConmy/redwood_attn_2l",
+    "llama-7b-hf",
+    "llama-13b-hf",
+    "llama-30b-hf", 
+    "llama-65b-hf",
 ]
 
 # Model Aliases:
 MODEL_ALIASES = {
     "NeelNanda/SoLU_1L_v9_old": ["solu-1l-pile", "solu-1l-old"],
     "NeelNanda/SoLU_2L_v10_old": ["solu-2l-pile", "solu-2l-old"],
     "NeelNanda/SoLU_4L_v11_old": ["solu-4l-pile", "solu-4l-old"],
@@ -217,14 +238,96 @@
         "pythia-6.7b-deduped",
     ],
     "EleutherAI/pythia-12b-deduped": [
         "pythia-12b-deduped",
         "EleutherAI/pythia-13b-deduped", # EleutherAI renamed this model
         "pythia-13b-deduped",
     ],
+
+    "EleutherAI/pythia-70m-v0": [
+        "pythia-70m-v0", 
+        "pythia-v0",
+        "EleutherAI/pythia-19m-v0",
+        "pythia-19m-v0", # EleutherAI renamed this model 
+    ],
+    "EleutherAI/pythia-160m-v0": [
+        "pythia-160m-v0",
+        "EleutherAI/pythia-125m-v0",
+        "pythia-125m-v0", # EleutherAI renamed this model"        
+    ],
+    "EleutherAI/pythia-410m-v0": [
+        "pythia-410m-v0",
+        "EleutherAI/pythia-350m-v0",
+        "pythia-350m-v0", # EleutherAI renamed this model
+    ],
+    "EleutherAI/pythia-1b-v0": [
+        "pythia-1b-v0",
+        "EleutherAI/pythia-800m-v0",
+        "pythia-800m-v0", # EleutherAI renamed this model
+    ],
+    "EleutherAI/pythia-1.4b-v0": [
+        "pythia-1.4b-v0",
+        "EleutherAI/pythia-1.3b-v0",
+        "pythia-1.3b-v0", # EleutherAI renamed this model
+    ],
+    "EleutherAI/pythia-2.8b-v0": [
+        "pythia-2.8b-v0",
+        "EleutherAI/pythia-2.7b-v0",
+        "pythia-2.7b-v0", # EleutherAI renamed this model
+    ],
+    "EleutherAI/pythia-6.9b-v0": [
+        "pythia-6.9b-v0",
+        "EleutherAI/pythia-6.7b-v0",
+        "pythia-6.7b-v0", # EleutherAI renamed this model
+    ],
+    "EleutherAI/pythia-12b-v0": [
+        "pythia-12b-v0",
+        "EleutherAI/pythia-13b-v0",
+        "pythia-13b-v0", # EleutherAI renamed this model
+    ],
+    "EleutherAI/pythia-70m-deduped-v0": [
+        "pythia-70m-deduped-v0",
+        "EleutherAI/pythia-19m-deduped-v0", # EleutherAI renamed this model 
+        "pythia-19m-deduped-v0",
+    ],
+    "EleutherAI/pythia-160m-deduped-v0": [
+        "pythia-160m-deduped-v0",
+        "EleutherAI/pythia-125m-deduped-v0", # EleutherAI renamed this model
+        "pythia-125m-deduped-v0",
+    ],
+    "EleutherAI/pythia-410m-deduped-v0": [
+        "pythia-410m-deduped-v0",
+        "EleutherAI/pythia-350m-deduped-v0", # EleutherAI renamed this model
+        "pythia-350m-deduped-v0",
+    ],
+    "EleutherAI/pythia-1b-deduped-v0": [
+        "pythia-1b-deduped-v0",
+        "EleutherAI/pythia-800m-deduped-v0", # EleutherAI renamed this model
+        "pythia-800m-deduped-v0",
+    ],
+    "EleutherAI/pythia-1.4b-deduped-v0": [
+        "pythia-1.4b-deduped-v0",
+        "EleutherAI/pythia-1.3b-deduped-v0", # EleutherAI renamed this model
+        "pythia-1.3b-deduped-v0",
+    ],
+    "EleutherAI/pythia-2.8b-deduped-v0": [
+        "pythia-2.8b-deduped-v0",
+        "EleutherAI/pythia-2.7b-deduped-v0", # EleutherAI renamed this model
+        "pythia-2.7b-deduped-v0",
+    ],
+    "EleutherAI/pythia-6.9b-deduped-v0": [
+        "pythia-6.9b-deduped-v0",
+        "EleutherAI/pythia-6.7b-deduped-v0", # EleutherAI renamed this model
+        "pythia-6.7b-deduped-v0",
+    ],
+    "EleutherAI/pythia-12b-deduped-v0": [
+        "pythia-12b-deduped-v0",
+        "EleutherAI/pythia-13b-deduped-v0", # EleutherAI renamed this model
+        "pythia-13b-deduped-v0",
+    ],
     
     "gpt2": ["gpt2-small"],
     "distilgpt2": ["distillgpt2", "distill-gpt2", "distil-gpt2", "gpt2-xs"],
     "facebook/opt-125m": ["opt-125m", "opt-small", "opt"],
     "facebook/opt-1.3b": ["opt-1.3b", "opt-medium"],
     "facebook/opt-2.7b": ["opt-2.7b", "opt-large"],
     "facebook/opt-6.7b": ["opt-6.7b", "opt-xl"],
@@ -292,14 +395,19 @@
     ],
     "stanford-crfm/eowyn-gpt2-medium-x777": [
         "stanford-gpt2-medium-e",
         "eowyn-gpt2-medium-x777",
         "gpt2-medium-small-e",
         "gpt2-stanford-medium-e",
     ],
+    "ArthurConmy/redwood_attn_2l": ["redwood_attn_2l"],
+    "llama-7b-hf": ["llama-7b"], 
+    "llama-13b-hf": ["llama-13b"],
+    "llama-30b-hf": ["llama-30b"],
+    "llama-65b-hf": ["llama-65b"],
 }
 
 # Sets a default model alias, by convention the first one in the model alias table, else the official name if it has no aliases
 DEFAULT_MODEL_ALIASES = [MODEL_ALIASES[name][0] if name in MODEL_ALIASES else name for name in OFFICIAL_MODEL_NAMES]
 
 def make_model_alias_map():
     """
@@ -335,17 +443,88 @@
     in the HookedTransformerConfig format.
 
     Takes the official_model_name as an input.
     """
     # In case the user passed in an alias
     official_model_name = get_official_model_name(official_model_name)
     # Load HuggingFace model config
-    hf_config = AutoConfig.from_pretrained(official_model_name)
-    architecture = hf_config.architectures[0]
-    if architecture == "GPTNeoForCausalLM":
+    if 'llama' not in official_model_name:
+        hf_config = AutoConfig.from_pretrained(official_model_name)
+        architecture = hf_config.architectures[0]
+    else: 
+        architecture = "LLaMAForCausalLM"
+    if 'llama-7b' in official_model_name:
+        cfg_dict = {
+            "d_model": 4096,
+            "d_head": 4096 // 32,
+            "n_heads": 32,
+            "d_mlp": 11008,
+            "n_layers": 32,
+            "n_ctx": 2048,
+            "eps": 1e-6, 
+            "d_vocab": 32000,
+            "act_fn": "silu", 
+            "normalization_type": "RMS", 
+            "positional_embedding_type": "rotary",
+            "rotary_dim": 4096 // 32, 
+            "final_rms": True, 
+            "gated_mlp": True, 
+        }
+    elif 'llama-13b' in official_model_name:
+        cfg_dict = {
+            "d_model": 5120,
+            "d_head": 5120 // 40,
+            "n_heads": 40,
+            "d_mlp": 13824,
+            "n_layers": 40,
+            "n_ctx": 2048,
+            "eps": 1e-6, 
+            "d_vocab": 32000,
+            "act_fn": "silu", 
+            "normalization_type": "RMS", 
+            "positional_embedding_type": "rotary",
+            "rotary_dim": 5120 // 40, 
+            "final_rms": True, 
+            "gated_mlp": True, 
+        }
+    elif 'llama-30b' in official_model_name:
+        cfg_dict = {
+            "d_model": 6656,
+            "d_head": 6656 // 52,
+            "n_heads": 52,
+            "d_mlp": 17920,
+            "n_layers": 60,
+            "n_ctx": 2048,
+            "eps": 1e-6, 
+            "d_vocab": 32000,
+            "act_fn": "silu", 
+            "normalization_type": "RMS", 
+            "positional_embedding_type": "rotary",
+            "rotary_dim": 6656 // 52, 
+            "final_rms": True, 
+            "gated_mlp": True, 
+        }
+    elif 'llama-65b' in official_model_name:
+        cfg_dict = {
+            "d_model": 8192,
+            "d_head": 8192 // 64,
+            "n_heads": 64,
+            "d_mlp": 22016,
+            "n_layers": 80,
+            "n_ctx": 2048,
+            "eps": 1e-6, 
+            "d_vocab": 32000,
+            "act_fn": "silu", 
+            "normalization_type": "RMS", 
+            "positional_embedding_type": "rotary",
+            "rotary_dim": 8192 // 64, 
+            "final_rms": True, 
+            "gated_mlp": True, 
+        }
+    elif architecture == "GPTNeoForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_heads,
             "n_heads": hf_config.num_heads,
             "d_mlp": hf_config.hidden_size * 4,
             "n_layers": hf_config.num_layers,
             "n_ctx": hf_config.max_position_embeddings,
@@ -353,14 +532,15 @@
             "d_vocab": hf_config.vocab_size,
             "attn_types": hf_config.attention_layers,
             "act_fn": hf_config.activation_function,
             "use_attn_scale": False,
             "use_local_attn": True,
             "window_size": hf_config.window_size,
             "scale_attn_by_inverse_layer_idx": False,
+            "normalization_type": "LN", 
         }
     elif architecture == "GPT2LMHeadModel":
         cfg_dict = {
             "d_model": hf_config.n_embd,
             "d_head": hf_config.n_embd // hf_config.n_head,
             "n_heads": hf_config.n_head,
             "d_mlp": hf_config.n_embd * 4,
@@ -368,14 +548,15 @@
             "n_ctx": hf_config.n_ctx,
             "eps": hf_config.layer_norm_epsilon,
             "d_vocab": hf_config.vocab_size,
             "act_fn": hf_config.activation_function,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": hf_config.scale_attn_by_inverse_layer_idx,
+            "normalization_type": "LN", 
         }
     elif architecture == "OPTForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
             "n_heads": hf_config.num_attention_heads,
             "d_mlp": hf_config.ffn_dim,
@@ -383,14 +564,15 @@
             "n_ctx": hf_config.max_position_embeddings,
             "eps": 1e-5,
             "d_vocab": hf_config.vocab_size,
             "act_fn": hf_config.activation_function,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": False,
+            "normalization_type": "LN", 
         }
     elif architecture == "GPTJForCausalLM":
         cfg_dict = {
             "d_model": hf_config.n_embd,
             "d_head": hf_config.n_embd // hf_config.n_head,
             "n_heads": hf_config.n_head,
             "d_mlp": 4 * hf_config.n_embd,
@@ -401,14 +583,15 @@
             "act_fn": hf_config.activation_function,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": False,
             "parallel_attn_mlp": True,
             "positional_embedding_type": "rotary",
             "rotary_dim": hf_config.rotary_dim,
+            "normalization_type": "LN", 
         }
     elif architecture == "GPTNeoXForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
             "n_heads": hf_config.num_attention_heads,
             "d_mlp": hf_config.intermediate_size,
@@ -418,21 +601,21 @@
             "d_vocab": hf_config.vocab_size,
             "act_fn": hf_config.hidden_act,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": False,
             "parallel_attn_mlp": True,
             "positional_embedding_type": "rotary",
+            "normalization_type": "LN", 
         }
         rotary_pct = hf_config.rotary_pct
         cfg_dict["rotary_dim"] = round(rotary_pct * cfg_dict["d_head"])
     else:
         raise NotImplementedError(f"{architecture} is not currently supported.")
     # All of these models use LayerNorm
-    cfg_dict["normalization_type"] = "LN"
     cfg_dict["original_architecture"] = architecture
     # The name such that AutoTokenizer.from_pretrained works
     cfg_dict["tokenizer_name"] = official_model_name
     return cfg_dict
 
 
 def convert_neel_model_config(official_model_name: str):
@@ -475,14 +658,15 @@
 
 def get_pretrained_model_config(
     model_name: str,
     checkpoint_index: Optional[int] = None,
     checkpoint_value: Optional[int] = None,
     fold_ln: bool = False,
     device: Optional[str] = None,
+    n_devices: int = 1,
 ):
     """Returns the pretrained model config as an HookedTransformerConfig object.
 
     There are two types of pretrained models: HuggingFace models (where
     AutoModel and AutoConfig work), and models trained by me (NeelNanda) which
     aren't as integrated with HuggingFace infrastructure.
 
@@ -497,18 +681,19 @@
             the checkpoint to load, ie the step or token number (each model has
             checkpoints labelled with exactly one of these). Defaults to None.
         fold_ln (bool, optional): Whether to fold the layer norm into the
             subsequent linear layers (see HookedTransformer.fold_layer_norm for
             details). Defaults to False.
         device (str, optional): The device to load the model onto. By
             default will load to CUDA if available, else CPU.
+        n_devices (int): The number of devices to split the model across. Defaults to 1.
 
     """
     official_model_name = get_official_model_name(model_name)
-    if official_model_name.startswith("NeelNanda"):
+    if official_model_name.startswith("NeelNanda") or official_model_name.startswith("ArthurConmy"):
         cfg_dict = convert_neel_model_config(official_model_name)
     else:
         cfg_dict = convert_hf_model_config(official_model_name)
     # Processing common to both model types
     # Remove any prefix, saying the organization who made a model.
     cfg_dict["model_name"] = official_model_name.split("/")[-1]
     # Don't need to initialize weights, we're loading from pretrained
@@ -536,14 +721,15 @@
             assert checkpoint_value in checkpoint_labels, f"Checkpoint value {checkpoint_value} is not in list of available checkpoints"
             cfg_dict["checkpoint_value"] = checkpoint_value
             cfg_dict["checkpoint_index"] = checkpoint_labels.index(checkpoint_value)
     else:
         cfg_dict["from_checkpoint"] = False
 
     cfg_dict["device"] = device
+    cfg_dict["n_devices"] = n_devices
 
     cfg = HookedTransformerConfig.from_dict(cfg_dict)
     return cfg
 
 
 def get_num_params_of_pretrained(model_name):
     """
@@ -560,25 +746,34 @@
     + list(range(100, 2000, 50))
     + list(range(2000, 20000, 100))
     + list(range(20000, 400000 + 1, 1000))
 )
 
 # Linearly spaced checkpoints for Pythia models, taken every 1000 steps. 
 # Batch size 2,097,152 tokens, so checkpoints every 2.1B tokens
-PYTHIA_CHECKPOINTS = list(range(1000, 143000+1, 1000))
+PYTHIA_CHECKPOINTS = (
+    [0, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512]
+    + list(range(1000, 143000+1, 1000))
+)
+# Pythia V1 has log-spaced early checkpoints (see line above), but V0 doesn't
+PYTHIA_V0_CHECKPOINTS = list(range(1000, 143000+1, 1000))
 
 
 def get_checkpoint_labels(model_name: str):
     """Returns the checkpoint labels for a given model, and the label_type
     (step or token). Raises an error for models that are not checkpointed."""
     official_model_name = get_official_model_name(model_name)
     if official_model_name.startswith("stanford-crfm/"):
         return STANFORD_CRFM_CHECKPOINTS, "step"
     elif official_model_name.startswith("EleutherAI/pythia"):
-        return PYTHIA_CHECKPOINTS, "step"
+        if "v0" in official_model_name:
+            return PYTHIA_V0_CHECKPOINTS, "step"
+        else:
+            logging.warning("Pythia models on HF were updated on 4/3/23! add '-v0' to model name to access the old models.")
+            return PYTHIA_CHECKPOINTS, "step"
     elif official_model_name.startswith("NeelNanda/"):
         api = HfApi()
         files_list = api.list_repo_files(official_model_name)
         labels = []
         for file_name in files_list:
             match = re.match(r"checkpoints/.*_(\d*)\.pth", file_name)
             if match:
@@ -605,15 +800,15 @@
     have the HookedTransformer parameter names and shapes. Supports checkpointed
     models (and expects the checkpoint info to be stored in the config object)
 
     hf_model: Optionally, a HuggingFace model object. If provided, we will use
     these weights rather than reloading the model.
     """
     official_model_name = get_official_model_name(official_model_name)
-    if official_model_name.startswith("NeelNanda"):
+    if official_model_name.startswith("NeelNanda") or official_model_name.startswith("ArthurConmy"):
         api = HfApi()
         repo_files = api.list_repo_files(official_model_name)
         if cfg.from_checkpoint:
             file_name = list(
                 filter(lambda x: x.endswith(f"{cfg.checkpoint_value}.pth"), repo_files)
             )[0]
         else:
@@ -631,27 +826,32 @@
             elif official_model_name.startswith("EleutherAI/pythia"):
                 hf_model = AutoModelForCausalLM.from_pretrained(
                     official_model_name, revision=f"step{cfg.checkpoint_value}"
                 )
             else:
                 raise ValueError(f"Checkpoints for model {official_model_name} are not supported")
         elif hf_model is None:
-            hf_model = AutoModelForCausalLM.from_pretrained(official_model_name)
+            if "llama" in official_model_name:
+                raise NotImplementedError("Must pass in hf_model for LLaMA models")
+            else: 
+                hf_model = AutoModelForCausalLM.from_pretrained(official_model_name)
 
             # Load model weights, and fold in layer norm weights
         if cfg.original_architecture == "GPT2LMHeadModel":
             state_dict = convert_gpt2_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTNeoForCausalLM":
             state_dict = convert_neo_weights(hf_model, cfg)
         elif cfg.original_architecture == "OPTForCausalLM":
             state_dict = convert_opt_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTJForCausalLM":
             state_dict = convert_gptj_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTNeoXForCausalLM":
             state_dict = convert_neox_weights(hf_model, cfg)
+        elif cfg.original_architecture == "LLaMAForCausalLM": 
+            state_dict = convert_llama_weights(hf_model, cfg)
         else:
             raise ValueError(
                 f"Loading weights from the architecture is not currently supported: {cfg.original_architecture}, generated from model name {cfg.model_name}. Feel free to open an issue on GitHub to request this feature."
             )
 
         return state_dict
 
@@ -897,14 +1097,61 @@
     state_dict["ln_final.w"] = neox.gpt_neox.final_layer_norm.weight
     state_dict["ln_final.b"] = neox.gpt_neox.final_layer_norm.bias
 
     state_dict["unembed.W_U"] = neox.embed_out.weight.T
     state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
     return state_dict
 
+def convert_llama_weights(llama, cfg: HookedTransformerConfig): 
+    state_dict = {}
+
+    state_dict["embed.W_E"] = llama.model.embed_tokens.weight
+
+    # llama has no biases anywhere and deals with everything else roughly like
+    # GPTNeoX with different names
+    
+    for l in range(cfg.n_layers):
+
+        state_dict[f"blocks.{l}.ln1.w"] = llama.model.layers[l].input_layernorm.weight
+
+        W_Q = llama.model.layers[l].self_attn.q_proj.weight
+        W_K = llama.model.layers[l].self_attn.k_proj.weight
+        W_V = llama.model.layers[l].self_attn.v_proj.weight
+        W_Q = einops.rearrange(W_Q, "(n h) m->n m h", n=cfg.n_heads)
+        W_K = einops.rearrange(W_K, "(n h) m->n m h", n=cfg.n_heads)
+        W_V = einops.rearrange(W_V, "(n h) m->n m h", n=cfg.n_heads)
+        state_dict[f"blocks.{l}.attn.W_Q"] = W_Q
+        state_dict[f"blocks.{l}.attn.W_K"] = W_K
+        state_dict[f"blocks.{l}.attn.W_V"] = W_V
+
+        state_dict[f"blocks.{l}.attn.b_Q"] = torch.zeros(cfg.n_heads, cfg.d_head)
+        state_dict[f"blocks.{l}.attn.b_K"] = torch.zeros(cfg.n_heads, cfg.d_head)
+        state_dict[f"blocks.{l}.attn.b_V"] = torch.zeros(cfg.n_heads, cfg.d_head)
+
+        W_O = llama.model.layers[l].self_attn.o_proj.weight
+        W_O = einops.rearrange(W_O, "m (n h)->n h m", n=cfg.n_heads)
+        state_dict[f"blocks.{l}.attn.W_O"] = W_O
+
+        state_dict[f"blocks.{l}.attn.b_O"] = torch.zeros(cfg.d_model)
+
+        state_dict[f"blocks.{l}.ln2.w"] = llama.model.layers[l].post_attention_layernorm.weight
+
+        state_dict[f"blocks.{l}.mlp.W_in"] = llama.model.layers[l].mlp.up_proj.weight.T
+        state_dict[f"blocks.{l}.mlp.W_gate"] = llama.model.layers[l].mlp.gate_proj.weight.T
+        state_dict[f"blocks.{l}.mlp.b_in"] = torch.zeros(cfg.d_mlp)
+
+        state_dict[f"blocks.{l}.mlp.W_out"] = llama.model.layers[l].mlp.down_proj.weight.T
+        state_dict[f"blocks.{l}.mlp.b_out"] = torch.zeros(cfg.d_model)
+    
+    state_dict["ln_final.w"] = llama.model.norm.weight
+
+    state_dict["unembed.W_U"] = llama.lm_head.weight.T
+    state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
+
+    return state_dict
 
 def convert_opt_weights(opt, cfg: HookedTransformerConfig):
     state_dict = {}
 
     state_dict["embed.W_E"] = opt.model.decoder.embed_tokens.weight
     state_dict["pos_embed.W_pos"] = opt.model.decoder.embed_positions.weight[2:, :]
 
@@ -1023,7 +1270,9 @@
     if reverse_pos:
         new_state_dict["pos_embed.W_pos"] = new_state_dict["pos_embed.W_pos"].T
     if reverse_weights:
         for k, v in new_state_dict.items():
             if "W_" in k and "W_pos" not in k:
                 new_state_dict[k] = v.transpose(-2, -1)
     return new_state_dict
+
+# %%
```

### Comparing `transformer_lens-1.2.1/transformer_lens/make_docs.py` & `transformer_lens-1.2.2/transformer_lens/make_docs.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.2.1/transformer_lens/model_properties_table.md` & `transformer_lens-1.2.2/transformer_lens/model_properties_table.md`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.2.1/transformer_lens/past_key_value_caching.py` & `transformer_lens-1.2.2/transformer_lens/past_key_value_caching.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
-import torch.nn as nn
 from dataclasses import dataclass
-from typing import Union, Tuple, List, Dict, Any, Optional
+from typing import List
 from transformer_lens.HookedTransformerConfig import HookedTransformerConfig
-from jaxtyping import Float 
+from transformer_lens.utilities.devices import get_device_for_block_index
+from jaxtyping import Float
 
 
 @dataclass
 class HookedTransformerKeyValueCacheEntry:
     past_keys: Float[torch.Tensor, "batch pos_so_far n_heads d_head"]
     past_values: Float[torch.Tensor, "batch pos_so_far n_heads d_head"]
 
@@ -28,19 +28,19 @@
         )
 
     def append(
         self,
         new_keys: Float[torch.Tensor, "batch new_tokens n_heads d_head"],
         new_values: Float[torch.Tensor, "batch new_tokens n_heads d_head"],
     ):
-        updated_keys: Float[torch.Tensor, 
-            "batch pos_so_far_plus_new_tokens n_heads d_head"
+        updated_keys: Float[
+            torch.Tensor, "batch pos_so_far_plus_new_tokens n_heads d_head"
         ] = torch.cat([self.past_keys, new_keys], dim=1)
-        updated_values: Float[torch.Tensor,
-            "batch pos_so_far_plus_new_tokens n_heads d_head"
+        updated_values: Float[
+            torch.Tensor, "batch pos_so_far_plus_new_tokens n_heads d_head"
         ] = torch.cat([self.past_values, new_values], dim=1)
         self.past_keys = updated_keys
         self.past_values = updated_values
         return updated_keys, updated_values
 
 
 @dataclass
@@ -59,15 +59,17 @@
     @classmethod
     def init_cache(
         cls, cfg: HookedTransformerConfig, device: torch.device, batch_size: int = 1
     ):
         return cls(
             entries=[
                 HookedTransformerKeyValueCacheEntry.init_cache_entry(
-                    cfg, device, batch_size
+                    cfg,
+                    get_device_for_block_index(i, cfg, device),
+                    batch_size,
                 )
-                for _ in range(cfg.n_layers)
+                for i in range(cfg.n_layers)
             ]
         )
 
     def __getitem__(self, idx):
         return self.entries[idx]
```

### Comparing `transformer_lens-1.2.1/transformer_lens/train.py` & `transformer_lens-1.2.2/transformer_lens/train.py`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.2.1/transformer_lens/utils.py` & `transformer_lens-1.2.2/transformer_lens/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -379,16 +379,16 @@
         elif input_slice is None:
             self.slice = slice(None)
             self.mode = "identity"
         else:
             raise ValueError(f"Invalid input_slice {input_slice}")
 
     def apply(
-        self, 
-        tensor: torch.Tensor, 
+        self,
+        tensor: torch.Tensor,
         dim: int = 0,
         ) -> torch.Tensor:
         """
         Takes in a tensor and a slice, and applies the slice to the given dimension (supports positive and negative dimension syntax). Returns the sliced tensor.
 
         Args:
             tensor (torch.Tensor): The tensor to slice.
@@ -399,15 +399,15 @@
         """
         ndim = tensor.ndim
         slices = [slice(None)] * ndim
         slices[dim] = self.slice
         return tensor[tuple(slices)]
 
     def indices(
-        self, 
+        self,
         max_ctx: Optional[int] = None,
         ) -> Union[np.ndarray, np.int64]:
         """
         Returns the indices when this slice is applied to an axis of size max_ctx. Returns them as a numpy array, for integer slicing it is eg array([4])
 
         Args:
             max_ctx (int, optional): The size of the axis to slice. Only used if the slice is not an integer.
@@ -435,17 +435,38 @@
 
 def get_act_name(
     name: str,
     layer: Optional[int] = None,
     layer_type: Optional[str] = None,
 ):
     """
-    Helper function to convert shorthand to an activation name. Pretty hacky, intended to be useful for short feedback loop hacking stuff together, more so than writing good, readable code. But it is deterministic!
+    Helper function to convert shorthand to an activation name. Pretty hacky, intended to be useful for short feedback
+    loop hacking stuff together, more so than writing good, readable code. But it is deterministic!
+
+    Returns a name corresponding to an activation point in a TransformerLens model.
+
+    Args:
+         name (str): Takes in the name of the activation. This can be used to specify any activation name by itself.
+         The code assumes the first sequence of digits passed to it (if any) is the layer number, and anything after
+         that is the layer type.
+
+         Given only a word and number, it leaves layer_type as is.
+         Given only a word, it leaves layer and layer_type as is.
+
+         Examples:
+             get_act_name('embed') = get_act_name('embed', None, None)
+             get_act_name('k6') = get_act_name('k', 6, None)
+             get_act_name('scale4ln1') = get_act_name('scale', 4, 'ln1')
+
+         layer (int, optional): Takes in the layer number. Used for activations that appear in every block.
+
+         layer_type (string, optional): Used to distinguish between activations that appear multiple times in one block.
+
+    Full Examples:
 
-    eg:
     get_act_name('k', 6, 'a')=='blocks.6.attn.hook_k'
     get_act_name('pre', 2)=='blocks.2.mlp.hook_pre'
     get_act_name('embed')=='hook_embed'
     get_act_name('normalized', 27, 'ln2')=='blocks.27.ln2.hook_normalized'
     get_act_name('k6')=='blocks.6.attn.hook_k'
     get_act_name('scale4ln1')=='blocks.4.ln1.hook_scale'
     get_act_name('pre5')=='blocks.5.mlp.hook_pre'
@@ -477,14 +498,16 @@
         "query":"q",
         "value":"v",
         "mlp_pre":"pre",
         "mlp_mid":"mid",
         "mlp_post":"post",
     }
 
+    layer_norm_names = ["scale", "normalized"]
+
     if name in act_name_alias:
         name = act_name_alias[name]
 
     full_act_name = ""
     if layer is not None:
         full_act_name += f"blocks.{layer}."
     if name in ["k", "v", "q", "z", "rot_k", "rot_q", "result", "pattern", "attn_scores"]:
@@ -493,14 +516,17 @@
         layer_type = "mlp"
     elif layer_type in layer_type_alias:
         layer_type = layer_type_alias[layer_type]
 
     if layer_type:
         full_act_name += f"{layer_type}."
     full_act_name += f"hook_{name}"
+
+    if name in layer_norm_names and layer is None:
+        full_act_name = f"ln_final.{full_act_name}"
     return full_act_name
 
 
 def remove_batch_dim(tensor: Float[torch.Tensor, "1 ..."]) -> Float[torch.Tensor, "..."]:
     """
     Removes the first dimension of a tensor if it is size 1, otherwise returns the tensor unchanged
     """
```

### Comparing `transformer_lens-1.2.1/PKG-INFO` & `transformer_lens-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,81 @@
 Metadata-Version: 2.1
 Name: transformer-lens
-Version: 1.2.1
+Version: 1.2.2
 Summary: An implementation of transformers tailored for mechanistic interpretability.
 License: MIT
 Author: Neel Nanda
 Author-email: 77788841+neelnanda-io@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: datasets (>=2.7.1,<3.0.0)
-Requires-Dist: einops (>=0.6.0,<0.7.0)
-Requires-Dist: fancy-einsum (>=0.0.3,<0.0.4)
-Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
-Requires-Dist: jaxtyping (>=0.2.11,<0.3.0)
-Requires-Dist: myst-parser (>=0.18.1,<0.19.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
-Requires-Dist: numpy (>=1.21,<2.0) ; python_version < "3.10"
-Requires-Dist: numpy (>=1.23,<2.0) ; python_version >= "3.10"
-Requires-Dist: pandas (>=1.1.5,<2.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: datasets (>=2.7.1)
+Requires-Dist: einops (>=0.6.0)
+Requires-Dist: fancy-einsum (>=0.0.3)
+Requires-Dist: furo (>=2022.12.7) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
+Requires-Dist: jaxtyping (>=0.2.11)
+Requires-Dist: myst-parser (>=0.18.1) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
+Requires-Dist: numpy (>=1.21) ; python_version < "3.10"
+Requires-Dist: numpy (>=1.23) ; python_version >= "3.10"
+Requires-Dist: pandas (>=1.1.5)
+Requires-Dist: rich (>=12.6.0)
 Requires-Dist: sphinx (==5.2.3) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
-Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
-Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
-Requires-Dist: torch (>=1.10,<2.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: transformers (>=4.25.1,<5.0.0)
-Requires-Dist: wandb (>=0.13.5,<0.14.0)
+Requires-Dist: sphinx-autobuild (>=2021.3.14) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
+Requires-Dist: sphinxcontrib-napoleon (>=0.7) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
+Requires-Dist: tabulate (>=0.9.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
+Requires-Dist: torch (>=1.10)
+Requires-Dist: tqdm (>=4.64.1)
+Requires-Dist: transformers (>=4.25.1)
+Requires-Dist: wandb (>=0.13.5)
 Description-Content-Type: text/markdown
 
 # TransformerLens
 
 [![Pypi](https://img.shields.io/pypi/v/transformer-lens)](https://pypi.org/project/transformer-lens/)
 
 (Formerly known as EasyTransformer)
 
 ## [Read the Docs Here](https://neelnanda-io.github.io/TransformerLens/)
 
 ## [Main Tutorial Here](https://neelnanda.io/transformer-lens-demo)
 
+See also this better and more in-depth, but still [work-in-progress tutorial from Callum McDougall](https://transformerlens-intro.streamlit.app/)
+
 ## A Library for Mechanistic Interpretability of Generative Language Models
 
-This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this! 
+This is a library for doing [mechanistic interpretability](https://distill.pub/2020/circuits/zoom-in/) of GPT-2 Style language models. The goal of mechanistic interpretability is to take a trained model and reverse engineer the algorithms the model learned during training from its weights. It is a fact about the world today that we have computer programs that can essentially speak English at a human level (GPT-3, PaLM, etc), yet we have no idea how they work nor how to write one ourselves. This offends me greatly, and I would like to solve this!
 
-TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make *my* experience of doing research easier and more fun, hopefully this transfers to you!
+TransformerLens lets you load in an open source language model, like GPT-2, and exposes the internal activations of the model to you. You can cache any internal activation in the model, and add in functions to edit, remove or replace these activations as the model runs. The core design principle I've followed is to enable exploratory analysis. One of the most fun parts of mechanistic interpretability compared to normal ML is the extremely short feedback loops! The point of this library is to keep the gap between having an experiment idea and seeing the results as small as possible, to make it easy for **research to feel like play** and to enter a flow state. Part of what I aimed for is to make _my_ experience of doing research easier and more fun, hopefully this transfers to you!
 
-I used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to *use* or *train* models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook! 
+I used to work for the [Anthropic interpretability team](transformer-circuits.pub), and I wrote this library because after I left and tried doing independent research, I got extremely frustrated by the state of open source tooling. There's a lot of excellent infrastructure like HuggingFace and DeepSpeed to _use_ or _train_ models, but very little to dig into their internals and reverse engineer how they work. **This library tries to solve that**, and to make it easy to get into the field even if you don't work at an industry org with real infrastructure! One of the great things about mechanistic interpretability is that you don't need large models or tons of compute. There are lots of important open problems that can be solved with a small model in a Colab notebook!
 
 The core features were heavily inspired by the interface to [Anthropic's excellent Garcon tool](https://transformer-circuits.pub/2021/garcon/index.html). Credit to Nelson Elhage and Chris Olah for building Garcon and showing me the value of good infrastructure for enabling exploratory research!
 
 ## Getting Started
 
 **Start with the [main demo](https://neelnanda.io/transformer-lens-demo) to learn how the library works, and the basic features**.
 
-To see what using it for exploratory analysis in practice looks like, check out [my notebook analysing Indirect Objection Identification](https://neelnanda.io/exploratory-analysis-demo) or [my recording of myself doing research](https://www.youtube.com/watch?v=yo4QvDn-vsU)! 
+To see what using it for exploratory analysis in practice looks like, check out [my notebook analysing Indirect Objection Identification](https://neelnanda.io/exploratory-analysis-demo) or [my recording of myself doing research](https://www.youtube.com/watch?v=yo4QvDn-vsU)!
 
-Mechanistic interpretability is a very young and small field, and there are a *lot* of open problems - if you would like to help, please try working on one! **Check out my [list of concrete open problems](https://docs.google.com/document/d/1WONBzNqfKIxERejrrPlQMyKqg7jSFW92x5UMXNrMdPo/edit) to figure out where to start.**. It begins with advice on skilling up, and key resources to check out. 
+Mechanistic interpretability is a very young and small field, and there are a _lot_ of open problems - if you would like to help, please try working on one! **Check out my [list of concrete open problems](https://docs.google.com/document/d/1WONBzNqfKIxERejrrPlQMyKqg7jSFW92x5UMXNrMdPo/edit) to figure out where to start.**. It begins with advice on skilling up, and key resources to check out.
 
 If you're new to transformers, check out my [what is a transformer tutorial](https://neelnanda.io/transformer-tutorial) and [tutorial on coding GPT-2 from scratch](https://neelnanda.io/transformer-tutorial-2) (with [an accompanying template](https://neelnanda.io/transformer-template) to write one yourself!
 
 ## Gallery
 
 User contributed examples of the library being used in action:
-* [Induction Heads Phase Change Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb): A partial replication of [In-Context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) from Connor Kissane
-* [Decision Transformer Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of scripts for training decision transformers which uses transformer lens to view intermediate activations, perform attribution and ablations. A write up of the initial work can be found [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
+
+- [Induction Heads Phase Change Replication](https://colab.research.google.com/github/ckkissane/induction-heads-transformer-lens/blob/main/Induction_Heads_Phase_Change.ipynb): A partial replication of [In-Context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) from Connor Kissane
+- [Decision Transformer Interpretability](https://github.com/jbloomAus/DecisionTransformerInterpretability): A set of scripts for training decision transformers which uses transformer lens to view intermediate activations, perform attribution and ablations. A write up of the initial work can be found [here](https://www.lesswrong.com/posts/bBuBDJBYHt39Q5zZy/decision-transformer-interpretability).
 
 ## Advice for Reading the Code
 
 One significant design decision made was to have a single transformer implementation that could support a range of subtly different GPT-style models. This has the upside of interpretability code just working for arbitrary models when you change the model name in `HookedTransformer.from_pretrained`! But it has the significant downside that the code implementing the model (in `HookedTransformer.py` and `components.py`) can be difficult to read. I recommend starting with my [Clean Transformer Demo](https://neelnanda.io/transformer-solution), which is a clean, minimal implementation of GPT-2 with the same internal architecture and activation names as HookedTransformer, but is significantly clearer and better documented.
 
 ## Installation
 
@@ -101,27 +104,33 @@
 
 Then the library can be imported as `import transformer_lens`.
 
 ### Testing
 
 If adding a feature, please add unit tests for it to the tests folder, and check that it hasn't broken anything major using the existing tests (install pytest and run it in the root TransformerLens/ directory).
 
-To run tests, you can use the following command:
+#### Running the tests
 
-```
-poetry run pytest -v tests
-```
+- All tests via `make test`
+- Unit tests only via `make unit-test`
+- Acceptance tests only via `make acceptance-test`
+
+### Demos
+
+If adding a feature, please add it to the demo notebook in the `demos` folder, and check that it works in the demo format. This can be tested by replacing `pip install git+https://github.com/JayBaileyCS/TransformerLens.git` with `pip install git+https://github.com/<YOUR_USERNAME_HERE>/TransformerLens.git` in the demo notebook, and running it in a fresh environment.
 
 ## Citation
 
 Please cite this library as:
+
 ```
 @misc{nandatransformerlens2022,
     title  = {TransformerLens},
     author = {Nanda, Neel},
     url    = {https://github.com/neelnanda-io/TransformerLens},
     year   = {2022}
 }
 ```
+
 (This is my best guess for how citing software works, feel free to send a correction!)
 Also, if you're actually using this for your research, I'd love to chat! Reach out at neelnanda27@gmail.com
```

