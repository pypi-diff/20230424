# Comparing `tmp/ex2mcmc-0.0.1.tar.gz` & `tmp/ex2mcmc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex2mcmc-0.0.1.tar", max compression
+gzip compressed data, was "ex2mcmc-0.0.3.tar", max compression
```

## Comparing `ex2mcmc-0.0.1.tar` & `ex2mcmc-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1068 2023-04-15 22:59:22.645505 ex2mcmc-0.0.1/LICENSE
--rw-r--r--   0        0        0     9348 2023-04-24 15:06:19.518225 ex2mcmc-0.0.1/README.md
--rw-r--r--   0        0        0       41 2023-04-14 14:56:29.127772 ex2mcmc-0.0.1/ex2mcmc/__init__.py
--rw-r--r--   0        0        0     3911 2023-04-14 08:56:49.769688 ex2mcmc-0.0.1/ex2mcmc/gan_distribution.py
--rw-r--r--   0        0        0       32 2023-04-24 15:06:19.531639 ex2mcmc-0.0.1/ex2mcmc/models/__init__.py
--rw-r--r--   0        0        0     2918 2023-04-14 09:14:56.940885 ex2mcmc-0.0.1/ex2mcmc/models/base.py
--rw-r--r--   0        0        0     2335 2023-04-24 15:06:19.532511 ex2mcmc-0.0.1/ex2mcmc/models/mmc.py
--rw-r--r--   0        0        0    10388 2023-04-24 15:06:19.533100 ex2mcmc-0.0.1/ex2mcmc/models/rnvp.py
--rw-r--r--   0        0        0     3728 2023-04-24 15:06:19.533908 ex2mcmc-0.0.1/ex2mcmc/models/rnvp_minimal.py
--rw-r--r--   0        0        0     5903 2023-04-24 15:06:19.534352 ex2mcmc-0.0.1/ex2mcmc/models/utils.py
--rw-r--r--   0        0        0     7780 2023-04-24 15:06:19.534767 ex2mcmc-0.0.1/ex2mcmc/old_samplers.py
--rw-r--r--   0        0        0     2723 2023-04-24 15:06:19.535110 ex2mcmc-0.0.1/ex2mcmc/pyro_samplers.py
--rw-r--r--   0        0        0     3837 2023-04-24 15:06:19.535424 ex2mcmc-0.0.1/ex2mcmc/sample.py
--rw-r--r--   0        0        0    18963 2023-04-24 15:06:19.535943 ex2mcmc-0.0.1/ex2mcmc/samplers.py
--rw-r--r--   0        0        0        0 2023-04-15 22:51:42.153665 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/__init__.py
--rw-r--r--   0        0        0    18662 2023-04-24 15:06:19.536503 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/adaptive_mc.py
--rw-r--r--   0        0        0     2475 2023-04-24 15:06:19.537089 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/adaptive_sir_loss.py
--rw-r--r--   0        0        0    23140 2023-04-24 15:06:19.538059 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/distributions.py
--rw-r--r--   0        0        0    59102 2023-04-24 15:06:19.539182 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/ebm_sampling.py
--rw-r--r--   0        0        0     1496 2023-04-24 15:06:19.539797 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/linear_regression.py
--rw-r--r--   0        0        0     6894 2023-04-24 15:06:19.540513 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/logistic_regression.py
--rw-r--r--   0        0        0     1838 2023-04-11 14:42:13.948565 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/mcmc_base.py
--rw-r--r--   0        0        0     8786 2023-04-15 22:50:04.145306 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/metrics.py
--rw-r--r--   0        0        0     3255 2023-04-15 23:02:17.635963 ex2mcmc-0.0.1/ex2mcmc/sampling_utils/total_variation.py
--rw-r--r--   0        0        0      117 2023-04-24 15:06:19.541059 ex2mcmc-0.0.1/ex2mcmc/utils/__init__.py
--rw-r--r--   0        0        0    11385 2023-04-14 14:56:32.377226 ex2mcmc-0.0.1/ex2mcmc/utils/callbacks.py
--rw-r--r--   0        0        0     2716 2023-04-24 15:06:19.541583 ex2mcmc-0.0.1/ex2mcmc/utils/general_utils.py
--rw-r--r--   0        0        0    15499 2023-04-14 14:56:29.744336 ex2mcmc-0.0.1/ex2mcmc/utils/metrics/compute_fid_tf.py
--rw-r--r--   0        0        0     7378 2023-04-14 14:56:29.733785 ex2mcmc-0.0.1/ex2mcmc/utils/metrics/inception_score.py
--rw-r--r--   0        0        0     3264 2023-04-24 15:06:19.669613 ex2mcmc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    10835 1970-01-01 00:00:00.000000 ex2mcmc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-15 22:59:22.645505 ex2mcmc-0.0.3/LICENSE
+-rw-r--r--   0        0        0     8956 2023-04-19 12:17:11.760477 ex2mcmc-0.0.3/README.md
+-rw-r--r--   0        0        0       41 2023-04-14 14:56:29.127772 ex2mcmc-0.0.3/ex2mcmc/__init__.py
+-rw-r--r--   0        0        0     3911 2023-04-14 08:56:49.769688 ex2mcmc-0.0.3/ex2mcmc/gan_distribution.py
+-rw-r--r--   0        0        0       84 2023-04-15 19:34:13.069624 ex2mcmc-0.0.3/ex2mcmc/models/__init__.py
+-rw-r--r--   0        0        0     2918 2023-04-14 09:14:56.940885 ex2mcmc-0.0.3/ex2mcmc/models/base.py
+-rw-r--r--   0        0        0     2335 2023-04-20 11:10:21.677698 ex2mcmc-0.0.3/ex2mcmc/models/mmc.py
+-rw-r--r--   0        0        0    10388 2023-04-20 12:49:47.363817 ex2mcmc-0.0.3/ex2mcmc/models/rnvp.py
+-rw-r--r--   0        0        0     3728 2023-04-20 12:54:19.247618 ex2mcmc-0.0.3/ex2mcmc/models/rnvp_minimal.py
+-rw-r--r--   0        0        0     5903 2023-04-20 11:10:24.692466 ex2mcmc-0.0.3/ex2mcmc/models/utils.py
+-rw-r--r--   0        0        0     7807 2023-04-20 11:10:24.648171 ex2mcmc-0.0.3/ex2mcmc/old_samplers.py
+-rw-r--r--   0        0        0     2723 2023-04-20 13:09:54.527679 ex2mcmc-0.0.3/ex2mcmc/pyro_samplers.py
+-rw-r--r--   0        0        0     4002 2023-04-20 12:54:21.386394 ex2mcmc-0.0.3/ex2mcmc/sample.py
+-rw-r--r--   0        0        0    18350 2023-04-20 12:54:19.401520 ex2mcmc-0.0.3/ex2mcmc/samplers.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:51:42.153665 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/__init__.py
+-rw-r--r--   0        0        0    18665 2023-04-20 13:06:56.089591 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/adaptive_mc.py
+-rw-r--r--   0        0        0     2475 2023-04-20 11:10:21.723615 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/adaptive_sir_loss.py
+-rw-r--r--   0        0        0    23140 2023-04-20 11:10:22.137375 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/distributions.py
+-rw-r--r--   0        0        0    59102 2023-04-19 12:33:25.167366 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/ebm_sampling.py
+-rw-r--r--   0        0        0     1496 2023-04-20 11:10:24.751393 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/linear_regression.py
+-rw-r--r--   0        0        0     6894 2023-04-20 11:10:24.723745 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/logistic_regression.py
+-rw-r--r--   0        0        0     1838 2023-04-11 14:42:13.948565 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/mcmc_base.py
+-rw-r--r--   0        0        0     8786 2023-04-15 22:50:04.145306 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/metrics.py
+-rw-r--r--   0        0        0     3255 2023-04-15 23:02:17.635963 ex2mcmc-0.0.3/ex2mcmc/sampling_utils/total_variation.py
+-rw-r--r--   0        0        0      117 2023-04-20 11:10:24.656035 ex2mcmc-0.0.3/ex2mcmc/utils/__init__.py
+-rw-r--r--   0        0        0    11385 2023-04-14 14:56:32.377226 ex2mcmc-0.0.3/ex2mcmc/utils/callbacks.py
+-rw-r--r--   0        0        0     2716 2023-04-20 11:10:21.900193 ex2mcmc-0.0.3/ex2mcmc/utils/general_utils.py
+-rw-r--r--   0        0        0    15499 2023-04-14 14:56:29.744336 ex2mcmc-0.0.3/ex2mcmc/utils/metrics/compute_fid_tf.py
+-rw-r--r--   0        0        0     7378 2023-04-14 14:56:29.733785 ex2mcmc-0.0.3/ex2mcmc/utils/metrics/inception_score.py
+-rw-r--r--   0        0        0     3428 2023-04-20 14:31:41.423736 ex2mcmc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10515 1970-01-01 00:00:00.000000 ex2mcmc-0.0.3/PKG-INFO
```

### Comparing `ex2mcmc-0.0.1/LICENSE` & `ex2mcmc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/README.md` & `ex2mcmc-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 
 - [Ex2MCMC: Local-Global MCMC kernels: the bost of both worlds (NeurIPS 2022) \[Paper\]](#ex2mcmc-local-global-mcmc-kernels-the-bost-of-both-worlds-neurips-2022-paper)
   - [Single chain mixing](#single-chain-mixing)
   - [Sampling from GAN as Energy-Based Models with MCMC](#sampling-from-gan-as-energy-based-models-with-mcmc)
   - [Algorithms](#algorithms)
   - [Installation](#installation)
-    - [Developement installation](#developement-installation)
-    - [Download checkpoints and stats](#download-checkpoints-and-stats)
   - [Usage](#usage)
     - [Demonstration on SNGAN](#demonstration-on-sngan)
     - [Experiments with synthetic distributions:](#experiments-with-synthetic-distributions)
     - [Experiments with GANs on MNIST dataset](#experiments-with-gans-on-mnist-dataset)
     - [Experiments with GANs on CIFAR10 dataset](#experiments-with-gans-on-cifar10-dataset)
     - [Sampling and FID computation](#sampling-and-fid-computation)
   - [Results](#results)
@@ -57,43 +55,35 @@
 Create environment:
 
 ```bash
 conda create -n ex2mcmc python=3.8
 conda activate ex2mcmc
 ```
 
-```bash
-pip install ex2mcmc==0.0.1
-pip install git+https://github.com/kwotsin/mimicry.git
-```
-
-### Developement installation
-
 Install poetry (if absent):
 ```bash
 curl -sSL https://install.python-poetry.org | python3 -
 poetry config virtualenvs.create false
 ```
 
 Install the project:
 ```bash
 poetry install
-poetry add git+https://github.com/kwotsin/mimicry.git@a7fda06c4aff1e6af8dc4c4a35ed6636e434c766
 ```
 
-### Download checkpoints and stats
+Download checkpoints:
 
-CIFAR10 checkpoints:
+CIFAR10:
 
 | GAN   |     Steps     |  Path, G |  Path, D |
 |:----------|:-------------:|:------:|:------:|
 | DCGAN NS  | 100k      |   [netG_100000_steps.pth](https://drive.google.com/file/d/1gv8_qr_xa8hJzdJpBXiKr8v922EqcE-E/view?usp=share_link) |   [netD_100000_steps.pth](https://drive.google.com/file/d/1u1sPUmlvyhcbNDX2DVsR-mGOzqQ6U8sh/view?usp=share_link) |
 | SNGAN, Hinge  | 100k      |   [netG.pth](https://drive.google.com/file/d/118zC_iEkN27jGLVNmDuQpMeyw7BKOUra/view?usp=share_link) |   [netD.pth](https://drive.google.com/file/d/1xU5FV59TLhAlkFubJGmJVS87HnZZ2xHT/view?usp=share_link) |
 
-MNIST checkpoints:
+MNIST:
 
 | GAN      |  Path |
 |:----------|:-------------:|
 | Vanilla  |   [vanilla_gan.pth](https://drive.google.com/file/d/1xa1v4hPQQdU2RkhjMn5sFZCITxTJ5Dhj/view?usp=share_link) |
 | WGAN CP  |   [wgan.pth](https://drive.google.com/file/d/17nQJnfs2_T6kyahnkW3fu8AVY54kmRmw/view?usp=share_link) |
 
 You also can run script to download checkpoints:
```

### Comparing `ex2mcmc-0.0.1/ex2mcmc/gan_distribution.py` & `ex2mcmc-0.0.3/ex2mcmc/gan_distribution.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/models/base.py` & `ex2mcmc-0.0.3/ex2mcmc/models/base.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/models/mmc.py` & `ex2mcmc-0.0.3/ex2mcmc/models/mmc.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/models/rnvp.py` & `ex2mcmc-0.0.3/ex2mcmc/models/rnvp.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/models/rnvp_minimal.py` & `ex2mcmc-0.0.3/ex2mcmc/models/rnvp_minimal.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/models/utils.py` & `ex2mcmc-0.0.3/ex2mcmc/models/utils.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/old_samplers.py` & `ex2mcmc-0.0.3/ex2mcmc/old_samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import torch
 import tqdm
 from torch.distributions import Categorical
 from torch.distributions import MultivariateNormal as MNormal
 
 
+# MALA
 def grad_log_and_output_target_dens(log_target_dens, z):
     """
     returns the gradient of log-density
     """
     inp = z.clone().detach()
     inp.requires_grad_(True)
 
@@ -88,14 +89,15 @@
         samples_traj.append(x_cur)
 
     samples_traj = torch.stack(samples_traj).transpose(0, 1)
 
     return samples_traj
 
 
+# I-SIR
 def i_sir_step(log_target_dens, x_cur, N_part, isir_proposal, return_all_stats=False):
     """
     function to sample with N-particles version of i-SIR
     args:
         N_part - number of particles, integer;
         x0 - current i-sir particle;
     return:
@@ -182,15 +184,16 @@
         samples_traj.append(x_cur)
 
     samples_traj = torch.stack(samples_traj).transpose(0, 1)
 
     return samples_traj
 
 
-def ex2mcmc(
+# Ex2MCMC
+def ex2_mcmc(
     log_target_dens,
     x0,
     N_steps,
     N_part,
     isir_proposal,
     gamma,
     mala_iters,
@@ -210,15 +213,15 @@
         samples_traj.append(x_cur)
 
     samples_traj = torch.stack(samples_traj).transpose(0, 1)
 
     return samples_traj
 
 
-def flex2mcmc(
+def flex2_mcmc(
     log_target_dens,
     x0,
     N_steps,
     N_part,
     isir_proposal,
     gamma,
     mala_iters,
```

### Comparing `ex2mcmc-0.0.1/ex2mcmc/pyro_samplers.py` & `ex2mcmc-0.0.3/ex2mcmc/pyro_samplers.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sample.py` & `ex2mcmc-0.0.3/ex2mcmc/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,17 +60,19 @@
     def ref_dist(self) -> Distribution:
         return self._ref_dist
 
     def step(
         self,
         z: torch.Tensor,
         it: int = 1,
+        # data_batch: Optional[torch.FloatTensor] = None,
         meta: Optional[Dict] = None,
         keep_graph: bool = False,
     ) -> Tuple[torch.Tensor, Dict]:
+        # self._ref_dist.data_batch = data_batch
         pts, meta = self.mcmc(
             self.sampling,
             z,
             self.target,
             proposal=self.gen.proposal,
             # n_samples=self.n_sampling_steps,
             # burn_in=self.n_sampling_steps - 1,
@@ -87,14 +89,15 @@
         return pts[-1], meta
 
     @time_comp_cls
     def __call__(
         self,
         z: torch.Tensor,
         n_steps: Optional[int] = None,
+        # data_batch: Optional[torch.FloatTensor] = None,
         collect_imgs: bool = False,
         keep_graph: bool = False,
     ) -> Tuple[List, List, List, List]:
         n_steps = n_steps if n_steps is not None else self.n_steps
         collect_imgs = collect_imgs or self.collect_imgs
         keep_graph = keep_graph or self.keep_graph
         zs = [z.cpu()]
```

### Comparing `ex2mcmc-0.0.1/ex2mcmc/samplers.py` & `ex2mcmc-0.0.3/ex2mcmc/samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 @MCMCRegistry.register()
 def ula(
     start: torch.FloatTensor,
     target: Union[Distribution, torchDist],
     proposal: Union[Distribution, torchDist],
     n_samples: int,
     burn_in: int,
-    project: Callable = lambda x: x,
+    project: Callable,
     *,
     step_size: float,
     verbose: bool = False,
     meta: Optional[Dict] = None,
     keep_graph: bool = False,
     natural_grad: bool = False,  # True,
     tikhonov_reg: float = 0.1,
@@ -86,14 +86,15 @@
         else:
             step_size_ = step_size
 
         noise = torch.randn_like(point, dtype=torch.float).to(point.device)
         noise_scale = (2.0 * step_size_) ** 0.5
 
         point = point + step_size_ * grad + noise_scale * noise
+        # point = point / torch.clamp(torch.norm(point, dim=-1), min=1)[:, None] * point.shape[-1]**.5
         point = project(point)
 
         if not keep_graph:
             point = point.detach().requires_grad_()
         if step_id >= burn_in:
             chains.append(point.cpu().clone())
     chains = torch.stack(chains, 0)
@@ -135,15 +136,15 @@
 @torch.no_grad()
 def isir(
     start: torch.FloatTensor,
     target,
     proposal: Union[Distribution, torchDist],
     n_samples: int,
     burn_in: int,
-    project: Callable = lambda x: x,
+    project: Callable,
     *,
     n_particles: int,
     verbose: bool = False,
     meta: Optional[Dict] = None,
     **kwargs,
 ) -> Tuple[torch.FloatTensor, Dict]:
     """
@@ -212,15 +213,15 @@
 @MCMCRegistry.register()
 def mala(
     start: torch.FloatTensor,
     target: Union[Distribution, torchDist],
     proposal: Union[Distribution, torchDist],
     n_samples: int,
     burn_in: int,
-    project: Callable = lambda x: x,
+    project: Callable,
     *,
     step_size: float,
     verbose: bool = False,
     target_acceptance=None,
     meta: Optional[Dict] = None,
     keep_graph: bool = False,
 ) -> Tuple[torch.FloatTensor, Dict]:
@@ -332,43 +333,24 @@
 @MCMCRegistry.register()
 def ex2mcmc(
     start: torch.FloatTensor,
     target: Union[Distribution, torchDist],
     proposal: Union[Distribution, torchDist],
     n_samples: int,
     burn_in: int,
-    project: Callable = lambda x: x,
+    project: Callable,
     *,
     step_size: float,
     n_particles: int,
     n_mala_steps: int = 1,
     target_acceptance: float = False,
     verbose: bool = False,
     meta: Optional[Dict] = None,
     keep_graph: bool = False,
 ):
-    """
-    Ex2MCMC
-
-    Args:
-        start - strating points of shape [n_chains x dim]
-        target - target distribution instance with method "log_prob"
-        proposal - proposal distribution
-        n_samples - number of last samples from each chain to return
-        burn_in - number of first samples from each chain to throw away
-        step_size - step size for drift term
-        n_particles - number of particles including one from previous step
-        n_mala_steps - number of MALA steps after each SIR step
-        verbose - whether to show iterations' bar
-
-    Returns:
-        tensor of chains with shape [n_samples, n_chains, dim],
-          acceptance rates for each iteration
-    """
-
     chains = []
     point = start.clone()
     point.requires_grad_(True)
     point.grad = None
 
     meta = meta or dict()
     meta["sir_accept"] = meta.get("sir_accept", [])
@@ -423,21 +405,70 @@
             chains.append(point.cpu().clone())
 
     chains = torch.stack(chains, 0)
     return chains, meta
 
 
 @MCMCRegistry.register()
+def hmc(
+    start: torch.FloatTensor,
+    target: Union[Distribution, torchDist],
+    proposal: Union[Distribution, torchDist],
+    n_samples: int,
+    burn_in: int,
+    project: Callable,
+    *,
+    step_size: float,
+    leapfrog_steps: int = 1,
+    target_acceptance: float = False,
+    adapt_step_size: bool = False,
+    verbose: bool = False,
+    meta: Optional[Dict] = None,
+):
+    meta = meta or dict()
+    meta["step_size"] = meta.get("step_size", [])
+    if "hmc_kernel" not in meta:
+        kernel = HMC(
+            potential_fn=lambda x: -target.log_prob(x["points"]),
+            full_mass=False,
+            step_size=step_size,
+            num_steps=leapfrog_steps,
+            adapt_step_size=adapt_step_size,
+            target_accept_prob=target_acceptance,
+        )
+        meta["hmc_kernel"] = kernel
+
+    x = start.clone()
+    x.requires_grad_(False)
+    x.grad = None
+
+    init_params = {"points": x}
+    mcmc = MCMC(
+        kernel=meta["hmc_kernel"],
+        num_samples=n_samples,
+        initial_params=init_params,
+        warmup_steps=burn_in,
+    )
+    mcmc.run()
+    meta["step_size"].append(meta["hmc_kernel"].step_size)
+
+    chains = mcmc.get_samples(group_by_chain=True)["points"]
+    chains = chains.view(-1, *start.shape)
+
+    return chains, meta
+
+
+@MCMCRegistry.register()
 def flex2mcmc(
     start: torch.FloatTensor,
     target,
     proposal,
     n_samples: int,
     burn_in: int,
-    project: Callable = lambda x: x,
+    project: Callable,
     *,
     n_particles: int,
     step_size: float,
     n_mala_steps: int = 1,
     # add_pop_size_train: int = 200, #4096,
     forward_kl_weight: float = 1.0,
     backward_kl_weight: float = 1.0,
@@ -496,17 +527,17 @@
             # logq_x=logq_x,
         )
         logp_x = log_ps[np.arange(point.shape[0]), indices]
         logq_x = log_qs[np.arange(point.shape[0]), indices]
         meta["sir_accept"].append((indices != 0).float().mean().item())
         point = point.detach().requires_grad_()
         meta["logp"] = logp_x
-        meta["mask"] = (
-            F.one_hot(indices, num_classes=n_particles).to(bool).detach().cpu()
-        )
+        # meta["mask"] = (
+        #     F.one_hot(indices, num_classes=n_particles).to(bool).detach().cpu()
+        # )
         if n_mala_steps > 0:
             points, meta = mala(
                 point,
                 target,
                 proposal.prior,
                 n_mala_steps,
                 n_mala_steps - 1,
@@ -534,14 +565,15 @@
                 -(log_qs * torch.softmax(logw.detach(), dim=-1)).sum(axis=-1).mean()
             )
             # KL(Q | P), MC with current flow samples
             kl_back = -logw[:, 1:].mean()
 
             loss = forward_kl_weight * kl_forw + backward_kl_weight * kl_back
 
+            # loss -= log_qs[:, 1:].mean() / kl_back.detach().item()
             proposal.zero_grad()
             loss.backward()
             torch.nn.utils.clip_grad_norm_(proposal.parameters(), 1.0)
             proposal.optim.step()
             proposal.scheduler.step()
 
             meta["forward_kl"].append(kl_forw.item())
@@ -552,56 +584,7 @@
                     f"KL forw {kl_forw.item():.3f}, \
                      KL back {kl_back.item():.3f} "  # Hentr {entr.item():.3f}"
                 )
 
     chains = torch.stack(chains, 0)
 
     return chains, meta
-
-
-@MCMCRegistry.register()
-def hmc(
-    start: torch.FloatTensor,
-    target: Union[Distribution, torchDist],
-    proposal: Union[Distribution, torchDist],
-    n_samples: int,
-    burn_in: int,
-    project: Callable = lambda x: x,
-    *,
-    step_size: float,
-    leapfrog_steps: int = 1,
-    target_acceptance: float = False,
-    adapt_step_size: bool = False,
-    verbose: bool = False,
-    meta: Optional[Dict] = None,
-):
-    meta = meta or dict()
-    meta["step_size"] = meta.get("step_size", [])
-    if "hmc_kernel" not in meta:
-        kernel = HMC(
-            potential_fn=lambda x: -target.log_prob(x["points"]),
-            full_mass=False,
-            step_size=step_size,
-            num_steps=leapfrog_steps,
-            adapt_step_size=adapt_step_size,
-            target_accept_prob=target_acceptance,
-        )
-        meta["hmc_kernel"] = kernel
-
-    x = start.clone()
-    x.requires_grad_(False)
-    x.grad = None
-
-    init_params = {"points": x}
-    mcmc = MCMC(
-        kernel=meta["hmc_kernel"],
-        num_samples=n_samples,
-        initial_params=init_params,
-        warmup_steps=burn_in,
-    )
-    mcmc.run()
-    meta["step_size"].append(meta["hmc_kernel"].step_size)
-
-    chains = mcmc.get_samples(group_by_chain=True)["points"]
-    chains = chains.view(-1, *start.shape)
-
-    return chains, meta
```

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/adaptive_mc.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/adaptive_mc.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             corr_coef,
             bernoulli_prob_corr,
             flow,
             verbose,
         )
 
 
-def ex2mcmc_mala_new_proposal(
+def ex2_mcmc_mala_new_proposal(
     z,
     target,
     proposal,
     n_steps,
     N,
     grad_step,
     noise_scale,
@@ -359,15 +359,15 @@
 
     # z_sp.append(z_pushed.detach().cpu())
     acceptance /= n_steps
 
     return z_sp, acceptance, mala_transition.adapt_grad_step
 
 
-def ex2mcmc_mala(
+def ex2_mcmc_mala(
     z,
     target,
     proposal,
     n_steps,
     N,
     grad_step,
     noise_scale,
@@ -525,15 +525,15 @@
         # torch.cuda.empty_cache()
         n_steps = self_kwargs.pop("n_steps")
         if len(args) > 0:
             n_steps = args[0]
 
         self_kwargs.pop("_steps_done")
 
-        return ex2mcmc_mala(start, target, proposal, n_steps, **self_kwargs)
+        return ex2_mcmc_mala(start, target, proposal, n_steps, **self_kwargs)
 
 
 class FlowMCMC:
     def __init__(self, target, proposal, device, flow, mcmc_call: callable, **kwargs):
         self.flow = flow
         self.proposal = proposal
         self.target = target
```

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/adaptive_sir_loss.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/adaptive_sir_loss.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/distributions.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/distributions.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/ebm_sampling.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/ebm_sampling.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/linear_regression.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/linear_regression.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/logistic_regression.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/mcmc_base.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/mcmc_base.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/metrics.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/sampling_utils/total_variation.py` & `ex2mcmc-0.0.3/ex2mcmc/sampling_utils/total_variation.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/utils/callbacks.py` & `ex2mcmc-0.0.3/ex2mcmc/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/utils/general_utils.py` & `ex2mcmc-0.0.3/ex2mcmc/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/utils/metrics/compute_fid_tf.py` & `ex2mcmc-0.0.3/ex2mcmc/utils/metrics/compute_fid_tf.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/ex2mcmc/utils/metrics/inception_score.py` & `ex2mcmc-0.0.3/ex2mcmc/utils/metrics/inception_score.py`

 * *Files identical despite different names*

### Comparing `ex2mcmc-0.0.1/pyproject.toml` & `ex2mcmc-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "ex2mcmc"
-version = "0.0.1"
+version = "0.0.3"
 description = "Local-Global MCMC kernels: the bost of both worlds (NeurIPS 2022)"
 authors = [
-    "Sergey Samsonov <svsamsonov@hse.ru>", "Evgeny Lagutin <lagutin.em@phystech.edu>", 
-    "Marylou Gabrié", "Alain Durmus", "Alexey Naumov", "Eric Moulines"
-    ]
-maintainers = [
-    "Sergey Samsonov <svsamsonov@hse.ru>", "Evgeny Lagutin <lagutin.em@phystech.edu>"
-]
+    "Sergey Samsonov <svsamsonov@hse.ru>", 
+    "Evgeny Lagutin <lagutin.em@phystech.edu>", 
+    "Marylou Gabrié", "Alain Durmus", "Alexey Naumov", "Eric Moulines"]
 readme = "README.md"
-repository = "http://github.com/svsamsonov/ex2mcmc_new.git"
+repository = "http://github.com/svsamsonov/ex2mcmc_new"
 documentation = "http://github.com/svsamsonov/ex2mcmc_new/blob/master/README.md"
 license = "MIT"
-keywords = ["mcmc", "adaptive mcmc", "ex2mcmc", ""]
+keywords = ["mcmc", "adaptive mcmc", "gan", "normalizing flow"]
+packages = [
+    { include = "ex2mcmc" },
+    # { include = "extra_package/**/*.py" },
+]
 
 [tool.black]
 target-version = ["py38"]
 line-length = 88
 include = '\.pyi?$'
 exclude = '''
 /(
@@ -32,46 +33,48 @@
   | dist
   | thirdparty
 )/
 '''
 
 [tool.poetry.dependencies]
 python = "~3.8"
-torch = "^2.0.0"
-torchvision = "*"
-tensorflow = "~2.11.1"
+# torch-mimicry = {git = "https://github.com/kwotsin/mimicry.git", rev = "a7fda06c4aff1e6af8dc4c4a35ed6636e434c766"}
+torch-mimicry = "0.1.16"
 black = {extras = ["jupyter"], version = "^23.3.0"}
 isort = "^5.12.0"
 flake8 = "5.0.4"
 ipykernel = "^6.21.3"
 ipython = "^8.11.0"
 seaborn = "^0.12.2"
 jupyter = "^1.0.0"
 ruamel-yaml = "^0.17.21"
+munch = "^2.5.0"
 pre-commit = "^3.1.1"
 pyro-ppl = "^1.8.4"
 pot = "^0.9.0"
 easydict = "^1.10"
 jaxlib = "^0.4.7"
 jax = "^0.4.8"
 gdown = "^4.7.1"
+wandb = "^0.14.2"
+vulture = "^2.7"
 docker = "^6.0.1"
+toml = "^0.10.2"
+flake8-pyproject = "^1.2.3"
 
 [tool.isort]
 src_paths = ["."]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 88
 lines_after_imports = 2
 skip_glob = 'thirdparty'
-known_third_party = ["PIL", "gdown", "imageio", "matplotlib", "numpy", "ruamel", "scipy", "seaborn", 
-    "skimage", "sklearn", "tensorflow", "torch", "torchvision",  "torch_mimicry"
-    ]
+known_third_party = ["PIL", "gdown", "imageio", "matplotlib", "numpy", "ruamel", "scipy", "seaborn", "skimage", "sklearn", "tensorflow", "torch", "torchvision",  "torch_mimicry"]
 
 [tool.flake8]
 min_python_version = "3.8.0"
 max-line-length = 88
 # ban-relative-imports = true
 # flake8-use-fstring: https://github.com/MichaelKim0407/flake8-use-fstring#--percent-greedy-and---format-greedy
 format-greedy = 1
```

### Comparing `ex2mcmc-0.0.1/PKG-INFO` & `ex2mcmc-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: ex2mcmc
-Version: 0.0.1
+Version: 0.0.3
 Summary: Local-Global MCMC kernels: the bost of both worlds (NeurIPS 2022)
-Home-page: http://github.com/svsamsonov/ex2mcmc_new.git
+Home-page: http://github.com/svsamsonov/ex2mcmc_new
 License: MIT
-Keywords: mcmc,adaptive mcmc,ex2mcmc,
+Keywords: mcmc,adaptive mcmc,gan,normalizing flow
 Author: Sergey Samsonov
 Author-email: svsamsonov@hse.ru
-Maintainer: Sergey Samsonov
-Maintainer-email: svsamsonov@hse.ru
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: black[jupyter] (>=23.3.0,<24.0.0)
 Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: easydict (>=1.10,<2.0)
 Requires-Dist: flake8 (==5.0.4)
+Requires-Dist: flake8-pyproject (>=1.2.3,<2.0.0)
 Requires-Dist: gdown (>=4.7.1,<5.0.0)
 Requires-Dist: ipykernel (>=6.21.3,<7.0.0)
 Requires-Dist: ipython (>=8.11.0,<9.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: munch (>=2.5.0,<3.0.0)
 Requires-Dist: pot (>=0.9.0,<0.10.0)
 Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
 Requires-Dist: pyro-ppl (>=1.8.4,<2.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
-Requires-Dist: tensorflow (>=2.11.1,<2.12.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
-Requires-Dist: torchvision
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: torch-mimicry (==0.1.16)
+Requires-Dist: vulture (>=2.7,<3.0)
+Requires-Dist: wandb (>=0.14.2,<0.15.0)
 Project-URL: Documentation, http://github.com/svsamsonov/ex2mcmc_new/blob/master/README.md
-Project-URL: Repository, http://github.com/svsamsonov/ex2mcmc_new.git
+Project-URL: Repository, http://github.com/svsamsonov/ex2mcmc_new
 Description-Content-Type: text/markdown
 
 # Ex2MCMC: Local-Global MCMC kernels: the bost of both worlds (NeurIPS 2022) [[Paper]](https://proceedings.neurips.cc/paper_files/paper/2022/hash/21c86d5b10cdc28664ccdadf0a29065a-Abstract-Conference.html)
 
 [[ArXiv]](https://arxiv.org/abs/2111.02702)
 
 Authors: Sergey Samsonov, Evgeny Lagutin, Marylou Gabrié, Alain Durmus, Alexey Naumov, Eric Moulines.
@@ -48,16 +49,14 @@
 
 
 - [Ex2MCMC: Local-Global MCMC kernels: the bost of both worlds (NeurIPS 2022) \[Paper\]](#ex2mcmc-local-global-mcmc-kernels-the-bost-of-both-worlds-neurips-2022-paper)
   - [Single chain mixing](#single-chain-mixing)
   - [Sampling from GAN as Energy-Based Models with MCMC](#sampling-from-gan-as-energy-based-models-with-mcmc)
   - [Algorithms](#algorithms)
   - [Installation](#installation)
-    - [Developement installation](#developement-installation)
-    - [Download checkpoints and stats](#download-checkpoints-and-stats)
   - [Usage](#usage)
     - [Demonstration on SNGAN](#demonstration-on-sngan)
     - [Experiments with synthetic distributions:](#experiments-with-synthetic-distributions)
     - [Experiments with GANs on MNIST dataset](#experiments-with-gans-on-mnist-dataset)
     - [Experiments with GANs on CIFAR10 dataset](#experiments-with-gans-on-cifar10-dataset)
     - [Sampling and FID computation](#sampling-and-fid-computation)
   - [Results](#results)
@@ -95,43 +94,35 @@
 Create environment:
 
 ```bash
 conda create -n ex2mcmc python=3.8
 conda activate ex2mcmc
 ```
 
-```bash
-pip install ex2mcmc==0.0.1
-pip install git+https://github.com/kwotsin/mimicry.git
-```
-
-### Developement installation
-
 Install poetry (if absent):
 ```bash
 curl -sSL https://install.python-poetry.org | python3 -
 poetry config virtualenvs.create false
 ```
 
 Install the project:
 ```bash
 poetry install
-poetry add git+https://github.com/kwotsin/mimicry.git@a7fda06c4aff1e6af8dc4c4a35ed6636e434c766
 ```
 
-### Download checkpoints and stats
+Download checkpoints:
 
-CIFAR10 checkpoints:
+CIFAR10:
 
 | GAN   |     Steps     |  Path, G |  Path, D |
 |:----------|:-------------:|:------:|:------:|
 | DCGAN NS  | 100k      |   [netG_100000_steps.pth](https://drive.google.com/file/d/1gv8_qr_xa8hJzdJpBXiKr8v922EqcE-E/view?usp=share_link) |   [netD_100000_steps.pth](https://drive.google.com/file/d/1u1sPUmlvyhcbNDX2DVsR-mGOzqQ6U8sh/view?usp=share_link) |
 | SNGAN, Hinge  | 100k      |   [netG.pth](https://drive.google.com/file/d/118zC_iEkN27jGLVNmDuQpMeyw7BKOUra/view?usp=share_link) |   [netD.pth](https://drive.google.com/file/d/1xU5FV59TLhAlkFubJGmJVS87HnZZ2xHT/view?usp=share_link) |
 
-MNIST checkpoints:
+MNIST:
 
 | GAN      |  Path |
 |:----------|:-------------:|
 | Vanilla  |   [vanilla_gan.pth](https://drive.google.com/file/d/1xa1v4hPQQdU2RkhjMn5sFZCITxTJ5Dhj/view?usp=share_link) |
 | WGAN CP  |   [wgan.pth](https://drive.google.com/file/d/17nQJnfs2_T6kyahnkW3fu8AVY54kmRmw/view?usp=share_link) |
 
 You also can run script to download checkpoints:
```

