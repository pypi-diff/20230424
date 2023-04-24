# Comparing `tmp/stable-ts-2.4.1.tar.gz` & `tmp/stable-ts-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.4.1.tar", last modified: Tue Apr 18 21:35:58 2023, max compression
+gzip compressed data, was "stable-ts-2.5.0.tar", last modified: Mon Apr 24 05:29:31 2023, max compression
```

## Comparing `stable-ts-2.4.1.tar` & `stable-ts-2.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 21:35:58.178899 stable-ts-2.4.1/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-04-18 21:35:58.177899 stable-ts-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 21:35:58.179901 stable-ts-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 21:35:58.126898 stable-ts-2.4.1/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 21:35:58.175899 stable-ts-2.4.1/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.4.1/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.4.1/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-18 21:09:40.000000 stable-ts-2.4.1/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     6525 2023-04-16 00:09:42.000000 stable-ts-2.4.1/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4328 2023-03-22 02:57:30.000000 stable-ts-2.4.1/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.4.1/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    28584 2023-04-18 21:10:38.000000 stable-ts-2.4.1/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.4.1/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.4.1/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0     9744 2023-04-08 16:34:45.000000 stable-ts-2.4.1/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.4.1/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    48816 2023-04-18 21:05:11.000000 stable-ts-2.4.1/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-04-24 05:29:31.643210 stable-ts-2.5.0/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     6890 2023-04-24 05:29:31.642207 stable-ts-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 05:29:31.643210 stable-ts-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 05:29:31.605197 stable-ts-2.5.0/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0     6890 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-24 05:29:31.000000 stable-ts-2.5.0/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 05:29:31.640208 stable-ts-2.5.0/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.5.0/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.5.0/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-24 04:49:38.000000 stable-ts-2.5.0/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     6537 2023-04-19 18:39:07.000000 stable-ts-2.5.0/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.5.0/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.5.0/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    34855 2023-04-24 05:25:29.000000 stable-ts-2.5.0/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.5.0/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.5.0/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.5.0/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.5.0/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    50175 2023-04-24 03:35:12.000000 stable-ts-2.5.0/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.4.1/LICENSE` & `stable-ts-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/PKG-INFO` & `stable-ts-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.4.1
+Version: 2.5.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.4.1/README.md` & `stable-ts-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/setup.py` & `stable-ts-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.5.0/stable_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.4.1
+Version: 2.5.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.4.1/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.5.0/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/stable_whisper/audio.py` & `stable-ts-2.5.0/stable_whisper/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 from typing import Union
 
 from whisper.audio import SAMPLE_RATE
 
 
 def is_ytdlp_available():
-    return subprocess.run('yt-dlp -h', capture_output=True).returncode == 0
+    return subprocess.run('yt-dlp -h', shell=True, capture_output=True).returncode == 0
 
 
 def _load_file(file: Union[str, bytes], verbose: bool = False):
     if isinstance(file, str) and '://' in file:
         if is_ytdlp_available():
             verbosity = ' -q' if verbose is None else (' --progress' if verbose else ' --progress -q')
             p = subprocess.run(
```

### Comparing `stable-ts-2.4.1/stable_whisper/decode.py` & `stable-ts-2.5.0/stable_whisper/decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                 # apply the logit filters, e.g. for suppressing or applying penalty to
                 for logit_filter in self.logit_filters:
                     logit_filter.apply(logits, tokens)
 
                 # suppress timestamp tokens where the audio is silent so that decoder ignores those timestamps
                 _suppress_ts(logits[:, self.tokenizer.timestamp_begin:], self.ts_token_mask)
 
+                logits.nan_to_num_(-np.inf)
                 # expand the tokens tensor with the selected next tokens
                 tokens, completed = self.decoder.update(tokens, logits, sum_logprobs)
 
                 if completed or tokens.shape[-1] > self.n_ctx:
                     break
         finally:
             self.inference.cleanup_caching()
```

### Comparing `stable-ts-2.4.1/stable_whisper/quantization.py` & `stable-ts-2.5.0/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/stable_whisper/result.py` & `stable-ts-2.5.0/stable_whisper/result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+import re
 import numpy as np
 from typing import Union, List, Tuple
 from dataclasses import dataclass
 from copy import deepcopy
 from itertools import chain
 
 from .stabilization import suppress_silence
@@ -753,14 +754,34 @@
             self
             .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
             .split_by_gap(.5)
             .merge_by_gap(.3, max_words=3)
             .split_by_punctuation([('.', ' '), '。', '?', '？'])
         )
 
