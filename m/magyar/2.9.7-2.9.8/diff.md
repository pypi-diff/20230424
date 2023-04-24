# Comparing `tmp/magyar-2.9.7.tar.gz` & `tmp/magyar-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.7.tar", last modified: Sun Apr 23 21:59:26 2023, max compression
+gzip compressed data, was "magyar-2.9.8.tar", last modified: Mon Apr 24 08:06:58 2023, max compression
```

## Comparing `magyar-2.9.7.tar` & `magyar-2.9.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-23 21:59:26.149057 magyar-2.9.7/
--rw-rw-r--   0 bela      (1000) bela      (1000)     4425 2023-04-23 21:59:26.149057 magyar-2.9.7/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     4027 2023-04-23 21:52:25.000000 magyar-2.9.7/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-23 21:59:26.149057 magyar-2.9.7/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     4425 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-23 21:59:26.000000 magyar-2.9.7/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    35788 2023-04-23 21:57:33.000000 magyar-2.9.7/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-23 21:59:26.149057 magyar-2.9.7/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      615 2023-04-23 20:29:52.000000 magyar-2.9.7/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-24 08:06:58.405506 magyar-2.9.8/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5329 2023-04-24 08:06:58.405506 magyar-2.9.8/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     4931 2023-04-24 08:05:27.000000 magyar-2.9.8/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-24 08:06:58.401506 magyar-2.9.8/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5329 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-24 08:06:58.000000 magyar-2.9.8/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    36025 2023-04-24 08:05:27.000000 magyar-2.9.8/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-24 08:06:58.405506 magyar-2.9.8/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      615 2023-04-24 07:32:32.000000 magyar-2.9.8/setup.py
```

### Comparing `magyar-2.9.7/magyar.py` & `magyar-2.9.8/magyar.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
            'lilakáposzta', 'padlizsán', 'paprika', 'paszternák', 'retek', 'sárgarépa', 'spárga', 'spenót',
            'sütőtök', 'tök', 'uborka', 'zeller', 'sárgarépa', 'feketeretek','zeller', 'kínai kel', 'retek',
            'jégcsapretek', 'fokhagyma', 'újhagyma', 'szárzeller']
 
 haszonallat = [ 'tehén', 'juh', 'kecske', 'disznó', 'tyúk', 'kacsa', 'liba', 'pulyka', 'strucc', 'ló', 'szamár', 'bivaly',
                  'jak', 'csirke', 'nyúl', 'szarvasmarha', 'szürkemarha', 'sertés', 'malac', 'gyöngytyúk', 'birka']
 
-vadallat = ['medve', 'farkas', 'róka', 'borz', 'őz', 'szarvas','nyest', 'vaddisznó','muflon','vidra',
+vad = ['medve', 'farkas', 'róka', 'borz', 'őz', 'szarvas','nyest', 'vaddisznó','muflon','vidra',
             'gímszarvas', 'molnárgörény','vadmacska']
 
 hal = ['keszeg', 'ponty', 'csuka', 'harcsa', 'süllő', 'kárász', 'angolna', 'márna', 'fogasponty', 'sügér', 'amur',
          'menyhal', 'domolykó', 'keszeg', 'garda', 'paduc', 'compó', 'bodorka', 'nyúldomolykó']
 
 madar = ['feketerigó', 'fülemüle', 'csalogány', 'kékvércse', 'széncinege', 'szajkó', 'szürkebegy', 'búbosbanka',
          'zöldike', 'sármány', 'fácán', 'kakukk', 'bölömbika', 'örvényi sas', 'szirti sas', 'parlagi sas',
@@ -356,7 +356,14 @@
     veletlen_kulcsok = []
     for i in range(n):
         kulcs_index = hash(str(i)) % len(kulcsok)
         veletlen_kulcs = kulcsok[kulcs_index]
         veletlen_kulcsok.append(veletlen_kulcs)
     return veletlen_kulcsok
 
+def tordel(lst, n=None):  # lst = kiírandó lista, n = hany kerüljön  egy sorba
+    if n is None:
+        n = 10
+    for i in range(0, len(lst), n):
+        row = lst[i:i+n]
+        print(", ".join(map(str, row)), end=", ")
+        print()
```

### Comparing `magyar-2.9.7/setup.py` & `magyar-2.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.7",
+    version="2.9.8",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names,animals,food, fruit, river ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

