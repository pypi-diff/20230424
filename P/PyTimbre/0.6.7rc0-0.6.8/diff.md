# Comparing `tmp/PyTimbre-0.6.7rc0.tar.gz` & `tmp/PyTimbre-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTimbre-0.6.7rc0.tar", last modified: Mon Apr 17 13:07:56 2023, max compression
+gzip compressed data, was "PyTimbre-0.6.8.tar", last modified: Mon Apr 24 21:56:27 2023, max compression
```

## Comparing `PyTimbre-0.6.7rc0.tar` & `PyTimbre-0.6.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.583383 PyTimbre-0.6.7rc0/
--rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.7rc0/LICENSE.txt
--rw-rw-rw-   0        0        0    13121 2023-04-17 13:07:56.582714 PyTimbre-0.6.7rc0/PKG-INFO
--rw-rw-rw-   0        0        0     5289 2023-04-13 01:01:21.000000 PyTimbre-0.6.7rc0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 13:07:56.583383 PyTimbre-0.6.7rc0/setup.cfg
--rw-rw-rw-   0        0        0     1074 2023-04-17 13:06:01.000000 PyTimbre-0.6.7rc0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.493721 PyTimbre-0.6.7rc0/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.507006 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/
--rw-rw-rw-   0        0        0    13121 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.521864 PyTimbre-0.6.7rc0/src/pytimbre/
--rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.7rc0/src/pytimbre/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.541779 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/
--rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/__init__.py
--rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/ansi_standard_formatted_files.py
--rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/calibrated_binary_files.py
--rw-rw-rw-   0        0        0    70669 2023-03-31 16:13:47.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/wavefile.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.581713 PyTimbre-0.6.7rc0/src/pytimbre/spectral/
--rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/__init__.py
--rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/acoustic_weights.py
--rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/fractional_octave_band.py
--rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/fundamental_frequency.py
--rw-rw-rw-   0        0        0    58655 2023-04-16 12:48:15.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectra.py
--rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectrogram.py
--rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/swipe.py
--rw-rw-rw-   0        0        0    30413 2023-04-16 01:00:36.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/time_histories.py
--rw-rw-rw-   0        0        0    84616 2023-04-13 01:25:20.000000 PyTimbre-0.6.7rc0/src/pytimbre/waveform.py
--rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.7rc0/src/pytimbre/yin.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.908564 PyTimbre-0.6.8/
+-rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    13338 2023-04-24 21:56:27.907567 PyTimbre-0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5289 2023-04-13 01:01:21.000000 PyTimbre-0.6.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 21:56:27.908564 PyTimbre-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-04-24 21:55:20.000000 PyTimbre-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.841008 PyTimbre-0.6.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.853483 PyTimbre-0.6.8/src/PyTimbre.egg-info/
+-rw-rw-rw-   0        0        0    13338 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.861785 PyTimbre-0.6.8/src/pytimbre/
+-rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.8/src/pytimbre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.881215 PyTimbre-0.6.8/src/pytimbre/audio_files/
+-rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/__init__.py
+-rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/ansi_standard_formatted_files.py
+-rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/calibrated_binary_files.py
+-rw-rw-rw-   0        0        0    70669 2023-03-31 16:13:47.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/wavefile.py
+drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.906556 PyTimbre-0.6.8/src/pytimbre/spectral/
+-rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.8/src/pytimbre/spectral/__init__.py
+-rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.8/src/pytimbre/spectral/acoustic_weights.py
+-rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.8/src/pytimbre/spectral/fractional_octave_band.py
+-rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.6.8/src/pytimbre/spectral/fundamental_frequency.py
+-rw-rw-rw-   0        0        0    58636 2023-04-21 14:52:01.000000 PyTimbre-0.6.8/src/pytimbre/spectral/spectra.py
+-rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.8/src/pytimbre/spectral/spectrogram.py
+-rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.8/src/pytimbre/spectral/swipe.py
+-rw-rw-rw-   0        0        0    32278 2023-04-24 21:48:22.000000 PyTimbre-0.6.8/src/pytimbre/spectral/time_histories.py
+-rw-rw-rw-   0        0        0    85520 2023-04-24 21:54:08.000000 PyTimbre-0.6.8/src/pytimbre/waveform.py
+-rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.8/src/pytimbre/yin.py
```

### Comparing `PyTimbre-0.6.7rc0/LICENSE.txt` & `PyTimbre-0.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/PKG-INFO` & `PyTimbre-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.7rc0
+Version: 0.6.8
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -191,14 +191,18 @@
 - Updated the information within the WaveFile to support writing multi-channel audio files to disk
 - Re-incorporated classes to read audio files generated as a pre-cursor to the StandardBinaryFile
 
 #### April
 - __Version 0.6.4__
 - Version 0.6.3 integrated the libf0 library. After attempting to integrate this library directly, it was determined that using the raw code would be a better implementation for this package.
 - The swipe.py file was taken from version 1.0.2 on 1 April 2023 to provide the fundamental frequency
