# Comparing `tmp/sitcom-1.0.2.tar.gz` & `tmp/sitcom-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitcom-1.0.2.tar", last modified: Mon Apr 24 14:18:05 2023, max compression
+gzip compressed data, was "sitcom-1.3.0.tar", last modified: Tue Apr 25 01:33:16 2023, max compression
```

## Comparing `sitcom-1.0.2.tar` & `sitcom-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.639774 sitcom-1.0.2/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.0.2/LICENSE
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 14:18:05.639774 sitcom-1.0.2/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-1.0.2/README.md
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-24 14:18:05.639774 sitcom-1.0.2/setup.cfg
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      496 2023-04-24 14:17:53.000000 sitcom-1.0.2/setup.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.627774 sitcom-1.0.2/sitcom/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.0.2/sitcom/__init__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    47375 2023-04-24 14:14:54.000000 sitcom-1.0.2/sitcom/__main__.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom/data/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    84116 2023-04-06 22:34:38.000000 sitcom-1.0.2/sitcom/data/Sine_curve.png
--rw-rw-r--   0 purvi     (1000) purvi     (1000)   539595 2023-04-06 14:35:36.000000 sitcom-1.0.2/sitcom/data/black.png
--rw-rw-r--   0 purvi     (1000) purvi     (1000)   599404 2023-04-06 14:33:58.000000 sitcom-1.0.2/sitcom/data/white.png
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom/icon/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     4022 2023-04-19 18:48:40.000000 sitcom-1.0.2/sitcom/icon/cme.ico
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    29744 2023-02-14 09:29:04.000000 sitcom-1.0.2/sitcom/icon/cme.png
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom/load/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)  9159608 2023-02-26 07:43:28.000000 sitcom-1.0.2/sitcom/load/sitcom.gif
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.0.2/sitcom/sfit.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.0.2/sitcom/sirgraf.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    37366 2023-04-24 14:16:42.000000 sitcom-1.0.2/sitcom/st1.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     4571 2023-04-24 13:39:46.000000 sitcom-1.0.2/sitcom/st2.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-24 14:18:05.631774 sitcom-1.0.2/sitcom.egg-info/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      408 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/SOURCES.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/dependency_links.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/requires.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-24 14:18:05.000000 sitcom-1.0.2/sitcom.egg-info/top_level.txt
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.767969 sitcom-1.3.0/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.3.0/LICENSE
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-25 01:33:16.767969 sitcom-1.3.0/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-1.3.0/README.md
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-25 01:33:16.767969 sitcom-1.3.0/setup.cfg
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      533 2023-04-25 01:32:58.000000 sitcom-1.3.0/setup.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    47787 2023-04-25 01:30:08.000000 sitcom-1.3.0/sitcom/__main__.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/data/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    84116 2023-04-06 22:34:38.000000 sitcom-1.3.0/sitcom/data/Sine_curve.png
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/data/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)   539595 2023-04-06 14:35:36.000000 sitcom-1.3.0/sitcom/data/black.png
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)   599404 2023-04-06 14:33:58.000000 sitcom-1.3.0/sitcom/data/white.png
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/icon/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/icon/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4022 2023-04-19 18:48:40.000000 sitcom-1.3.0/sitcom/icon/cme.ico
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    29744 2023-02-14 09:29:04.000000 sitcom-1.3.0/sitcom/icon/cme.png
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/load/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/load/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)  9159608 2023-02-26 07:43:28.000000 sitcom-1.3.0/sitcom/load/sitcom.gif
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.3.0/sitcom/sfit.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.3.0/sitcom/sirgraf.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    37469 2023-04-24 18:02:33.000000 sitcom-1.3.0/sitcom/st1.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4635 2023-04-24 18:08:08.000000 sitcom-1.3.0/sitcom/st2.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom.egg-info/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      480 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/requires.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/top_level.txt
```

### Comparing `sitcom-1.0.2/LICENSE` & `sitcom-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/README.md` & `sitcom-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/__main__.py` & `sitcom-1.3.0/sitcom/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 import matplotlib.pyplot as plt
 import matplotlib.patches as pa
 import matplotlib.animation as animation
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 import numpy as np
 import glob,os,cv2,platform
