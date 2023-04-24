# Comparing `tmp/tzconv-1.3.tar.gz` & `tmp/tzconv-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzconv-1.3.tar", last modified: Sun Apr 23 18:54:27 2023, max compression
+gzip compressed data, was "tzconv-1.3.1.tar", last modified: Mon Apr 24 19:05:58 2023, max compression
```

## Comparing `tzconv-1.3.tar` & `tzconv-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-23 18:54:27.907143 tzconv-1.3/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3935 2023-04-23 18:54:27.907143 tzconv-1.3/PKG-INFO
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3696 2023-04-23 18:44:19.000000 tzconv-1.3/README.md
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       38 2023-04-23 18:54:27.907143 tzconv-1.3/setup.cfg
--rw-r--r--   0 bigmac    (1000) bigmac    (1000)      608 2023-04-23 18:47:13.000000 tzconv-1.3/setup.py
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-23 18:54:27.907143 tzconv-1.3/tzconv/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     9457 2023-04-23 18:49:57.000000 tzconv-1.3/tzconv/__init__.py
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     2716 2023-04-23 18:16:07.000000 tzconv-1.3/tzconv/test_tzconv.py
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-23 18:54:27.907143 tzconv-1.3/tzconv.egg-info/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3935 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/PKG-INFO
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)      241 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/SOURCES.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        1 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/dependency_links.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       39 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/entry_points.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        6 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/requires.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        7 2023-04-23 18:54:27.000000 tzconv-1.3/tzconv.egg-info/top_level.txt
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-24 19:05:58.607799 tzconv-1.3.1/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3937 2023-04-24 19:05:58.607799 tzconv-1.3.1/PKG-INFO
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3696 2023-04-23 18:44:19.000000 tzconv-1.3.1/README.md
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       38 2023-04-24 19:05:58.607799 tzconv-1.3.1/setup.cfg
+-rw-r--r--   0 bigmac    (1000) bigmac    (1000)      610 2023-04-24 19:05:13.000000 tzconv-1.3.1/setup.py
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-24 19:05:58.607799 tzconv-1.3.1/tzconv/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     9395 2023-04-24 18:40:01.000000 tzconv-1.3.1/tzconv/__init__.py
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3712 2023-04-24 18:37:16.000000 tzconv-1.3.1/tzconv/test_tzconv.py
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-24 19:05:58.607799 tzconv-1.3.1/tzconv.egg-info/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3937 2023-04-24 19:05:58.000000 tzconv-1.3.1/tzconv.egg-info/PKG-INFO
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)      241 2023-04-24 19:05:58.000000 tzconv-1.3.1/tzconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        1 2023-04-24 19:05:58.000000 tzconv-1.3.1/tzconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       39 2023-04-24 19:05:58.000000 tzconv-1.3.1/tzconv.egg-info/entry_points.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        6 2023-04-24 19:05:58.000000 tzconv-1.3.1/tzconv.egg-info/requires.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        7 2023-04-24 19:05:58.000000 tzconv-1.3.1/tzconv.egg-info/top_level.txt
```

### Comparing `tzconv-1.3/PKG-INFO` & `tzconv-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzconv
-Version: 1.3
+Version: 1.3.1
 Summary: command-line tool to convert a date and time to several time zones at once
 Home-page: https://codeberg.org/gnyeki/tzconv
 Author: Gabor Nyeki
 Description-Content-Type: text/markdown
 
 
 # `tzconv`: convert a date and time to several time zones at once
