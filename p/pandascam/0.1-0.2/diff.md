# Comparing `tmp/pandascam-0.1-py3-none-any.whl.zip` & `tmp/pandascam-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3892 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     5997 b- defN 23-Apr-23 19:42 pandascam/__init__.py
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-23 19:46 pandascam-0.1.dist-info/License.txt
--rw-rw-rw-  2.0 fat      364 b- defN 23-Apr-23 19:46 pandascam-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 19:46 pandascam-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-23 19:46 pandascam-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      464 b- defN 23-Apr-23 19:46 pandascam-0.1.dist-info/RECORD
-6 files, 6934 bytes uncompressed, 3046 bytes compressed:  56.1%
+Zip file size: 3894 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     5993 b- defN 23-Apr-24 18:20 pandascam/__init__.py
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-24 20:05 pandascam-0.2.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      364 b- defN 23-Apr-24 20:05 pandascam-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 20:05 pandascam-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-24 20:05 pandascam-0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      464 b- defN 23-Apr-24 20:05 pandascam-0.2.dist-info/RECORD
+6 files, 6930 bytes uncompressed, 3048 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pandascam/__init__.py
 Comment: 
 
-Filename: pandascam-0.1.dist-info/License.txt
+Filename: pandascam-0.2.dist-info/License.txt
 Comment: 
 
-Filename: pandascam-0.1.dist-info/METADATA
+Filename: pandascam-0.2.dist-info/METADATA
 Comment: 
 
-Filename: pandascam-0.1.dist-info/WHEEL
+Filename: pandascam-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pandascam-0.1.dist-info/top_level.txt
+Filename: pandascam-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pandascam-0.1.dist-info/RECORD
+Filename: pandascam-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pandascam/__init__.py

```diff
@@ -130,15 +130,15 @@
 #map reduce
     
 Text="" "MapReduce is a processing technique and a program model for distributed
 computing based on java. The MapReduce algorithm contains two important tasks, namely
 Map and Reduce.
 "" "
 # Cleaning text and lower casing all words
-for char in '-.,\n':
+for char in '-.,"\n"':
         Text=Text.replace(char,' ')
 Text = Text.lower()
 # split returns a list of words delimited by sequences of whitespace(including tabs, newlines, etc, like re's \s)
 word_list = Text.split()
 from collections import Counter
 Counter(word_list).most_common()
 # Initializing Dictionary
@@ -167,17 +167,16 @@
 soup = BeautifulSoup(res,'lxml')
 states=[]
 for items in soup.find('table', class_='wikitable').find_all('tr')[1::1]:
     data = items.find_all(['th','td'])
     #print(data[0].text)
     states.append(data[0].text)
     print(states)
-
     
-    """)
+""")
 
 def pr10():
     print(""" 
 #parse xml text
 
 xml file code :
 <?xml version="1.0" encoding="UTF-8" standalone="no"?>
```

