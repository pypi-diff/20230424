# Comparing `tmp/pynir-0.5.tar.gz` & `tmp/pynir-0.6.tar.gz`

## Comparing `pynir-0.5.tar` & `pynir-0.6.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0    17752 2020-02-02 00:00:00.000000 pynir-0.5/src/pynir/Calibration.py
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 pynir-0.5/src/pynir/CalibrationTransfer.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.5/src/pynir/FeatureSelection.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pynir-0.5/src/pynir/OutlierDection.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.5/src/pynir/Preprocessing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.5/src/pynir/__init__.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 pynir-0.5/src/pynir/utils.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo10_calibrationTransfer_PFCE.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo11_calibrationTransfer_PFCE_Tablet.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo1_SimulateNIR.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo2_Regression.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo3_Binary_Classification.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo4_Multiclass_Classification.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo5_dataPreprocessing.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo6_outierDection.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo7_FeatureSelection_oneStep.py
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo8_FeatureSelection_multiSteps.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pynir-0.5/tests/Demo9_calibrationTransfer.py
--rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.5/tests/Tablet.mat
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.5/LICENSE.txt
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pynir-0.5/README.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pynir-0.5/pyproject.toml
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pynir-0.5/PKG-INFO
+-rw-r--r--   0        0        0    18437 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/Calibration.py
+-rw-r--r--   0        0        0    10981 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/CalibrationTransfer.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/FeatureSelection.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/OutlierDection.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/Preprocessing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/untitled0.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 pynir-0.6/src/pynir/utils.py
+-rw-r--r--   0        0        0  1215471 2020-02-02 00:00:00.000000 pynir-0.6/tests/Data_Corn.mat
+-rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.6/tests/Data_Tablet.mat
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo10_calibrationTransfer_PFCE.py
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo11_calibrationTransfer_PFCE_Tablet.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo12_calibrationTransfer_PFCE_Corn.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo1_SimulateNIR.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo2_Regression.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo3_Binary_Classification.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo4_Multiclass_Classification.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo5_dataPreprocessing.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo6_outierDection.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo7_FeatureSelection_oneStep.py
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo8_FeatureSelection_multiSteps.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pynir-0.6/tests/Demo9_calibrationTransfer.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pynir-0.6/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pynir-0.6/pyproject.toml
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pynir-0.6/PKG-INFO
```

### Comparing `pynir-0.5/src/pynir/Calibration.py` & `pynir-0.6/src/pynir/Calibration.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 from scipy.spatial.distance import cdist
 
 from sklearn.cross_decomposition import PLSRegression
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
 from sklearn.svm import LinearSVC, SVC
 from sklearn.ensemble import RandomForestClassifier
 
-from sklearn.model_selection import GridSearchCV
+from sklearn.model_selection import GridSearchCV, cross_val_predict
 
 import matplotlib.pyplot as plt
 
+
 class nirData():
     def __init__(self, X, y, trainIdx=None, testIdx=None):
         self.X = X
         self.y = y
         self.trainIdx = trainIdx
         self.testIdx = testIdx
 
@@ -146,81 +147,94 @@
                 transform = ax.transAxes)
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
         ax.legend(loc='upper left', bbox_to_anchor=(0.0, 1.0))
         ax.set_title(title)
 
 
-class plsda():
-    def __init__(self, nComp = 2):
-        self.nComp = nComp
+class plsda(PLSRegression):
+    def __init__(self, n_components=2, scale=True, **kwargs):
+        super().__init__(n_components=n_components, scale=scale, **kwargs)
+        self.lda = LinearDiscriminantAnalysis()
 
     def fit(self, X, y):
         self.X = X
         self.y = y
-        self.classes = np.unique(y)
-        if len(self.classes) > 2 :
-            multi_2_Model = multiClass_to_binaryMatrix().fit(y)
-            ymulti = multi_2_Model.transform(y)
-        else:
-            ymulti = y
-
-        plsModel = PLSRegression(n_components = self.nComp, scale=False)
-        plsModel.fit(X,ymulti)
-
-        ldaModel = LinearDiscriminantAnalysis().fit(plsModel.transform(X), y)
-
-        model=dict()
-        model["plsModel"] = plsModel
-        model["ldaModel"] = ldaModel
-        self.model = model
+        super().fit(X, y)
+        self.lda.fit(self.x_scores_, y)
         return self
 
     def predict(self, X):
-        return self.model["ldaModel"].predict(self.model["plsModel"].transform(X))
+        return self.lda.predict(self.transform(X))
 
     def predict_log_proba(self, X):
