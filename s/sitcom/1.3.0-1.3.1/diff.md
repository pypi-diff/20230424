# Comparing `tmp/sitcom-1.3.0.tar.gz` & `tmp/sitcom-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitcom-1.3.0.tar", last modified: Tue Apr 25 01:33:16 2023, max compression
+gzip compressed data, was "sitcom-1.3.1.tar", last modified: Tue Apr 25 04:02:53 2023, max compression
```

## Comparing `sitcom-1.3.0.tar` & `sitcom-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.767969 sitcom-1.3.0/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.3.0/LICENSE
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-25 01:33:16.767969 sitcom-1.3.0/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1349 2023-04-06 17:47:58.000000 sitcom-1.3.0/README.md
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-25 01:33:16.767969 sitcom-1.3.0/setup.cfg
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      533 2023-04-25 01:32:58.000000 sitcom-1.3.0/setup.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/__init__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    47787 2023-04-25 01:30:08.000000 sitcom-1.3.0/sitcom/__main__.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/data/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    84116 2023-04-06 22:34:38.000000 sitcom-1.3.0/sitcom/data/Sine_curve.png
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/data/__init__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)   539595 2023-04-06 14:35:36.000000 sitcom-1.3.0/sitcom/data/black.png
--rw-rw-r--   0 purvi     (1000) purvi     (1000)   599404 2023-04-06 14:33:58.000000 sitcom-1.3.0/sitcom/data/white.png
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/icon/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/icon/__init__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     4022 2023-04-19 18:48:40.000000 sitcom-1.3.0/sitcom/icon/cme.ico
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    29744 2023-02-14 09:29:04.000000 sitcom-1.3.0/sitcom/icon/cme.png
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom/load/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.0/sitcom/load/__init__.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)  9159608 2023-02-26 07:43:28.000000 sitcom-1.3.0/sitcom/load/sitcom.gif
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.3.0/sitcom/sfit.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.3.0/sitcom/sirgraf.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)    37469 2023-04-24 18:02:33.000000 sitcom-1.3.0/sitcom/st1.py
--rw-rw-r--   0 purvi     (1000) purvi     (1000)     4635 2023-04-24 18:08:08.000000 sitcom-1.3.0/sitcom/st2.py
-drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 01:33:16.759968 sitcom-1.3.0/sitcom.egg-info/
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      280 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/PKG-INFO
--rw-rw-r--   0 purvi     (1000) purvi     (1000)      480 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/SOURCES.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/dependency_links.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/requires.txt
--rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-25 01:33:16.000000 sitcom-1.3.0/sitcom.egg-info/top_level.txt
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 04:02:53.191918 sitcom-1.3.1/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1069 2023-04-19 21:19:14.000000 sitcom-1.3.1/LICENSE
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     3253 2023-04-25 04:02:53.191918 sitcom-1.3.1/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     2695 2023-04-25 02:38:45.000000 sitcom-1.3.1/README.md
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       38 2023-04-25 04:02:53.191918 sitcom-1.3.1/setup.cfg
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1058 2023-04-25 04:02:39.000000 sitcom-1.3.1/setup.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 04:02:53.179918 sitcom-1.3.1/sitcom/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      124 2023-04-25 03:58:50.000000 sitcom-1.3.1/sitcom/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    49165 2023-04-25 03:51:27.000000 sitcom-1.3.1/sitcom/__main__.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 04:02:53.183918 sitcom-1.3.1/sitcom/data/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    84116 2023-04-06 22:34:38.000000 sitcom-1.3.1/sitcom/data/Sine_curve.png
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.1/sitcom/data/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)   539595 2023-04-06 14:35:36.000000 sitcom-1.3.1/sitcom/data/black.png
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)   599404 2023-04-06 14:33:58.000000 sitcom-1.3.1/sitcom/data/white.png
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 04:02:53.183918 sitcom-1.3.1/sitcom/icon/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.1/sitcom/icon/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4022 2023-04-19 18:48:40.000000 sitcom-1.3.1/sitcom/icon/cme.ico
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    29744 2023-02-14 09:29:04.000000 sitcom-1.3.1/sitcom/icon/cme.png
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 04:02:53.183918 sitcom-1.3.1/sitcom/load/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        0 2023-04-24 12:50:03.000000 sitcom-1.3.1/sitcom/load/__init__.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)  9159608 2023-02-26 07:43:28.000000 sitcom-1.3.1/sitcom/load/sitcom.gif
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     1611 2023-04-17 18:18:20.000000 sitcom-1.3.1/sitcom/sfit.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     6413 2023-04-19 22:32:54.000000 sitcom-1.3.1/sitcom/sirgraf.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)    37807 2023-04-25 03:54:06.000000 sitcom-1.3.1/sitcom/st1.py
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     4955 2023-04-25 03:54:44.000000 sitcom-1.3.1/sitcom/st2.py
+drwxrwxr-x   0 purvi     (1000) purvi     (1000)        0 2023-04-25 04:02:53.179918 sitcom-1.3.1/sitcom.egg-info/
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)     3253 2023-04-25 04:02:53.000000 sitcom-1.3.1/sitcom.egg-info/PKG-INFO
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)      480 2023-04-25 04:02:53.000000 sitcom-1.3.1/sitcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        1 2023-04-25 04:02:53.000000 sitcom-1.3.1/sitcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)       64 2023-04-25 04:02:53.000000 sitcom-1.3.1/sitcom.egg-info/requires.txt
+-rw-rw-r--   0 purvi     (1000) purvi     (1000)        7 2023-04-25 04:02:53.000000 sitcom-1.3.1/sitcom.egg-info/top_level.txt
```

### Comparing `sitcom-1.3.0/LICENSE` & `sitcom-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/__main__.py` & `sitcom-1.3.1/sitcom/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,26 @@
         MainWindow.setFixedHeight(550)
         icon = QtGui.QIcon()
         ci=os.path.join(site.USER_SITE,'sitcom/icon/cme.png')
         icon.addPixmap(QtGui.QPixmap(ci), QtGui.QIcon.Normal, QtGui.QIcon.On)
         MainWindow.setWindowIcon(icon)
         MainWindow.setIconSize(QtCore.QSize(40, 30))
         cf=os.path.join(site.USER_SITE,'sitcom/font/lato/Lato-Semibold.ttf')
