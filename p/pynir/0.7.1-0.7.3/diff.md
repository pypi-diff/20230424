# Comparing `tmp/pynir-0.7.1.tar.gz` & `tmp/pynir-0.7.3.tar.gz`

## Comparing `pynir-0.7.1.tar` & `pynir-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,67 @@
--rw-r--r--   0        0        0    19542 2020-02-02 00:00:00.000000 pynir-0.7.1/src/pynir/Calibration.py
--rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 pynir-0.7.1/src/pynir/CalibrationTransfer.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.7.1/src/pynir/FeatureSelection.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pynir-0.7.1/src/pynir/OutlierDection.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.7.1/src/pynir/Preprocessing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.7.1/src/pynir/__init__.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 pynir-0.7.1/src/pynir/utils.py
--rw-r--r--   0        0        0  1215471 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Data_Corn.mat
--rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Data_Tablet.mat
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo10_calibrationTransfer_PFCE_simulateNIR.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo11_calibrationTransfer_PFCE_Tablet.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo12_calibrationTransfer_PFCE_Corn.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo1_SimulateNIR.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo2_Regression.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo3_Binary_Classification.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo4_Multiclass_Classification.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo5_dataPreprocessing.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo6_outierDection.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo7_FeatureSelection_oneStep.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo8_FeatureSelection_multiSteps.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pynir-0.7.1/tests/Demo9_calibrationTransfer.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 pynir-0.7.1/README.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pynir-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 pynir-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynir-0.7.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/Makefile
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/conf.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/make.bat
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/modules.rst
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/pynir.rst
+-rw-r--r--   0        0        0   530403 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/doctrees/modules.doctree
+-rw-r--r--   0        0        0   279145 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/doctrees/pynir.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    21444 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/index.html
+-rw-r--r--   0        0        0    26832 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/modules.html
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0   118287 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/pynir.html
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/search.html
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_modules/index.html
+-rw-r--r--   0        0        0   102728 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_modules/pynir/Calibration.html
+-rw-r--r--   0        0        0    73899 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_modules/pynir/CalibrationTransfer.html
+-rw-r--r--   0        0        0    53422 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_modules/pynir/FeatureSelection.html
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_modules/pynir/OutlierDection.html
+-rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_modules/pynir/Preprocessing.html
+-rw-r--r--   0        0        0    25985 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_modules/pynir/utils.html
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_sources/pynir.rst.txt
+-rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pynir-0.7.3/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0  1215471 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Data_Corn.mat
+-rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Data_Tablet.mat
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo11_calibrationTransfer_PFCE_Tablet.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo12_calibrationTransfer_PFCE_Corn.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo1_SimulateNIR.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo2_Regression.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo3_Binary_Classification.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo4_Multiclass_Classification.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo5_dataPreprocessing.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo6_outierDection.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo7_FeatureSelection_oneStep.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo8_FeatureSelection_multiSteps.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pynir-0.7.3/examples/Demo9_calibrationTransfer.py
+-rw-r--r--   0        0        0    19671 2020-02-02 00:00:00.000000 pynir-0.7.3/src/pynir/Calibration.py
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 pynir-0.7.3/src/pynir/CalibrationTransfer.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.7.3/src/pynir/FeatureSelection.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pynir-0.7.3/src/pynir/OutlierDection.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.7.3/src/pynir/Preprocessing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.7.3/src/pynir/__init__.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 pynir-0.7.3/src/pynir/utils.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.7.3/LICENSE.txt
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 pynir-0.7.3/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pynir-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 pynir-0.7.3/PKG-INFO
```

### Comparing `pynir-0.7.1/src/pynir/Calibration.py` & `pynir-0.7.3/src/pynir/Calibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from sklearn.model_selection import GridSearchCV, cross_val_predict
 
 import matplotlib.pyplot as plt
 
 
 class pls:
-    def __init__(self, n_components = 2):
+    def __init__(self, n_components=2):
         """
         Initialize the number of components in PLS model.
         """
 
         self.n_components = n_components
 
     def fit(self, X, y):