-        return self.model["ldaModel"].predict_log_proba(self.model["plsModel"].transform(X))
+        return self.lda.predict_log_proba(self.predict(X))
 
     def predict_proba(self, X):
-        return self.model["ldaModel"].predict_proba(self.model["plsModel"].transform(X))
+        return self.lda.predict_proba(self.predict(X))
 
     def crossValidation_predict(self, nfold = 10):
         X = self.X
         y = self.y
-        yhat = np.zeros((y.shape[0],self.nComp))
-        for i in range(self.nComp):
-            model = plsda(nComp = i+1)
+        yhat = np.zeros((y.shape[0],self.n_components))
+        for i in range(self.n_components):
+            model = plsda(n_components = i+1)
             for train, test in KFold(n_splits=nfold).split(X):
                 model.fit(X[train,:], y[train])
                 yhat[test,i] = model.predict(X[test,:])
         return yhat
 
     def get_optLV(self, nfold = 10):
         yhat_cv = self.crossValidation_predict(nfold)
         accuracy_cv = []
         for i in range(yhat_cv.shape[1]):
-            if len(self.classes) == 2 :
+            if len(self.lda.classes_) == 2 :
                 report_cv = binaryClassificationReport(self.y, yhat_cv[:,i])
                 accuracy_cv.append(report_cv["accuracy"])
-            elif len(self.classes) > 2:
+            elif len(self.lda.classes_) > 2:
                 report_cv = multiClassificationReport(self.y, yhat_cv[:,i])
                 accuracy_tmp = [rep["accuracy"] for rep in report_cv.values()]
                 accuracy_cv.append(sum(accuracy_tmp))
 
         optLV = int(np.argmax(accuracy_cv)+1)
         self.optLV = optLV
         return optLV
 
-
     def get_confusion_matrix(self, X, y):
         yhat = self.predict(X)
         cm = confusion_matrix(y, yhat)
         return cm
 
+    def get_vip(self):
+        t = self.x_scores_ / self.x_scores_.std(axis=0)
+        s = np.sum(t**2, axis=1)
+        s /= np.sum(t**2)
+        vip = s * np.sum(t**2, axis=1)
+        return vip
+
+    def permutation_test(self, X, y, n_repeats=100,n_jobs = None):
+        # Initialize arrays to store Q2 and R2 values
+        q2 = np.zeros(n_repeats)
+        r2 = np.zeros(n_repeats)
+        permutation_ratio = np.zeros(n_repeats)
+        # Perform the permutation test
+        for i in range(n_repeats):
+            # Shuffle the target variable
+            y_shuffled = np.random.permutation(y)
+
+            # Fit the model to the shuffled target variable
+            self.fit(X, y_shuffled)
+
+            # Calculate the cross-validated Q2 and R2 values
+            y_pred = cross_val_predict(self, X, y_shuffled, cv=10, n_jobs = n_jobs)
+            q2[i] = self.score(X, y_shuffled)
+            r2[i] = r2_score(y_shuffled, y_pred)
+            permutation_ratio[i] = np.sum(y_shuffled != y) / len(y)
+        return q2, r2, permutation_ratio
+
 class lsvc(LinearSVC):# linear svc
     def get_optParams(self, X, y, Params = None, nfold = 10, n_jobs = None):
         if Params is None:
             Params = {'C': np.logspace(-4, 5, 10),
                       'penalty': ('l1', 'l2')}
         self.gsh = GridSearchCV(estimator=self,  param_grid=Params,
                            cv = nfold, n_jobs = n_jobs)
```

### Comparing `pynir-0.5/src/pynir/CalibrationTransfer.py` & `pynir-0.6/src/pynir/CalibrationTransfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,130 +5,130 @@
 @author: chinn
 """
 import numpy as np
 from sklearn.linear_model import LinearRegression
 from sklearn.cross_decomposition import PLSRegression
 from sklearn.decomposition import TruncatedSVD
 
-from scipy.optimize import (BFGS, SR1, Bounds, 
+from scipy.optimize import (BFGS, SR1, Bounds,
                             NonlinearConstraint, minimize)
 
 
 class PDS():
     def __init__(self, halfWindowSize = 7, regType = 'mlr',**kwargs):
         self.halfWindowSize = halfWindowSize
         self.regType = regType
         self.kwargs = kwargs
-    
+
     def get_windowRange(halfWindowSize, nFeatrues, i):
         if i < halfWindowSize:
             band = np.arange(i)
         elif i > nFeatrues-halfWindowSize:
             band = np.arange(i)
         else:
             band = np.arange(i-halfWindowSize, i+halfWindowSize)
         return band
-    
+
     def fit(self, X1, X2):
         """
         Parameters
         ----------
         X1 : 2D array
             Standard spectra of master.