+- __Version 0.6.7__
+- Updates to the calculation of the fundamental frequency
+- Updates to the calculation of the harmonic features
+- Updates to methods to get the features from the spectrum and time history objects
 
 
 MIT License
 
 Copyright (c) 2021 Frank Mobley, Gregory Bowers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyTimbre-0.6.7rc0/README.md` & `PyTimbre-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/setup.py` & `PyTimbre-0.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         HISTORY = history_file.read()
 
         with open('LICENSE.txt') as license_file:
             LICENSE = license_file.read()
 
 setup(
     name='PyTimbre',
-    version='0.6.7c0',
+    version='0.6.8',
     description='Python conversion of Timbre Toolbox',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY + '\n\n' + LICENSE,
     license='MIT',
     packages=find_packages('src'),
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
```

### Comparing `PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/PKG-INFO` & `PyTimbre-0.6.8/src/PyTimbre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.7rc0
+Version: 0.6.8
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -191,14 +191,18 @@
 - Updated the information within the WaveFile to support writing multi-channel audio files to disk
 - Re-incorporated classes to read audio files generated as a pre-cursor to the StandardBinaryFile
 
 #### April
 - __Version 0.6.4__
 - Version 0.6.3 integrated the libf0 library. After attempting to integrate this library directly, it was determined that using the raw code would be a better implementation for this package.
 - The swipe.py file was taken from version 1.0.2 on 1 April 2023 to provide the fundamental frequency
+- __Version 0.6.7__
+- Updates to the calculation of the fundamental frequency
+- Updates to the calculation of the harmonic features
+- Updates to methods to get the features from the spectrum and time history objects
 
 
 MIT License
 
 Copyright (c) 2021 Frank Mobley, Gregory Bowers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/SOURCES.txt` & `PyTimbre-0.6.8/src/PyTimbre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/audio_files/ansi_standard_formatted_files.py` & `PyTimbre-0.6.8/src/pytimbre/audio_files/ansi_standard_formatted_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/audio_files/calibrated_binary_files.py` & `PyTimbre-0.6.8/src/pytimbre/audio_files/calibrated_binary_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/audio_files/wavefile.py` & `PyTimbre-0.6.8/src/pytimbre/audio_files/wavefile.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/spectral/acoustic_weights.py` & `PyTimbre-0.6.8/src/pytimbre/spectral/acoustic_weights.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/spectral/fractional_octave_band.py` & `PyTimbre-0.6.8/src/pytimbre/spectral/fractional_octave_band.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/spectral/fundamental_frequency.py` & `PyTimbre-0.6.8/src/pytimbre/spectral/fundamental_frequency.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectra.py` & `PyTimbre-0.6.8/src/pytimbre/spectral/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
         return AcousticWeights.la(self.pressures_decibels, self.frequencies)[0]
 
     @property
     def perceived_noise_level(self):
         spl = self.pressures_decibels
         while len(spl) < 31:
-            spl = np.concatenate([[0], self.pressures_pascals])
+            spl = np.concatenate([[0], spl])
         return AcousticWeights.pnl(spl)
 
     @property
     def fractional_octave_bandwidth(self):
         return self._bandwidth
 
     @fractional_octave_bandwidth.setter
```

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectrogram.py` & `PyTimbre-0.6.8/src/pytimbre/spectral/spectrogram.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/spectral/swipe.py` & `PyTimbre-0.6.8/src/pytimbre/spectral/swipe.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/spectral/time_histories.py` & `PyTimbre-0.6.8/src/pytimbre/spectral/time_histories.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,14 @@
 
         Parameters
         ----------
 
         filename: str - the full path to the
         """
         import os.path
-        import pandas as pd
 
         if not os.path.exists(filename):
             raise ValueError("The filename must exist")
 
         file = open(filename, "rt")
         contents = file.readlines()
         file.close()
@@ -663,14 +662,51 @@
         tpm = np.zeros((len(self.spectra),))
 
         for i in range(len(tpm)):
             tpm[i] = self.spectra[i].time_past_midnight
 
         return tpm
 
+    def concatenate(self, b=None, inplace: bool = False):
+        if not isinstance(b, TimeHistory):
+            raise ValueError("The first argument is required to be a TimeHistory object.")
+        if not np.array_equal(self.frequencies, b.frequencies):
+            raise ValueError("Two TimeHistory objects must have same frequency content.")
+        if self.integration_time != b.integration_time:
+            raise AttributeError("Two TimeHistory objects must have same integration time.")
+        warnings.warn('Concatenated TimeHistory object currently returns the header equal to the header of the first '
+                      'TimeHistory object only.')
+
+        if not inplace:
+            th = TimeHistory(integration_time=self.integration_time)
+
+            th._header = self._header
+
+            th._spectra = np.empty(len(self.times) + len(b.times), dtype=Spectrum)
+            for i in range(len(self.times)):
+                th._spectra[i] = self.spectra[i]
+                th._spectra[i]._time0 = i * self._integration_time
+            for i in range(len(b.times)):
+                th._spectra[len(self.times) + i] = b.spectra[i]
+                th._spectra[len(self.times) + i]._time0 = (len(self.times) + i) * self._integration_time
+
+            return th
+
+        else:
+
+            # self._spectra = np.empty(len(self.times) + len(b.times), dtype=Spectrum)
+            # for i in range(len(self.times)):
+            #     self._spectra[i] = self.spectra[i]
+            #     self._spectra[i]._time0 = i * self._integration_time
+            # for i in range(len(b.times)):
+            #     self._spectra[len(self.times) + i] = b.spectra[i]
+            #     self._spectra[len(self.times) + i]._time0 = (len(self.times) + i) * self._integration_time
+
+            raise NotImplementedError("inplace concatenation not yet implemented.")
+
 
 class NarrowbandTimeHistory(TimeHistory):
     """
     This class implements the _calculate_spectrogram function using the Narrowband_Spectrum class
     """
 
     def __init__(self, a: Waveform, integration_time: float = 0.25, fft_size: int = None):
```

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/waveform.py` & `PyTimbre-0.6.8/src/pytimbre/waveform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1120,51 +1120,72 @@
 
             return None
         else:
             return Waveform(self._samples * scale_factor, self.sample_rate, self.start_time)
 
     # -------------------- Public functions for operations on the samples within the Waveform --------------------------
 
-    def apply_calibration(self, wfm, level: float = 114, frequency: float = 1000, inplace: bool = False):
+    def determine_calibration_scale_factor(self, level: float = 114, frequency: float = 1000):
         """
-        This function assumes that the current Waveform, and the item provided as the first argument, possess the
-        same parameters for the acquisition system. This assumes that the Waveform (wfm) is a calibration data that
-        is collected with the same level and frequency passed to the function. This will scale the current samples to
-        the same amplitude based on the data within the wfm.
+        This function will take the information within the current Waveform and determine the scaling factor that can be
+        applied to this, or any other file, to ensure that the acoustic reference is obtained.
 
         Parameters
         ----------
-        wfm - The Waveform that possesses a calibration signal that can be analyzed to determine the scaling factor
-        level: float, default = 114 - the expected acoustic level for the calibration signal in wfm
-        frequency: float, default = 1000 - the frequency of the calibration signal in wfm
-        inplace: bool, default = False - whether the manipulation is applied to the current Waveform,
-            or a new Waveform object is returned to the user.
+        :param level: float
+            default = 114 dB, this is the acoustic level at the specified frequency that we expect the calibration tone
+            to generate
+        :param frequency: float
+            default = 1000 Hz, this is the acoustic frequency of the calibration device
         """
 
         from .spectral.fractional_octave_band import FractionalOctaveBandTools as fob
 
         #   ensure that the calibration frequency is actually located within the Waveform.
-        calibration, detected_frequency = wfm.is_calibration()
+        calibration, detected_frequency = self.is_calibration()
         if not calibration or abs(detected_frequency - frequency) > 25:
             raise ValueError("The Waveform passed to the function does not contain a calibration tone or the tone is "
                              "not at the expected frequency, based on the arguments of the function.")
 
         #   Now we need to calculate the scale factor required to adjust the level of the calibration Waveform to the
         #   desired magnitude.
-        filtered_wfm = wfm.apply_bandpass(fob.lower_frequency(3, fob.nearest_band(3, frequency)),
-                                          fob.upper_frequency(3, fob.nearest_band(3, frequency)))
+        filtered_wfm = self.apply_bandpass(fob.lower_frequency(3, fob.nearest_band(3, frequency)),
+                                           fob.upper_frequency(3, fob.nearest_band(3, frequency)))
 
         #   Now assuming that the data within the samples array is a pressure
         rms_level = 20 * np.log10(np.std(filtered_wfm.samples) / 20e-6)
 
         sens = level - rms_level
         sens /= 20
         sens *= -1
         sens = 10.0 ** sens
 
+        return sens
+
+    def apply_calibration(self, wfm, level: float = 114, frequency: float = 1000, inplace: bool = False):
+        """
+        This function assumes that the current Waveform, and the item provided as the first argument, possess the
+        same parameters for the acquisition system. This assumes that the Waveform (wfm) is a calibration data that
+        is collected with the same level and frequency passed to the function. This will scale the current samples to
+        the same amplitude based on the data within the wfm.
+
+        Parameters
+        ----------
+        wfm - The Waveform that possesses a calibration signal that can be analyzed to determine the scaling factor
+        level: float, default = 114 - the expected acoustic level for the calibration signal in wfm
+        frequency: float, default = 1000 - the frequency of the calibration signal in wfm
+        inplace: bool, default = False - whether the manipulation is applied to the current Waveform,
+            or a new Waveform object is returned to the user.
+        """
+
+        if not isinstance(wfm, Waveform):
+            raise ValueError("The wfm is expected to be a Waveform object")
+
+        sens = wfm.determine_calibration_scale_factor(level, frequency)
+
         #   Now scale the calibration signal and determine whether the overall level is close to the expected level
         scaled_calibration_wfm = wfm.scale_signal(1 / sens)
 
         if abs(np.any(scaled_calibration_wfm.overall_level() - level)) > 2:
             raise ValueError("The method did not appropriately scale the calibration signal")
 
         return self.scale_signal(1 / sens, inplace=inplace)
```

### Comparing `PyTimbre-0.6.7rc0/src/pytimbre/yin.py` & `PyTimbre-0.6.8/src/pytimbre/yin.py`

 * *Files identical despite different names*

