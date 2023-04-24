# Comparing `tmp/spatiotemporal-1.0.0.tar.gz` & `tmp/spatiotemporal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spatiotemporal-1.0.0.tar", last modified: Sat Mar 12 18:32:33 2022, max compression
+gzip compressed data, was "dist/spatiotemporal-1.0.1.tar", last modified: Mon Apr 24 16:53:05 2023, max compression
```

## Comparing `spatiotemporal-1.0.0.tar` & `spatiotemporal-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/
--rw-rw-r--   0 max       (1000) max       (1000)     1336 2022-03-12 17:46:50.000000 spatiotemporal-1.0.0/setup.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/spatiotemporal/
--rw-rw-r--   0 max       (1000) max       (1000)       22 2022-03-12 14:43:00.000000 spatiotemporal-1.0.0/spatiotemporal/_version.py
--rw-rw-r--   0 max       (1000) max       (1000)    10537 2022-03-12 17:48:03.000000 spatiotemporal-1.0.0/spatiotemporal/models.py
--rw-rw-r--   0 max       (1000) max       (1000)      988 2022-03-12 17:48:20.000000 spatiotemporal-1.0.0/spatiotemporal/tools.py
--rw-rw-r--   0 max       (1000) max       (1000)     5242 2022-03-12 17:48:14.000000 spatiotemporal-1.0.0/spatiotemporal/surrogates.py
--rw-rw-r--   0 max       (1000) max       (1000)     5176 2022-03-12 17:48:10.000000 spatiotemporal-1.0.0/spatiotemporal/stats.py
--rw-rw-r--   0 max       (1000) max       (1000)      451 2022-03-12 17:46:48.000000 spatiotemporal-1.0.0/spatiotemporal/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     2152 2022-03-12 17:47:56.000000 spatiotemporal-1.0.0/spatiotemporal/extras.py
--rw-rw-r--   0 max       (1000) max       (1000)     2097 2022-03-12 18:29:48.000000 spatiotemporal-1.0.0/README.md
--rw-rw-r--   0 max       (1000) max       (1000)       38 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)     3394 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/PKG-INFO
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/spatiotemporal.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)       19 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/spatiotemporal.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/spatiotemporal.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)     3394 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/spatiotemporal.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      388 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/spatiotemporal.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)       15 2022-03-12 18:32:33.000000 spatiotemporal-1.0.0/spatiotemporal.egg-info/top_level.txt
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/
+-rw-rw-r--   0 max       (1000) max       (1000)     1336 2022-03-12 17:46:50.000000 spatiotemporal-1.0.1/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/spatiotemporal/
+-rw-rw-r--   0 max       (1000) max       (1000)       22 2023-04-24 06:46:43.000000 spatiotemporal-1.0.1/spatiotemporal/_version.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11307 2023-04-24 05:50:56.000000 spatiotemporal-1.0.1/spatiotemporal/models.py
+-rw-rw-r--   0 max       (1000) max       (1000)      988 2022-03-12 17:48:20.000000 spatiotemporal-1.0.1/spatiotemporal/tools.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5233 2023-04-24 05:51:50.000000 spatiotemporal-1.0.1/spatiotemporal/surrogates.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5184 2023-04-24 05:51:29.000000 spatiotemporal-1.0.1/spatiotemporal/stats.py
+-rw-rw-r--   0 max       (1000) max       (1000)      476 2023-04-24 06:31:51.000000 spatiotemporal-1.0.1/spatiotemporal/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     6036 2023-04-24 06:51:19.000000 spatiotemporal-1.0.1/spatiotemporal/extras.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2059 2023-04-24 05:49:38.000000 spatiotemporal-1.0.1/README.md
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)     2913 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/PKG-INFO
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/spatiotemporal.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)       19 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/spatiotemporal.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/spatiotemporal.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)     2913 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/spatiotemporal.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      388 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/spatiotemporal.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       15 2023-04-24 16:53:05.000000 spatiotemporal-1.0.1/spatiotemporal.egg-info/top_level.txt
```

### Comparing `spatiotemporal-1.0.0/setup.py` & `spatiotemporal-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `spatiotemporal-1.0.0/spatiotemporal/models.py` & `spatiotemporal-1.0.1/spatiotemporal/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Available under the MIT license
 import numpy as np
 import scipy.signal
 import scipy.optimize
 from .tools import spatial_exponential_floor
 
 def spatiotemporal_model_timeseries(distance_matrix, sa_lambda, sa_inf, ta_delta1s, num_timepoints, sample_rate, highpass_freq, seed=None):
-    """Simulate the spatiotemporal model from [Shinn et al (2022)](https://www.biorxiv.org/content/10.1101/2021.06.01.446561v1)
+    """Simulate the spatiotemporal model from [Shinn et al (2023)](https://www.nature.com/articles/s41593-023-01299-3)
 
     Args:
       distance_matrix (NxN numpy array): the NxN distance matrix, representing the spatial distance
           between location of each of the timeseries.  This should usually be the
           output of the `distance_matrix_euclidean` function.
       sa_lambda (float): the SA-λ parameter
       sa_inf (float): the SA-∞ parameter
@@ -29,24 +29,24 @@
     assert num_timepoints % 2 == 0, "Must be even timeseries length"
     # Filtered brown noise spectrum
     spectrum = make_spectrum(tslen=num_timepoints, sample_rate=sample_rate, alpha=2, highpass_freq=highpass_freq)
     spectra = np.asarray([spectrum]*len(ta_delta1s))
     # Spatial autocorrelation matrix
     corr = spatial_exponential_floor(distance_matrix, sa_lambda, sa_inf)
     # Create spatially embedded timeseries with the given spectra
-    tss = spatial_temporal_timeseries(corr, spectra, seed=seed)
+    tss = correlated_spectral_sampling(corr, spectra, seed=seed)
     # Compute the standard deviation of nosie we need to add to get the desired TA-delta1
     noises = [how_much_noise(spectrum, max(.001, ta_delta1)) for ta_delta1 in ta_delta1s]
     # Add noise to the timeseries
     rng = np.random.RandomState(seed)
     tss += rng.randn(tss.shape[0], tss.shape[1]) * np.asarray(noises).reshape(-1,1)
     return tss
 
-def spatiotemporal_noiseless_model_timeseries(distance_matrix, sa_lambda, sa_inf, ta_delta1s, num_timepoints, sample_rate, highpass_freq, seed=0):
-    """Simulate the noiseless spatiotemporal model from [Shinn et al (2022)](https://www.biorxiv.org/content/10.1101/2021.06.01.446561v1)
+def intrinsic_timescale_sa_model_timeseries(distance_matrix, sa_lambda, sa_inf, ta_delta1s, num_timepoints, sample_rate, highpass_freq, seed=0):
+    """Simulate the intrinsic timescale + spatial autocorrelation model from [Shinn et al (2023)](https://www.nature.com/articles/s41593-023-01299-3)
 
     Args:
       distance_matrix (NxN numpy array): the NxN distance matrix, representing the spatial distance
           between location of each of the timeseries.  This should usually be the
           output of the `distance_matrix_euclidean` function.
       sa_lambda (float): the SA-λ parameter
       sa_inf (float): the SA-∞ parameter
@@ -55,41 +55,45 @@
       sample_rate (float): the spacing between timepoints (e.g. TR in fMRI)
       highpass_freq (float): if non-zero, apply a highpass filter above the
           given frequency.  A good default is 0.01 for fMRI timeseries.
       seed (int, optional): the random seed.  If not specified, it will use
           the current state of the numpy random number generator.
 
     Returns:
-      NxT numpy array: For each of the N nodes, a timeseries of length T=`num_timepoints` according to the noiseless spatiotemporal model
+      NxT numpy array: For each of the N nodes, a timeseries of length T=`num_timepoints` according to the intrinsic timescale + spatial autocorrelation model
     """
     assert num_timepoints % 2 == 0, "Must be even timeseries length"
     # Determine the pink noise exponent alpha from the TA-delta1
     alphas = [ta_to_alpha_fast(sample_rate=sample_rate, tslen=num_timepoints, highpass_freq=highpass_freq, target_ta=max(0,ta_delta1)) for ta_delta1 in ta_delta1s]
     # Use these alpha values to construct desired frequency spectra
     spectra = np.asarray([make_spectrum(tslen=num_timepoints, sample_rate=sample_rate, alpha=alpha, highpass_freq=highpass_freq) for alpha in alphas])
     # Spatial autocorrelation matrix
     corr = spatial_exponential_floor(distance_matrix, sa_lambda, sa_inf)
     # Compute timeseries from desired correlation matrix and frequency spectra
-    tss = spatial_temporal_timeseries(cm=corr, spectra=spectra, seed=seed)
+    tss = correlated_spectral_sampling(cm=corr, spectra=spectra, seed=seed)
     return tss
 
 
-def spatial_temporal_timeseries(cm, spectra, seed=None):
+def correlated_spectral_sampling(cm, spectra, seed=None):
     """Generate timeseries with given amplitude spectra and correlation matrices
 
+    This implements Correlated Spectral Sampling, as described in [Shinn et al
+    (2023)](https://www.nature.com/articles/s41593-023-01299-3).
+
     Args:
       cm (NxN numpy array): The correlation matrix
       spectra (Nxk numpy array): A list of Fourier spectra generated by [make_spectrum][spatiotemporal.models.make_spectrum]
           Each of the N spectra are associated with a row/column of `cm`.
       seed (int, optional): the random seed.  If not specified, it will use
           the current state of the numpy random number generator.
 
     Returns:
       NxT numpy array: N timeseries of length T.  Timeseries i will have a power spectrum given by `spectra[i]`,
           and will be correlated with the other timeseries with correlations cm[i].
+
     """
     N_regions = cm.shape[0]
     N_freqs = len(spectra[0])
     N_timepoints = (N_freqs-1)*2
     assert spectra.shape == (N_regions, N_freqs)
     sum_squares = np.sum(spectra**2, axis=1, keepdims=True)
     cosine_similarity = (spectra @ spectra.T)/np.sqrt(sum_squares @ sum_squares.T)
@@ -206,9 +210,24 @@
     key = (tslen, sample_rate, highpass_freq, taround)
     if key in ta_to_alpha_cache.keys():
         return ta_to_alpha_cache[key]
     val = ta_to_alpha(*key)
     ta_to_alpha_cache[key] = val
     return val
 
+def make_noisy_spectrum(tslen, sample_rate, alpha, highpass_freq, target_ar1):
+    """Similar to make_spectrum, except adds white noise to the spectrum
+    (i.e. uniform distribution).  Returns the fourier spectrum (amplitude
+    spectrum).
+
+    This also applies the same filter as make_spectrum.
+
+    """
+    noiseless_spectrum = make_spectrum(tslen, sample_rate, alpha, highpass_freq)
+    N = len(noiseless_spectrum)
+    noise = how_much_noise(noiseless_spectrum, target_ar1)
+    noisy_spectrum = np.sqrt(noiseless_spectrum**2 + noise**2 * N)
+    noisy_spectrum[0] = 0
+    return noisy_spectrum
+
 class PositiveSemidefiniteError(Exception):
     pass
```