-            
+
         X2 : 2D array
             Standard spectra of master.
         """
-        
+
         if X1.shape != X2.shape:
             raise("The dimension of two spectral matrix doesn't match.")
-        
+
         Models = []
 
         for i in range(X1.shape[1]):
             if i < self.halfWindowSize:
                 X2i = X2[:,:2*self.halfWindowSize+1]
             elif i >= self.halfWindowSize and i < X2.shape[1]-self.halfWindowSize:
                 X2i = X2[:,i-self.halfWindowSize:i+self.halfWindowSize+1]
             elif i > X2.shape[1]-self.halfWindowSize:
                 X2i = X2[:,X2.shape[1]-2*self.halfWindowSize-1:]
 
 
-            
+
             if self.regType == 'mlr':
                 Models.append(LinearRegression().fit(X2i,X1[:,i][:,None]))
             elif self.regType == 'pls':
                 Models.append(PLSRegression(n_components=self.nComp).fit(X2i,X1[:,i][:,None]))
-        
+
         self.Models = Models
         return self
-    
+
     def transform(self, X):
         Xnew = np.zeros(X.shape)
         for i in range(X.shape[1]):
             if i < self.halfWindowSize:
                 Xi = X[:,:2*self.halfWindowSize+1]
             elif i >= self.halfWindowSize and i < X.shape[1]-self.halfWindowSize:
                 Xi = X[:,i-self.halfWindowSize:i+self.halfWindowSize+1]
             elif i > X.shape[1]-self.halfWindowSize:
                 Xi = X[:,X.shape[1]-2*self.halfWindowSize-1:]
-            
+
             Xnew[:,i] = self.Models[i].predict(Xi).ravel()
         return Xnew
-    
-    
+
+
 class SST():
     def __init__(self, nComp=2):
         self.nComp = nComp
-        
+
     def fit(self,X1,X2):
         """
         Parameters
         ----------
         X1 : 2D array
             Standard spectra of the first instrument.
-            
+
         X2 : 2D array
             Standard spectra of the second instrument.
         """
         svd = TruncatedSVD(n_components=self.nComp).fit(np.hstack((X1,X2)))
         P = svd.components_
         nFeature_X1 = X1.shape[1]
         W1 = P[:,:nFeature_X1]
         W2 = P[:,nFeature_X1:]
         self.F = np.dot(np.linalg.pinv(W2),  (W1-W2))
         return self
-    
+
     def transform(self,X):
         return X + np.dot(X,self.F)
- 
-    
+
+
 class BS():
     """
