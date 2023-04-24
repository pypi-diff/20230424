# Comparing `tmp/met-brewer-1.0.1.tar.gz` & `tmp/met-brewer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "met-brewer-1.0.1.tar", last modified: Mon Apr 24 09:43:47 2023, max compression
+gzip compressed data, was "met-brewer-1.0.2.tar", last modified: Mon Apr 24 09:49:20 2023, max compression
```

## Comparing `met-brewer-1.0.1.tar` & `met-brewer-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:43:47.757023 met-brewer-1.0.1/
--rw-rw-rw-   0        0        0    21147 2023-04-24 09:43:47.755028 met-brewer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    20561 2023-04-24 08:58:03.000000 met-brewer-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:43:47.739030 met-brewer-1.0.1/met_brewer/
--rw-rw-rw-   0        0        0      265 2023-04-22 19:04:51.000000 met-brewer-1.0.1/met_brewer/__init__.py
--rw-rw-rw-   0        0        0    19399 2023-04-24 08:45:56.000000 met-brewer-1.0.1/met_brewer/palettes.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:43:47.752025 met-brewer-1.0.1/met_brewer.egg-info/
--rw-rw-rw-   0        0        0    21147 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 09:43:47.757023 met-brewer-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      420 2023-04-24 09:41:40.000000 met-brewer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:49:20.056883 met-brewer-1.0.2/
+-rw-rw-rw-   0        0        0    19382 2023-04-24 09:49:20.054883 met-brewer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18867 2023-04-24 09:47:26.000000 met-brewer-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:49:20.043882 met-brewer-1.0.2/met_brewer/
+-rw-rw-rw-   0        0        0      265 2023-04-22 19:04:51.000000 met-brewer-1.0.2/met_brewer/__init__.py
+-rw-rw-rw-   0        0        0    19399 2023-04-24 08:45:56.000000 met-brewer-1.0.2/met_brewer/palettes.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:49:20.052883 met-brewer-1.0.2/met_brewer.egg-info/
+-rw-rw-rw-   0        0        0    19382 2023-04-24 09:49:19.000000 met-brewer-1.0.2/met_brewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-24 09:49:19.000000 met-brewer-1.0.2/met_brewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:49:19.000000 met-brewer-1.0.2/met_brewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-24 09:49:19.000000 met-brewer-1.0.2/met_brewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 09:49:19.000000 met-brewer-1.0.2/met_brewer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:49:20.056883 met-brewer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      420 2023-04-24 09:47:46.000000 met-brewer-1.0.2/setup.py
```

### Comparing `met-brewer-1.0.1/PKG-INFO` & `met-brewer-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: met-brewer
-Version: 1.0.1
+Version: 1.0.2
 Description-Content-Type: text/markdown
 
 # MetBrewer <img align="right" src="https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Hex/MetBrewerHex.jpg" width=400>
 Palettes inspired by works at the Metropolitan Museum of Art in New York. Pieces selected come from various time periods, regions, and mediums.
 
 ![CRAN Version](https://www.r-pkg.org/badges/version/MetBrewer)
 ![CRAN Downloads](https://cranlogs.r-pkg.org/badges/MetBrewer)
@@ -21,25 +21,14 @@
     - [Python](#python)
   - [Palettes](#palettes)
   - [Functions](#functions)
     - [ggplot2 Examples](#ggplot2-examples)
   - [Colorblind Friendly Checking](#colorblind-friendly-checking)
 
 ## Install Package
-### R
-MetBrewer is now able to be downloaded directly through R. You can still download through GitHub as well.
-
-```r
-install.packages("MetBrewer")
-
-install.packages("devtools")
-devtools::install_github("BlakeRMills/MetBrewer")
-```
-
-### Python
 Install via PyPA:
 ```
 pip install met-brewer
 ```
 or via pip directly from GitHub:
 ```
 pip install -e git+https://github.com/BlakeRMills/MetBrewer#subdirectory=Python
@@ -366,126 +355,66 @@
 
 ### Wissing
 ![Wissing](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Wissing.png)
 - Portrait of a Woman, 1687, Willem Wissing, Dutch, [Link](https://www.metmuseum.org/art/collection/search/437945)
 
 
 ## Functions
-```r
 You can retrieve palettes using various methods listed below.
 
-Python
+```python
 met_brew(name="VanGogh1", n=7, brew_type="discrete")
-
-R
-met.brewer(name="VanGogh1", n=7, type="discrete")
 ```
 ![Ex1](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%201.png)
 
-```r
-Python
+```python
 met_brew(name="Manet", n=5)
-
-R
-met.brewer("Manet", 5)
 ```
 ![Ex2](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%202.png)
 
 
-```r
-Python
+```python
 met_brew("Morgenstern")
-
-R
-met.brewer("Morgenstern")
 ```
 ![Ex3](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%203%20(Update).png)
 
-
-```r
-Python
+```python
 met_brew("Troy", n=15, brew_type="continuous")
-
-R
-met.brewer("Troy", n=15, type="continuous")
 ```
 ![Ex4](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%204.png)
 
-```r
-Python
+```python
 met_brew("Hokusai1", n=100, brew_type="continuous")
-
-R
-met.brewer("Hokusai1", n=100)
 ```
 ![Ex5](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example5.png)
 
 ### ggplot2 Examples
 
 Here are also some ways you can incorporate this package into {ggplot2}
 
-```r
-ggplot(data=iris, aes(x=Species, y=Petal.Length, fill=Species)) +
-  geom_violin() +
-  scale_fill_manual(values=met.brewer("Greek", 3))
-```
 ![Ex6](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/FillExample.png)
 
-```r
-ggplot(data=iris, aes(x=Sepal.Length, y=Sepal.Width, color=Species)) +
-  geom_point(size=2) +
-  scale_color_manual(values=met.brewer("Renoir", 3))
-```
 ![Ex7](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/ColorExample.png)
 
-```r
-ggplot(data=iris, aes(x=Species, y=Sepal.Width, color=Sepal.Width)) +
-  geom_point(size=3) +
-  scale_color_gradientn(colors=met.brewer("Isfahan1"))
-```
 ![Ex8](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/GradientColorExample.png)
 
-```r
-library(urbnmapr)
-countydata %>%
-  left_join(counties, by = "county_fips") %>%
-  filter(state_name =="Nebraska") %>%
-  ggplot(mapping=aes(long,lat,group = group, fill = horate)) +
-  geom_polygon(color="black",size=.25) +
-  scale_fill_gradientn(colors = met.brewer("Morgenstern")) +
-  coord_fixed() +
-  labs(fill="Homeownership rate") +
-  theme_void()
-```
 ![Ex9](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/GradientFillExample%20(Update).png)
 
 
 ## Colorblind Friendly Checking
 The package has been updated to check for colorblind-friendlyness
 You can list out the colorblind-friendly palettes with the following code
 ```r
 Python
 for palette_name, palette_dict in COLORBLIND_PALETTES.items():
     print(palette_name)
 
 [1] Cassatt1, Cassatt2, Derain, Egypt, Greek, Hiroshige, Hokusai2, Hokusai3, Ingres
 [2] Isfahan1, Isfahan2, Morgenstern, OKeeffe1, OKeeffe2, Pillement, Troy, VanGogh3, Veronese
-
-R
-MetBrewer::colorblind_palettes
-
- [1] "Archambault" "Cassatt1"    "Cassatt2"    "Demuth"      "Derain"      "Egypt"       "Greek"       "Hiroshige"
- [9] "Hokusai2"    "Hokusai3"    "Ingres"      "Isfahan1"    "Isfahan2"    "Java"        "Johnson"     "Kandinsky"
-[17] "Morgenstern" "OKeeffe1"    "OKeeffe2"    "Pillement"   "Tam"         "Troy"        "VanGogh3"    "Veronese"
 ```
 
 You can also test if a palette is colorblind friendly using the function provided
 
-```r
-Python
+```python
 is_colorblind_friendly("Ingres")
 [1] True
-
-R
-MetBrewer::colorblind.friendly("Ingres")
-[1] TRUE
 ```
```

### Comparing `met-brewer-1.0.1/README.md` & `met-brewer-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,14 @@
     - [Python](#python)
   - [Palettes](#palettes)
   - [Functions](#functions)
     - [ggplot2 Examples](#ggplot2-examples)
   - [Colorblind Friendly Checking](#colorblind-friendly-checking)
 
 ## Install Package
-### R
-MetBrewer is now able to be downloaded directly through R. You can still download through GitHub as well.
-
-```r
-install.packages("MetBrewer")
-
-install.packages("devtools")
-devtools::install_github("BlakeRMills/MetBrewer")
-```
-
-### Python
 Install via PyPA:
 ```
 pip install met-brewer
 ```
 or via pip directly from GitHub:
 ```
 pip install -e git+https://github.com/BlakeRMills/MetBrewer#subdirectory=Python
@@ -361,126 +350,66 @@
 
 ### Wissing
 ![Wissing](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Wissing.png)
 - Portrait of a Woman, 1687, Willem Wissing, Dutch, [Link](https://www.metmuseum.org/art/collection/search/437945)
 
 
 ## Functions
-```r
 You can retrieve palettes using various methods listed below.
 
-Python
+```python
 met_brew(name="VanGogh1", n=7, brew_type="discrete")
-
-R
-met.brewer(name="VanGogh1", n=7, type="discrete")
 ```
 ![Ex1](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%201.png)
 
-```r
-Python
+```python
 met_brew(name="Manet", n=5)
-
-R
-met.brewer("Manet", 5)
 ```
 ![Ex2](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%202.png)
 
 
-```r
-Python
+```python
 met_brew("Morgenstern")
-
-R
-met.brewer("Morgenstern")
 ```
 ![Ex3](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%203%20(Update).png)
 
-
-```r
-Python
+```python
 met_brew("Troy", n=15, brew_type="continuous")
-
-R
-met.brewer("Troy", n=15, type="continuous")
 ```
 ![Ex4](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%204.png)
 
-```r
-Python
+```python
 met_brew("Hokusai1", n=100, brew_type="continuous")
-
-R
-met.brewer("Hokusai1", n=100)
 ```
 ![Ex5](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example5.png)
 
 ### ggplot2 Examples
 
 Here are also some ways you can incorporate this package into {ggplot2}
 
-```r
-ggplot(data=iris, aes(x=Species, y=Petal.Length, fill=Species)) +
-  geom_violin() +
-  scale_fill_manual(values=met.brewer("Greek", 3))
-```
 ![Ex6](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/FillExample.png)
 
-```r
-ggplot(data=iris, aes(x=Sepal.Length, y=Sepal.Width, color=Species)) +
-  geom_point(size=2) +
-  scale_color_manual(values=met.brewer("Renoir", 3))
-```
 ![Ex7](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/ColorExample.png)
 
-```r
-ggplot(data=iris, aes(x=Species, y=Sepal.Width, color=Sepal.Width)) +
-  geom_point(size=3) +
-  scale_color_gradientn(colors=met.brewer("Isfahan1"))
-```
 ![Ex8](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/GradientColorExample.png)
 
-```r
-library(urbnmapr)
-countydata %>%
-  left_join(counties, by = "county_fips") %>%
-  filter(state_name =="Nebraska") %>%
-  ggplot(mapping=aes(long,lat,group = group, fill = horate)) +
-  geom_polygon(color="black",size=.25) +
-  scale_fill_gradientn(colors = met.brewer("Morgenstern")) +
-  coord_fixed() +
-  labs(fill="Homeownership rate") +
-  theme_void()
-```
 ![Ex9](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/GradientFillExample%20(Update).png)
 
 
 ## Colorblind Friendly Checking
 The package has been updated to check for colorblind-friendlyness
 You can list out the colorblind-friendly palettes with the following code
 ```r
 Python
 for palette_name, palette_dict in COLORBLIND_PALETTES.items():
     print(palette_name)
 
 [1] Cassatt1, Cassatt2, Derain, Egypt, Greek, Hiroshige, Hokusai2, Hokusai3, Ingres
 [2] Isfahan1, Isfahan2, Morgenstern, OKeeffe1, OKeeffe2, Pillement, Troy, VanGogh3, Veronese
-
-R
-MetBrewer::colorblind_palettes
-
- [1] "Archambault" "Cassatt1"    "Cassatt2"    "Demuth"      "Derain"      "Egypt"       "Greek"       "Hiroshige"
- [9] "Hokusai2"    "Hokusai3"    "Ingres"      "Isfahan1"    "Isfahan2"    "Java"        "Johnson"     "Kandinsky"
-[17] "Morgenstern" "OKeeffe1"    "OKeeffe2"    "Pillement"   "Tam"         "Troy"        "VanGogh3"    "Veronese"
 ```
 
 You can also test if a palette is colorblind friendly using the function provided
 
-```r
-Python
+```python
 is_colorblind_friendly("Ingres")
 [1] True
-
-R
-MetBrewer::colorblind.friendly("Ingres")
-[1] TRUE
 ```
```

### Comparing `met-brewer-1.0.1/met_brewer/palettes.py` & `met-brewer-1.0.2/met_brewer/palettes.py`

 * *Files identical despite different names*

### Comparing `met-brewer-1.0.1/met_brewer.egg-info/PKG-INFO` & `met-brewer-1.0.2/met_brewer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: met-brewer
-Version: 1.0.1
+Version: 1.0.2
 Description-Content-Type: text/markdown
 
 # MetBrewer <img align="right" src="https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Hex/MetBrewerHex.jpg" width=400>
 Palettes inspired by works at the Metropolitan Museum of Art in New York. Pieces selected come from various time periods, regions, and mediums.
 
 ![CRAN Version](https://www.r-pkg.org/badges/version/MetBrewer)
 ![CRAN Downloads](https://cranlogs.r-pkg.org/badges/MetBrewer)
@@ -21,25 +21,14 @@
     - [Python](#python)
   - [Palettes](#palettes)
   - [Functions](#functions)
     - [ggplot2 Examples](#ggplot2-examples)
   - [Colorblind Friendly Checking](#colorblind-friendly-checking)
 
 ## Install Package
-### R
-MetBrewer is now able to be downloaded directly through R. You can still download through GitHub as well.
-
-```r
-install.packages("MetBrewer")
-
-install.packages("devtools")
-devtools::install_github("BlakeRMills/MetBrewer")
-```
-
-### Python
 Install via PyPA:
 ```
 pip install met-brewer
 ```
 or via pip directly from GitHub:
 ```
 pip install -e git+https://github.com/BlakeRMills/MetBrewer#subdirectory=Python
@@ -366,126 +355,66 @@
 
 ### Wissing
 ![Wissing](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Wissing.png)
 - Portrait of a Woman, 1687, Willem Wissing, Dutch, [Link](https://www.metmuseum.org/art/collection/search/437945)
 
 
 ## Functions
-```r
 You can retrieve palettes using various methods listed below.
 
-Python
+```python
 met_brew(name="VanGogh1", n=7, brew_type="discrete")
-
-R
-met.brewer(name="VanGogh1", n=7, type="discrete")
 ```
 ![Ex1](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%201.png)
 
-```r
-Python
+```python
 met_brew(name="Manet", n=5)
-
-R
-met.brewer("Manet", 5)
 ```
 ![Ex2](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%202.png)
 
 
-```r
-Python
+```python
 met_brew("Morgenstern")
-
-R
-met.brewer("Morgenstern")
 ```
 ![Ex3](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%203%20(Update).png)
 
-
-```r
-Python
+```python
 met_brew("Troy", n=15, brew_type="continuous")
-
-R
-met.brewer("Troy", n=15, type="continuous")
 ```
 ![Ex4](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example%204.png)
 
-```r
-Python
+```python
 met_brew("Hokusai1", n=100, brew_type="continuous")
-
-R
-met.brewer("Hokusai1", n=100)
 ```
 ![Ex5](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/Example5.png)
 
 ### ggplot2 Examples
 
 Here are also some ways you can incorporate this package into {ggplot2}
 
-```r
-ggplot(data=iris, aes(x=Species, y=Petal.Length, fill=Species)) +
-  geom_violin() +
-  scale_fill_manual(values=met.brewer("Greek", 3))
-```
 ![Ex6](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/FillExample.png)
 
-```r
-ggplot(data=iris, aes(x=Sepal.Length, y=Sepal.Width, color=Species)) +
-  geom_point(size=2) +
-  scale_color_manual(values=met.brewer("Renoir", 3))
-```
 ![Ex7](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/ColorExample.png)
 
-```r
-ggplot(data=iris, aes(x=Species, y=Sepal.Width, color=Sepal.Width)) +
-  geom_point(size=3) +
-  scale_color_gradientn(colors=met.brewer("Isfahan1"))
-```
 ![Ex8](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/GradientColorExample.png)
 
-```r
-library(urbnmapr)
-countydata %>%
-  left_join(counties, by = "county_fips") %>%
-  filter(state_name =="Nebraska") %>%
-  ggplot(mapping=aes(long,lat,group = group, fill = horate)) +
-  geom_polygon(color="black",size=.25) +
-  scale_fill_gradientn(colors = met.brewer("Morgenstern")) +
-  coord_fixed() +
-  labs(fill="Homeownership rate") +
-  theme_void()
-```
 ![Ex9](https://github.com/BlakeRMills/MetBrewer/blob/main/PaletteImages/Examples/GradientFillExample%20(Update).png)
 
 
 ## Colorblind Friendly Checking
 The package has been updated to check for colorblind-friendlyness
 You can list out the colorblind-friendly palettes with the following code
 ```r
 Python
 for palette_name, palette_dict in COLORBLIND_PALETTES.items():
     print(palette_name)
 
 [1] Cassatt1, Cassatt2, Derain, Egypt, Greek, Hiroshige, Hokusai2, Hokusai3, Ingres
 [2] Isfahan1, Isfahan2, Morgenstern, OKeeffe1, OKeeffe2, Pillement, Troy, VanGogh3, Veronese
-
-R
-MetBrewer::colorblind_palettes
-
- [1] "Archambault" "Cassatt1"    "Cassatt2"    "Demuth"      "Derain"      "Egypt"       "Greek"       "Hiroshige"
- [9] "Hokusai2"    "Hokusai3"    "Ingres"      "Isfahan1"    "Isfahan2"    "Java"        "Johnson"     "Kandinsky"
-[17] "Morgenstern" "OKeeffe1"    "OKeeffe2"    "Pillement"   "Tam"         "Troy"        "VanGogh3"    "Veronese"
 ```
 
 You can also test if a palette is colorblind friendly using the function provided
 
-```r
-Python
+```python
 is_colorblind_friendly("Ingres")
 [1] True
-
-R
-MetBrewer::colorblind.friendly("Ingres")
-[1] TRUE
 ```
```