@@ -40,108 +40,111 @@
         y (np.array): dependent variable of the training data
 
         Returns:
         self: the PLS model
         """
         self.X = X
         self.y = y
-        meanX = np.mean(X,axis = 0)
+        meanX = np.mean(X, axis=0)
         meany = np.mean(y)
         Xcentered = X - meanX
         ycentered = y - meany
         model = simpls(Xcentered, ycentered, self.n_components)
         meanX_hat = -1 * np.dot(meanX, model['B']) + meany
-        model['B'] = np.append(meanX_hat[np.newaxis,:], model['B'],axis=0)
+        model['B'] = np.append(meanX_hat[np.newaxis, :], model['B'], axis=0)
         self.model = model
         return self
 
-    def predict(self, Xnew, n_components = None):
+    def predict(self, Xnew, n_components=None):
         """
         Predict the dependent variable based on independent variable(s).
 
         Parameters:
         Xnew (np.array): independent variable(s) of the new data to predict
         n_components (int): number of components used to predict
                             (default is None, which uses the optimal number of
                              components obtained by cross validation)
 
         Returns:
         ynew_hat (np.array): predicted dependent variable based on Xnew
         """
 
         if n_components is None:
-            B = self.model['B'][:,-1]
+            B = self.model['B'][:, -1]
         else:
             B = self.model['B'][:, n_components-1]
         if Xnew.shape[1] != B.shape[0]-1:
-            raise ValueError('The feature number of predictor is isconsistent with that of indepnentent.')
-        Xnew = np.append(np.ones([Xnew.shape[0],1]), Xnew, axis=1)
-        ynew_hat = np.dot(Xnew,B)
+            raise ValueError(
+                'The feature number of predictor is isconsistent with that of indepnentent.')
+        Xnew = np.append(np.ones([Xnew.shape[0], 1]), Xnew, axis=1)
+        ynew_hat = np.dot(Xnew, B)
         return ynew_hat
 
-    def crossValidation_predict(self, nfold = 10):
+    def crossValidation_predict(self, nfold=10):
         """
         Predict dependent variable using cross validation method.
 
         Parameters:
         nfold (int): number of folds for cross validation (default is 10)
 
         Returns:
         yhat (np.array): predicted dependent variable based on cross validation method
         """
         X = self.X
         y = self.y
-        yhat = np.zeros((y.shape[0],self.n_components))
-        model = pls(n_components = self.n_components)
+        yhat = np.zeros((y.shape[0], self.n_components))
+        model = pls(n_components=self.n_components)
         for train, test in KFold(n_splits=nfold).split(X):
-            model.fit(X[train,:], y[train])
-            yhat[test,:] = model.predict(X[test,:],np.arange(self.n_components)+1)
+            model.fit(X[train, :], y[train])
+            yhat[test, :] = model.predict(
+                X[test, :], np.arange(self.n_components)+1)
         return yhat
 
-    def get_optLV(self, nfold = 10):
+    def get_optLV(self, nfold=10):
         yhat_cv = self.crossValidation_predict(nfold)
         rmsecv = []
         r2cv = []
         for i in range(yhat_cv.shape[1]):
-            reportcv = regresssionReport(self.y, yhat_cv[:,i])
+            reportcv = regresssionReport(self.y, yhat_cv[:, i])
             rmsecv.append(reportcv["rmse"])
             r2cv.append(reportcv["r2"])
         optLV = int(np.argmin(rmsecv)+1)
         self.optLV = optLV
         return optLV
 
     def transform(self, Xnew):
-        meanX = np.mean(self.X, axis = 0)
+        meanX = np.mean(self.X, axis=0)
         Xnew_c = Xnew - meanX
-        Tnew = np.dot(Xnew_c,self.model['x_weights'])
+        Tnew = np.dot(Xnew_c, self.model['x_weights'])
         return Tnew
 
     def get_vip(self):
         # ref. https://www.sciencedirect.com/topics/engineering/variable-importance-in-projection
-        x_scores, x_loadings,y_loadings,x_weights = \
-            self.model['x_scores'],self.model['x_loadings'],\
-            self.model['y_loadings'],self.model['x_weights']
+        x_scores, x_loadings, y_loadings, x_weights = \
+            self.model['x_scores'], self.model['x_loadings'],\
+            self.model['y_loadings'], self.model['x_weights']
 
         n_samples, n_components = x_scores.shape
         W0 = x_weights / np.sqrt(np.sum(x_weights**2, axis=0))
         p = x_loadings.shape[0]
         sumSq = np.sum(x_scores**2, axis=0) * np.sum(y_loadings**2, axis=1)
         vipScore = np.sqrt(p * np.sum(sumSq * (W0**2), axis=1) / np.sum(sumSq))
         return vipScore
 
-    def plot_prediction(self, y, yhat, xlabel = "Reference", ylabel = "Prediction", title = "", ax = None):
-        report = regresssionReport(y,yhat)
+    def plot_prediction(self, y, yhat, xlabel="Reference", ylabel="Prediction", title="", ax=None):
+        report = regresssionReport(y, yhat)
         if ax == None:
             fig, ax = plt.subplots()
-        ax.plot([np.min(y)*0.95,np.max(y)*1.05],[np.min(y)*0.95,np.max(y)*1.05],
-                color = 'black',label = "y=x")
-        ax.scatter(y, yhat,color = 'tab:green', marker='*', label ='Prediction')
+        ax.plot([np.min(y)*0.95, np.max(y)*1.05], [np.min(y)*0.95, np.max(y)*1.05],
+                color='black', label="y=x")
+        ax.scatter(y, yhat, color='tab:green', marker='*', label='Prediction')
         ax.text(0.7, 0.03,
-                "RMSEP = {:.4f}\nR$^2$ = {:.2}".format(report["rmse"],report["r2"]),
-                transform = ax.transAxes)
+                "RMSEP = {:.4f}\nR$^2$ = {:.2}".format(
+                    report["rmse"], report["r2"]),
+                transform=ax.transAxes)
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
         ax.legend(loc='upper left', bbox_to_anchor=(0.0, 1.0))
         ax.set_title(title)
 
 
 class plsda(PLSRegression):
@@ -161,34 +164,34 @@
 
     def predict_log_proba(self, X):
         return self.lda.predict_log_proba(self.predict(X))
 
     def predict_proba(self, X):
         return self.lda.predict_proba(self.predict(X))
 
-    def crossValidation_predict(self, nfold = 10):
+    def crossValidation_predict(self, nfold=10):
         X = self.X
         y = self.y
-        yhat = np.zeros((y.shape[0],self.n_components))
+        yhat = np.zeros((y.shape[0], self.n_components))
         for i in range(self.n_components):
-            model = plsda(n_components = i+1)
+            model = plsda(n_components=i+1)
             for train, test in KFold(n_splits=nfold).split(X):
-                model.fit(X[train,:], y[train])
-                yhat[test,i] = model.predict(X[test,:])
+                model.fit(X[train, :], y[train])
+                yhat[test, i] = model.predict(X[test, :])
         return yhat
 
-    def get_optLV(self, nfold = 10):
+    def get_optLV(self, nfold=10):
         yhat_cv = self.crossValidation_predict(nfold)
         accuracy_cv = []
         for i in range(yhat_cv.shape[1]):
-            if len(self.lda.classes_) == 2 :
-                report_cv = binaryClassificationReport(self.y, yhat_cv[:,i])
+            if len(self.lda.classes_) == 2:
+                report_cv = binaryClassificationReport(self.y, yhat_cv[:, i])
                 accuracy_cv.append(report_cv["accuracy"])
             elif len(self.lda.classes_) > 2:
-                report_cv = multiClassificationReport(self.y, yhat_cv[:,i])
+                report_cv = multiClassificationReport(self.y, yhat_cv[:, i])
                 accuracy_tmp = [rep["accuracy"] for rep in report_cv.values()]
                 accuracy_cv.append(sum(accuracy_tmp))
 
         optLV = int(np.argmax(accuracy_cv)+1)
         self.optLV = optLV
         return optLV
 
@@ -205,72 +208,76 @@
 
         W0 = Xw / np.sqrt(np.sum(Xw**2, axis=0))
         p = XL.shape[0]
         sumSq = np.sum(Xw**2, axis=0) * np.sum(yl**2, axis=0)
         vipScore = np.sqrt(p * np.sum(sumSq * (W0**2), axis=1) / np.sum(sumSq))
         return vipScore
 
-    def permutation_test(self, X, y, n_repeats=100,n_jobs = None):
+    def permutation_test(self, X, y, n_repeats=100, n_jobs=None):
         # Initialize arrays to store Q2 and R2 values
         q2 = np.zeros(n_repeats)
         r2 = np.zeros(n_repeats)
         permutation_ratio = np.zeros(n_repeats)
         # Perform the permutation test
         for i in range(n_repeats):
             # Shuffle the target variable
             y_shuffled = np.random.permutation(y)
 
             # Fit the model to the shuffled target variable
             self.fit(X, y_shuffled)
 
             # Calculate the cross-validated Q2 and R2 values
-            y_pred = cross_val_predict(self, X, y_shuffled, cv=10, n_jobs = n_jobs)
+            y_pred = cross_val_predict(
+                self, X, y_shuffled, cv=10, n_jobs=n_jobs)
             q2[i] = self.score(X, y_shuffled)
             r2[i] = r2_score(y_shuffled, y_pred)
             permutation_ratio[i] = np.sum(y_shuffled != y) / len(y)
         return q2, r2, permutation_ratio
 
-class lsvc(LinearSVC):# linear svc
-    def get_optParams(self, X, y, Params = None, nfold = 10, n_jobs = None):
+
+class lsvc(LinearSVC):  # linear svc
+    def get_optParams(self, X, y, Params=None, nfold=10, n_jobs=None):
         if Params is None:
             Params = {'C': np.logspace(-4, 5, 10),
                       'penalty': ('l1', 'l2')}
         self.gsh = GridSearchCV(estimator=self,  param_grid=Params,
-                           cv = nfold, n_jobs = n_jobs)
+                                cv=nfold, n_jobs=n_jobs)
         self.gsh.fit(X, y)
         return self.gsh.best_params_
 
     def get_confusion_matrix(self, X, y):
         yhat = self.predict(X)
         cm = confusion_matrix(y, yhat)
         return cm
 
-class svc(SVC):# linear svc
-    def get_optParams(self, X, y, Params = None, nfold = 10, n_jobs = None):
+
+class svc(SVC):  # linear svc
+    def get_optParams(self, X, y, Params=None, nfold=10, n_jobs=None):
         if Params is None:
             Params = {'C': np.logspace(-4, 5, 10),
-                      'gamma':np.logspace(-4, 5, 10),
+                      'gamma': np.logspace(-4, 5, 10),
                       'kernel': ('poly', 'rbf', 'sigmoid')}
         self.gsh = GridSearchCV(estimator=self,  param_grid=Params,
-                           cv = nfold, n_jobs = n_jobs)
+                                cv=nfold, n_jobs=n_jobs)
         self.gsh.fit(X, y)
         return self.gsh.best_params_
 
     def get_confusion_matrix(self, X, y):
         yhat = self.predict(X)
         cm = confusion_matrix(y, yhat)
         return cm
 
+
 class rf(RandomForestClassifier):
-    def get_optParams(self, X, y, Params = None, nfold = 10, n_jobs = None):
+    def get_optParams(self, X, y, Params=None, nfold=10, n_jobs=None):
         if Params is None:
             Params = {'n_estimators': np.arange(100)+1,
                       'max_depth': np.arange(3)+1}
         self.gsh = GridSearchCV(estimator=self,  param_grid=Params,
-                           cv = nfold, n_jobs = n_jobs)
+                                cv=nfold, n_jobs=n_jobs)
         self.gsh.fit(X, y)
         return self.gsh.best_params_
 
     def get_confusion_matrix(self, X, y):
         yhat = self.predict(X)
         cm = confusion_matrix(y, yhat)
         return cm
@@ -281,24 +288,25 @@
         pass
 
     def fit(self, x):
         self.classes = np.unique(x)
         return self
 
     def transform(self, x):
-        Xnew = np.zeros((len(x),len(self.classes)), dtype=int)
-        if len(self.classes) > 2 :
+        Xnew = np.zeros((len(x), len(self.classes)), dtype=int)
+        if len(self.classes) > 2:
             for i, classi in enumerate(self.classes):
-                Xnew[:,i] = x==classi
+                Xnew[:, i] = x == classi
         return Xnew
 
     def reTransform(self, xnew):
-        x = [np.classes(np.where(xnew[i,:])) for i in range(xnew.shape[0])]
+        x = [np.classes(np.where(xnew[i, :])) for i in range(xnew.shape[0])]
         return x
 
+
 def plot_confusion_matrix(cm,
                           target_names,
                           title='Confusion matrix',
                           cmap=None,
                           normalize=True):
     """
     given a sklearn confusion matrix (cm), make a nice plot