-        _id=QtGui.QFontDatabase.addApplicationFont(cf)
-        custom_font = QtGui.QFontDatabase.applicationFontFamilies(_id)[0] 
-        font = QtGui.QFont(custom_font, 11)
-        font.setWeight(30)
+        QtGui.QFontDatabase.addApplicationFont(cf)
+        font = QtGui.QFont('Lato-SemiBold', 10)
+        font.setWeight(50)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
+        if 'conda' in sys.version or 'Continuum' in sys.version:
+        	# conda environment detected
+        	site_packages_path = site.getusersitepackages(prefix=sys.prefix)
+        else:
+        	# not a conda environment, use standard site-packages path
+        	site_packages_path = site.USER_SITE
+        self.sitep=site_packages_path
         #########################################################
         self.Browse = QtWidgets.QPushButton(self.centralwidget)
         self.Browse.setGeometry(QtCore.QRect(330, 10, 89, 31))
         self.Browse.setObjectName("Browse")
         self.Browse_le = QtWidgets.QLineEdit(self.centralwidget)
         self.Browse_le.setGeometry(QtCore.QRect(10, 10, 301, 31))
         self.Browse_le.setObjectName("Browse_le")
@@ -305,14 +311,15 @@
         self.actionLight.triggered.connect(self.light)
         self.actionLight.trigger()
         self.actionDark.triggered.connect(self.dark)
         self.actionPNG.triggered.connect(self.pminimum)
         self.actionFITS.triggered.connect(self.fminimum)
         self.actionPNG_2.triggered.connect(self.puniform)
         self.actionFITS_2.triggered.connect(self.funiform)
+        self.actionAverage_Intensity_Plot.triggered.connect(self.faverage)
         self.menuFile.setEnabled(False)
 
         self.retranslateUi(MainWindow)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
         MainWindow.setTabOrder(self.Browse_le, self.Browse)
         MainWindow.setTabOrder(self.Browse, self.Start)
         MainWindow.setTabOrder(self.Start, self.Uniform)
@@ -435,33 +442,49 @@
         msg.setWindowTitle("Saved!")
         msg.setStandardButtons(QtWidgets.QMessageBox.Ok)
         retval = msg.exec_()
     def fminimum(self):
         fpath=os.path.expanduser('~')
         f1=fits.PrimaryHDU(self.min_image)
         cnm=os.path.join(fpath,self.date)
-        f1.writeto(cnm+'_min.fits')
+        f1.writeto(cnm+'_min.fits',overwrite=True)
         msg = QtWidgets.QMessageBox()
         msg.setStyleSheet("color:'black';")
         msg.setIcon(QtWidgets.QMessageBox.Information)
         msg.setText("The image has been saved to "+cnm+'_min.fits')
         msg.setWindowTitle("Saved!")
         msg.setStandardButtons(QtWidgets.QMessageBox.Ok)
