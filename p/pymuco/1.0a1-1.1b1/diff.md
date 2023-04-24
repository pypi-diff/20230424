# Comparing `tmp/pymuco-1.0A1.tar.gz` & `tmp/pymuco-1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymuco-1.0A1.tar", last modified: Sat Apr 30 13:08:52 2022, max compression
+gzip compressed data, was "pymuco-1.1b1.tar", last modified: Mon Apr 24 09:28:52 2023, max compression
```

## Comparing `pymuco-1.0A1.tar` & `pymuco-1.1b1.tar`

### file list

```diff
@@ -1,6 +1,29 @@
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2022-04-30 13:08:52.000000 pymuco-1.0A1/
--rw-r--r--   0 germanmargon   (501) staff       (20)      200 2022-04-30 13:08:52.000000 pymuco-1.0A1/PKG-INFO
-drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2022-04-30 13:08:52.000000 pymuco-1.0A1/pymuco/
--rw-r--r--   0 germanmargon   (501) staff       (20)        0 2022-04-30 13:04:11.000000 pymuco-1.0A1/pymuco/__init__.py
--rw-r--r--   0 germanmargon   (501) staff       (20)        0 2022-04-30 13:04:15.000000 pymuco-1.0A1/pymuco/file.py
--rw-r--r--   0 germanmargon   (501) staff       (20)      246 2022-04-30 13:07:40.000000 pymuco-1.0A1/setup.py
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-24 09:28:52.866638 pymuco-1.1b1/
+-rw-r--r--   0 germanmargon   (501) staff       (20)     1505 2023-04-24 09:26:41.000000 pymuco-1.1b1/LICENSE
+-rw-r--r--   0 germanmargon   (501) staff       (20)      875 2023-04-24 09:28:52.866215 pymuco-1.1b1/PKG-INFO
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-24 09:28:52.864103 pymuco-1.1b1/pymuco/
+-rw-r--r--   0 germanmargon   (501) staff       (20)    17825 2023-04-20 07:51:40.000000 pymuco-1.1b1/pymuco/AudioConverter.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7956 2023-04-20 07:33:57.000000 pymuco-1.1b1/pymuco/Chord.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7420 2023-04-19 21:10:47.000000 pymuco-1.1b1/pymuco/CircleOfFifths.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     5230 2023-04-19 21:07:01.000000 pymuco-1.1b1/pymuco/Enharmonic.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     4087 2023-04-19 21:02:01.000000 pymuco-1.1b1/pymuco/EnharmonicMapping.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)    17548 2023-04-19 20:59:04.000000 pymuco-1.1b1/pymuco/Interval.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     8558 2023-04-19 20:46:05.000000 pymuco-1.1b1/pymuco/KeySignature.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     5690 2023-04-20 07:35:27.000000 pymuco-1.1b1/pymuco/MIDIUtils.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3752 2023-04-19 20:36:53.000000 pymuco-1.1b1/pymuco/MusicComputationNotation.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     2886 2023-04-19 20:31:25.000000 pymuco-1.1b1/pymuco/MusicData.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7514 2023-04-20 07:43:41.000000 pymuco-1.1b1/pymuco/NoteDuration.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3600 2023-04-20 10:05:17.000000 pymuco-1.1b1/pymuco/NoteFrequencyConverter.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     8081 2023-04-20 11:34:01.000000 pymuco-1.1b1/pymuco/NoteMapping.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     3465 2023-04-20 11:34:09.000000 pymuco-1.1b1/pymuco/Player.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)    12792 2023-04-20 10:55:29.000000 pymuco-1.1b1/pymuco/Scale.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)     7438 2023-04-20 11:33:33.000000 pymuco-1.1b1/pymuco/ScientificPitchNotation.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)      764 2023-04-20 12:09:54.000000 pymuco-1.1b1/pymuco/Tonality.py
+-rw-r--r--   0 germanmargon   (501) staff       (20)        0 2022-12-29 20:39:36.000000 pymuco-1.1b1/pymuco/__init__ .py
+drwxr-xr-x   0 germanmargon   (501) staff       (20)        0 2023-04-24 09:28:52.865733 pymuco-1.1b1/pymuco.egg-info/
+-rw-r--r--   0 germanmargon   (501) staff       (20)      875 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/PKG-INFO
+-rw-r--r--   0 germanmargon   (501) staff       (20)      552 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/SOURCES.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)        1 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/dependency_links.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)        7 2023-04-24 09:28:52.000000 pymuco-1.1b1/pymuco.egg-info/top_level.txt
+-rw-r--r--   0 germanmargon   (501) staff       (20)       38 2023-04-24 09:28:52.866730 pymuco-1.1b1/setup.cfg
+-rw-r--r--   0 germanmargon   (501) staff       (20)      951 2023-04-22 20:58:24.000000 pymuco-1.1b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