-import time,sys
+import time,sys,site
 import sitcom.sirgraf as sf
 
 
 from astropy.io import fits
 from astropy.visualization import ZScaleInterval
 
 if platform.system()=='Windows':
 	import moviepy.editor as mpe
 
 mp.use('Qt5Agg')
 mp.rcParams['font.family'] = 'monospace'
 
 from sitcom.st1 import Ui_SecondWindow
 
+
+
 import warnings
 warnings.filterwarnings("ignore")
 class Load_Window(QtWidgets.QSplashScreen):
     def __init__(self, movie, parent=None):
         movie.jumpToFrame(0)
         pixmap = QtGui.QPixmap(movie.frameRect().size())
 
@@ -44,17 +46,23 @@
         painter.drawPixmap(0, 0, pixmap)
 class Ui_MainWindow(object):     
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.setFixedWidth(1000)
         MainWindow.setFixedHeight(550)
         icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap("icon/cme.png"), QtGui.QIcon.Normal, QtGui.QIcon.On)
+        ci=os.path.join(site.USER_SITE,'sitcom/icon/cme.png')
+        icon.addPixmap(QtGui.QPixmap(ci), QtGui.QIcon.Normal, QtGui.QIcon.On)
         MainWindow.setWindowIcon(icon)
         MainWindow.setIconSize(QtCore.QSize(40, 30))
+        cf=os.path.join(site.USER_SITE,'sitcom/font/lato/Lato-Semibold.ttf')
+        _id=QtGui.QFontDatabase.addApplicationFont(cf)
+        custom_font = QtGui.QFontDatabase.applicationFontFamilies(_id)[0] 
+        font = QtGui.QFont(custom_font, 11)
+        font.setWeight(30)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         #########################################################
         self.Browse = QtWidgets.QPushButton(self.centralwidget)
         self.Browse.setGeometry(QtCore.QRect(330, 10, 89, 31))
         self.Browse.setObjectName("Browse")
         self.Browse_le = QtWidgets.QLineEdit(self.centralwidget)
@@ -543,15 +551,16 @@
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()
     def light(self):
         self.t.append('Light')
         #MainWindow=QtWidgets.QMainWindow()
-        MainWindow.setStyleSheet("QMainWindow{border-image: url(data/white.png); background-repeat:no-repeat; background-position: center;}")
+        cw=os.path.join(site.USER_SITE,'sitcom/data/white.png')
+        MainWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}")
         self.figure.set_facecolor('white')
         mp.rcParams.update({'text.color' : "black",'axes.labelcolor' : "black",'axes.edgecolor':"black",'axes.facecolor':"white",'xtick.color':"black",'ytick.color':"black"})
         #self.setupUi(MainWindow)
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
           self.Minimum.click()
@@ -563,15 +572,16 @@
           self.Final.click()
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()   
     def dark(self):
         self.t.append('Dark')