@@ -348,72 +356,77 @@
         tick_marks = np.arange(len(target_names))
         plt.xticks(tick_marks, target_names, rotation=45)
         plt.yticks(tick_marks, target_names)
 
     if normalize:
         cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
 
-
     thresh = cm.max() / 1.5 if normalize else cm.max() / 2
     for i in range(cm.shape[0]):
         for j in range(cm.shape[1]):
             if normalize:
                 plt.text(j, i, "{:0.4f}".format(cm[i, j]),
                          horizontalalignment="center",
                          color="white" if cm[i, j] > thresh else "black")
             else:
                 plt.text(j, i, "{:,}".format(cm[i, j]),
                          horizontalalignment="center",
                          color="white" if cm[i, j] > thresh else "black")
 
-
     plt.tight_layout()
     plt.ylabel('True label')
-    plt.xlabel('Predicted label\naccuracy={:0.4f}; misclass={:0.4f}'.format(accuracy, misclass))
+    plt.xlabel('Predicted label\naccuracy={:0.4f}; misclass={:0.4f}'.format(
+        accuracy, misclass))
     plt.show()
 
-def multiClassificationReport(ytrue,ypred):
+
+def multiClassificationReport(ytrue, ypred):
     labels = np.unique(ytrue)
     report = dict()
     for labeli in labels:
