# Comparing `tmp/magyar-2.9.6.tar.gz` & `tmp/magyar-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.6.tar", last modified: Wed Apr 19 15:07:36 2023, max compression
+gzip compressed data, was "magyar-2.9.7.tar", last modified: Sun Apr 23 21:59:26 2023, max compression
```

## Comparing `magyar-2.9.6.tar` & `magyar-2.9.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-19 15:07:36.954181 magyar-2.9.6/
--rw-rw-r--   0 bela      (1000) bela      (1000)     3912 2023-04-19 15:07:36.954181 magyar-2.9.6/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     3541 2023-04-19 15:02:33.000000 magyar-2.9.6/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-19 15:07:36.954181 magyar-2.9.6/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     3912 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-19 15:07:36.000000 magyar-2.9.6/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    31836 2023-04-19 15:02:33.000000 magyar-2.9.6/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-19 15:07:36.954181 magyar-2.9.6/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-19 15:05:49.000000 magyar-2.9.6/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-23 21:59:26.149057 magyar-2.9.7/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     4425 2023-04-23 21:59:26.149057 magyar-2.9.7/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     4027 2023-04-23 21:52:25.000000 magyar-2.9.7/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-23 21:59:26.149057 magyar-2.9.7/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     4425 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    35788 2023-04-23 21:57:33.000000 magyar-2.9.7/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-23 21:59:26.149057 magyar-2.9.7/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      615 2023-04-23 20:29:52.000000 magyar-2.9.7/setup.py
```

### Comparing `magyar-2.9.6/PKG-INFO` & `magyar-2.9.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,34 @@
-Metadata-Version: 2.1
-Name: magyar
-Version: 2.9.6
-Summary: Hungarian names...
-Home-page: https://github.com/kobanya/nevek
-Author: Nagy Béla
-Author-email: nagy.belabudapest@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # magyar
 
 
 ## Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
-1. vezetéknevek   =  magyar.vezeteknev
-2. női keresztnevek  = magyar.keresztnev_n
-3. férfi keresztnevek = magyar.keresztnev_f
-4. Vegyes magyar keresztnevek= magyar.keresztnev_v
-5. utcanevek = magyar.utca
-6. telelpülésnevek= magyar.telepules
-7. vármegyék nevei = magyar.megye
-8. folyók nevei = magyar.folyo
-9. a hét napjai = magyar.nap
-10. az év hónapjai = magyar.honap
-11. gyümölcsok = magyar.gyumolcs
-12. zöldségek = magyar.zoldseg
-13. haszonállatok = magyar.haszonallat
-14. vadallatok Magyarországon = magyar.vadallat
+1. Magyar vezetéknevek   =  magyar.vezeteknev
+2. Magyar női keresztnevek  = magyar.keresztnev_n
+3. Magyar férfi keresztnevek = magyar.keresztnev_f
+4. Magyar vegyes keresztnevek= magyar.keresztnev_v
+5. Magyar utcanevek = magyar.utca
+6. Magyar telelpülésnevek= magyar.telepules
+7. Magyar vármegyék nevei = magyar.megye
+8. Magyar folyók nevei = magyar.folyo
+9. A hét napjai magyarul = magyar.nap
+10. Az év hónapjai magyarul = magyar.honap
+11. A gyümölcsök magyar nevei = magyar.gyumolcs
+12. A zöldségek magyar nevei = magyar.zoldseg
+13. A haszonállatok magyar nevei = magyar.haszonallat
+14. Vadallatok Magyarországon = magyar.vadallat
 15. Magyarország halai = magyar.hal
 16. Magyarország madarai = magyar.madar
 17. A naprendszer bolygóinak magyar neve = magyar.bolygo
+18. Magyar leves nevek =  magyar.leves
+19. Magyar főételek = magyar.foetel
+20. Magyar köretek = magyar.koret
+21. Magyar egytál ételek = magyar.egytal
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -45,23 +37,28 @@
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
-8. he days of the week = magyar.nap
+8. The days of the week = magyar.nap
 9. the months of the year = magyar.honap
 10. fruits = magyar.gyumolcs
 11. vegetables = magyar.zoldseg
 12. domesticated animals = magyar.haszonallat
 13. hungarian wildlife  = magyar.vadallat
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
 16. Hungarian names of planets = magyar.bolygo