```

### Comparing `tzconv-1.3/README.md` & `tzconv-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tzconv-1.3/setup.py` & `tzconv-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as handle:
     readme = handle.read()
 
 setup(
     name="tzconv",
-    version="1.3",
+    version="1.3.1",
     description="command-line tool to convert a date and time to several time zones at once",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Gabor Nyeki",
     url="https://codeberg.org/gnyeki/tzconv",
     packages=["tzconv"],
     install_requires=["click"],
```

### Comparing `tzconv-1.3/tzconv/__init__.py` & `tzconv-1.3.1/tzconv/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import re
 import datetime as dt
 import zoneinfo as zi
 
-from typing import List, cast
+from typing import List, Set, cast
 
 import click
 
 
 def make_datetime(date_time: str, timezone: zi.ZoneInfo) -> dt.datetime:
     """Construct a `datetime` instance from a date-time string formatted
     as `YYYY-MM-DD HH:MM` or `HH:MM` and attach timezone information."""
@@ -42,25 +42,17 @@
 
     tz_name = obj.tzname()
     tz_key = cast(zi.ZoneInfo, obj.tzinfo).key
 
     return f"{tz_name}: {obj.strftime('%Y-%m-%d %H:%M')} ({tz_key})"
 
 
-def match_time_zone_prefix(pattern: str, time_zone: str) -> bool:
-    """Predicate that returns True if `pattern` is a prefix of
-    `time_zone`.  Case-sensitive."""
-
-    return time_zone.startswith(pattern)
-
-
-def match_time_zone_abbreviation(pattern: str,
-                                 time_zone: str) -> bool:
-    """Predicate that returns True if `pattern` is an abbreviation of
-    `time_zone`.  Case-sensitive."""
+def match_time_zone(pattern: str, time_zone: str) -> bool:
+    """Predicate that returns True if `pattern` matches `time_zone`.
+    Case-sensitive."""
 
     def get_segments(string: str) -> List[str]:
         return re.findall(r"/?[a-z_]+", string, flags=re.IGNORECASE)
 
     def get_words(string: str) -> List[str]:
         return re.findall(r"[_]?[a-z]+", string, flags=re.IGNORECASE)
 
@@ -93,15 +85,15 @@
         pattern_segment = pattern_segments[pattern_index]
         time_zone_segment = time_zone_segments[time_zone_index]
 
         # Check if the pattern segment is a prefix of the time zone
         # segment.  E.g., "Lo" for "Los_Angeles".
         #
 
-        if match_time_zone_prefix(pattern_segment, time_zone_segment):
+        if time_zone_segment.startswith(pattern_segment):
             pattern_index += 1
             time_zone_index += 1
 
             continue
 
         # Check if the pattern segment is the initials of the time zone
         # words.  E.g., "LA" for "Los_Angeles".
@@ -123,82 +115,82 @@
         #
 
         time_zone_words = get_words(time_zone_segment)
 
         if len(pattern_words) <= len(time_zone_words):
             for pattern_word, time_zone_word in zip(pattern_words,
                                                     time_zone_words):
-                if not match_time_zone_prefix(pattern_word,
-                                              time_zone_word):
+                if not time_zone_word.startswith(pattern_word):
                     break
             else:
                 pattern_index += 1
                 time_zone_index += 1
 
                 continue
 
         # Try this pattern segment on the next time zone segment.
         #
         time_zone_index += 1
 
     return True
 
 
-def match_time_zone(pattern: str, time_zone: str) -> bool:
-    """Predicate that returns True if `pattern` matches `time_zone`.
-    Case-insensitive."""
+def get_time_zones(pattern: str, time_zones: Set[str]) -> Set[str]:
+    """Get the subset of `time_zones` that matches `pattern`.
+    Case-insensitive and treats hyphens and underscores as the same."""
 
-    lowercase_pattern = pattern.lower().replace("-", "_")
-    lowercase_time_zone = time_zone.lower().replace("-", "_")
+    def normalize(string: str) -> str:
+        return string.lower().replace("-", "_")
 
-    return (match_time_zone_prefix(lowercase_pattern,
-                                   lowercase_time_zone)
-            or match_time_zone_abbreviation(lowercase_pattern,
-                                            lowercase_time_zone))
+    normalized_pattern = normalize(pattern)
 
+    return {
+        name
+        for name in time_zones
+        if match_time_zone(
+                normalized_pattern, normalize(name))
+    }
 
-def get_time_zones(pattern: str | None) -> set:
-    """Get the names of those time zones that match `pattern`.  If
-    `pattern` is None, then get all available time zones."""
 
-    time_zones = zi.available_timezones()
+def get_unique_time_zone(pattern: str, time_zones: Set[str]) -> str:
+    """Get the unique value from `time_zones` that matches `pattern`.
+    Raises `ValueError` if there is no match or there is more than one
+    match and none of them are exact.  Case-insensitive and treats
+    hyphens and underscores as the same."""
 
-    if pattern is not None:
-        time_zones = set(
-            name
-            for name in time_zones
-            if match_time_zone(pattern, name))
-
-    return time_zones
+    matching_tz = get_time_zones(pattern, time_zones)
 
+    if len(matching_tz) == 0:
+        raise ValueError(f"No available time zone matches '{pattern}'.")
 
-def get_time_zone(pattern: str) -> str:
-    """Get the name of the time zone that matches `pattern`.  Raises
-    `ValueError` if there is no match or more than one match."""
+    if len(matching_tz) == 1:
+        return matching_tz.pop()
 
-    time_zones = get_time_zones(pattern)
+    # More than one match.
+    #
 
-    if len(time_zones) == 0:
-        raise ValueError(f"No available time zone matches '{pattern}'.")
+    exact_match = {
+        x for x in matching_tz if x.lower() == pattern.lower()
+    }
 
-    if len(time_zones) > 1:
-        raise ValueError(
-            "Multiple available time zones are matched by "
-            + f"'{pattern}': {', '.join(sorted(time_zones))}.")
+    if len(exact_match) == 1:
+        return exact_match.pop()
 
-    return time_zones.pop()
+    raise ValueError(
+        f"Multiple available time zones are matched by '{pattern}': "
+        + f"{', '.join(sorted(matching_tz))}.")
 
 
-def print_time_zones(pattern: str | None) -> None:
+def print_time_zones(pattern: str | None, time_zones: Set[str]) -> None:
     """Print all available time zones whose names match `pattern`.  If
     `pattern` is `None`, then print everything."""
 
-    time_zones = get_time_zones(pattern)
-
     if pattern is not None:
+        time_zones = get_time_zones(pattern, time_zones)
+
         if len(time_zones) == 0:
             print(f"No available time zone matches '{pattern}'.")
             return
 
         print("The following time zones are available that match "
               + f"'{pattern}':\n")
     else:
@@ -248,37 +240,46 @@
 @click.option("-f", "--from-tz", required=False, type=str,
               help="The name of the time zone to convert from.")
 @click.option("-t", "--to-tz", required=False, type=str, multiple=True,
               help=("The name of a time zone to convert to. Can use "
                     + "this option multiple times in order to specify "
                     + "several."))
 @click.argument("date_time", required=False, type=str)
-def main(from_tz, to_tz, date_time, list_tz=False, debug=False):
+def main(from_tz: str | None, to_tz: List[str], date_time: str | None,
+         list_tz: bool = False, debug: bool = False) -> None:
     if not debug:
         sys.tracebacklimit = 0
 
     if list_tz:
         if from_tz is not None or len(to_tz) > 0:
             print_argument_error_and_exit(
                 "--list-tz cannot be used together with --from-tz or "
                 "--to-tz.")
 
-        print_time_zones(date_time)
+        print_time_zones(
+            pattern=date_time,
+            time_zones=zi.available_timezones())
     elif from_tz is None and len(to_tz) == 0:
         print_argument_error_and_exit(
             "Must specify either --list-tz or --from-tz and --to-tz.")
     elif from_tz is None:
         print_argument_error_and_exit(
             "Must specify --from-tz if using --to-tz.")
     elif len(to_tz) == 0:
         print_argument_error_and_exit(
             "Must specify --to-tz if using --from-tz.")
     else:
-        from_tz_obj = zi.ZoneInfo(get_time_zone(from_tz))
-        to_tz_objs = [zi.ZoneInfo(get_time_zone(x)) for x in to_tz]
+        all_time_zones = zi.available_timezones()
+
+        from_tz_obj = zi.ZoneInfo(get_unique_time_zone(from_tz,
+                                                       all_time_zones))
+        to_tz_objs = [
+            zi.ZoneInfo(get_unique_time_zone(x, all_time_zones))
+            for x in to_tz
+        ]
 
         if date_time is None:
             base_dt = dt.datetime.now(tz=from_tz_obj)
         else:
             base_dt = make_datetime(date_time, from_tz_obj)
 
         print(format_datetime(base_dt))
```

### Comparing `tzconv-1.3/tzconv/test_tzconv.py` & `tzconv-1.3.1/tzconv/test_tzconv.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 
 
 class TestMatchTimeZone(unittest.TestCase):
     def test_different_pattern_is_not_matched(self):
         self.assertFalse(m.match_time_zone("foo", "asdf"))
         self.assertFalse(m.match_time_zone("foo/baz", "foo/bar"))
 
-    def test_match_is_case_insensitive(self):
-        self.assertTrue(m.match_time_zone("fOO", "Foo"))
-        self.assertTrue(m.match_time_zone("Foo/bAR", "Foo/Bar"))
-
     def test_prefix_pattern_matches_name(self):
         self.assertTrue(m.match_time_zone("foo", "foobar"))
         self.assertTrue(m.match_time_zone("foo", "foo/bar"))
         self.assertTrue(m.match_time_zone("foo", "foob/ar"))
         self.assertTrue(m.match_time_zone("foo/b", "foo/bar"))
 
     def test_initials_pattern_match_name(self):
@@ -49,7 +45,39 @@
 
     def test_pattern_cannot_insert_nonexisting_segments(self):
         self.assertFalse(m.match_time_zone("foo/bar/baz", "foo/baz"))
         self.assertFalse(m.match_time_zone("f/bar/baz", "foo/baz"))
         self.assertFalse(m.match_time_zone("f/bar", "foo/baz"))
         self.assertFalse(m.match_time_zone("foo/bar/baz", "bar/baz"))
         self.assertFalse(m.match_time_zone("f/bar/baz", "bar/baz"))
+
+
+class GetUniqueTimeZone(unittest.TestCase):
+    def test_nonunique_inexact_match_raises_error(self):
+        with self.assertRaises(ValueError):
+            m.get_unique_time_zone("foo/bar", {"foo/barre", "foo/bart"})
+
+    def test_nonunique_exact_match_works(self):
+        self.assertEqual(
+            "foo/bar",
+            m.get_unique_time_zone("foo/bar", {"foo/bar", "foo/bart"}))
+
+    def test_unique_match_works(self):
+        self.assertEqual(
+            "foo/bart",
+            m.get_unique_time_zone("foo/bart",
+                                   {"foo/barre", "foo/bart"}))
+
+    def test_no_match_raises_error(self):
+        with self.assertRaises(ValueError):
+            m.get_unique_time_zone("foo/bar", {"foo/baz", "bar"})
+
+    def get_unique_time_zone_is_case_insensitive(self):
+        self.assertEqual(
+            "Foo/Bar",
+            m.get_unique_time_zone("foo/bar", {"Foo/Bar", "Foo/Bart"}))
+        self.assertEqual(
+            "Foo/Bar",
+            m.get_unique_time_zone("fOO/bAR", {"Foo/Bar", "Foo/Bart"}))
+        self.assertEqual(
+            "Foo/Bart",
+            m.get_unique_time_zone("foo/bart", {"Foo/Bar", "Foo/Bart"}))
```

### Comparing `tzconv-1.3/tzconv.egg-info/PKG-INFO` & `tzconv-1.3.1/tzconv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzconv
-Version: 1.3
+Version: 1.3.1
 Summary: command-line tool to convert a date and time to several time zones at once
 Home-page: https://codeberg.org/gnyeki/tzconv
 Author: Gabor Nyeki
 Description-Content-Type: text/markdown
 
 
 # `tzconv`: convert a date and time to several time zones at once
```

