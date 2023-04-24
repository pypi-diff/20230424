# Comparing `tmp/cowch-0.1-py3-none-any.whl.zip` & `tmp/cowch-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3774 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     6604 b- defN 23-Apr-23 20:08 cowch/__init__.py
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-23 20:08 cowch-0.1.dist-info/License.txt
--rw-rw-rw-  2.0 fat      360 b- defN 23-Apr-23 20:08 cowch-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 20:08 cowch-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-23 20:08 cowch-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      439 b- defN 23-Apr-23 20:08 cowch-0.1.dist-info/RECORD
-6 files, 7508 bytes uncompressed, 2976 bytes compressed:  60.4%
+Zip file size: 4254 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     7721 b- defN 23-Apr-24 19:45 cowch/__init__.py
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      360 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      439 b- defN 23-Apr-24 19:59 cowch-0.2.dist-info/RECORD
+6 files, 8625 bytes uncompressed, 3456 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: cowch/__init__.py
 Comment: 
 
-Filename: cowch-0.1.dist-info/License.txt
+Filename: cowch-0.2.dist-info/License.txt
 Comment: 
 
-Filename: cowch-0.1.dist-info/METADATA
+Filename: cowch-0.2.dist-info/METADATA
 Comment: 
 
-Filename: cowch-0.1.dist-info/WHEEL
+Filename: cowch-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cowch-0.1.dist-info/top_level.txt
+Filename: cowch-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cowch-0.1.dist-info/RECORD
+Filename: cowch-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cowch/__init__.py

```diff
@@ -89,14 +89,38 @@
 library(class)
 install.packages("e1071")
 library(e1071)
 mod1 <- naiveBayes(iris[,1:4],iris[,5])
 mod2 <- naiveBayes(model2_scores,iris[,5])
 table(predict(mod1,iris[,1:4]),iris[,5])
 table(predict(mod2,model2_scores),iris[,5])    
+
+
+
+chatgpt
+# Load the iris dataset
+data(iris)
+
+# Select the numeric columns of the dataset
+numeric_cols <- c("Sepal.Length", "Sepal.Width", "Petal.Length", "Petal.Width")
+iris_numeric <- iris[numeric_cols]
+#iris_numeric <- iris[1:4]
+
+# Perform PCA on the dataset
+pca <- prcomp(iris_numeric, center = TRUE, scale. = TRUE)
+
+# Print the summary of the PCA results
+summary(pca)
+biplot(pca)
+screeplot(pca,type="lines")
+
+# Plot the first two principal components
+#plot(pca$x[,1], pca$x[,2], col = iris$Species)
+
+
     
     
     """)
 
 def pr4():
     print(""" 
 Practical 4 RUN Practical of Clustering
@@ -165,64 +189,85 @@
 
 def pr7():
     print("""     
     
 
 Practical 7 Principal of Logistics Regression
 
-
-data("wrapbreaks")
-head(warpbreaks)
-summary("warpbreaks")
-model_1 <- aov(breaks~wook+tension,data=warpbreaks)
-summary(model_1)
-plot(model_1)
-model_2 <- aov(breaks~wool+tension+wool:tension,data=warpbreaks)
-model
+height<-c(102,117,105,141,135,115,138,144,137,100,131,119,115,121,113)
+weight<-c(61,46,62,54,60,69,51,50,46,69,48,56,64,48,59)
+student<-lm(weight~height)
+student
+predict(student,data.frame(height=199),interval="confidence")
+plot(student)
+student
 
     
     """)
 
 def pr8():
     print(""" 
     
-Practical 8 Principal of Hypothesis testing
-
-
-dataf <- seq(1,20,by = 1)
-dataf
-mean(dataf)
-a <- t.test(dataf.alternate = "two.sided",mu=10,conf.int=0.95)
+#practical 8 hypothesis
+dataset1<-c(12,123,13,434,2342,1231,3424,2343)
+dataset2 <-c(323,234,455,54534)
+dataset1
+dataset2
+mean(dataset1)
+mean(dataset2)
+sd(dataset1)
+sd(dataset2)
+a<-t.test(dataset1,dataset2,alternate="two.sided",mu=10,conf.int=0.95)
 a
 a$p.value
 a$statistic
-(10.5-10)/sd(dataf)/sqrt(length(dataf))
-length(dataf)
-dataf
-dataf <- seq(1,20,by=1)
-length(dataf)
-t.test(x,mu)
-    
-    
+
     """)
 
 def pr9():
     print("""   
     
-Practical No 9 RUN
+Practical No 9 RUN  Analysis variance
+
 # import inbuilt dataset
 data("warpbreaks")
-head("warpbreaks")
+head(warpbreaks)
 summary("warpbreaks")
-model_1<-aov(breaks~wool+tension,data=warpbreaks)
+model_1 <- aov(breaks~wool+tension,data=warpbreaks)
 summary(model_1)
 plot(model_1)
-model_2<-aov(breaks~wool+tension+wool:tension,data=warpbreaks)
-summary(model_2)
-plot(model_2)
+model_2 <- aov(breaks~wool+tension+wool:tension,data=warpbreaks)
+model
+    
+    """)
+
+def csv():
+    print(""" 
+    create csv file 
+
+    
+# Create a data frame
+#create a CSV file  student.csv file with fields (name ,roll no, gender, tmarks)
+student <- data.frame(
+  roll_no = 1:5,
+  name = c("John", "Jane", "Bob", "Alice", "Tom"),
+  age = c(25, 32, 19, 41, 28),
+  gender = c("male","male","female","female","male"),
+  tmarks = c(67,25,74,77,57)
+)
+
+# Write the data frame to a CSV file
+write.csv(student, "student.csv", row.names = FALSE)
+
+# import and store the dataset in data1
+data <- read.csv("student.csv")
+print(data)
+
+
+   
     
     """)
 
 def pr10():
     print("""  
 Practical 10 RUN Practical of Decision Tree
```