+17. Hungarian soup names = magyar.leves
+18. Hugarian given names M+F  magyar.keresztnev_v
+19. Hungarian main foods = magyar.foetel
+20. Hungarian side dishes  = magyar.koret
+21. Hungarian one-pot meals = magyar.egytal
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
@@ -102,8 +99,8 @@
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható.
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-2.9.6/README.md` & `magyar-2.9.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,46 @@
+Metadata-Version: 2.1
+Name: magyar
+Version: 2.9.7
+Summary: Hungarian names,animals,food, fruit, river ..
+Home-page: https://github.com/kobanya/nevek
+Author: Nagy Béla
+Author-email: nagy.belabudapest@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # magyar
 
 
 ## Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
-1. vezetéknevek   =  magyar.vezeteknev
-2. női keresztnevek  = magyar.keresztnev_n
-3. férfi keresztnevek = magyar.keresztnev_f
-4. Vegyes magyar keresztnevek= magyar.keresztnev_v
-5. utcanevek = magyar.utca
-6. telelpülésnevek= magyar.telepules
-7. vármegyék nevei = magyar.megye
-8. folyók nevei = magyar.folyo
-9. a hét napjai = magyar.nap
-10. az év hónapjai = magyar.honap
-11. gyümölcsok = magyar.gyumolcs
-12. zöldségek = magyar.zoldseg
-13. haszonállatok = magyar.haszonallat
-14. vadallatok Magyarországon = magyar.vadallat
+1. Magyar vezetéknevek   =  magyar.vezeteknev
+2. Magyar női keresztnevek  = magyar.keresztnev_n
+3. Magyar férfi keresztnevek = magyar.keresztnev_f
+4. Magyar vegyes keresztnevek= magyar.keresztnev_v
+5. Magyar utcanevek = magyar.utca
+6. Magyar telelpülésnevek= magyar.telepules
+7. Magyar vármegyék nevei = magyar.megye
+8. Magyar folyók nevei = magyar.folyo
+9. A hét napjai magyarul = magyar.nap
+10. Az év hónapjai magyarul = magyar.honap
+11. A gyümölcsök magyar nevei = magyar.gyumolcs
+12. A zöldségek magyar nevei = magyar.zoldseg
+13. A haszonállatok magyar nevei = magyar.haszonallat
+14. Vadallatok Magyarországon = magyar.vadallat
 15. Magyarország halai = magyar.hal
 16. Magyarország madarai = magyar.madar
 17. A naprendszer bolygóinak magyar neve = magyar.bolygo
+18. Magyar leves nevek =  magyar.leves
+19. Magyar főételek = magyar.foetel
+20. Magyar köretek = magyar.koret
+21. Magyar egytál ételek = magyar.egytal
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -33,23 +49,28 @@
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
-8. he days of the week = magyar.nap
+8. The days of the week = magyar.nap
 9. the months of the year = magyar.honap
 10. fruits = magyar.gyumolcs
 11. vegetables = magyar.zoldseg
 12. domesticated animals = magyar.haszonallat
 13. hungarian wildlife  = magyar.vadallat
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
 16. Hungarian names of planets = magyar.bolygo
+17. Hungarian soup names = magyar.leves
+18. Hugarian given names M+F  magyar.keresztnev_v
+19. Hungarian main foods = magyar.foetel
+20. Hungarian side dishes  = magyar.koret
+21. Hungarian one-pot meals = magyar.egytal
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
@@ -90,8 +111,8 @@
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható.
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-2.9.6/magyar.egg-info/PKG-INFO` & `magyar-2.9.7/magyar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.6
-Summary: Hungarian names...
+Version: 2.9.7
+Summary: Hungarian names,animals,food, fruit, river ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # magyar
 
 
 ## Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
-1. vezetéknevek   =  magyar.vezeteknev
-2. női keresztnevek  = magyar.keresztnev_n
-3. férfi keresztnevek = magyar.keresztnev_f
-4. Vegyes magyar keresztnevek= magyar.keresztnev_v
-5. utcanevek = magyar.utca
-6. telelpülésnevek= magyar.telepules
-7. vármegyék nevei = magyar.megye
-8. folyók nevei = magyar.folyo
-9. a hét napjai = magyar.nap
-10. az év hónapjai = magyar.honap
-11. gyümölcsok = magyar.gyumolcs
-12. zöldségek = magyar.zoldseg
-13. haszonállatok = magyar.haszonallat
-14. vadallatok Magyarországon = magyar.vadallat
+1. Magyar vezetéknevek   =  magyar.vezeteknev
+2. Magyar női keresztnevek  = magyar.keresztnev_n
+3. Magyar férfi keresztnevek = magyar.keresztnev_f
+4. Magyar vegyes keresztnevek= magyar.keresztnev_v
+5. Magyar utcanevek = magyar.utca
+6. Magyar telelpülésnevek= magyar.telepules
+7. Magyar vármegyék nevei = magyar.megye
+8. Magyar folyók nevei = magyar.folyo
+9. A hét napjai magyarul = magyar.nap
+10. Az év hónapjai magyarul = magyar.honap
+11. A gyümölcsök magyar nevei = magyar.gyumolcs
+12. A zöldségek magyar nevei = magyar.zoldseg
+13. A haszonállatok magyar nevei = magyar.haszonallat
+14. Vadallatok Magyarországon = magyar.vadallat
 15. Magyarország halai = magyar.hal
 16. Magyarország madarai = magyar.madar
 17. A naprendszer bolygóinak magyar neve = magyar.bolygo