### Comparing `spatiotemporal-1.0.0/spatiotemporal/tools.py` & `spatiotemporal-1.0.1/spatiotemporal/tools.py`

 * *Files identical despite different names*

### Comparing `spatiotemporal-1.0.0/spatiotemporal/surrogates.py` & `spatiotemporal-1.0.1/spatiotemporal/surrogates.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright 2022 Max Shinn <m.shinn@ucl.ac.uk>
 # Available under the MIT license
 import numpy as np
 from .tools import get_eigenvalues, make_perfectly_symmetric
 import scipy.stats
 
 def eigensurrogate_matrix(cm, seed=None):
-    """Eigensurrogate model, from [Shinn et al (2022)](https://www.biorxiv.org/content/10.1101/2021.06.01.446561v1)
+    """Eigensurrogate model, from [Shinn et al (2023)](https://www.nature.com/articles/s41593-023-01299-3)
 
     Determine the eigenvalues of the correlation matrix, and then sample a new
     correlation matrix with the same eigenvalues.
 
     Args:
       cm (NxN numpy array): a correlation matrix
       seed (int, optional): the random seed.  If not specified, it will use
```

### Comparing `spatiotemporal-1.0.0/spatiotemporal/stats.py` & `spatiotemporal-1.0.1/spatiotemporal/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Available under the MIT license
 import numpy as np
 import pandas
 import scipy.spatial
 import scipy.optimize
 
 def spatial_autocorrelation(cm, dist, discretization=1):
-    """Calculate the SA-λ and SA-∞ measures of spatial autocorrelation, defined in [Shinn et al (2022)](https://www.biorxiv.org/content/10.1101/2021.06.01.446561v1)
+    """Calculate the SA-λ and SA-∞ measures of spatial autocorrelation, defined in [Shinn et al (2023)](https://www.nature.com/articles/s41593-023-01299-3)
 
     Args:
       cm (NxN numpy array): NxN correlation matrix of timeseries, where N is the number of
           timeseries
       dist (NxN numpy array): the NxN distance matrix, representing the spatial distance
           between location of each of the timeseries.  This should usually be the
           output of the `distance_matrix_euclidean` function.
@@ -19,15 +19,15 @@
           The size of the discretization should ensure that there are a sufficient number of
           observations in each bin, but also enough total bins to make a meaningful estimation.
           Try increasing it or decreasing it according to the scale of your data.  Data that has values
           up to around 100 should be fine with the default.  Decrease or increase as necessary
           to get an appropriate estimation.
 
     Returns:
-      tuple of (SA-λ, SA-∞)
+      tuple of floats: tuple of (SA-λ, SA-∞)
     """
     cm_flat = cm.flatten()
     dist_flat = dist.flatten()
     df = pandas.DataFrame(np.asarray([dist_flat, cm_flat]).T, columns=["dist", "corr"])
     df['dist_bin'] = np.round(df['dist']/discretization)*discretization
     df_binned = df.groupby('dist_bin').mean().reset_index().sort_values('dist_bin')
     binned_dist_flat = df_binned['dist_bin']
```