+    def find(self, pattern: str, word_level=True, flags=None) -> "WhisperResultMatches":
+        """
+
+        Find segments/words and timestamps with regular expression.
+
+        Parameters
+        ----------
+        pattern: str
+            RegEx pattern to search for.
+        word_level: bool
+            Whether to search at word-level
+        flags:
+            RegEx flags.
+
+        Returns
+        -------
+        An instance of WhisperResultMatches class to allow for continuous chaining of this method.
+        """
+        return WhisperResultMatches(self).find(pattern, word_level=word_level, flags=flags)
+
     @property
     def text(self):
         return ''.join(s.text for s in self.segments)
 
     def __len__(self):
         return len(self.segments)
 
@@ -773,7 +794,160 @@
         self.language = self.ori_dict.get('language')
         segments = self.ori_dict.get('segments')
         self.segments: List[Segment] = [Segment(**s) for s in segments] if segments else []
 
     to_srt_vtt = result_to_srt_vtt
     to_ass = result_to_ass
     save_as_json = save_as_json
+
+
+class SegmentMatch:
+
+    def __init__(
+            self,
+            segments: Union[List[Segment], Segment],
+            _word_indices: List[List[int]] = None,
+            _text_match: str = None
+    ):
+        self.segments = [segments] if isinstance(segments, Segment) else segments
+        self.word_indices = [] if _word_indices is None else _word_indices
+        self.words = [self.segments[i].words[j] for i, indices in enumerate(self.word_indices) for j in indices]
+        if len(self.words) != 0:
+            self.text = ''.join(
+                self.segments[i].words[j].word
+                for i, indices in enumerate(self.word_indices)
+                for j in indices
+            )
+        else:
+            self.text = ''.join(seg.text for seg in self.segments)
+        self.text_match = _text_match
+
+    @property
+    def start(self):
+        return (
+            self.words[0].start
+            if len(self.words) != 0 else
+            (self.segments[0].start if len(self.segments) != 0 else None)
+        )
+
+    @property
+    def end(self):
+        return (
+            self.words[-1].end
+            if len(self.words) != 0 else
+            (self.segments[-1].end if len(self.segments) != 0 else None)
+        )
+
+    def __len__(self):
+        return len(self.segments)
+
+    def __repr__(self):
+        return self.__dict__.__repr__()
+
+    def __str__(self):
+        return self.__dict__.__str__()
+
+
+class WhisperResultMatches:
+    """
+    RegEx matches for WhisperResults
+    """
+    # Use WhisperResult.find() instead of instantiating this class directly.
+    def __init__(
+            self,
+            matches: Union[List[SegmentMatch], WhisperResult],
+            _segment_indices: List[List[int]] = None
+    ):
+        if isinstance(matches, WhisperResult):
+            self.matches = list(map(SegmentMatch, matches.segments))
+            self._segment_indices = [[i] for i in range(len(matches.segments))]
+        else:
+            self.matches = matches
+            assert _segment_indices is not None
+            assert len(self.matches) == len(_segment_indices)
+            assert all(len(match.segments) == len(_segment_indices[i]) for i, match in enumerate(self.matches))
+            self._segment_indices = _segment_indices
+
+    @property
+    def segment_indices(self):
+        return self._segment_indices
+
+    def _curr_seg_groups(self) -> List[List[Tuple[int, Segment]]]:
+        seg_groups, curr_segs = [], []
+        curr_max = -1
+        for seg_indices, match in zip(self._segment_indices, self.matches):
+            for i, seg in zip(sorted(seg_indices), match.segments):
+                if i > curr_max:
+                    curr_segs.append((i, seg))
+                    if i - 1 != curr_max:
+                        seg_groups.append(curr_segs)
+                        curr_segs = []
+                    curr_max = i
+
+        if curr_segs:
+            seg_groups.append(curr_segs)
+        return seg_groups
+
+    def find(self, pattern: str, word_level=True, flags=None) -> "WhisperResultMatches":
+        """
+
+        Find segments/words and timestamps with regular expression.
+
+        Parameters
+        ----------
+        pattern: str
+            RegEx pattern to search for.
+        word_level: bool
+            Whether to search at word-level
+        flags:
+            RegEx flags.
+
+        Returns
+        -------
+        An instance of WhisperResultMatches class to allow for continuous chaining of this method.
+        """
+
+        seg_groups = self._curr_seg_groups()
+        matches: List[SegmentMatch] = []
+        match_seg_indices: List[List[int]] = []
+        if word_level:
+            if not all(all(seg.has_words for seg in match.segments) for match in self.matches):
+                warnings.warn('Cannot perform word-level search with segment(s) missing word timestamps.')
+                word_level = False
+
+        for segs in seg_groups:
+            if word_level:
+                idxs = list(chain.from_iterable(
+                    [(i, j)]*len(word.word) for (i, seg) in segs for j, word in enumerate(seg.words)
+                ))
+                text = ''.join(word.word for (_, seg) in segs for word in seg.words)
+            else:
+                idxs = list(chain.from_iterable([(i, None)]*len(seg.text) for (i, seg) in segs))
+                text = ''.join(seg.text for (_, seg) in segs)
+            assert len(idxs) == len(text)
+            for curr_match in re.finditer(pattern, text, flags=flags or 0):
+                start, end = curr_match.span()
+                curr_idxs = idxs[start: end]
+                curr_seg_idxs = sorted(set(i[0] for i in curr_idxs))
+                if word_level:
+                    curr_word_idxs = [
+                        sorted(set(j for i, j in curr_idxs if i == seg_idx))
+                        for seg_idx in curr_seg_idxs
+                    ]
+                else:
+                    curr_word_idxs = None
+                matches.append(SegmentMatch(
+                    segments=[s for i, s in segs if i in curr_seg_idxs],
+                    _word_indices=curr_word_idxs,
+                    _text_match=curr_match.group()
+                ))
+                match_seg_indices.append(curr_seg_idxs)
+        return WhisperResultMatches(matches, match_seg_indices)
+
+    def __len__(self):
+        return len(self.matches)
+
+    def __bool__(self):
+        return self.__len__() != 0
+
+    def __getitem__(self, idx):
+        return self.matches[idx]
```

### Comparing `stable-ts-2.4.1/stable_whisper/stabilization.py` & `stable-ts-2.5.0/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/stable_whisper/text_output.py` & `stable-ts-2.5.0/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/stable_whisper/timing.py` & `stable-ts-2.5.0/stable_whisper/timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,61 +196,80 @@
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         audio_features: torch.Tensor = None,
         ts_num: int = 0,
         ts_noise: float = 0.1,
         min_word_dur: float = 0.1,
         split_callback: Callable = None,
