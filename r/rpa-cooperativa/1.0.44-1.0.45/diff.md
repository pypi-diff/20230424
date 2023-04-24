# Comparing `tmp/rpa_cooperativa-1.0.44.tar.gz` & `tmp/rpa_cooperativa-1.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.44.tar", last modified: Fri Apr 14 16:19:48 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.45.tar", last modified: Mon Apr 24 14:20:46 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.44.tar` & `rpa_cooperativa-1.0.45.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.582793 rpa_cooperativa-1.0.44/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.44/LICENSE
--rw-rw-rw-   0        0        0     6237 2023-04-14 16:19:48.571153 rpa_cooperativa-1.0.44/PKG-INFO
--rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.44/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.014308 rpa_cooperativa-1.0.44/rpa_coop/
--rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.44/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.456875 rpa_cooperativa-1.0.44/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.44/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.44/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.44/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      347 2023-02-28 19:51:44.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siac_verde.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0      336 2023-02-28 19:52:19.000000 rpa_cooperativa-1.0.44/rpa_coop/img/siat_verde.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.44/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.44/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    71296 2023-04-14 13:41:26.000000 rpa_cooperativa-1.0.44/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:19:48.553872 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6237 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 16:19:46.000000 rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 16:19:48.587124 rpa_cooperativa-1.0.44/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-04-14 12:23:09.000000 rpa_cooperativa-1.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:20:46.088781 rpa_cooperativa-1.0.45/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.45/LICENSE
+-rw-rw-rw-   0        0        0     6237 2023-04-24 14:20:46.077597 rpa_cooperativa-1.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0     5088 2023-04-13 17:54:03.000000 rpa_cooperativa-1.0.45/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 14:20:45.445193 rpa_cooperativa-1.0.45/rpa_coop/
+-rw-rw-rw-   0        0        0      545 2023-04-13 14:56:13.000000 rpa_cooperativa-1.0.45/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:20:45.846178 rpa_cooperativa-1.0.45/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.45/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.45/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.45/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.45/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.45/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.45/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    71299 2023-04-24 14:17:17.000000 rpa_cooperativa-1.0.45/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:20:46.054700 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6237 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-04-24 14:20:44.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 14:20:43.000000 rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 14:20:46.092352 rpa_cooperativa-1.0.45/setup.cfg
+-rw-rw-rw-   0        0        0     2323 2023-04-24 14:20:34.000000 rpa_cooperativa-1.0.45/setup.py
```

### Comparing `rpa_cooperativa-1.0.44/LICENSE` & `rpa_cooperativa-1.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/PKG-INFO` & `rpa_cooperativa-1.0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.44
+Version: 1.0.45
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.44/README.md` & `rpa_cooperativa-1.0.45/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.45/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.45/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.45/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.45/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.45/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1124,22 +1124,22 @@
         if 'SACG' in str(siat_siac_sacg).upper():
             try:
                 posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png')
             except:
                 posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png')
         elif 'SIAT' in str(siat_siac_sacg).upper():
             try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png')
             except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_verde.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png')
         elif 'SIAC' in str(siat_siac_sacg).upper():
             try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png')
             except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_verde.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png')
         time.sleep(1)
         self.p.click(posicao)
         print('selecionou o menu: siat, siac, sacg')
         time.sleep(3)
         
         if transacional:
             self.p.moveTo(janela.left + 48, janela.top + 165)
```

### Comparing `rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.44
+Version: 1.0.45
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 rpa_coop/rpa_coop.py
 rpa_coop/img/hash
 rpa_coop/img/relatorios_azul.PNG
 rpa_coop/img/relatorios_verde.PNG
 rpa_coop/img/sacg_branco.PNG
 rpa_coop/img/sagc_verde.PNG
 rpa_coop/img/siac_amarelo.PNG
-rpa_coop/img/siac_verde.PNG
+rpa_coop/img/siac_branco.PNG
+rpa_coop/img/siat_amarelo.PNG
 rpa_coop/img/siat_branco.PNG
-rpa_coop/img/siat_verde.PNG
 rpa_coop/img/transacional_azul.PNG
 rpa_coop/img/transacional_verde.PNG
 rpa_cooperativa.egg-info/PKG-INFO
 rpa_cooperativa.egg-info/SOURCES.txt
 rpa_cooperativa.egg-info/dependency_links.txt
 rpa_cooperativa.egg-info/not-zip-safe
 rpa_cooperativa.egg-info/requires.txt
```

### Comparing `rpa_cooperativa-1.0.44/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.45/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.44/setup.py` & `rpa_cooperativa-1.0.45/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.44",
+    version="1.0.45",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