+18. Magyar leves nevek =  magyar.leves
+19. Magyar főételek = magyar.foetel
+20. Magyar köretek = magyar.koret
+21. Magyar egytál ételek = magyar.egytal
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -45,23 +49,28 @@
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
-8. he days of the week = magyar.nap
+8. The days of the week = magyar.nap
 9. the months of the year = magyar.honap
 10. fruits = magyar.gyumolcs
 11. vegetables = magyar.zoldseg
 12. domesticated animals = magyar.haszonallat
 13. hungarian wildlife  = magyar.vadallat
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
 16. Hungarian names of planets = magyar.bolygo
+17. Hungarian soup names = magyar.leves
+18. Hugarian given names M+F  magyar.keresztnev_v
+19. Hungarian main foods = magyar.foetel
+20. Hungarian side dishes  = magyar.koret
+21. Hungarian one-pot meals = magyar.egytal
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
```

### Comparing `magyar-2.9.6/magyar.py` & `magyar-2.9.7/magyar.py`

 * *Files 7% similar despite different names*

```diff
@@ -137,14 +137,55 @@
 madar = ['feketerigó', 'fülemüle', 'csalogány', 'kékvércse', 'széncinege', 'szajkó', 'szürkebegy', 'búbosbanka',
          'zöldike', 'sármány', 'fácán', 'kakukk', 'bölömbika', 'örvényi sas', 'szirti sas', 'parlagi sas',
          'réti keselyű', 'héja', 'pávaszemes fecske', 'gyurgyalag', 'gólya', 'kócsag', 'hattyú', 'vadkacsa', 'vadlúd',
          'szárcsa', 'rigó', 'szajkó']
 
 bolygo =['Merkúr', 'Vénusz', 'Föld', 'Mars', 'Jupiter','Szaturnusz', 'Uránusz', 'Neptunusz']
 
