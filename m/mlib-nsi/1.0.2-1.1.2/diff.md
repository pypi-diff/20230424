# Comparing `tmp/mlib-nsi-1.0.2.tar.gz` & `tmp/mlib-nsi-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlib-nsi-1.0.2.tar", last modified: Tue Feb 14 12:57:48 2023, max compression
+gzip compressed data, was "mlib-nsi-1.1.2.tar", last modified: Mon Apr 24 09:51:37 2023, max compression
```

## Comparing `mlib-nsi-1.0.2.tar` & `mlib-nsi-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 12:57:48.673078 mlib-nsi-1.0.2/
--rw-rw-rw-   0        0        0     1086 2023-02-14 10:48:34.000000 mlib-nsi-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2208 2023-02-14 12:57:48.673078 mlib-nsi-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-02-14 11:48:10.000000 mlib-nsi-1.0.2/README.md
--rw-rw-rw-   0        0        0    63259 2023-02-14 10:21:50.000000 mlib-nsi-1.0.2/mlib.py
-drwxrwxrwx   0        0        0        0 2023-02-14 12:57:48.673078 mlib-nsi-1.0.2/mlib_nsi.egg-info/
--rw-rw-rw-   0        0        0     2208 2023-02-14 12:57:48.000000 mlib-nsi-1.0.2/mlib_nsi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-02-14 12:57:48.000000 mlib-nsi-1.0.2/mlib_nsi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 12:57:48.000000 mlib-nsi-1.0.2/mlib_nsi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-02-14 12:57:48.000000 mlib-nsi-1.0.2/mlib_nsi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-14 12:57:48.000000 mlib-nsi-1.0.2/mlib_nsi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      736 2023-02-14 12:56:42.000000 mlib-nsi-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-14 12:57:48.673078 mlib-nsi-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 09:51:37.600472 mlib-nsi-1.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 10:48:34.000000 mlib-nsi-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2216 2023-04-24 09:51:37.600472 mlib-nsi-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-02-14 11:48:10.000000 mlib-nsi-1.1.2/README.md
+-rw-rw-rw-   0        0        0    63683 2023-04-23 19:33:16.000000 mlib-nsi-1.1.2/mlib.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:51:37.600472 mlib-nsi-1.1.2/mlib_nsi.egg-info/
+-rw-rw-rw-   0        0        0     2216 2023-04-24 09:51:37.000000 mlib-nsi-1.1.2/mlib_nsi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-24 09:51:37.000000 mlib-nsi-1.1.2/mlib_nsi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:51:37.000000 mlib-nsi-1.1.2/mlib_nsi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-24 09:51:37.000000 mlib-nsi-1.1.2/mlib_nsi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-24 09:51:37.000000 mlib-nsi-1.1.2/mlib_nsi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      750 2023-04-24 09:50:16.000000 mlib-nsi-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:51:37.608622 mlib-nsi-1.1.2/setup.cfg
```

### Comparing `mlib-nsi-1.0.2/LICENSE.txt` & `mlib-nsi-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlib-nsi-1.0.2/PKG-INFO` & `mlib-nsi-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlib-nsi
-Version: 1.0.2
+Version: 1.1.2
 Summary: MLib is a little python library make by a 12 degrees french students
 Author-email: Matt_o <mmattmmo@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Matt_o]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://matto.glitch.me/?mlib=go
-Keywords: feed,reader,tutorial
+Keywords: mlib,mgui,nsi,premiere,lycee
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlib-nsi-1.0.2/mlib.py` & `mlib-nsi-1.1.2/mlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,34 @@
 from PIL import Image
 from pyperclip import *
 from math import *
 import os
 from pygame import *
 from sys import *
 from time import time_ns
+from tkinter import Tk
+from tkinter import filedialog
 import pygame
 pygame.init()
 
 ALPHA_UPPER = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 ALPHA_LOWER = "abcdefghijklmnopqrstuvwxyz"
 NUMERICS = "1234567890"
 SYMBOLS_KEYPAD_LITTLE = " &é\"'(-è_çà)=^$*ù!:;,~#}{[|`\\^@]¤"
 
+def openDialogFile(fileTypes): #Ouvrir un fichier grâce à une fenêtre de dialogue
+
+    if(fileTypes == "Image"):
+        fileTypes = [("Images", "*.png;*.jpg;*.jpeg")]
+
+    root = Tk()
+    root.withdraw()
+    file_path = filedialog.askopenfilename(filetypes=fileTypes)
+    return file_path
+
 def fichierInfo(fichier: str, type: str): #Obtenir des informations sur un fichier
     fichier.replace("\\", "/") #Formater le lien du fichier
     if len(fichier) > 0:
         if fichier[0] == "\"": #Retirez des guillemets au début et à la fin du lien
             fichier = fichier[1:-1]+ fichier[-1]
         if fichier[-1] == "\"":
             fichier = fichier[0:-1]
