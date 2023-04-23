# Comparing `tmp/integerbook-0.0.2.tar.gz` & `tmp/integerbook-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integerbook-0.0.2.tar", last modified: Thu Apr  6 22:25:59 2023, max compression
+gzip compressed data, was "integerbook-0.0.3.tar", last modified: Sun Apr 23 23:25:48 2023, max compression
```

## Comparing `integerbook-0.0.2.tar` & `integerbook-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.839844 integerbook-0.0.2/
--rw-r--r--   0 jvo        (501) staff       (20)    35149 2022-03-18 13:05:53.000000 integerbook-0.0.2/LICENSE
--rw-r--r--   0 jvo        (501) staff       (20)       84 2023-04-02 11:42:30.000000 integerbook-0.0.2/MANIFEST.in
--rw-r--r--   0 jvo        (501) staff       (20)    42493 2023-04-06 22:25:59.839115 integerbook-0.0.2/PKG-INFO
--rw-r--r--   0 jvo        (501) staff       (20)     1479 2023-03-21 13:10:54.000000 integerbook-0.0.2/README.md
--rw-r--r--   0 jvo        (501) staff       (20)      645 2023-04-06 22:25:44.000000 integerbook-0.0.2/pyproject.toml
--rw-r--r--   0 jvo        (501) staff       (20)       38 2023-04-06 22:25:59.840016 integerbook-0.0.2/setup.cfg
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.781892 integerbook-0.0.2/src/
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.793846 integerbook-0.0.2/src/integerbook/
--rw-r--r--   0 jvo        (501) staff       (20)     2475 2023-03-31 14:26:15.000000 integerbook-0.0.2/src/integerbook/CanvasCreator.py
--rw-r--r--   0 jvo        (501) staff       (20)     5918 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/LocationFinder.py
--rw-r--r--   0 jvo        (501) staff       (20)     9562 2023-04-06 22:08:28.000000 integerbook-0.0.2/src/integerbook/Settings.py
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/__init__.py
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.806069 integerbook-0.0.2/src/integerbook/auxiliary_scripts/
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)     6139 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/chordTypes.py
--rw-r--r--   0 jvo        (501) staff       (20)      680 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/createBatchJson.py
--rw-r--r--   0 jvo        (501) staff       (20)      173 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/printSettings.py
--rw-r--r--   0 jvo        (501) staff       (20)     1463 2023-03-28 15:56:16.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/runMultiple.py
--rw-r--r--   0 jvo        (501) staff       (20)     3588 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/separateRealbook.py
--rw-r--r--   0 jvo        (501) staff       (20)      537 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/setMode.py
--rw-r--r--   0 jvo        (501) staff       (20)     1855 2023-03-28 15:56:16.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/setModes.py
--rw-r--r--   0 jvo        (501) staff       (20)     1544 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/auxiliary_scripts/writeTexFile.py
--rw-r--r--   0 jvo        (501) staff       (20)      709 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/fontDimensions.json
--rw-r--r--   0 jvo        (501) staff       (20)     1374 2023-03-31 15:07:57.000000 integerbook-0.0.2/src/integerbook/fontSettings.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.806887 integerbook-0.0.2/src/integerbook/fonts/
--rw-r--r--   0 jvo        (501) staff       (20)     6148 2023-04-02 10:13:05.000000 integerbook-0.0.2/src/integerbook/fonts/.DS_Store
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.807965 integerbook-0.0.2/src/integerbook/fonts/Realbook/
--rw-r--r--   0 jvo        (501) staff       (20)    66232 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/fonts/Realbook/Realbook.ttf
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.811404 integerbook-0.0.2/src/integerbook/fonts/symbola/
--rw-r--r--   0 jvo        (501) staff       (20)  2240100 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/fonts/symbola/Symbola.ttf
--rw-r--r--   0 jvo        (501) staff       (20)     2093 2023-04-06 22:23:15.000000 integerbook-0.0.2/src/integerbook/main.py
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.837138 integerbook-0.0.2/src/integerbook/plotter/
--rw-r--r--   0 jvo        (501) staff       (20)    13336 2023-03-28 15:56:16.000000 integerbook-0.0.2/src/integerbook/plotter/PlotterBarLines.py
--rw-r--r--   0 jvo        (501) staff       (20)     1741 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/plotter/PlotterBase.py
--rw-r--r--   0 jvo        (501) staff       (20)    14194 2023-03-28 15:56:16.000000 integerbook-0.0.2/src/integerbook/plotter/PlotterChords.py
--rw-r--r--   0 jvo        (501) staff       (20)     1367 2023-03-28 15:56:16.000000 integerbook-0.0.2/src/integerbook/plotter/PlotterMain.py
--rw-r--r--   0 jvo        (501) staff       (20)     3121 2023-03-28 15:56:16.000000 integerbook-0.0.2/src/integerbook/plotter/PlotterMetadata.py
--rw-r--r--   0 jvo        (501) staff       (20)    22712 2023-03-31 15:07:40.000000 integerbook-0.0.2/src/integerbook/plotter/PlotterNotes.py
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/plotter/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)    10373 2023-03-28 15:54:15.000000 integerbook-0.0.2/src/integerbook/plotter/patches.py
--rw-r--r--   0 jvo        (501) staff       (20)    10347 2023-04-06 22:23:15.000000 integerbook-0.0.2/src/integerbook/runSingle.py
--rw-r--r--   0 jvo        (501) staff       (20)     1455 2023-03-31 14:51:33.000000 integerbook-0.0.2/src/integerbook/settings.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-06 22:25:59.797708 integerbook-0.0.2/src/integerbook.egg-info/
--rw-r--r--   0 jvo        (501) staff       (20)    42493 2023-04-06 22:25:59.000000 integerbook-0.0.2/src/integerbook.egg-info/PKG-INFO
--rw-r--r--   0 jvo        (501) staff       (20)     1390 2023-04-06 22:25:59.000000 integerbook-0.0.2/src/integerbook.egg-info/SOURCES.txt
--rw-r--r--   0 jvo        (501) staff       (20)        1 2023-04-06 22:25:59.000000 integerbook-0.0.2/src/integerbook.egg-info/dependency_links.txt
--rw-r--r--   0 jvo        (501) staff       (20)       11 2023-04-06 22:25:59.000000 integerbook-0.0.2/src/integerbook.egg-info/requires.txt
--rw-r--r--   0 jvo        (501) staff       (20)       12 2023-04-06 22:25:59.000000 integerbook-0.0.2/src/integerbook.egg-info/top_level.txt
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.789423 integerbook-0.0.3/
+-rw-r--r--   0 jvo        (501) staff       (20)    35149 2022-03-18 13:05:53.000000 integerbook-0.0.3/LICENSE
+-rw-r--r--   0 jvo        (501) staff       (20)       84 2023-04-23 18:25:14.000000 integerbook-0.0.3/MANIFEST.in
+-rw-r--r--   0 jvo        (501) staff       (20)    42511 2023-04-23 23:25:48.788907 integerbook-0.0.3/PKG-INFO
+-rw-r--r--   0 jvo        (501) staff       (20)     1497 2023-04-23 18:25:14.000000 integerbook-0.0.3/README.md
+-rw-r--r--   0 jvo        (501) staff       (20)      645 2023-04-23 23:24:26.000000 integerbook-0.0.3/pyproject.toml
+-rw-r--r--   0 jvo        (501) staff       (20)       38 2023-04-23 23:25:48.789609 integerbook-0.0.3/setup.cfg
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.692858 integerbook-0.0.3/src/
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.710028 integerbook-0.0.3/src/integerbook/
+-rw-r--r--   0 jvo        (501) staff       (20)     2475 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/CanvasCreator.py
+-rw-r--r--   0 jvo        (501) staff       (20)     5918 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/LocationFinder.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10154 2023-04-23 23:09:59.000000 integerbook-0.0.3/src/integerbook/Settings.py
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1186 2023-04-23 18:31:12.000000 integerbook-0.0.3/src/integerbook/alternativeSymbols.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.723699 integerbook-0.0.3/src/integerbook/auxiliary_scripts/
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)      756 2023-04-23 22:57:26.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/changeNameMxl.py
+-rw-r--r--   0 jvo        (501) staff       (20)     6139 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/chordTypes.py
+-rw-r--r--   0 jvo        (501) staff       (20)      680 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/createBatchJson.py
+-rw-r--r--   0 jvo        (501) staff       (20)      173 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/printSettings.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1619 2023-04-23 21:43:41.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/runMultiple.py
+-rw-r--r--   0 jvo        (501) staff       (20)     3588 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/separateRealbook.py
+-rw-r--r--   0 jvo        (501) staff       (20)      537 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/setMode.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1855 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/setModes.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1544 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/auxiliary_scripts/writeTexFile.py
+-rw-r--r--   0 jvo        (501) staff       (20)      709 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/fontDimensions.json
+-rw-r--r--   0 jvo        (501) staff       (20)     1485 2023-04-23 19:15:02.000000 integerbook-0.0.3/src/integerbook/fontSettings.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.724714 integerbook-0.0.3/src/integerbook/fonts/
+-rw-r--r--   0 jvo        (501) staff       (20)     6148 2023-04-02 10:13:05.000000 integerbook-0.0.3/src/integerbook/fonts/.DS_Store
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.725621 integerbook-0.0.3/src/integerbook/fonts/Realbook/
+-rw-r--r--   0 jvo        (501) staff       (20)    66232 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/fonts/Realbook/Realbook.ttf
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.728002 integerbook-0.0.3/src/integerbook/fonts/symbola/
+-rw-r--r--   0 jvo        (501) staff       (20)  2240100 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/fonts/symbola/Symbola.ttf
+-rw-r--r--   0 jvo        (501) staff       (20)     2093 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/main.py
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.782059 integerbook-0.0.3/src/integerbook/plotter/
+-rw-r--r--   0 jvo        (501) staff       (20)    13336 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterBarLines.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1741 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterBase.py
+-rw-r--r--   0 jvo        (501) staff       (20)    14571 2023-04-23 23:16:48.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterChords.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1367 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterMain.py
+-rw-r--r--   0 jvo        (501) staff       (20)     3121 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterMetadata.py
+-rw-r--r--   0 jvo        (501) staff       (20)    23638 2023-04-23 21:51:35.000000 integerbook-0.0.3/src/integerbook/plotter/PlotterNotes.py
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10373 2023-04-23 18:25:14.000000 integerbook-0.0.3/src/integerbook/plotter/patches.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10593 2023-04-23 21:46:46.000000 integerbook-0.0.3/src/integerbook/runSingle.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1580 2023-04-23 23:09:59.000000 integerbook-0.0.3/src/integerbook/settings.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-04-23 23:25:48.713530 integerbook-0.0.3/src/integerbook.egg-info/
+-rw-r--r--   0 jvo        (501) staff       (20)    42511 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/PKG-INFO
+-rw-r--r--   0 jvo        (501) staff       (20)     1481 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/SOURCES.txt
+-rw-r--r--   0 jvo        (501) staff       (20)        1 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/dependency_links.txt
+-rw-r--r--   0 jvo        (501) staff       (20)       11 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/requires.txt
+-rw-r--r--   0 jvo        (501) staff       (20)       12 2023-04-23 23:25:48.000000 integerbook-0.0.3/src/integerbook.egg-info/top_level.txt
```

### Comparing `integerbook-0.0.2/LICENSE` & `integerbook-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/PKG-INFO` & `integerbook-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integerbook
-Version: 0.0.2
+Version: 0.0.3
 Summary: sheet music converter
 Author-email: Jesse van Oostrum <integerbook@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,37 +687,33 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # music-visualisation
 
 This library converts sheet music in musicxml format to visualisations that refer to notes and chords with their relative position within the key of the song. More about how this notational system works [here](https://integerbook.com/about). 
 
-### running the code
-From the root folder of the repository, run the following line in the terminal:
+### installation
 
-``` $ python run.py ```
+1. Download python
+2. install the [integerbook package](https://pypi.org/project/integerbook/0.0.2/) using pip: ``` $ pip install integerbook ```
+3. Download or copy the file ```run.py``` from the repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
 
-This will convert the file "All_Of_Me.musicxml" located in the examples folder and place the result in the root folder of the repository. 
 
-The most important options are the following:
-- -s set song path (can be either .musicxml or .mxl file)
-- -o set output directory  (without "/" at the end)
+### running the code
+1. In the terminal, navigate to the folder where ```run.py``` is stored. 
+2. In the terminal, type: ``` $ python run.py -s <path-to-song>```  e.g.   
+``` $ python run.py -s "/Users/jvo/Documents/music-visualisation/example/Summertime.musicxml" ```
 
-example: 
-``` $ python run.py -s "/Users/jvo/Documents/music-visualisation/example/Summertime.musicxml" -o "/Users/jvo/Downloads/output" ```
+This will convert the musicxml file you specified to a pdf and store it in the current folder. 
 
 Further options include:
+- -o set output directory  (without "/" at the end)
 - -b for bassline output
 - -l for printing lyrics
 - -c for colouring notes according to circle of fifths
-- -r for realbook font (note that you first have to install the font (located in fonts folder))
 - -cn for printing chord notes
 - -cp for printing chord progressions (no melody, 8 measures per line)
 - -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See 'sample/settings.json' for the default settings.
 
-### requirements
-- music21
-- matplotlib
-
 
 ### example musicxml files
 In the folder example, there are some musicxml files that can be used to try out the program.
```

### Comparing `integerbook-0.0.2/pyproject.toml` & `integerbook-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integerbook"
-version = "0.0.2"
+version = "0.0.3"
 description = "sheet music converter"
 readme = "README.md"
 authors = [{ name = "Jesse van Oostrum", email = "integerbook@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `integerbook-0.0.2/src/integerbook/CanvasCreator.py` & `integerbook-0.0.3/src/integerbook/CanvasCreator.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/LocationFinder.py` & `integerbook-0.0.3/src/integerbook/LocationFinder.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/Settings.py` & `integerbook-0.0.3/src/integerbook/Settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,20 +64,19 @@
         self.timeSignatureWithBarlines = settings['timeSignatureWithBarlines']
         self.lyrics = settings['lyrics']
         self.thickBarlines = settings['thickBarlines']
         self.printArranger = settings['printArranger']
         self.xMarginNoteThickBarline = self.widthThickBarline - 0.5 * self.lineWidth0
         self.usePlt = settings["usePlt"]
         self.vMarginLyricsRelative = settings["vMarginLyricsRelative"]
-
+        self.alternativeSymbols = settings["alternativeSymbols"]
+        self.chordVerbosity = settings["chordVerbosity"]
 
         # Font stuff
 
-        self.fontSettings = FontSettings(self.font)
-
         self.fontDirectory = settings['fontDirectory']
         self.fontPath = settings["fontPath"]
         self.fontPathRoman = settings["fontPathRoman"]
         self.fontStyle = settings["fontStyle"]
         self.fontWeight = settings["fontWeight"]
         self.fontSizeAccidentalRelative = settings['fontSizeAccidentalRelative']
 
@@ -106,34 +105,43 @@
         self.fontSizeChords = self.fontSizeChordsPerFontSizeNotes * self.fontSizeNotes
         self.capsizeChord = fD["capsize"] * self.fontSizeChords
         self.fontWidthChord = fD["width"] * self.fontSizeChords
 
         self.capsizeLyric = fDLyrics["capsize"] * self.fontSizeLyrics
         self.fontWidthLyric = fDLyrics["width"] * self.fontSizeLyrics
 
-        self.capsizeType = fD["capsize"] * self.fontSettings.fontSizeType
+        self.fontSizeType = settings['fontSizeTypeRelative'] * self.fontSizeChords
+        self.fontSizeTypeSmall = settings['fontSizeTypeSmallRelative'] * self.fontSizeType
+
+        self.fontSettings = FontSettings(self.font, self.fontSizeType)
+
+
+        self.capsizeType = fD["capsize"] * self.fontSizeType
 
         self.fontSizeSegno = self.capsizeNumberRelative / fontDimensions["segno"] * self.fontSizeNotes
         self.fontSizeCoda = self.capsizeNumberRelative / fontDimensions["coda"] * self.fontSizeNotes
         self.lyricHeightMax = self._countLinesLyrics() * self.capsizeLyric * (1 + self.vMarginLyricsRelative) + self.capsizeLyric * self.vMarginLyricsRelative
 
         self.fontSizeNoteAccidental = self.fontSizeAccidentalRelative * self.fontSizeNotes
         self.barSpace = self.barSpacePerCapsize * self.capsizeNote
         self.fontSizeChords = self.fontSizeChordsPerFontSizeNotes * self.fontSizeNotes
         self.fontSizeGraceNotes = self.fontSizeGraceNotesPerFontSizeNotes * self.fontSizeNotes
 
+
+
         self.heightBarline0Extension = self.capsizeNote
         self.lengthFirstMeasure = self._getLengthFirstMeasure()
         self.offsetLineMax = self.lengthFirstMeasure * self.measuresPerLine
         self.xMinimalPickupMeasureSpace = self.xMinimalPickupMeasureSpaceFraction * self.offsetLineMax
         self.noteLowest, self.noteHighest = self._getRangeNotes()
         self.yMin, self.yMax = self._getRangeYs()
 
-        key = self.getKey(0)
-        if key.mode == 'major':
+        self.firstKey = self.getKey(0)
+
+        if self.firstKey.mode == 'major':
             self.facecolor = settings['facecolor']
             self.facecolor2 = settings['facecolor2']
 
         else:
             self.facecolor = settings['facecolor2']
             self.facecolor2 = settings['facecolor']
 
@@ -169,20 +177,25 @@
         if self.setInMajorKey and key.mode == 'minor':
             key = key.relative
 
         return key
 
 
     def _getRangeNotes(self):
-        p = music21.analysis.discrete.Ambitus()
-        if p.getPitchSpan(self.streamObj):
-            pitchSpan = [int(thisPitch.ps) for thisPitch in p.getPitchSpan(self.streamObj)]
-            return pitchSpan[0], pitchSpan[1]
+        if self.plotMelody:
+            p = music21.analysis.discrete.Ambitus()
+            if p.getPitchSpan(self.streamObj):
+                pitchSpan = [int(thisPitch.ps) for thisPitch in p.getPitchSpan(self.streamObj)]
+                return pitchSpan[0], pitchSpan[1]
+            else:
+                return 1, 10
         else:
-            return 1, 10
+            nL = int(self.getKey(0).getTonic().ps)
+            nH = nL + 12
+            return nL, nH
 
     def _getRangeYs(self):
         numTones = self.noteHighest - self.noteLowest + 1
         yMax = numTones * self.barSpace * (1 - self.overlapFactor) + self.barSpace * self.overlapFactor
         yMin = 0
 
         chords = len(self.streamObj.flatten().getElementsByClass('ChordSymbol')) > 0
@@ -206,29 +219,28 @@
 
     def _getLengthFirstMeasure(self):
         length = self.streamObj.measure(1)[music21.stream.Measure][0].quarterLength
         return length
 
 class FontSettings:
 
-    def __init__(self, font):
+    def __init__(self, font, fontSizeType):
 
         pathFontDimensions = os.path.join(os.path.dirname(__file__), 'fontSettings.json')
         f = open(pathFontDimensions)
         fontSettings = json.load(f)
         if font in fontSettings.keys():
             fontSettings = fontSettings[font]
         else:
             fontSettings = fontSettings['DejaVu Sans']
             print("no fontsettings available")
 
-        self.fontSizeType = fontSettings['fontSizeType']
-        self.fontSizeTypeSmall = fontSettings['fontSizeTypeSmall']
-        self.widthCharacter = fontSettings['widthCharacter']
-        self.widthMinus = fontSettings['widthMinus']
-        self.accidentalSpace = fontSettings['accidentalSpace']
-        self.accidentalSizeRelative = fontSettings["accidentalSizeRelative"]
-        self.widthDelta = fontSettings["widthDelta"]
-        self.widthCircle = fontSettings["widthCircle"]
-        self.spaceAddSus = fontSettings["spaceAddSus"]
-        self.accidentalXPositionRelative = fontSettings["accidentalXPositionRelative"]
-        self.hDistanceChordAddition = fontSettings['hDistanceChordAddition']
+
+        self.widthCharacter = fontSettings['widthCharacterRelative'] * fontSizeType
+        self.widthMinus = fontSettings['widthMinusRelative'] * fontSizeType
+        self.accidentalSpace = fontSettings['accidentalSpaceRelative'] * fontSizeType
+        self.accidentalSizeRelative = fontSettings["accidentalSizeRelativeRelative"] * fontSizeType
+        self.widthDelta = fontSettings["widthDeltaRelative"] * fontSizeType
+        self.widthCircle = fontSettings["widthCircleRelative"] * fontSizeType
+        self.spaceAddSus = fontSettings["spaceAddSusRelative"] * fontSizeType
+        self.accidentalXPositionRelative = fontSettings["accidentalXPositionRelativeRelative"] * fontSizeType
+        self.hDistanceChordAddition = fontSettings['hDistanceChordAdditionRelative'] * fontSizeType
```

### Comparing `integerbook-0.0.2/src/integerbook/auxiliary_scripts/chordTypes.py` & `integerbook-0.0.3/src/integerbook/auxiliary_scripts/chordTypes.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/auxiliary_scripts/createBatchJson.py` & `integerbook-0.0.3/src/integerbook/auxiliary_scripts/createBatchJson.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/auxiliary_scripts/runMultiple.py` & `integerbook-0.0.3/src/integerbook/auxiliary_scripts/runMultiple.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,43 +14,51 @@
 
 
 f = open('../settings.json')
 settings = json.load(f)
 
 settings["measuresPerLine"] = 4
 settings["subdivision"] = 0
+settings['thickBarlines'] = True
+
 settings["setInMajorKey"] = True
+
 settings["lyrics"] = False
+settings["usePlt"] = False
+
 settings['coloursVoices'] = False
 settings['coloursCircleOfFifths'] = False
-settings['thickBarlines'] = True
 
-settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Vulf Mono/Vulf Mono/Desktop/"
-settings['font'] = 'Vulf Mono'
-settings['fontStyle'] = 'italic'
-settings['fontWeight'] = 'light'
+# settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Vulf Mono/Vulf Mono/Desktop/"
+# settings['font'] = 'Vulf Mono'
+# settings['fontStyle'] = 'italic'
+# settings['fontWeight'] = 'light'
 settings['printArranger'] = False
 
+settings["alternativeSymbols"] = "SBJ"
+settings["fontSizeNotes"] = 7
+settings["xShiftNumberNote"] = 0.001
 
 lines1 = glob.glob(dirSongs + '*' + '.mxl')
 lines2 = glob.glob(dirSongs + '*' + '.musicxml')
 lines = lines1 + lines2
 lines = [os.path.basename(line) for line in lines]
 lines.sort()
 
 
 for line in lines:
 
     print(line)
 
-    line = line.rstrip('\n')
-
     try:
         pathSong = dirSongs + line
 
         vis = Visualiser(pathSong, settings)
-        vis.generate("../../output/outputDickSchmitt/")
+
+        dirName = "../../../output/outputDickSchmittSteve"
+
+        vis.saveFig(dirName=dirName)
 
     except Exception as e:
         print("ERROR", "\n")
         print(repr(e))
```

### Comparing `integerbook-0.0.2/src/integerbook/auxiliary_scripts/separateRealbook.py` & `integerbook-0.0.3/src/integerbook/auxiliary_scripts/separateRealbook.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/auxiliary_scripts/setMode.py` & `integerbook-0.0.3/src/integerbook/auxiliary_scripts/setMode.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/auxiliary_scripts/setModes.py` & `integerbook-0.0.3/src/integerbook/auxiliary_scripts/setModes.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/auxiliary_scripts/writeTexFile.py` & `integerbook-0.0.3/src/integerbook/auxiliary_scripts/writeTexFile.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/fontDimensions.json` & `integerbook-0.0.3/src/integerbook/fontDimensions.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/fonts/.DS_Store` & `integerbook-0.0.3/src/integerbook/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/fonts/Realbook/Realbook.ttf` & `integerbook-0.0.3/src/integerbook/fonts/Realbook/Realbook.ttf`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/fonts/symbola/Symbola.ttf` & `integerbook-0.0.3/src/integerbook/fonts/symbola/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/main.py` & `integerbook-0.0.3/src/integerbook/main.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/plotter/PlotterBarLines.py` & `integerbook-0.0.3/src/integerbook/plotter/PlotterBarLines.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/plotter/PlotterBase.py` & `integerbook-0.0.3/src/integerbook/plotter/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/plotter/PlotterChords.py` & `integerbook-0.0.3/src/integerbook/plotter/PlotterChords.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
         fontSize = self.Settings.fontSizeChords
         widthNumber = self.Settings.widthNumberRelative * fontSize
 
         xPos = xPos + widthNumber + self.Settings.fontSettings.hDistanceChordAddition
         yPos = yPos + self.Settings.capsizeChord * self.Settings.heightChordAddition
 
-        self.fontSizeType = self.Settings.fontSettings.fontSizeType
-        self.fontSizeTypeSmall = self.Settings.fontSettings.fontSizeTypeSmall
+        self.fontSizeType = self.Settings.fontSizeType
+        self.fontSizeTypeSmall = self.Settings.fontSizeTypeSmall
         self.width = self.Settings.fontSettings.widthCharacter
         self.accidentalSpace = self.Settings.fontSettings.accidentalSpace
 
         xPos = self._plotTypes(chordSymbol, xPos, yPos, page)
 
         self._plotModifications(chordSymbol, xPos, yPos, page)
 
@@ -66,75 +66,80 @@
         chordTypes = self._getTypeList(chordSymbol)
 
         for i, chordType in enumerate(chordTypes):
 
             width = 0
             if chordType == "minor":
                 width = self._plotTypeMinor(xPos, yPos, page)
-            if chordType == "major" and len(chordTypes) != 1 and chordTypes[i+1] != 'sixth':
-                width = self._plotTypeMajor(xPos, yPos, page)
-            if chordType == 'half-diminished':
-                width = self._plotTypeHalfDiminished(xPos, yPos, page)
-            if chordType == 'diminished':
-                width = self._plotTypeDiminished(xPos, yPos, page)
-
-            if chordType == "sixth":
-                width = self._plotTypeSixth(xPos, yPos, page)
-
-            if chordType == "seventh":
-                width = self._plotTypeSeventh(xPos, yPos, page)
-            if chordType == "ninth":
-                width = self._plotTypeNinth(xPos, yPos, page)
-            if chordType == "11th":
-                width = self._plotType11th(xPos, yPos, page)
-            if chordType == "13th":
-                width = self._plotType13th(xPos, yPos, page)
-
-            if chordType == 'augmented':
-                if i == 0:
-                    xPos -= 0.7 * self.Settings.fontSettings.accidentalSpace
-                width = self._plotTypeAugmented(xPos, yPos, page)
-            if chordType == 'flat-five':
-                width = self._plotTypeFlatFive(xPos, yPos, page)
-            if chordType == 'suspended-second':
-                width = self._plotTypeSuspendedSecond(xPos, yPos, page)
-            if chordType == 'suspended-fourth':
-                width = self._plotTypeSuspendedFourth(xPos, yPos, page)
+
+            if self.Settings.chordVerbosity > 0:
+
+                if chordType == "major" and len(chordTypes) != 1 and chordTypes[i+1] != 'sixth':
+                    width = self._plotTypeMajor(xPos, yPos, page)
+                if chordType == 'half-diminished':
+                    width = self._plotTypeHalfDiminished(xPos, yPos, page)
+                if chordType == 'diminished':
+                    width = self._plotTypeDiminished(xPos, yPos, page)
+
+                if chordType == "sixth":
+                    width = self._plotTypeSixth(xPos, yPos, page)
+
+                if chordType == "seventh":
+                    width = self._plotTypeSeventh(xPos, yPos, page)
+                if chordType == "ninth":
+                    width = self._plotTypeNinth(xPos, yPos, page)
+                if chordType == "11th":
+                    width = self._plotType11th(xPos, yPos, page)
+                if chordType == "13th":
+                    width = self._plotType13th(xPos, yPos, page)
+
+                if chordType == 'augmented':
+                    if i == 0:
+                        xPos -= 0.7 * self.Settings.fontSettings.accidentalSpace
+                    width = self._plotTypeAugmented(xPos, yPos, page)
+                if chordType == 'flat-five':
+                    width = self._plotTypeFlatFive(xPos, yPos, page)
+                if chordType == 'suspended-second':
+                    width = self._plotTypeSuspendedSecond(xPos, yPos, page)
+                if chordType == 'suspended-fourth':
+                    width = self._plotTypeSuspendedFourth(xPos, yPos, page)
             xPos += width
         return xPos
 
     def _plotModifications(self, chordSymbol, xPos, yPos, page):
 
-        for csMod in chordSymbol.chordStepModifications:
-            if csMod.interval is not None:
-                width = 0
-                if csMod.modType == 'add':
-                    width = self._plotModificationAdd(xPos, yPos, page)
-                if csMod.modType == 'subtract':
-                    width = self._plotModificationSubtract(xPos, yPos, page)
-                if csMod.modType == 'alter':
-                    width = self._plotModificationAlter(xPos, yPos, page)
-
-                xPos += width
-
-                number = csMod.degree
-
-                accidental = None
-                if csMod.interval.semitones == -1:
-                    accidental = music21.pitch.Accidental('flat')
-                if csMod.interval.semitones == 1:
-                    accidental = music21.pitch.Accidental('sharp')
+        if self.Settings.chordVerbosity > 1:
+
+            for csMod in chordSymbol.chordStepModifications:
+                if csMod.interval is not None:
+                    width = 0
+                    if csMod.modType == 'add':
+                        width = self._plotModificationAdd(xPos, yPos, page)
+                    if csMod.modType == 'subtract':
+                        width = self._plotModificationSubtract(xPos, yPos, page)
+                    if csMod.modType == 'alter':
+                        width = self._plotModificationAlter(xPos, yPos, page)
+
+                    xPos += width
+
+                    number = csMod.degree
+
+                    accidental = None
+                    if csMod.interval.semitones == -1:
+                        accidental = music21.pitch.Accidental('flat')
+                    if csMod.interval.semitones == 1:
+                        accidental = music21.pitch.Accidental('sharp')
 
-                if accidental:
-                    xPos -= 0.003
+                    if accidental:
+                        xPos -= 0.003
 
-                width = self._plotTypeAndModificationNumberAndAccidental(number, accidental, xPos, yPos, page)
-                width += 0.002
+                    width = self._plotTypeAndModificationNumberAndAccidental(number, accidental, xPos, yPos, page)
+                    width += 0.002
 
-                xPos += width
+                    xPos += width
 
     def _plotTypeAndModificationNumberAndAccidental(self, number, accidental, xPos, yPos, page):
 
         if self.Settings.fontVShift:
             yPos += self.Settings.fontVShift * self.Settings.capsizeNumberRelative * self.fontSizeType
 
         width = 0
@@ -148,34 +153,34 @@
                             f"{number}", fontsize=self.fontSizeType,
                             va='baseline', ha='left')
         width += len(str(number)) * self.width
 
         return width
 
     def _plotTypeMinor(self, xPos, yPos, page):
-        self.axs[page].text(xPos, yPos,
+        self.axs[page].text(xPos, yPos + 0.00005 * self.fontSizeType,
                             "-", fontsize = self.fontSizeType,
                             va='baseline', ha='left')
         return self.Settings.fontSettings.widthMinus
 
     def _plotTypeMajor(self, xPos, yPos, page):
         self.axs[page].text(xPos + 0.001, yPos - 0.00035,  # - 0.0005
                             "$\mathbb{\Delta}$", fontsize=self.fontSizeType,
                             va='baseline', ha='left')
         return self.Settings.fontSettings.widthDelta
 
     def _plotTypeHalfDiminished(self, xPos, yPos, page):
         self.axs[page].text(xPos, yPos - 0.00034,
-                            "$\\varnothing$", fontsize=8, math_fontfamily='dejavusans',
+                            "$\\varnothing$", fontsize=self.fontSizeTypeSmall, math_fontfamily='dejavusans',
                             va='baseline', ha='left')
         return self.Settings.fontSettings.widthCircle
 
     def _plotTypeDiminished(self, xPos, yPos, page):
         self.axs[page].text(xPos, yPos - 0.0014,
-                            "$\\circ$", fontsize=15, fontstyle='normal', math_fontfamily='cm',
+                            "$\\circ$", fontsize=self.fontSizeType*1.5, fontstyle='normal', math_fontfamily='cm',
                             va='baseline', ha='left')
         return self.Settings.fontSettings.widthCircle + 0.0003
 
     def _plotTypeSixth(self, xPos, yPos, page):
         width = self._plotTypeAndModificationNumberAndAccidental(6, None, xPos, yPos, page)
         return width
 
@@ -253,21 +258,21 @@
                             va='baseline', ha='left')
         return self.Settings.fontSettings.spaceAddSus
 
     def _plotModificationSubtract(self, xPos, yPos, page):
         self.axs[page].text(xPos, yPos,
                             "sub", fontsize=self.fontSizeTypeSmall, fontstyle='normal',
                             va='baseline', ha='left')
-        return self.width * 3
+        return self.Settings.fontSettings.spaceAddSus
 
     def _plotModificationAlter(self, xPos, yPos, page):
         self.axs[page].text(xPos, yPos,
                             "alt", fontsize=self.fontSizeTypeSmall, fontstyle='normal',
                             va='baseline', ha='left')
-        return self.width * 3
+        return self.Settings.fontSettings.spaceAddSus
 
     def _getTypeList(self, chordSymbol):
 
         chordType = chordSymbol.chordKind
 
         # use the alias of the chord type that is used by music21
         if chordType in music21.harmony.CHORD_ALIASES:
```

### Comparing `integerbook-0.0.2/src/integerbook/plotter/PlotterMain.py` & `integerbook-0.0.3/src/integerbook/plotter/PlotterMain.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/plotter/PlotterMetadata.py` & `integerbook-0.0.3/src/integerbook/plotter/PlotterMetadata.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/plotter/PlotterNotes.py` & `integerbook-0.0.3/src/integerbook/plotter/PlotterNotes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import json
 import music21
 from matplotlib.patches import FancyBboxPatch, Rectangle, Ellipse
 from itertools import tee, islice, chain
 import numpy as np
 
 from integerbook.plotter.patches import Parallelogram
 from integerbook.plotter.PlotterBase import Plotter
@@ -29,14 +31,19 @@
                                  "3": 0,
                                  "4": 0}
         self.lastSyllabic = {"1": 0,
                              "2": 0,
                              "3": 0,
                              "4": 0}
 
+        if self.Settings.alternativeSymbols:
+            pathAlternativeSymbols = os.path.join(os.path.dirname(__file__), '../alternativeSymbols.json')
+            f = open(pathAlternativeSymbols)
+            self.alternativeSymbolsDict = json.load(f)[self.Settings.alternativeSymbols]
+
     def plotNotes(self):
 
         notes = self.streamObj[music21.note.Note]
         chords = self.streamObj[music21.chord.Chord]
 
         for idx in range(len(notes)):
 
@@ -57,14 +64,17 @@
                     noteNext = None
                     self._plotNote(note, noteNext, measure, offset=chord.getOffsetInHierarchy(self.streamObj))
 
     def plotChordNotes(self):
 
         chords = self.streamObj[music21.harmony.ChordSymbol]
 
+        nL = self.Settings.noteLowest
+        nH = self.Settings.noteHighest
+
         for idx in range(len(chords)):
 
             chord = chords[idx]
 
             if idx < len(chords) - 1:
                 chordNext = chords[idx+1]
             else:
@@ -79,16 +89,14 @@
             else:
                 offsetNext = self.streamObj.quarterLength
                 measureEnd = self.streamObj[music21.stream.Measure][-1]
 
             notes = chord.notes
             for note in notes:
                 midiNumber = note.pitch.ps
-                nL = self.Settings.noteLowest
-                nH = self.Settings.noteHighest
 
                 midiNumberPlottedNote = nL + (midiNumber - nL) % 12
                 while midiNumberPlottedNote <= nH:
                     plottedNote = music21.note.Note(midiNumberPlottedNote, quarterLength=offsetNext - offset)
                     self._plotNote(plottedNote, None, measure, offset=offset, measureEnd=measureEnd, isChordNote=True)
                     midiNumberPlottedNote += 12
 
@@ -247,20 +255,27 @@
             alpha = 1
             zorder = 1
             if isChordNote:
                 textColor = 'grey'
                 alpha = 0.5
                 zorder = .5
 
+            if not self.Settings.alternativeSymbols:
+                self.axs[page].text(xPos, yPos, number,
+                                    fontsize=fontSize,
+                                    va='baseline', ha=horizontalAlignment, color=textColor, zorder=zorder)
 
-            self.axs[page].text(xPos, yPos, number,
-                                fontsize=fontSize,
-                                va='baseline', ha=horizontalAlignment, color=textColor, zorder=zorder)
 
-            self._plotAccidental(accidental, fontSize, xPos, yPos, page)
+                self._plotAccidental(accidental, fontSize, xPos, yPos, page)
+
+            else:
+                symbol = self._getSymbol(number, accidental)
+                self.axs[page].text(xPos, yPos, symbol,
+                                    fontsize=fontSize,
+                                    va='baseline', ha=horizontalAlignment, color=textColor, zorder=zorder)
 
     def _plotLyric(self, page, el, xPos, yPosLineBase):
         """lyrics are plotted with vertical_alignment='top' at yPosLineBass.
         By multiple lines, the lyric already contains a newline command within it"""
 
         if el.lyrics:
             for lyric in el.lyrics:
@@ -541,14 +556,23 @@
 
     def _getMeasureByNumber(self, number):
         measures = self.streamObj[music21.stream.Measure]
         for measure in measures:
             if measure.number == number:
                 return measure
 
+    def _getSymbol(self, number, accidental):
+
+        if accidental:
+            accidentalName = accidental.name
+        else:
+            accidentalName = "natural"
+        symbol = self.alternativeSymbolsDict[str(number)][accidentalName]
+        return symbol
+
     def _colorwheel(self, circleOfFifthIndex):
         """index must be between 0 and 11"""
 
         rgbs = [(0.18062, 0.13244, 0.91856, 1.0),
                  (0.44913, 0.17088, 0.97129, 1.0),
                  (0.69537, 0.25408, 0.98496, 1.0),
                  (0.93769, 0.33352, 0.94809, 1.0),
```

### Comparing `integerbook-0.0.2/src/integerbook/plotter/patches.py` & `integerbook-0.0.3/src/integerbook/plotter/patches.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.2/src/integerbook/runSingle.py` & `integerbook-0.0.3/src/integerbook/runSingle.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,56 +77,56 @@
 song71 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/Summertime.musicxml"
 song72 = "/Users/jvo/Downloads/Summertime in G.musicxml"
 song73 = '/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/ultimate-guitar-top-100/Hallelujah__Leonard_Cohen_Lead_sheet_with_lyrics_.mxl'
 song74 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/ultimate-guitar-top-100/2021 -- HALLELUJAH RJS mods.mscz"
 song75 = "/Users/jvo/Downloads/tempMxl/2021 -- HALLELUJAH RJS mods.musicxml"
 song76 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/musescore/Think_About_Things_-_Iceland_Eurovision_2020_-_Dai_Freyr-Part.mscz"
 song77 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/All_Of_Me.musicxml"
-
-# f = open('Settings.json')
-# settings = json.load(f)
+song78 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/All_Of_Me-different-key.musicxml"
+song79 = "/Users/jvo/Downloads/favicon.musicxml"
+song80 = '/Users/jvo/Downloads/DickSchmittMxl/2020 --  Home, Sweet Home RJSReformat.musicxml'
 
 settings = {}
-settings["measuresPerLine"] = 4
+settings["measuresPerLine"] = 8
 settings["subdivision"] = 0
 settings["setInMajorKey"] = True
-settings["lyrics"] = True
+settings["lyrics"] = False
 settings['coloursVoices'] = False
 settings['coloursCircleOfFifths'] = False
-settings['thickBarlines'] = False
+settings['thickBarlines'] = True
 settings['plotTimeSignature'] = True
 settings['printArranger'] = False
 settings['saveCropped'] = True
 settings['alpha'] = 0.2
 settings['xkcd'] = False
 
-settings['overlapFactor'] = .5
-settings["plotChordTones"] = False
-settings["plotMelody"] = True
-
-settings["alternativeSymbols"] = "SBJ"
+settings['overlapFactor'] = 0
+settings["plotChordTones"] = True
+settings["plotMelody"] = False
 
 # settings["usePlt"] = True
 
+# settings["alternativeSymbols"] = "SBJ"
+# settings["fontSizeNotes"] = 7
+
 
 # Settings['font'] = 'Sathu'
 # Settings['font'] = 'STIXGeneral'
 # Settings['fontStyle'] = 'italic'
 
 # settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Vulf Mono/Vulf Mono/Desktop"
 # settings['fontStyle'] = 'italic'
 # settings['fontWeight'] = 'light'
 # settings['font'] = 'Vulf Mono'
 
 # Settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Realbook"
 # Settings['font'] = 'Realbook'
 
-# Settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Humor Sans"
-# Settings['font'] = 'Humor Sans'
-
+# settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Humor Sans"
+# settings['font'] = 'Humor Sans'
 
 song = song77
 
 if song[-5:] == ".mscz":
 
     dirSongsMxl = "/Users/jvo/Downloads/tempMxl"
     filename = os.path.basename(song).split("/")[-1]
```

### Comparing `integerbook-0.0.2/src/integerbook/settings.json` & `integerbook-0.0.3/src/integerbook/settings.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.923728813559322%*

 * *Differences: {"'alternativeSymbols'": 'False',*

 * * "'chordVerbosity'": '1',*

 * * "'fontSizeTypeRelative'": '0.8333',*

 * * "'fontSizeTypeSmallRelative'": '0.8',*

 * * "'printArranger'": 'False'}*

```diff
@@ -1,40 +1,44 @@
 {
     "alpha": 0.2,
+    "alternativeSymbols": false,
     "barSpacePerCapsize": 1.33,
     "capHeightRatio": 0.673,
     "chordToneRatio": 2.5,
+    "chordVerbosity": 1,
     "coloursCircleOfFifths": false,
     "coloursVoices": false,
     "facecolor": "blue",
     "facecolor2": "red",
     "font": "DejaVu Sans",
     "fontDirectory": null,
     "fontPath": null,
     "fontPathRoman": null,
     "fontSizeAccidentalRelative": 0.7,
     "fontSizeChordsPerFontSizeNotes": 1.2,
     "fontSizeGraceNotesPerFontSizeNotes": 0.7,
     "fontSizeLyrics": 6,
     "fontSizeMetadata": 10,
     "fontSizeNotes": 10,
+    "fontSizeTypeRelative": 0.8333,
+    "fontSizeTypeSmallRelative": 0.8,
     "fontStyle": "normal",
     "fontWeight": "normal",
     "heightA4": 11.69,
     "heightChordAddition": 0.7,
     "lineWidth0": 0.0017,
     "lineWidth1": 0.0017,
     "lineWidth2": 0.0003,
     "lyrics": false,
     "measuresPerLine": 4,
     "overlapFactor": 0.5,
     "plotChordTones": false,
     "plotMelody": true,
     "plotTimeSignature": true,
-    "printArranger": true,
+    "printArranger": false,
     "ptToInches": 0.01389,
     "saveCropped": false,
     "setInMajorKey": true,
     "subdivision": 0,
     "thickBarlines": true,
     "timeSignatureWithBarlines": true,
     "usePlt": false,
```

### Comparing `integerbook-0.0.2/src/integerbook.egg-info/PKG-INFO` & `integerbook-0.0.3/src/integerbook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integerbook
-Version: 0.0.2
+Version: 0.0.3
 Summary: sheet music converter
 Author-email: Jesse van Oostrum <integerbook@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,37 +687,33 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # music-visualisation
 
 This library converts sheet music in musicxml format to visualisations that refer to notes and chords with their relative position within the key of the song. More about how this notational system works [here](https://integerbook.com/about). 
 
-### running the code
-From the root folder of the repository, run the following line in the terminal:
+### installation
 
-``` $ python run.py ```
+1. Download python
+2. install the [integerbook package](https://pypi.org/project/integerbook/0.0.2/) using pip: ``` $ pip install integerbook ```
+3. Download or copy the file ```run.py``` from the repository to a folder on your computer, e.g. ```~/Documents/music-visualisation```.
 
-This will convert the file "All_Of_Me.musicxml" located in the examples folder and place the result in the root folder of the repository. 
 
-The most important options are the following:
-- -s set song path (can be either .musicxml or .mxl file)
-- -o set output directory  (without "/" at the end)
+### running the code
+1. In the terminal, navigate to the folder where ```run.py``` is stored. 
+2. In the terminal, type: ``` $ python run.py -s <path-to-song>```  e.g.   
+``` $ python run.py -s "/Users/jvo/Documents/music-visualisation/example/Summertime.musicxml" ```
 
-example: 
-``` $ python run.py -s "/Users/jvo/Documents/music-visualisation/example/Summertime.musicxml" -o "/Users/jvo/Downloads/output" ```
+This will convert the musicxml file you specified to a pdf and store it in the current folder. 
 
 Further options include:
+- -o set output directory  (without "/" at the end)
 - -b for bassline output
 - -l for printing lyrics
 - -c for colouring notes according to circle of fifths
-- -r for realbook font (note that you first have to install the font (located in fonts folder))
 - -cn for printing chord notes
 - -cp for printing chord progressions (no melody, 8 measures per line)
 - -d <path-to-settings-dictionary> can be used to pass a custom settings dictionary. (most flexible) See 'sample/settings.json' for the default settings.
 
-### requirements
-- music21
-- matplotlib
-
 
 ### example musicxml files
 In the folder example, there are some musicxml files that can be used to try out the program.
```

### Comparing `integerbook-0.0.2/src/integerbook.egg-info/SOURCES.txt` & `integerbook-0.0.3/src/integerbook.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/integerbook/CanvasCreator.py
 src/integerbook/LocationFinder.py
 src/integerbook/Settings.py
 src/integerbook/__init__.py
+src/integerbook/alternativeSymbols.json
 src/integerbook/fontDimensions.json
 src/integerbook/fontSettings.json
 src/integerbook/main.py
 src/integerbook/runSingle.py
 src/integerbook/settings.json
 src/integerbook.egg-info/PKG-INFO
 src/integerbook.egg-info/SOURCES.txt
 src/integerbook.egg-info/dependency_links.txt
 src/integerbook.egg-info/requires.txt
 src/integerbook.egg-info/top_level.txt
 src/integerbook/auxiliary_scripts/__init__.py
+src/integerbook/auxiliary_scripts/changeNameMxl.py
 src/integerbook/auxiliary_scripts/chordTypes.py
 src/integerbook/auxiliary_scripts/createBatchJson.py
 src/integerbook/auxiliary_scripts/printSettings.py
 src/integerbook/auxiliary_scripts/runMultiple.py
 src/integerbook/auxiliary_scripts/separateRealbook.py
 src/integerbook/auxiliary_scripts/setMode.py
 src/integerbook/auxiliary_scripts/setModes.py
```