-        report[labeli] = binaryClassificationReport(ytrue = ytrue == labeli, ypred = ypred == labeli)
+        report[labeli] = binaryClassificationReport(
+            ytrue=ytrue == labeli, ypred=ypred == labeli)
     return report
 
-def binaryClassificationReport(ytrue,ypred):
-    if len(np.unique(ytrue))>2:
-        raise("Use the multiClassificationReport function for multiple classification.")
+
+def binaryClassificationReport(ytrue, ypred):
+    if len(np.unique(ytrue)) > 2:
+        raise ("Use the multiClassificationReport function for multiple classification.")
     else:
-        tn, fp, fn, tp = confusion_matrix(ytrue,ypred).ravel()
+        tn, fp, fn, tp = confusion_matrix(ytrue, ypred).ravel()
         report = dict()
         report["accuracy"] = accuracy_score(ytrue, ypred)
-        report["sensitivity"] = recall_score(ytrue, ypred)#recall
+        report["sensitivity"] = recall_score(ytrue, ypred)  # recall
         report["specificity"] = tn/(tn+fp)
         report["f1"] = f1_score(ytrue, ypred)
         return report
 
-def regresssionReport(ytrue,ypred):
+
+def regresssionReport(ytrue, ypred):
     report = dict()
     report["rmse"] = mean_squared_error(ytrue, ypred, squared=False)