@@ -538,25 +550,25 @@
         display.set_caption(titre)
 
 
 
 class MBordure(MWidget): #Définition d'une représentant un widget avec une bordure
     def __init__(self, position, taille, parent, bordureLargeur = 2, bordureCouleur = (0, 0, 0), bordureRayon = 0, borduresLargeurs = [None, None, None, None], borduresRayons=[None, None, None, None], arrierePlanCouleur=(0, 0, 0, 0), curseurSurvol=SYSTEM_CURSOR_ARROW, renderAuFocus = False, renderAuSurvol = False, type="Bordure"): #Constructeur de la classe
         MWidget.__init__(self, position, taille, parent, arrierePlanCouleur, curseurSurvol, renderAuFocus, renderAuSurvol, type) #Appeler le constructeur de la classe MWidget
-        for i in enumerate(borduresLargeurs): #Actualisation des largeurs des bordures
-            if borduresLargeurs[i[0]] == None:
-                borduresLargeurs[i[0]] = bordureLargeur
         self.bordureLargeur = bordureLargeur
-        self.borduresLargeurs = borduresLargeurs
-        for i in enumerate(borduresRayons): #Actualisation des rayons des bordures
-            if borduresRayons[i[0]] == None:
-                borduresRayons[i[0]] = bordureRayon
-        self.bordureRayon = bordureRayon
-        self.borduresRayons = borduresRayons
+        self.borduresLargeurs = borduresLargeurs.copy()
+        for i in enumerate(self.borduresLargeurs): #Actualisation des largeurs des bordures
+            if self.borduresLargeurs[i[0]] == None:
+                self.borduresLargeurs[i[0]] = self.bordureLargeur
+        self.borduresRayons = borduresRayons.copy()
         self.bordureCouleur = bordureCouleur
+        self.bordureRayon = bordureRayon
+        for i in enumerate(self.borduresRayons): #Actualisation des rayons des bordures
+            if self.borduresRayons[i[0]] == None:
+                self.borduresRayons[i[0]] = self.bordureRayon
     def _renderBeforeHierarchy(self, surface): #Ré-implémentation de la fonction pour afficher la bordure
         surfaceBordure = Surface(self.taille, SRCALPHA).convert_alpha() #Création de l'image qui contient la bordure
         surfaceBordure.fill((0, 0, 0, 0))
         draw.rect(surfaceBordure, self.bordureCouleur, (0, 0, self.taille[0], self.taille[1]), border_bottom_left_radius=self.borduresRayons[2], border_top_left_radius=self.borduresRayons[3], border_bottom_right_radius=self.borduresRayons[1], border_top_right_radius=self.borduresRayons[0]) #Dessiner la bordure
         draw.rect(surfaceBordure, self.arrierePlanCouleur, (self.borduresLargeurs[3], self.borduresLargeurs[0], self.taille[0] - (self.borduresLargeurs[1] + self.borduresLargeurs[3]), self.taille[1] - (self.borduresLargeurs[2] + self.borduresLargeurs[0])), border_bottom_left_radius=self.borduresRayons[2], border_top_left_radius=self.borduresRayons[3], border_bottom_right_radius=self.borduresRayons[1], border_top_right_radius=self.borduresRayons[0]) #Dessiner l'intèrieur de la bordure
         masque = mask.from_surface(surfaceBordure, 1) #Masque pour éviter des débordements
         surface = (masque.to_surface(surface, setsurface=surface, unsetcolor=(0,0,0,0)).convert_alpha())
@@ -603,15 +615,15 @@
         self.curseurLargeur = curseurLargeur
         self.curseurPosition = 0 #Défini la position du curseur dans le texte
         self.curseurRepositionnementSouris = curseurRepositionnementSouris #Savoir si la souris peu influencé le positionnement du curseur
         self.curseurTempsDAffichage = curseurTempsDAffichage
         self.curseurTempsDAffichageAffiche = True
         self.curseurTempsDAffichageEcoule = 0 #Temps écoulé depuis le changement de curseur
         if ligneLongueurMax < 0:
-            self.ligneLongueurMax = taille[0] - (borduresLargeurs[1] + borduresLargeurs[3])
+            self.ligneLongueurMax = taille[0] - (self.borduresLargeurs[1] + self.borduresLargeurs[3])
         else:
             self.ligneLongueurMax = ligneLongueurMax
         self.ligneMax = ligneMax
         self.longueurMax = longueurMax
         self.policeTaille = policeTaille #Affectation des variables de la classe
         if policeType == "defaut":
             policeType = font.get_default_font()
```

### Comparing `mlib-nsi-1.0.2/mlib_nsi.egg-info/PKG-INFO` & `mlib-nsi-1.1.2/mlib_nsi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlib-nsi
-Version: 1.0.2
+Version: 1.1.2
 Summary: MLib is a little python library make by a 12 degrees french students
 Author-email: Matt_o <mmattmmo@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Matt_o]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://matto.glitch.me/?mlib=go
-Keywords: feed,reader,tutorial
+Keywords: mlib,mgui,nsi,premiere,lycee
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlib-nsi-1.0.2/pyproject.toml` & `mlib-nsi-1.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlib-nsi"
-version = "1.0.2"
+version = "1.1.2"
 description = "MLib is a little python library make by a 12 degrees french students"
 readme = "README.md"
 authors = [{ name = "Matt_o", email = "mmattmmo@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["feed", "reader", "tutorial"]
+keywords = ["mlib", "mgui", "nsi", "premiere", "lycee"]
 dependencies = [
     "pygame",
     "Pillow",
     "pyperclip",
 ]
 requires-python = ">=3.7"
```