-    Ref Osborne B. G., Fearn T. Collaborative evaluation of universal 
-        calibrations for the measurement of protein and moisture in flour by near 
-        infrared reflectance [J]. International Journal of Food Science & Technology, 
+    Ref Osborne B. G., Fearn T. Collaborative evaluation of universal
+        calibrations for the measurement of protein and moisture in flour by near
+        infrared reflectance [J]. International Journal of Food Science & Technology,
         1983, 18(4): 453-460.
     """
     def __init__(self):
         pass
-    
+
     def fit(self, y1, y2):
         self.lrModel = LinearRegression().fit(y2.reshape(-1,1), y1.reshape(-1,1))
         return self
-    
+
     def transform(self, y2):
         return self.lrModel.predict(y2.reshape(-1,1))
 
 
 class NS_PFCE():
     def __init__(self,thres = 0.98, constrType = 1):
         self.thres = thres
         self.constrType = constrType
-    
+
     def fit(self, X1, X2, b1):
         ntask = 2
         lb = -np.inf
         ub = 0.0
         if self.constrType == 1:
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr1(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
@@ -137,29 +137,29 @@
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr2(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
                                        self.thres), lb, ub)
         elif self.constrType == 3:
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr3(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
                                        self.thres), lb, ub)
-            
+
         b2 = minimize(lambda b2:cost_NS_PFCE(b1,b2,X1,X2),
                       x0 = b1, method='SLSQP', constraints=[nlc])
         self.b2 = b2
         return self
-    
+
     def transform(self, X):
-        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)), 
+        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)),
                       np.reshape(self.b2.x,(-1,1)))
 
 class SS_PFCE():
     def __init__(self,thres = 0.98, constrType = 1):
         self.thres = thres
         self.constrType = constrType
-    
+
     def fit(self, X2, y, b1):
         ntask = 2
         lb = -np.inf
         ub = 0.0
         if self.constrType == 1:
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr1(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
@@ -170,30 +170,30 @@
                                        self.thres), lb, ub)
         elif self.constrType == 3:
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr3(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
                                        self.thres), lb, ub)
         else:
             raise("PFCE only support the constrint type of 1, 2, or 3")
-        
+
         b2 = minimize(lambda b2:cost_SS_PFCE(b2,X2, np.ravel(y)),
                       x0 = b1, method='SLSQP', constraints=[nlc])
         self.b2 = b2
         return self
-    
+
     def transform(self, X):
-        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)), 
+        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)),
                       np.reshape(self.b2.x,(-1,1)))
 
 
 class FS_PFCE():
     def __init__(self,thres = 0.98, constrType = 1):
         self.thres = thres
         self.constrType = constrType
-    
+
     def fit(self, X1, X2, y, b1):
         ntask = 2
         lb = -np.inf
         ub = 0.0
         if self.constrType == 1:
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr1(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
@@ -202,30 +202,30 @@
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr2(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
                                        self.thres), lb, ub)
         elif self.constrType == 3:
             nlc = NonlinearConstraint(
                 lambda b2:pfce_constr3(np.hstack((b1.reshape(-1,1), b2.reshape(-1,1))),
                                        self.thres), lb, ub)
-            
+
         b2 = minimize(lambda b2:cost_FS_PFCE(b1,b2,X1,X2,np.ravel(y)),
                       x0 = b1,  method='SLSQP', constraints=[nlc])
         self.b2 = b2
         return self
-    
+
     def transform(self, X):
-        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)), 
+        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)),
                       np.reshape(self.b2.x,(-1,1)))
-    
+
 
 class MT_PFCE():
     def __init__(self,thres = 0.98, constrType = 1):
         self.thres = thres
         self.constrType = constrType
-    
+
     def fit(self, X, y, b1):
         ntask = len(X)
         y = [np.ravel(yi) for yi in y]
         self.ntask = ntask
         lb = -np.inf
         ub = 0.0
         if self.constrType == 1:
@@ -236,22 +236,22 @@
             nlc = NonlinearConstraint(
                 lambda B:pfce_constr2(np.transpose(np.reshape(B,(ntask,-1))),
                                        self.thres), lb, ub)
         elif self.constrType == 3:
             nlc = NonlinearConstraint(
                 lambda B:pfce_constr3(np.transpose(np.reshape(B,(ntask,-1))),
                                        self.thres), lb, ub)
-         
+
         B = minimize(lambda B:cost_MT_PFCE(B.reshape(ntask,-1).transpose(),X,y),
-                      x0 = np.repeat(b1,ntask,axis=0).ravel(),method='SLSQP',constraints=[nlc])
+                      x0 = np.tile(b1,ntask),method='SLSQP',constraints=[nlc])
         self.B = B
         return self
-    
+
     def transform(self, X, itask):
-        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)), 
+        return np.dot(np.hstack((np.ones([X.shape[0],1]), X)),
                       ((self.B.x).reshape(self.ntask,-1).transpose()[:,itask]).reshape((-1,1)))
 
 
 def cost_NS_PFCE(b1, b2, X1, X2):
     yhat1 = np.dot(np.hstack((np.ones([X1.shape[0],1]), X1)), b1)
     yhat2 = np.dot(np.hstack((np.ones([X2.shape[0],1]), X2)), b2)
     error = yhat1-yhat2
@@ -288,24 +288,30 @@
 
 def pfce_constr2(B,thres):
     B = B[1:,]
     Vars = np.diag(np.dot(B.transpose(),B))
     VarErr = 0
     for i in range(B.shape[1]):
         Err = B-B[:,i][:,None]
-        VarErr += np.sum(Err**2)
-    VarErr = VarErr/np.sum(np.arange(B.shape[1]))/2
-    dist = VarErr/np.prod(Vars)**(1/B.shape[1])
+        Erri = Err;
+        Erri = np.delete(Erri, i, axis =1)
+        Varsi = Vars
+        Varsi = np.delete(Varsi, i)
+        VarErr += np.sum(Erri**2,axis = 0)/np.sqrt(Vars[i]*Varsi)
+    dist = VarErr/(B.shape[1] * (B.shape[1]-1))
     constr_cost = thres - 1 + dist
     return constr_cost
 
 def pfce_constr3(B,thres):
     B = B[1:,]
     norm1s = np.sum(np.abs(B),axis=0)
     norm1Err = 0
     for i in range(B.shape[1]):
         Err = B-B[:,i][:,None]
-        norm1Err += np.sum(np.abs(Err))
-    norm1Err = norm1Err/np.sum(np.arange(B.shape[1]))/2
-    dist = norm1Err/np.prod(norm1s)**(1/B.shape[1])
+        Erri = Err
+        Erri = np.delete(Erri, i,axis = 1)
+        norm1si = norm1s
+        norm1si = np.delete(norm1si, i)
+        norm1Err += np.sum(np.abs(Erri),axis = 0)/np.sqrt(norm1s[i]*norm1si)
+    dist = norm1Err/(B.shape[1] * (B.shape[1]-1))
     constr_cost = thres - 1 + dist
-    return constr_cost
+    return constr_cost
```

### Comparing `pynir-0.5/src/pynir/FeatureSelection.py` & `pynir-0.6/src/pynir/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/src/pynir/OutlierDection.py` & `pynir-0.6/src/pynir/OutlierDection.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/src/pynir/Preprocessing.py` & `pynir-0.6/src/pynir/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/src/pynir/utils.py` & `pynir-0.6/src/pynir/utils.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/tests/Demo10_calibrationTransfer_PFCE.py` & `pynir-0.6/tests/Demo10_calibrationTransfer_PFCE.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/tests/Demo11_calibrationTransfer_PFCE_Tablet.py` & `pynir-0.6/tests/Demo11_calibrationTransfer_PFCE_Tablet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+import sys
+from pathlib import Path
+
+pynir_path = str(Path(__file__).parent.parent / 'src')
+
+if pynir_path not in sys.path:
+    sys.path.append(pynir_path)
+    print("add pynir path")
+
 from pynir.utils import simulateNIR_calibrationTransfer
 from pynir.Calibration import pls, regresssionReport
 from pynir.CalibrationTransfer import NS_PFCE,SS_PFCE,FS_PFCE,MT_PFCE
 import matplotlib.pyplot as plt
 import numpy as np
 
 from scipy.io import loadmat
 
 from sklearn.model_selection import train_test_split
 
 import time
 
 
-RawData = loadmat("./Tablet.mat")
+RawData = loadmat("./Data_Tablet.mat")
 wv = RawData["wv"].ravel()
 Xcal1 = RawData["Xcal1"]
 Xcal2 = RawData["Xcal2"]
 Xtrans1 = RawData["Xtrans1"]
 Xtrans2 = RawData["Xtrans2"]
 Xtest1 = RawData["Xtest1"]
 Xtest2 = RawData["Xtest2"]
@@ -48,15 +57,15 @@
 fig, ax = plt.subplots()
 ax.plot(wv, plsModel1.model['B'][1:,-1])
 ax.set_xlabel("wavelength (nm)")
 ax.set_ylabel("Regression Coefficients")
 
 ## PFCE
 thres = 0.98
-constrType = 3
+constrType = 1
 
 tic = time.time()
 b1 = plsModel1.model['B'][:,-1]
 NS_PFCE_model = NS_PFCE(thres=thres, constrType=constrType).fit(Xtrans1,Xtrans2,b1)
 yhat2_NS_PFCE = NS_PFCE_model.transform(Xtest2)
 plsModel1.plot_prediction(ytest, yhat2_NS_PFCE, title= "NS-PFCE")
 
@@ -93,23 +102,29 @@
 ax.set_xlabel("wavelength (nm)")
 ax.set_ylabel("Regression Coefficients")
 ax.set_title("FS-PFCE")
 print("cost {:.2f} seconds".format(time.time()-tic))
 
 
 tic = time.time()
-b1 = plsModel1.model['B'][:,-1]
+plsModel_global = pls(nComp=nComp).fit(np.vstack((Xcal1,Xtrans2)),
+                                       np.vstack((ycal,ytrans)))
+optLV_global = plsModel_global.get_optLV()
+plsModel_global = pls(nComp=optLV_global).fit(np.vstack((Xcal1,Xtrans2)),
+                                       np.vstack((ycal,ytrans)))
+
+bglb = plsModel_global.model['B'][:,-1]
 MT_PFCE_model = MT_PFCE(thres=thres, constrType=constrType)
-MT_PFCE_model.fit([Xcal1,Xtrans2],(ycal,ytrans),b1)
+MT_PFCE_model.fit([Xcal1,Xtrans2],(ycal,ytrans),bglb)
 yhat1_MT_PFCE = MT_PFCE_model.transform(Xtest1,0)
 yhat2_MT_PFCE = MT_PFCE_model.transform(Xtest2,1)
 
 fig, ax = plt.subplots(2,sharex=True,figsize=(8,16))
 plsModel1.plot_prediction(ytest, yhat1_MT_PFCE, title= "MT-PFCE_First", ax= ax[0])
 plsModel1.plot_prediction(ytest, yhat2_MT_PFCE, title= "MT-PFCE_Second", ax= ax[1])
 
 fig, ax = plt.subplots()
 ax.plot(wv, MT_PFCE_model.B.x.reshape(2,-1).transpose()[1:,:])
 ax.set_xlabel("wavelength (nm)")
 ax.set_ylabel("Regression Coefficients")
 ax.set_title("MT-PFCE")
-print("cost {:.2f} seconds".format(time.time()-tic))
+print("cost {:.2f} seconds".format(time.time()-tic))
```

### Comparing `pynir-0.5/tests/Demo2_Regression.py` & `pynir-0.6/tests/Demo2_Regression.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/tests/Demo3_Binary_Classification.py` & `pynir-0.6/tests/Demo4_Multiclass_Classification.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pynir.utils import simulateNIR
 from pynir.Calibration import plsda
-from pynir.Calibration import binaryClassificationReport,plot_confusion_matrix
+from pynir.Calibration import multiClassificationReport,plot_confusion_matrix
 
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import confusion_matrix
 
 # simulate NIR data
-X,y,wv = simulateNIR(nSample=200,nComp=10,refType=2, noise=1e-5)
+nclass = 4
+X,y,wv = simulateNIR(nSample=200,nComp=10,refType=nclass, noise=1e-5)
 
 Xtrain, Xtest, ytrain,ytest = train_test_split(X,y,test_size=0.2)
 
 # estabilish PLS model
 nComp = 10
-plsdaModel = plsda(nComp = nComp).fit(Xtrain,ytrain)
+plsdaModel = plsda(nComp = nComp)
+plsdaModel.fit(Xtrain,ytrain)
 
 # 10 fold cross validation for selecting optimal nlv
 accuracy_cv = []
 yhat_cv  = plsdaModel.crossValidation_predict(nfold = 10)
 for i in range(nComp):
-    report_cv = binaryClassificationReport(ytrain, yhat_cv[:,i])
-    accuracy_cv.append(report_cv["accuracy"])
+    report_cv = multiClassificationReport(ytrain, yhat_cv[:,i])
+    accuracy_cv.append(np.mean([rep["accuracy"] for rep in report_cv.values()]))
 
 
 fig,ax = plt.subplots()
 ax.plot(np.arange(nComp)+1,accuracy_cv, marker = "*",label = "Accuracy$_c$$_v$")
 ax.set_xlabel("nLV")
 ax.set_ylabel("Accuracy")
 ax.legend()
```

### Comparing `pynir-0.5/tests/Demo5_dataPreprocessing.py` & `pynir-0.6/tests/Demo5_dataPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/tests/Demo7_FeatureSelection_oneStep.py` & `pynir-0.6/tests/Demo7_FeatureSelection_oneStep.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/tests/Demo8_FeatureSelection_multiSteps.py` & `pynir-0.6/tests/Demo8_FeatureSelection_multiSteps.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/tests/Demo9_calibrationTransfer.py` & `pynir-0.6/tests/Demo9_calibrationTransfer.py`

 * *Files identical despite different names*

### Comparing `pynir-0.5/tests/Tablet.mat` & `pynir-0.6/tests/Data_Tablet.mat`

 * *Files identical despite different names*

### Comparing `pynir-0.5/LICENSE.txt` & `pynir-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynir-0.5/README.md` & `pynir-0.6/README.md`

 * *Files identical despite different names*

### Comparing `pynir-0.5/pyproject.toml` & `pynir-0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pynir"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="Jin Zhang", email="jinzhang@nankai.edu.cn" },
 ]
 description = "NIR calibration toolbox in python"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pynir-0.5/PKG-INFO` & `pynir-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynir
-Version: 0.5
+Version: 0.6
 Summary: NIR calibration toolbox in python
 Project-URL: Homepage, https://github.com/JinZhangLab/pynir
 Project-URL: Bug Tracker, https://github.com/JinZhangLab/pynir/issues
 Author-email: Jin Zhang <jinzhang@nankai.edu.cn>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