-    report["r2"] =  r2_score(ytrue, ypred)
+    report["r2"] = r2_score(ytrue, ypred)
     return report
 
+
 def simpls(X, y, n_components):
     '''
     Partial Least Squares, SIMPLS
     Ref https://github.com/freesiemens/SpectralMultivariateCalibration/blob/master/pypls.py
     :param X: independent variables, numpy array of shape (n_samples, n_variables)
     :param y: dependent variable, numpy array of shape (n_samples,) or (n_samples, 1)
     :param n_components: number of latent variables to decompose the data into
     :return: dictionary containing the results of the SIMPLS algorithm
     '''
     n_samples, n_variables = X.shape
     if np.ndim(y) == 1:
         y = y[:, np.newaxis]
     if n_samples != y.shape[0]:
-        raise ValueError('The number of independent and dependent variable are inconsistent')
+        raise ValueError(
+            'The number of independent and dependent variable are inconsistent')
 
     n_components = np.min((n_components, n_samples, n_variables))
     V = np.zeros((n_variables, n_components))
     x_scores = np.zeros((n_samples, n_components))  # X scores (standardized)
     x_weights = np.zeros((n_variables, n_components))  # X weights
     x_loadings = np.zeros((n_variables, n_components))  # X loadings
     y_loadings = np.zeros((1, n_components))  # Y loadings
@@ -437,26 +450,26 @@
         x_weights[:, i] = r
         x_scores[:, i] = t
         x_loadings[:, i] = p
         y_loadings[:, i] = q
         y_scores[:, i] = u
         V[:, i] = v
     B = np.cumsum(np.dot(x_weights, np.diag(y_loadings.ravel())), axis=1)
-    return {'B': B, 'x_scores': x_scores, 'x_loadings': x_loadings, 'y_loadings': y_loadings, \
-            'x_scores_weights': x_weights, 'x_weights': x_weights, 'y_scores':y_scores}
-
+    return {'B': B, 'x_scores': x_scores, 'x_loadings': x_loadings, 'y_loadings': y_loadings,
+            'x_scores_weights': x_weights, 'x_weights': x_weights, 'y_scores': y_scores}
 
 
-def sampleSplit_random(X,test_size=0.25, random_state=1, shuffle=False):
+def sampleSplit_random(X, test_size=0.25, random_state=1, shuffle=False):
     sampleIdx = np.arange(X.shape[0])