-        MainWindow.setStyleSheet("QMainWindow{border-image: url(data/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
+        cw=os.path.join(site.USER_SITE,'sitcom/data/black.png')
+        MainWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
         self.figure.patch.set_facecolor('black')
         mp.rcParams.update({'text.color' : "white",'axes.labelcolor' : "white",'axes.labelcolor' : "white",'axes.edgecolor':"white",'axes.facecolor':"black",'xtick.color':"white",'ytick.color':"white"})
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
           self.Minimum.click()
         elif self.s[-1]=="Filtered":
@@ -910,16 +920,16 @@
       self.ani.event_source.start()
 
 
  
 
 if __name__ == "__main__":
     app = QtWidgets.QApplication(sys.argv)
-    movie=QtGui.QMovie('sitcom/load/sitcom.gif')
-    QtGui.QFontDatabase.addApplicationFont('font/lato/Lato-Semibold.ttf')
+    cl=os.path.join(site.USER_SITE,'sitcom/load/sitcom.gif')
+    movie=QtGui.QMovie(cl)
     splash = Load_Window(movie)
     splash.show()
     splash.movie.start()
     start = time.time()
     while movie.state() == QtGui.QMovie.Running and time.time() < start + 4:
         app.processEvents()
     MainWindow = QtWidgets.QMainWindow()
```

### Comparing `sitcom-1.0.2/sitcom/data/Sine_curve.png` & `sitcom-1.3.0/sitcom/data/Sine_curve.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/data/black.png` & `sitcom-1.3.0/sitcom/data/black.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/data/white.png` & `sitcom-1.3.0/sitcom/data/white.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/icon/cme.ico` & `sitcom-1.3.0/sitcom/icon/cme.ico`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/icon/cme.png` & `sitcom-1.3.0/sitcom/icon/cme.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/load/sitcom.gif` & `sitcom-1.3.0/sitcom/load/sitcom.gif`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/sfit.py` & `sitcom-1.3.0/sitcom/sfit.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/sirgraf.py` & `sitcom-1.3.0/sitcom/sirgraf.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.0.2/sitcom/st1.py` & `sitcom-1.3.0/sitcom/st1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import matplotlib.patches as pa
 import matplotlib.animation as animation
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 import numpy as np
 from astropy.visualization import ZScaleInterval
 from astropy.visualization import MinMaxInterval
-import cv2,os
+import cv2,os,site
 from scipy.interpolate import interp1d
 from scipy.optimize import curve_fit
 
 import sitcom.sirgraf as sf
 import sitcom.sfit as sn
 from sitcom.st2 import Ui_SWindow
 
@@ -191,25 +191,27 @@
         self.plot_button.setText(_translate("SecondWindow", "Plot"))
         self.plot_button.setEnabled(False)
         self.menuTheme.setTitle(_translate("SecondWindow", "Theme"))
         self.actionLight.setText(_translate("SecondWindow", "Light"))
         self.actionDark.setText(_translate("SecondWindow", "Dark"))
 
     def light(self,SecondWindow):
-        SecondWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/data/white.png); background-repeat:no-repeat; background-position: center;}")
+        cw=os.path.join(site.USER_SITE,'sitcom/data/white.png')
+        SecondWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}")
         self.figure.set_facecolor('white')
         mp.rcParams.update({'text.color' : "black",'axes.labelcolor' : "black",'axes.edgecolor':"black",'axes.facecolor':"white",'xtick.color':"black",'ytick.color':"black"})
         if self.t==[]:
           pass
         elif self.t[-1]=='Movie':
           self.pmovie.click()
         elif self.t[-1]=='HTP':
           self.htp.click()
     def dark(self,SecondWindow):
-        SecondWindow.setStyleSheet("QMainWindow{border-image: url(sitcom/data/black.png); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
+        cw=os.path.join(site.USER_SITE,'sitcom/data/black.png')
+        SecondWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
         self.figure.patch.set_facecolor('black')
         mp.rcParams.update({'text.color' : "white",'axes.labelcolor' : "white",'axes.edgecolor':"white",'axes.facecolor':"black",'xtick.color':"white",'ytick.color':"white"})
         if self.t==[]:
           pass
         elif self.t[-1]=='Movie':
           self.pmovie.click()
         elif self.t[-1]=='HTP':
```

### Comparing `sitcom-1.0.2/sitcom/st2.py` & `sitcom-1.3.0/sitcom/st2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
+import site,os
 
 class Ui_SWindow(object):
     def setupUi(self, SWindow):
         SWindow.setObjectName("SWindow")
         SWindow.setFixedWidth(596)
         SWindow.setFixedHeight(442)
         self.centralwidget = QtWidgets.QWidget(SWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.horizontalFrame = QtWidgets.QFrame(self.centralwidget)
         self.horizontalFrame.setGeometry(QtCore.QRect(10, 10, 571, 331))
-        self.horizontalFrame.setStyleSheet("QFrame{border-image: url(sitcom/data/Sine_curve.png); background-repeat:no-repeat; background-position: center;}")
+        cw=os.path.join(site.USER_SITE,'sitcom/data/Sine_curve.png')
+        self.horizontalFrame.setStyleSheet("QFrame{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}")
         self.horizontalFrame.setObjectName("horizontalFrame")
         self.diagram = QtWidgets.QHBoxLayout(self.horizontalFrame)
         self.diagram.setObjectName("diagram")
         
         self.p0SpinBox = QtWidgets.QDoubleSpinBox(self.centralwidget)
         self.p0SpinBox.setGeometry(QtCore.QRect(40, 370, 61, 41))
         self.p0SpinBox.setRange(-100000,100000)
```