+        retval=msg.exec_()
+    def faverage(self):
+        fpath=os.path.expanduser('~')
+        g=np.log10(self.avg)
+        r=np.round(np.mean(g[np.where((np.isnan(g)==False) & (g!=np.inf))]))
+        f1=fits.PrimaryHDU([self.y[np.where(self.y>=0)],self.avg/10**r])
+        cnm=os.path.join(fpath,self.date)
+        f1.writeto(cnm+'_avg.fits',overwrite=True)
+        msg = QtWidgets.QMessageBox()
+        msg.setStyleSheet("color:'black';")
+        msg.setIcon(QtWidgets.QMessageBox.Information)
+        msg.setText("The image has been saved to "+cnm+'_avg.fits')
+        msg.setWindowTitle("Saved!")
+        msg.setStandardButtons(QtWidgets.QMessageBox.Ok)
+        retval=msg.exec_()
 
     def funiform(self):
         fpath=os.path.expanduser('~')
         f1=fits.PrimaryHDU(self.uniform_image)
         cnm=os.path.join(fpath,self.date)
-        f1.writeto(cnm+'_uniform.fits')
+        f1.writeto(cnm+'_uniform.fits',overwrite=True)
         msg = QtWidgets.QMessageBox()
         msg.setStyleSheet("color:'black';")
         msg.setIcon(QtWidgets.QMessageBox.Information)
         msg.setText("The image has been saved to "+cnm+'_uniform.fits')
         msg.setWindowTitle("Saved!")
         msg.setStandardButtons(QtWidgets.QMessageBox.Ok)
+        retval=msg.exec_()
     def puniform(self):
         fpath=os.path.expanduser('~')
         cnm=os.path.join(fpath,self.date)
         plt.imsave(cnm+'_uniform.png',self.uniform_image,cmap=self.colorm,format='png')
         msg = QtWidgets.QMessageBox()
         msg.setStyleSheet("color:'black';")
         msg.setIcon(QtWidgets.QMessageBox.Information)
@@ -551,15 +574,15 @@
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()
     def light(self):
         self.t.append('Light')
         #MainWindow=QtWidgets.QMainWindow()
-        cw=os.path.join(site.USER_SITE,'sitcom/data/white.png')
+        cw=os.path.join(self.sitep,'sitcom/data/white.png')
         MainWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}")
         self.figure.set_facecolor('white')
         mp.rcParams.update({'text.color' : "black",'axes.labelcolor' : "black",'axes.edgecolor':"black",'axes.facecolor':"white",'xtick.color':"black",'ytick.color':"black"})
         #self.setupUi(MainWindow)
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
@@ -572,15 +595,15 @@
           self.Final.click()
         elif self.s[-1]=="Average":
           self.Average.click()
         elif self.s[-1]=="Movie":
           self.Movie.click()   
     def dark(self):
         self.t.append('Dark')
-        cw=os.path.join(site.USER_SITE,'sitcom/data/black.png')
+        cw=os.path.join(self.sitep,'sitcom/data/black.png')
         MainWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
         self.figure.patch.set_facecolor('black')
         mp.rcParams.update({'text.color' : "white",'axes.labelcolor' : "white",'axes.labelcolor' : "white",'axes.edgecolor':"white",'axes.facecolor':"black",'xtick.color':"white",'ytick.color':"white"})
         if self.s==[]:
           pass
         elif self.s[-1]=="Minimum":
           self.Minimum.click()
@@ -920,15 +943,21 @@
       self.ani.event_source.start()
 
 
  
 
 if __name__ == "__main__":
     app = QtWidgets.QApplication(sys.argv)
-    cl=os.path.join(site.USER_SITE,'sitcom/load/sitcom.gif')
+    if 'conda' in sys.version or 'Continuum' in sys.version:
+        	# conda environment detected
+        	site_packages_path = site.getusersitepackages(prefix=sys.prefix)
+    else:
+        	# not a conda environment, use standard site-packages path
+        	site_packages_path = site.USER_SITE
+    cl=os.path.join(site_packages_path,'sitcom/load/sitcom.gif')
     movie=QtGui.QMovie(cl)
     splash = Load_Window(movie)
     splash.show()
     splash.movie.start()
     start = time.time()
     while movie.state() == QtGui.QMovie.Running and time.time() < start + 4:
         app.processEvents()
```

### Comparing `sitcom-1.3.0/sitcom/data/Sine_curve.png` & `sitcom-1.3.1/sitcom/data/Sine_curve.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/data/black.png` & `sitcom-1.3.1/sitcom/data/black.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/data/white.png` & `sitcom-1.3.1/sitcom/data/white.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/icon/cme.ico` & `sitcom-1.3.1/sitcom/icon/cme.ico`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/icon/cme.png` & `sitcom-1.3.1/sitcom/icon/cme.png`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/load/sitcom.gif` & `sitcom-1.3.1/sitcom/load/sitcom.gif`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/sfit.py` & `sitcom-1.3.1/sitcom/sfit.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/sirgraf.py` & `sitcom-1.3.1/sitcom/sirgraf.py`

 * *Files identical despite different names*