+        gap_padding: str = ' ...',
         **kwargs,
 ):
     if len(segments) == 0:
         return
 
     if min_word_dur is None:
         min_word_dur = 0
 
-    for segment in segments:
-        segment['words'] = []
-
     if prepend_punctuations is None:
         prepend_punctuations = "\"'“¿([{-"
 
     if append_punctuations is None:
         append_punctuations = "\"'.。,，!！?？:：”)]}、"
 
-    text_tokens, token_split, seg_indices = split_word_tokens(segments, tokenizer,
-                                                              padding=' ...', split_callback=split_callback)
-
-    alignment = find_alignment_stable(model, tokenizer, text_tokens, mel, num_samples,
-                                      **kwargs,
-                                      token_split=token_split,
-                                      audio_features=audio_features,
-                                      ts_num=ts_num,
-                                      ts_noise=ts_noise)
-    alt_beginning_alignment = pop_empty_alignment(alignment)
-
-    merge_punctuations(alignment, prepend_punctuations, append_punctuations)
-
-    time_offset = segments[0]["seek"]
-
-    assert len(alignment) == len(seg_indices) and len(segments) == len(alt_beginning_alignment)
-    for i, timing in zip(seg_indices, alignment):
-        if len(timing.tokens) != 0:
-            start = timing.start
-            end = timing.end
-            if len(segments[i]['words']) == 0 and ((end - start) < min_word_dur):
-                start = alt_beginning_alignment[i].start
-            segments[i]['words'].append(
-                dict(
-                    word=timing.word,
-                    start=round(time_offset + start, 3),
-                    end=round(time_offset + end, 3),
-                    probability=timing.probability,
-                    tokens=timing.tokens
+    def align():
+        for seg in segments:
+            seg['words'] = []
+
+        text_tokens, token_split, seg_indices = split_word_tokens(segments, tokenizer,
+                                                                  padding=gap_padding, split_callback=split_callback)
+
+        alignment = find_alignment_stable(model, tokenizer, text_tokens, mel, num_samples,
+                                          **kwargs,
+                                          token_split=token_split,
+                                          audio_features=audio_features,
+                                          ts_num=ts_num,
+                                          ts_noise=ts_noise)
+        alt_beginning_alignment = pop_empty_alignment(alignment)
+
+        merge_punctuations(alignment, prepend_punctuations, append_punctuations)
+
+        time_offset = segments[0]["seek"]
+
+        assert len(alignment) == len(seg_indices)
+        assert (gap_padding is None or len(segments) == len(alt_beginning_alignment))
+        for i, timing in zip(seg_indices, alignment):
+            if len(timing.tokens) != 0:
+                start = timing.start
+                end = timing.end
+                if (
+                        len(segments[i]['words']) == 0 and
+                        ((end - start) < min_word_dur) and
+                        len(alt_beginning_alignment)
+                ):
+                    start = alt_beginning_alignment[i].start
+                segments[i]['words'].append(
+                    dict(
+                        word=timing.word,
+                        start=round(time_offset + start, 3),
+                        end=round(time_offset + end, 3),
+                        probability=timing.probability,
+                        tokens=timing.tokens
+                    )
                 )
+
+    align()
+    if (
+            gap_padding is not None and
+            any(
+                (word['end'] - word['start']) < min_word_dur
+                for seg in segments
+                for word in seg['words']
             )
+    ):
+        gap_padding = None
+        align()
 
     for segment in segments:
         if len(words := segment["words"]) > 0:
             # adjust the segment-level timestamps based on the word-level timestamps
             segment["start"] = words[0]["start"]
             segment["end"] = words[-1]["end"]
```

### Comparing `stable-ts-2.4.1/stable_whisper/video_output.py` & `stable-ts-2.5.0/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.1/stable_whisper/whisper_word_level.py` & `stable-ts-2.5.0/stable_whisper/whisper_word_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         vad_onnx: bool = False,
         min_word_dur: float = 0.1,
         only_voice_freq: bool = False,
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         mel_first: bool = False,
         split_callback: Callable = None,
+        suppress_ts_tokens: bool = True,
+        gap_padding: str = ' ...',
         **decode_options) \
         -> WhisperResult:
     """
     Transcribe an audio file using Whisper
 
     Parameters
     ----------
@@ -176,14 +178,23 @@
         Used if odd behavior seen in stable-ts but not in whisper, but use significantly more memory for long audio.
 
     split_callback: Callable
         Custom callback for grouping tokens up with their corresponding words.
         Takes argument: list of tokens; default tokenizer
         Returns a tuple pair containing: list of words; list of token groups (i.e. each group is list of token(s))
 
+    suppress_ts_tokens: bool
+        Whether to use silence mask to suppress silent timestamp tokens during inference. (Default: True)
+        Reduces hallucinations in some cases,
+            but also can reduce 'verbatimness' (i.e. ignores disfluencies and repetitions).
+
+    gap_padding: str
+        Padding prepend to each segments for word timing alignment. (Default: ' ...')
+        Used to reduce the probability of model predicting timestamps earlier than the first utterance.
+
     decode_options: dict
         Keyword arguments to construct `DecodingOptions` instances
 
     Returns
     -------
     A dictionary containing the resulting text ("text") and segment-level details ("segments"), and
     the spoken language ("language"), which is detected when `decode_options["language"]` is None.
@@ -281,15 +292,15 @@
             else:
                 # disable best_of when t == 0
                 kwargs.pop("best_of", None)
 
             options = DecodingOptions(**kwargs, temperature=t)
             decode_result, audio_features = model.decode(seg,
                                                          options,
-                                                         ts_token_mask=ts_token_mask,
+                                                         ts_token_mask=ts_token_mask if suppress_ts_tokens else None,
                                                          audio_features=audio_features)
 
             needs_fallback = False
             if (
                     compression_ratio_threshold is not None
                     and decode_result.compression_ratio > compression_ratio_threshold
             ):
@@ -500,15 +511,16 @@
                     mel=mel_segment,
                     num_samples=segment_samples,
                     prepend_punctuations=prepend_punctuations,
                     append_punctuations=append_punctuations,
                     audio_features=audio_features,
                     ts_num=ts_num,
                     ts_noise=ts_noise,
-                    split_callback=split_callback
+                    split_callback=split_callback,
+                    gap_padding=gap_padding
                 )
 
             if segment_silence_timing is not None:
                 for seg_i, segment in enumerate(current_segments):
                     current_segments[seg_i] = (
                         Segment(**segment)
                         .suppress_silence(
@@ -682,14 +694,19 @@
                         help="language spoken in the audio, specify None to perform language detection")
 
     parser.add_argument("--prepend_punctuations", '-pp', type=str, default="\"'“¿([{-",
                         help="Punctuations to prepend to next word")
     parser.add_argument("--append_punctuations", '-ap', type=str, default="\"'.。,，!！?？:：”)]}、",
                         help="Punctuations to append to previous word")
 
+    parser.add_argument("--gap_padding", type=str, default=" ...",
+                        help="padding prepend to each segments for word timing alignment;"
+                             "used to reduce the probability of model predicting timestamps "
+                             "earlier than the first utterance")
+
     parser.add_argument("--word_timestamps", type=str2bool, default=True,
                         help="extract word-level timestamps using the cross-attention pattern and dynamic time warping,"
                              "and include the timestamps for each word in each segment;"
                              "disabling this will prevent segments from splitting/merging properly.")
 
     parser.add_argument("--regroup", type=str2bool, default=True,
                         help="regroup all words into segments with more natural boundaries;"
@@ -703,14 +720,19 @@
     parser.add_argument('--suppress_silence', type=str2bool, default=True,
                         help="whether to suppress timestamp where audio is silent at segment-level"
                              "and word-level if [suppress_word_ts]=True")
     parser.add_argument('--suppress_word_ts', type=str2bool, default=True,
                         help="whether to suppress timestamps where audio is silent at word-level; "
                              "ignored if [suppress_silence]=False")
 
+    parser.add_argument('--suppress_ts_tokens', type=str2bool, default=True,
+                        help="whether to use silence mask to suppress silent timestamp tokens during inference; "
+                             "increases word accuracy in some cases, but tends reduce 'verbatimness' of the transcript"
+                             "ignored if [suppress_silence]=False")
+
     parser.add_argument("--q_levels", type=int, default=20,
                         help="quantization levels for generating timestamp suppression mask; "
                              "acts as a threshold to marking sound as silent;"
                              "fewer levels will increase the threshold of volume at which to mark a sound as silent")
 
     parser.add_argument("--k_size", type=int, default=5,
                         help="Kernel size for average pooling waveform to generate suppression mask; "
```