+
+leves = ["Gulyásleves", "Halászlé", "Hideg meggyleves", "Zöldborsóleves", "Jókai bableves", "Csontleves",
+           "Marhahúsleves", "Zellerkrémleves", "Sárgaborsóleves", "Babgulyásleves", "Karalábéleves", "Zöldségleves",
+           "Kukoricaleves", "Karfiolleves", "Hideg gyümölcsleves", "Korhelyleves", "Tyúkhúsleves",
+           "Pirított tarhonyaleves", "Gombaleves", "Lencseleves", "Gulyáskrémleves", "Csülökleves", "Paradicsomleves",
+           "Borleves", "Tárkonyos raguleves", "Zöldbableves", "Kapros-joghurtos leves", "Paradicsomleves betűtésztával",
+           "Sajtos-tejfölös leves", "Burgonyaleves", "Csirkeleves", "Krumplileves",  "Tavaszi zöldségleves",
+           "Karfiol krémleves", "Tojásleves", "Tárkonyos csirkeraguleves", "Káposztaleves", "Húsos zöldborsóleves",
+           "Sárgadinnyeleves", "Tavaszi zöldségleves tarhonyával", "Hagymaleves",  "Húsleves gazdagon",
+           "Gesztenyekrémleves", "Jérceleves", "Kolbászos bableves", "Uborkaleves", "Tejszínes karfiolleves",
+           "Tarkabableves", "Hideg szilvaleves", "Fokhagymaleves", "Májgombócleves", "Brokkolileves",
+           "Savanyú káposztaleves", "Erőleves", "Tejfölös gombaleves",  "Húsos káposztaleves", "Zöldspárga krémleves",
+           "Sóska krémleves", "Burgonyapüréleves", "Laskaleves",  "Paradicsomleves húsgombóccal", "Csirkemájleves",
+           "Ribizlileves", "Cukkinikrémleves", "Fokhagymás zöldbableves", "Zöldségleves tojással"]
+
+foetel= ['Vadörkölt', 'Sült csirke',
+         'Sertésszelet', 'Rántott hús', 'Paprikás csirke', 'Sült kolbász', 'Rántott sajt', 'Rántott karfiol',
+         'Kacsacomb rántva', 'Kakaspörkölt',  'Sült hal', 'Túrós csusza', 'Gombapaprikás',
+         'Székelykáposzta', 'Marhapörkölt', 'Pacalpörkölt', 'Paprikás krumpli', 'Roston sült csirke',
+         'Rántott gomba', 'Rántott karaj', 'Rántott csirkemell', 'Rakott padlizsán', 'Halpaprikás', 'Libamáj',
+         'Sült sertés', 'Halpaprikás', 'Csülök Pékné módra', 'Borjúpörkölt ',
+        'Párizsi csirkemell', 'Rántott karaj', 'Kacsapörkölt', 'Csirkepaprikás',  'Rántott csirkeszárny', 'Pacalpörkölt',
+         'Rántott jércemell', 'Sertéspörkölt','Mátrai borzaska',
+       'Grillezett csirkecomb', 'Lecsós csirke', 'Rántott gomba tartármártással', 'Rántott ponty', 'Lazacsteak', 'Roston sült hal',
+       'Rántott camembert', 'Sült kacsacomb', 'Sült libacomb', 'Sült pulykamell', 'Sült tarja', 'Báránytokány',
+       'Szűzérmék',  'Cordon bleu', 'Sült Kacsamáj',
+       'Kapros-túrós csusza', 'Lecsós tarja', 'Stefánia vagdalt']
+
+koret = ['Párolt rizs', 'Hagymás tört burgonya', 'Burgonyapüré', 'Tócsni', 'Párolt zöldségek', 'Hasábburgonya',
+           'Grillezett zöldségek', 'Köleskása', 'Galuska', 'Zöldségköret', 'Kukoricás rizs', 'Sárgarépa püré',
+            'Zöldségpüré',  'Burgonyakrokett', 'Kuszkusz', 'Brokkolipüré', 'Párolt sárgarépa', 'Zellerpüré',
+           'Tarhonya',  'Zöldborsós rizs', 'Sajtos tócsni', 'Gombás rizs', 'Gersli',  'Sült édesburgonya',
+           'Édesburgonya püré',  'Hercegnő burgonya', 'Csónak burgonya', 'Tepsis burgonya']
+
+egytal = ['Rakott krumpli', 'Töltött káposzta', 'Lecsó','Töltött paprika','Lencsefőzelék sültkolbásszal','Hortobágyi húsos palacsinta',
+          'Sztrapacska szalonna pörccel','Burgonyás tészta','Csirkés rizottó','Rakott kelkáposzta csőben sütve',
+           'Rakott zöldbab', 'Disznótoros káposzta', 'Bácskai rizseshús', 'Brassói aprópecsenye','Tarhonyás hús',
+          'Székelykáposzta','Paradicsomos töltött káposzta','Rakott cukkini', 'Pásztortarhonya','Húsos-szaftos tészta',
+          'Lecsó Mezőcsáti módra', 'Sonkás-paradicsomos tészta', 'Sajtos-sonkás rakott tészta', 'Kolozsvári rakott káposzta',
+          'Sonkás tészta csőben sütve']
+
 kiraly = {'Árpád': (895, 907), 'Zoltán': (907, 947), 'Fajsz': (947, 955), 'Taksony': (955, 972), 'Géza': (972, 997),
     'I.István': (997, 1038),'I. Péter': (1038, 1041), 'Sámuel': (1041, 1044), 'Péter-2': (1044, 1045), 'I.András': (1041, 1060),
     'I. Béla': (1060, 1063), 'Salamon': (1063, 1074), 'I. Géza': (1074, 1077), 'I. László': (1077, 1095),
     'Kálmán': (1095, 1116),'II. István': (1116, 1131), 'II. Béla': (1131, 1141), 'II. Géza': (1141,1162),
     'III. István': (1162, 1172), 'III. Béla': (1172, 1196), 'Imre':(1196, 1204), 'III. László': (1204, 1205),
     'II. András': (1205, 1235),'IV. Béla': (1235, 1270), 'V. István': (1270, 1272), 'IV. László': (1272, 1290),
     'III. András': (1290, 1301), 'Vencel': (1301, 1305), 'Ottó': (1305, 1307), 'I. Károly': (1308, 1342),
```

### Comparing `magyar-2.9.6/setup.py` & `magyar-2.9.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.6",
+    version="2.9.7",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
-    description="Hungarian names...",
+    description="Hungarian names,animals,food, fruit, river ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