### Comparing `sitcom-1.3.0/sitcom/st1.py` & `sitcom-1.3.1/sitcom/st1.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,21 @@
         SecondWindow.setFixedWidth(803)
         SecondWindow.setFixedHeight(550)
         self.centralwidget = QtWidgets.QWidget(SecondWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayoutWidget = QtWidgets.QWidget(self.centralwidget)
         self.verticalLayoutWidget.setGeometry(QtCore.QRect(0, 0, 541, 501))
         self.verticalLayoutWidget.setObjectName("verticalLayoutWidget")
+        if 'conda' in sys.version or 'Continuum' in sys.version:
+          # conda environment detected
+          site_packages_path = site.getusersitepackages(prefix=sys.prefix)
+        else:
+          # not a conda environment, use standard site-packages path
+          site_packages_path = site.USER_SITE
+        self.sitep=site_packages_path
         self.plot = QtWidgets.QVBoxLayout(self.verticalLayoutWidget)
         self.plot.setContentsMargins(0, 0, 0, 0)
         self.plot.setObjectName("plot")
         self.figure = plt.figure()
         self.canvas = FigureCanvas(self.figure)
         self.toolbar = NavigationToolbar(self.canvas,SecondWindow)
         self.toolbar.setStyleSheet("QWidget {background-color:grey;}")
@@ -191,26 +198,26 @@
         self.plot_button.setText(_translate("SecondWindow", "Plot"))
         self.plot_button.setEnabled(False)
         self.menuTheme.setTitle(_translate("SecondWindow", "Theme"))
         self.actionLight.setText(_translate("SecondWindow", "Light"))
         self.actionDark.setText(_translate("SecondWindow", "Dark"))
 
     def light(self,SecondWindow):
-        cw=os.path.join(site.USER_SITE,'sitcom/data/white.png')
+        cw=os.path.join(self.sitep,'sitcom/data/white.png')
         SecondWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}")
         self.figure.set_facecolor('white')
         mp.rcParams.update({'text.color' : "black",'axes.labelcolor' : "black",'axes.edgecolor':"black",'axes.facecolor':"white",'xtick.color':"black",'ytick.color':"black"})
         if self.t==[]:
           pass
         elif self.t[-1]=='Movie':
           self.pmovie.click()
         elif self.t[-1]=='HTP':
           self.htp.click()
     def dark(self,SecondWindow):
-        cw=os.path.join(site.USER_SITE,'sitcom/data/black.png')
+        cw=os.path.join(self.sitep,'sitcom/data/black.png')
         SecondWindow.setStyleSheet("QMainWindow{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}QLabel{color:white;}")
         self.figure.patch.set_facecolor('black')
         mp.rcParams.update({'text.color' : "white",'axes.labelcolor' : "white",'axes.edgecolor':"white",'axes.facecolor':"black",'xtick.color':"white",'ytick.color':"white"})
         if self.t==[]:
           pass
         elif self.t[-1]=='Movie':
           self.pmovie.click()
```

### Comparing `sitcom-1.3.0/sitcom/st2.py` & `sitcom-1.3.1/sitcom/st2.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 class Ui_SWindow(object):
     def setupUi(self, SWindow):
         SWindow.setObjectName("SWindow")
         SWindow.setFixedWidth(596)
         SWindow.setFixedHeight(442)
         self.centralwidget = QtWidgets.QWidget(SWindow)
         self.centralwidget.setObjectName("centralwidget")
+        if 'conda' in sys.version or 'Continuum' in sys.version:
+            # conda environment detected
+            site_packages_path = site.getusersitepackages(prefix=sys.prefix)
+        else:
+            # not a conda environment, use standard site-packages path
+            site_packages_path = site.USER_SITE
         self.horizontalFrame = QtWidgets.QFrame(self.centralwidget)
         self.horizontalFrame.setGeometry(QtCore.QRect(10, 10, 571, 331))
-        cw=os.path.join(site.USER_SITE,'sitcom/data/Sine_curve.png')
+        cw=os.path.join(site_packages_path,'sitcom/data/Sine_curve.png')
         self.horizontalFrame.setStyleSheet("QFrame{border-image: url("+cw+"); background-repeat:no-repeat; background-position: center;}")
         self.horizontalFrame.setObjectName("horizontalFrame")
         self.diagram = QtWidgets.QHBoxLayout(self.horizontalFrame)
         self.diagram.setObjectName("diagram")
         
         self.p0SpinBox = QtWidgets.QDoubleSpinBox(self.centralwidget)
         self.p0SpinBox.setGeometry(QtCore.QRect(40, 370, 61, 41))
```