-    trainIdx, testIdx = train_test_split(sampleIdx,test_size=test_size,
+    trainIdx, testIdx = train_test_split(sampleIdx, test_size=test_size,
                                          random_state=random_state,
                                          shuffle=shuffle)
     return trainIdx, testIdx
 
+
 def sampleSplit_KS(X, test_size=0.25, metric='euclidean', *args, **kwargs):
     """Kennard Stone Sample Split method
     Parameters
     ----------
     spectra: ndarray, shape of i x j
         i spectrums and j variables (wavelength/wavenumber/ramam shift and so on)
     test_size : float, int
@@ -494,15 +507,16 @@
         # find the maximum minimum distance
         select_distance = distance[select_pts, :]
         min_distance = select_distance[:, remaining_pts]
         min_distance = np.min(min_distance, axis=0)
         max_min_distance = np.max(min_distance)
 
         # select the first point (in case that several distances are the same, choose the first one)
-        points = np.argwhere(select_distance == max_min_distance)[:, 1].tolist()
+        points = np.argwhere(select_distance == max_min_distance)[
+            :, 1].tolist()
         for point in points:
             if point in select_pts:
                 pass
             else:
                 select_pts.append(point)
                 remaining_pts.remove(point)
                 break
```

### Comparing `pynir-0.7.1/src/pynir/CalibrationTransfer.py` & `pynir-0.7.3/src/pynir/CalibrationTransfer.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/src/pynir/FeatureSelection.py` & `pynir-0.7.3/src/pynir/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/src/pynir/OutlierDection.py` & `pynir-0.7.3/src/pynir/OutlierDection.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/src/pynir/Preprocessing.py` & `pynir-0.7.3/src/pynir/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/src/pynir/utils.py` & `pynir-0.7.3/src/pynir/utils.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Data_Corn.mat` & `pynir-0.7.3/examples/Data_Corn.mat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Data_Tablet.mat` & `pynir-0.7.3/examples/Data_Tablet.mat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo10_calibrationTransfer_PFCE_simulateNIR.py` & `pynir-0.7.3/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo11_calibrationTransfer_PFCE_Tablet.py` & `pynir-0.7.3/examples/Demo11_calibrationTransfer_PFCE_Tablet.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo12_calibrationTransfer_PFCE_Corn.py` & `pynir-0.7.3/examples/Demo12_calibrationTransfer_PFCE_Corn.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo2_Regression.py` & `pynir-0.7.3/examples/Demo2_Regression.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo3_Binary_Classification.py` & `pynir-0.7.3/examples/Demo3_Binary_Classification.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo4_Multiclass_Classification.py` & `pynir-0.7.3/examples/Demo4_Multiclass_Classification.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo5_dataPreprocessing.py` & `pynir-0.7.3/examples/Demo5_dataPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo7_FeatureSelection_oneStep.py` & `pynir-0.7.3/examples/Demo7_FeatureSelection_oneStep.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo8_FeatureSelection_multiSteps.py` & `pynir-0.7.3/examples/Demo8_FeatureSelection_multiSteps.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/tests/Demo9_calibrationTransfer.py` & `pynir-0.7.3/examples/Demo9_calibrationTransfer.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/LICENSE.txt` & `pynir-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynir-0.7.1/README.md` & `pynir-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # Commom Calibration methods for multivariate calibration
 
 This is a Python library for dealing with multivariate calibration, e.g., Near infrared spectra regression and classification tasks.
 
 ## Installation
 
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [pynir](https://pypi.org/project/pynir/)
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [pynir](https://pypi.org/project/pynir/). 
 
 ```bash
 pip install pynir
 ```
+
+In addition, we have also provide an online version at [link](https://nir.chemoinfolab.com)
+
+
 ## Usage
-### Simulata NIR spectra (spc) and reference values (conc) 
+
+### Simulata NIR spectra (spc) and reference values (conc)
+
 ```python
 from pynir.utils import simulateNIR
 
 spc, conc = simulateNIR()
 ```
 
 ### Regression
+
 ```python
 from pynir.utils import simulateNIR
 from pynir.Calibration import pls
 
 # estabilish PLS model
 n_components = 10
 plsModel = pls(n_components = n_components)
 plsModel.fit(X,y)
 
 yhat = plsModel.predict(X)
 ```
 
-
 ### Classification
+
 ```python
 
 # simulate NIR data
 from pynir.utils import simulateNIR
 from pynir.Calibration import plsda
 
 nclass = 4
@@ -47,30 +54,31 @@
 plsdaModel.fit(X,y)
 
 yhat = plsdaModel.predict(X)
 
 ```
 
 ### Feature selection
+
 ```python
 # Feature selection
 from pynir.utils import simulateNIR
 from pynir.Calibration import pls
 from pynir.FeatureSelection import MCUVE
 
 # simulate NIR data
 X,y,wv = simulateNIR(nSample=200,n_components=10,noise=1e-5)
 
 mcModel = MCUVE(X, y, n_components, nrep=nrep).fit()
 featureSelected_MC_UVE = mcModel.featureRank[:nSel]
 
 ```
 
-
 ### Outlier dection
+
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pynir.utils import simulateNIR
 
 from pynir.OutlierDection import outlierDection_PLS
@@ -79,17 +87,16 @@
 X,y,wv = simulateNIR(nSample=200,n_components=10,noise=1e-5)
 
 ODModel = outlierDection_PLS(ncomp=3)
 Q, Tsq, Q_conf, Tsq_conf, idxOutlier = ODModel.fit(X, y).detect(X,y)
 ODModel.plot_HotellingT2_Q(Q, Tsq, Q_conf, Tsq_conf)
 ```
 
-
-
 ### Calibration Transfer
+
 ```python
 from pynir.utils import simulateNIR_calibrationTransfer
 from pynir.Calibration import pls, regresssionReport
 from pynir.CalibrationTransfer import PDS,SST, BS
 import matplotlib.pyplot as plt
 import numpy as np
 
@@ -133,16 +140,16 @@
 # Calibration transfer on prediction
 ## BS
 yhat2_BS = BS().fit(yhat1, yhat2).transform(yhat2)
 plsModel1.plot_prediction(y[idxTest], yhat2_BS, title= "BS")
 
 ```
 
-
 ### Calibration Enhancement
+
 ```python
 from pynir.utils import simulateNIR_calibrationTransfer
 from pynir.Calibration import pls, regresssionReport
 from pynir.CalibrationTransfer import NS_PFCE,SS_PFCE,FS_PFCE,MT_PFCE
 import matplotlib.pyplot as plt
 import numpy as np
 
@@ -224,23 +231,25 @@
 ax.set_xlabel("wavelength (nm)")
 ax.set_ylabel("Regression Coefficients")
 ax.set_title("MT-PFCE")
 print("cost {:.2f} seconds for MT-PFCE".format(time.time()-tic))
 
 ```
 
-
-
 ## Demon
+
 First, execute
+
 ```bash
 git clone https://github.com/JinZhangLab/pynir.git
-cd ./pynir/tests
+cd ./pynir/examples
 ```
+
 Then, execute code in your python coding environment or just in terminal as follows:
+
 ```bash
 python Demo1_SimulateNIR.py
 python Demo2_Regression.py
 python Demo3_Binary_Classification.py
 python Demo4_Multiclass_Classification.py
 python Demo5_dataPreprocessing.py
 python Demo6_outierDection.py
@@ -249,18 +258,22 @@
 python Demo9_calibrationTransfer.py
 python Demo10_calibrationTransfer_PFCE_simulateNIR.py
 python Demo11_calibrationTransfer_PFCE_Tablet.py
 python Demo12_calibrationTransfer_PFCE_Corn.py
 ```
 
 ## Ref
-[_1. Zhang, J.;  Cui, X. Y.;  Cai, W. S.; Shao, X. G., A variable importance criterion for variable selection in near-infrared spectral analysis. Sci. China Chem. 2018, 62, 271-79._](https://link.springer.com/article/10.1007%2Fs11426-018-9368-9)
-[_2. Zhang J., Li B. Y., Hu Y., Zhou L. X., Wang G. Z., Guo G., Zhang Q. H., Lei S. C., Zhang A. H. A parameter-free framework for calibration enhancement of near-infrared spectroscopy based on correlation constraint [J]. Analytica Chimica Acta, 2021, 1142: 169-178.
-_](https://linkinghub.elsevier.com/retrieve/pii/S0003-2670(20)31110-7)
+
+- Zhang, J.; Cui, X. Y.; Cai, W. S.; Shao, X. G., A variable importance criterion for variable selection in near-infrared spectral analysis. Sci. China Chem. 2018, 62, 271-79.[link](https://link.springer.com/article/10.1007%2Fs11426-018-9368-9)
+
+- Zhang J., Li B. Y., Hu Y., Zhou L. X., Wang G. Z., Guo G., Zhang Q. H., Lei S. C., Zhang A. H. A parameter-free framework for calibration enhancement of near-infrared spectroscopy based on correlation constraint [J]. Analytica Chimica Acta, 2021, 1142: 169-178.
+  [link](<https://linkinghub.elsevier.com/retrieve/pii/S0003-2670(20)31110-7>)
 
 ## Contributing
+
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
+
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `pynir-0.7.1/pyproject.toml` & `pynir-0.7.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pynir"
-version = "0.7.1"
-authors = [
-  { name="Jin Zhang", email="jinzhang@nankai.edu.cn" },
-]
+version = "0.7.3"
+authors = [{ name = "Jin Zhang", email = "jinzhang@nankai.edu.cn" }]
 description = "NIR calibration toolbox in python"
 readme = "README.md"
 requires-python = ">=3.7"
 
 dependencies = [
   "numpy>=1.13.3",
-  "scipy>=1.9.1",
+  "scipy>=1.7.1",
   "scikit-learn>=1.0.2",
   "PyWavelets>=1.4.1",
   "matplotlib>=3.6.0",
 ]
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/JinZhangLab/pynir"
 "Bug Tracker" = "https://github.com/JinZhangLab/pynir/issues"
+"Documentation" = "https://pynir.readthedocs.io/en/latest/"
```

### Comparing `pynir-0.7.1/PKG-INFO` & `pynir-0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 Metadata-Version: 2.1
 Name: pynir
-Version: 0.7.1
+Version: 0.7.3
 Summary: NIR calibration toolbox in python
 Project-URL: Homepage, https://github.com/JinZhangLab/pynir
 Project-URL: Bug Tracker, https://github.com/JinZhangLab/pynir/issues
+Project-URL: Documentation, https://pynir.readthedocs.io/en/latest/
 Author-email: Jin Zhang <jinzhang@nankai.edu.cn>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: pywavelets>=1.4.1
 Requires-Dist: scikit-learn>=1.0.2
-Requires-Dist: scipy>=1.9.1
+Requires-Dist: scipy>=1.7.1
 Description-Content-Type: text/markdown
 
 # Commom Calibration methods for multivariate calibration
 
 This is a Python library for dealing with multivariate calibration, e.g., Near infrared spectra regression and classification tasks.
 
 ## Installation
 
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [pynir](https://pypi.org/project/pynir/)
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [pynir](https://pypi.org/project/pynir/). 
 
 ```bash
 pip install pynir
 ```
+
+In addition, we have also provide an online version at [link](https://nir.chemoinfolab.com)
+
+
 ## Usage
-### Simulata NIR spectra (spc) and reference values (conc) 
+
+### Simulata NIR spectra (spc) and reference values (conc)
+
 ```python
 from pynir.utils import simulateNIR
 
 spc, conc = simulateNIR()
 ```
 
 ### Regression
+
 ```python
 from pynir.utils import simulateNIR
 from pynir.Calibration import pls
 
 # estabilish PLS model
 n_components = 10
 plsModel = pls(n_components = n_components)
 plsModel.fit(X,y)
 
 yhat = plsModel.predict(X)
 ```
 
-
 ### Classification
+
 ```python
 
 # simulate NIR data
 from pynir.utils import simulateNIR
 from pynir.Calibration import plsda
 
 nclass = 4
@@ -66,30 +74,31 @@
 plsdaModel.fit(X,y)
 
 yhat = plsdaModel.predict(X)
 
 ```
 
 ### Feature selection
+
 ```python
 # Feature selection
 from pynir.utils import simulateNIR
 from pynir.Calibration import pls
 from pynir.FeatureSelection import MCUVE
 
 # simulate NIR data
 X,y,wv = simulateNIR(nSample=200,n_components=10,noise=1e-5)
 
 mcModel = MCUVE(X, y, n_components, nrep=nrep).fit()
 featureSelected_MC_UVE = mcModel.featureRank[:nSel]
 
 ```
 
-
 ### Outlier dection
+
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pynir.utils import simulateNIR
 
 from pynir.OutlierDection import outlierDection_PLS
@@ -98,17 +107,16 @@
 X,y,wv = simulateNIR(nSample=200,n_components=10,noise=1e-5)
 
 ODModel = outlierDection_PLS(ncomp=3)
 Q, Tsq, Q_conf, Tsq_conf, idxOutlier = ODModel.fit(X, y).detect(X,y)
 ODModel.plot_HotellingT2_Q(Q, Tsq, Q_conf, Tsq_conf)
 ```
 
-
-
 ### Calibration Transfer
+
 ```python
 from pynir.utils import simulateNIR_calibrationTransfer
 from pynir.Calibration import pls, regresssionReport
 from pynir.CalibrationTransfer import PDS,SST, BS
 import matplotlib.pyplot as plt
 import numpy as np
 
@@ -152,16 +160,16 @@
 # Calibration transfer on prediction
 ## BS
 yhat2_BS = BS().fit(yhat1, yhat2).transform(yhat2)
 plsModel1.plot_prediction(y[idxTest], yhat2_BS, title= "BS")
 
 ```
 
-
 ### Calibration Enhancement
+
 ```python
 from pynir.utils import simulateNIR_calibrationTransfer
 from pynir.Calibration import pls, regresssionReport
 from pynir.CalibrationTransfer import NS_PFCE,SS_PFCE,FS_PFCE,MT_PFCE
 import matplotlib.pyplot as plt
 import numpy as np
 
@@ -243,23 +251,25 @@
 ax.set_xlabel("wavelength (nm)")
 ax.set_ylabel("Regression Coefficients")
 ax.set_title("MT-PFCE")
 print("cost {:.2f} seconds for MT-PFCE".format(time.time()-tic))
 
 ```
 
-
-
 ## Demon
+
 First, execute
+
 ```bash
 git clone https://github.com/JinZhangLab/pynir.git
-cd ./pynir/tests
+cd ./pynir/examples
 ```
+
 Then, execute code in your python coding environment or just in terminal as follows:
+
 ```bash
 python Demo1_SimulateNIR.py
 python Demo2_Regression.py
 python Demo3_Binary_Classification.py
 python Demo4_Multiclass_Classification.py
 python Demo5_dataPreprocessing.py
 python Demo6_outierDection.py
@@ -268,18 +278,22 @@
 python Demo9_calibrationTransfer.py
 python Demo10_calibrationTransfer_PFCE_simulateNIR.py
 python Demo11_calibrationTransfer_PFCE_Tablet.py
 python Demo12_calibrationTransfer_PFCE_Corn.py
 ```
 
 ## Ref
-[_1. Zhang, J.;  Cui, X. Y.;  Cai, W. S.; Shao, X. G., A variable importance criterion for variable selection in near-infrared spectral analysis. Sci. China Chem. 2018, 62, 271-79._](https://link.springer.com/article/10.1007%2Fs11426-018-9368-9)
-[_2. Zhang J., Li B. Y., Hu Y., Zhou L. X., Wang G. Z., Guo G., Zhang Q. H., Lei S. C., Zhang A. H. A parameter-free framework for calibration enhancement of near-infrared spectroscopy based on correlation constraint [J]. Analytica Chimica Acta, 2021, 1142: 169-178.
-_](https://linkinghub.elsevier.com/retrieve/pii/S0003-2670(20)31110-7)
+
+- Zhang, J.; Cui, X. Y.; Cai, W. S.; Shao, X. G., A variable importance criterion for variable selection in near-infrared spectral analysis. Sci. China Chem. 2018, 62, 271-79.[link](https://link.springer.com/article/10.1007%2Fs11426-018-9368-9)
+
+- Zhang J., Li B. Y., Hu Y., Zhou L. X., Wang G. Z., Guo G., Zhang Q. H., Lei S. C., Zhang A. H. A parameter-free framework for calibration enhancement of near-infrared spectroscopy based on correlation constraint [J]. Analytica Chimica Acta, 2021, 1142: 169-178.
+  [link](<https://linkinghub.elsevier.com/retrieve/pii/S0003-2670(20)31110-7>)
 
 ## Contributing
+
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
+
 [MIT](https://choosealicense.com/licenses/mit/)
```

