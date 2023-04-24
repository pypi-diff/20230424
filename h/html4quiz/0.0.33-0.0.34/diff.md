# Comparing `tmp/html4quiz-0.0.33.tar.gz` & `tmp/html4quiz-0.0.34.tar.gz`

## Comparing `html4quiz-0.0.33.tar` & `html4quiz-0.0.34.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 html4quiz-0.0.33/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.33/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.33/src/html4quiz/_common.py
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.33/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.33/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.33/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.33/LICENSE.txt
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 html4quiz-0.0.33/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.33/pyproject.toml
--rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 html4quiz-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 html4quiz-0.0.34/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.34/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.34/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    29328 2020-02-02 00:00:00.000000 html4quiz-0.0.34/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.34/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.34/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.34/LICENSE.txt
+-rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 html4quiz-0.0.34/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 html4quiz-0.0.34/PKG-INFO
```

### Comparing `html4quiz-0.0.33/updatePackage.txt` & `html4quiz-0.0.34/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.33/src/html4quiz/_common.py` & `html4quiz-0.0.34/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.33/src/html4quiz/_generateEm.py` & `html4quiz-0.0.34/src/html4quiz/_generateEm.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,62 +97,79 @@
         if not self.QGs or not self.STDs: return
         
         if self.Flag4Preview:
             for std, v in self.Sheets.items():
                 tmp=[]
                 for seed, j in zip(v['seed'], v['orders']):
                     out=self.getQA(self.QGs[std], j, seed, self.resources) #<--- 아래와 차이, 2023.04-15 추가
-                    origAnswer=copy.deepcopy(out[1])
                     if out[0] is None:
                         print(std, out, self.QGs[cat][name].Name, '????---Try again!')
                         self.Sheets.clear()
                         return
 
-                    if self.QGs[std][-1] == 'python':
-                        tmp.append(out)
-                    elif isinstance(out[1], (int, float)) and self.Flag4Choice:
-                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
-                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
-                        tmp.append(out)
-                    elif isinstance(out[1], dict) and 'choices' in out[1]:
-                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
-                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
-                        tmp.append(out)
-                    else:
-                        tmp.append(out)
+##                    if self.QGs[std][-1] == 'python': #<--- 아래와 차이
+##                        tmp.append(out)
+##                    elif isinstance(out[1], (int, float)) and self.Flag4Choice:
+##                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
+##                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
+##                        tmp.append(out)
+##                    elif isinstance(out[1], dict) and 'choices' in out[1]:
+##                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
+##                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
+##                        tmp.append(out)
+##                    else:
+##                        tmp.append(out)
+                    tmp.append(self.out2out(self.QGs[std][-1], out))
 
                 v['Q&A'] = tmp
                 
         else:
             for std, v in self.Sheets.items():
                 tmp=[]
                 for seed, j in zip(v['seed'], v['orders']):
                     out=self.getQA(self.QGs[j], -1, seed, self.resources) #<--- 위와 차이, 2023.04-15 추가
-                    origAnswer=copy.deepcopy(out[1])
                     if out[0] is None:
                         print(std, out, self.QGs[cat][name].Name, '????---Try again!')
                         self.Sheets.clear()
                         return
 
-                    if self.QGs[j][-1] == 'python':
-                        tmp.append(out)
-                    elif isinstance(out[1], (int, float)) and self.Flag4Choice:
-                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
-                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
-                        tmp.append(out)
-                    elif isinstance(out[1], dict) and 'choices' in out[1]: # and isinstance(out[1]['ans'], (int, float)):
-                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
-                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
-                        tmp.append(out)
-                    else:
-                        tmp.append(out)
+##                    if self.QGs[j][-1] == 'python': #<--- 위와 차이
+##                        tmp.append(out)
+##                    elif isinstance(out[1], (int, float)) and self.Flag4Choice:
+##                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
+##                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
+##                        tmp.append(out)
+##                    elif isinstance(out[1], dict) and 'choices' in out[1]:
+##                        xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
+##                        out = (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
+##                        tmp.append(out)
+##                    else:
+##                        tmp.append(out)
+                    tmp.append(self.out2out(self.QGs[j][-1], out))
 
                 v['Q&A'] = tmp
 
 
+    def out2out(self, qType, out):
+        if qType == 'python':
+            return out
+        elif isinstance(out[1], (int, float)) and self.Flag4Choice:
+            origAnswer=copy.deepcopy(out[1])
+            xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
+            return (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
+        elif isinstance(out[1], dict) and 'choices' in out[1]:
+            origAnswer=copy.deepcopy(out[1])
+            xtra, ansChoice, ans, choicesUsed = generateChoices(out[1])
+            return (out[0]+xtra, int(ansChoice), out[-1], (origAnswer, choicesUsed))
+        else:
+            return out
+        
+
+
+
     def getAnswers(self):
         return {std:[item[1] for item in v['Q&A']] for std,v in self.Sheets.items()}
 
 
     def saveWork(self):
         if self.Flag4Preview:
             print("'Preview' flag is True, ignoring calls to saveWork(). Change the Flag4Preview to False and try again")
@@ -342,19 +359,19 @@
 ##                if itemStripped:
 ##                    figObjts.append(itemStripped)
 ##                    txt=txt.replace(f'FIG%{item}%FIG', '')
 ##
         if 'figure(' in txt: # 한 번 만든 것.. 직접 변경 불가능..
             for item in re.findall(figurePattern, txt):
                 figureKey=item.strip()
-                if figureKey and figureKey in resources:
+                if figureKey and figureKey in resources and resources[figureKey] and resources[figureKey] != 'HTTP Error 404: Not Found':
                     figObjts.append(resources[figureKey])
                     txt=txt.replace(f'figure({item})','')
                 else:
-                    txt=txt.replace(f'figure({item})',f'figure({item}):Error of not finding it')        
+                    txt=txt.replace(f'figure({item})',f'figure({item}):<font color="#dd0000">HTTP Error 404: Not Found</font>')
 
         txt=txt.replace("'", "&#39;") # 2022.08.07 둘다 사용하지 않는 것으로...
 
         if 'chr(9)' in txt:
             txt=txt.replace('chr(9)','&nbsp;&nbsp;&nbsp;&nbsp;')
 
         if 'EQ%' in txt:
@@ -364,15 +381,15 @@
             txt=txt.replace('\\', '\\\\')
 
         if str2bUsed:
             for j, obj in enumerate(figObjts):
                 if '//init();' in obj:
                     figObjts[j] = obj.replace('//init();', str2bUsed)
 
-        txt = f'<p><font color=red><strong>{qJ+1}.</strong></font> '+txt
+        txt = f'<p><font color="#dd0000"><strong>{qJ+1}.</strong></font> '+txt
         #indx = txt.find('<form')
         indx = txt.find('<div> ')  # 반드시 makeChoices._ChoicesWithRadiobuttons() 와 맞춰야 함....
         if indx == -1:
             txt += '</p>'
         else:
             txt = txt[:indx]+'</p>'+txt[indx:]
 
@@ -449,41 +466,62 @@
 <body oncontextmenu="return false">
 <center><h4>TITLE</h4></center>'''
 
 templateBodyR='''<hr> <div id="Qs" style="word-break:keep-all; display: block; font-family: malgun; font-size: 18px; margin: 0px 10px 0px 10px; padding: 0px 5px 0px 5px;"></div>
 <canvas id="canvas" width="800" height="0"></canvas>
 '''
 
+# backtick `    python의 '''와 동일
 templateF='''function display_QqNUM() {
+document.getElementById("Qs").innerHTML=`TEXT`;
+Qnumber = qNUM;
+prmtrQ = qNUM;
+setCheckedRadio(qNUM);
+
+var cnvs = document.getElementById("canvas");
+var ctx = cnvs.getContext("2d");
+ctx.clearRect(0,0, cnvs.width, cnvs.height);
+JS_CODE
+}
+'''
+
+
+templateF_000='''function display_QqNUM() {
 document.getElementById("Qs").innerHTML='TEXT';
 Qnumber = qNUM;
+prmtrQ = qNUM;
 setCheckedRadio(qNUM);
 
 var cnvs = document.getElementById("canvas");
 var ctx = cnvs.getContext("2d");
 ctx.clearRect(0,0, cnvs.width, cnvs.height);
 JS_CODE
 }
 '''
 
+
+
+
 templateEnd='''
 document.onkeydown = function (e) {
   if (e.altKey && e.keyCode == 39) {
     Qnumber += 1;
     if (Qnumber>Qmax) {Qnumber = 0};
     eval("display_Q"+Qnumber+"()");}
   else if (e.altKey && e.keyCode == 37) {
     Qnumber -= 1;
     if (Qnumber<0) {Qnumber = Qmax};
     eval("display_Q"+Qnumber+"()");}
 }
 var Qnumber = 0;
 var Qmax = QMAX;
 var answers = [];
-for (let j=0; j<=Qmax; j++) {answers.push(null);}
+var prmtrs = [];
+var prmtrQ = null;
+for (let j=0; j<=Qmax; j++) {answers.push(null);prmtrs.push(null);}
 
 display_Q0();</script>\n</body>\n</html>
 '''
 
 templateTable='''<ul style="font-size: 14px">
 <li>객관식 질문의 답은 정수로 답하시오. For multiple-choice questions, answer with an integer.</li>
 <li>단답형 질문의 숫자 답은, 가장 중요한 3개의 숫자로 반올림하시오. For numerical answer to short questions, round to the three most significant digits.</li>
@@ -534,14 +572,15 @@
 
 function setCheckedRadio(q) {
   var radios = document.getElementsByName('Q'+q.toString());
   //for (let j=0; j<radios.length; j++) {radios[j].removeAttribute("checked");}
   if (radios.length > 0 && answers[q] != null) {radios[answers[q]-1].setAttribute("checked", true);}
 }
 
+
 function destroyClickedElement(event) {
     document.body.removeChild(event.target);
 }
 </script>
 '''
```

### Comparing `html4quiz-0.0.33/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.34/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.33/src/html4quiz/makeChoices.py` & `html4quiz-0.0.34/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.33/LICENSE.txt` & `html4quiz-0.0.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.33/README.md` & `html4quiz-0.0.34/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 html4quiz is a package that helps you generate question sheets with as many HTML files as you want and grade answers from text files submitted by students.
 
 ## Features
 <ul>
 <li><strong>Local</strong>: Everything is on your local PC, grows with your creativity, and you own everything, unlike the many quiz generators available online.</li>
 <li><strong>HTML files</strong>: Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
-<ul><li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
-<li>Saving answers to a file can be repeated as many times as desired.</li></ul>
+<ul><li>Each HTML file is complete in itself with everything included.</li>
+<li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
+<li>Answers can be changed, and saving answers to a text file can be repeated as many times as desired until the file is submitted.</li></ul>
 <li><strong>Easy grading</strong>: Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
 <li><strong>Two kinds of HTML files</strong></li>
 <ol><li>First kind is to preview questions before generating sheets.</li>
 <li>Second kind is the set of sheets.</li></ol>
 <li><strong>Two kinds of questions</strong></li>
 <ol><li>Short answr questions of requiring a number of a word.</li>
-<li>Multiple choice questions whose choices are genterated randomly by one of various methods or by Python coding.</li></ol>
+<li>Multiple choice questions whose choices are genterated randomly by one of various methods or by Python coding.</li>
+<li>A third type of question that can be answered by a <strong>"game" simulation</strong> will be available in the near future.</li></ol>
 <li><strong>Figures</strong> as well as <strong>mathematical expressions</strong> in LaTeX format can be included in both question texts and choices.</li>
 <li><strong>Randomness</strong> is controlled completely by users with Python scripts.</li>
 <li><strong>Easy correction</strong>: When some answers are found incorrect after question sheets are distributed, the answers can be corrected by simply re-generate the sheets with the "work" pickle file (refer to Version 0.0.29). </li></ul>
 
 
 ## Where to get it
 
@@ -29,16 +31,20 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
+<li>Version 0.0.34</li>
+<ul><li>Third kind question is added (refer to Ex005).</li></ul>
+<br>
+
 <li>Version 0.0.33</li>
-<ul><li>A small re-recoding is done.</li></ul>
+<ul><li>A small re-coding is done.</li></ul>
 <br>
 
 <li>Version 0.0.30</li>
 <ul><li>In addition to using a user-defined function for answers, a new way to use resources saved in <a href="https://github.com/generateNscore/html4quiz/tree/main/res">html4quiz/res</a> is added.</li>
 <li>For details, please look at <a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004.py">Ex004.py</a></li>
 <li><a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004/Ex004/index.html">Previews</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -2,41 +2,48 @@
 question sheets with as many HTML files as you want and grade answers from text
 files submitted by students. ## Features
     * Local: Everything is on your local PC, grows with your creativity, and
       you own everything, unlike the many quiz generators available online.
     * HTML files: Question sheets in HTML files, each named with a
       corresponding identification number, are distributed to students over the
       network.
+          o Each HTML file is complete in itself with everything included.
           o Students use their mobile devices to read, answer questions, save
             answers to a text file for submission within the same HTML page,
             and submit the text file as directed over the network.
-          o Saving answers to a file can be repeated as many times as desired.
+          o Answers can be changed, and saving answers to a text file can be
+            repeated as many times as desired until the file is submitted.
     * Easy grading: Grade answers in text files submitted by all students can
       be achieved with a few keystrokes.
     * Two kinds of HTML files
          1. First kind is to preview questions before generating sheets.
          2. Second kind is the set of sheets.
     * Two kinds of questions
          1. Short answr questions of requiring a number of a word.
          2. Multiple choice questions whose choices are genterated randomly by
             one of various methods or by Python coding.
+         3. A third type of question that can be answered by a "game"
+            simulation will be available in the near future.
     * Figures as well as mathematical expressions in LaTeX format can be
       included in both question texts and choices.
     * Randomness is controlled completely by users with Python scripts.
     * Easy correction: When some answers are found incorrect after question
       sheets are distributed, the answers can be corrected by simply re-
       generate the sheets with the "work" pickle file (refer to Version
       0.0.29).
 ## Where to get it
 pip install html4quiz
 ## Dependencies
     * None
 ## Changes
+    * Version 0.0.34
+          o Third kind question is added (refer to Ex005).
+    *
     * Version 0.0.33
-          o A small re-recoding is done.
+          o A small re-coding is done.
     *
     * Version 0.0.30
           o In addition to using a user-defined function for answers, a new way
             to use resources saved in html4quiz/res is added.
           o For details, please look at Ex004.py
           o Previews
     *
```

### Comparing `html4quiz-0.0.33/pyproject.toml` & `html4quiz-0.0.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.33"
+version = "0.0.34"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.33/PKG-INFO` & `html4quiz-0.0.34/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.33
+Version: 0.0.34
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -23,23 +23,25 @@
 
 html4quiz is a package that helps you generate question sheets with as many HTML files as you want and grade answers from text files submitted by students.
 
 ## Features
 <ul>
 <li><strong>Local</strong>: Everything is on your local PC, grows with your creativity, and you own everything, unlike the many quiz generators available online.</li>
 <li><strong>HTML files</strong>: Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
-<ul><li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
-<li>Saving answers to a file can be repeated as many times as desired.</li></ul>
+<ul><li>Each HTML file is complete in itself with everything included.</li>
+<li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
+<li>Answers can be changed, and saving answers to a text file can be repeated as many times as desired until the file is submitted.</li></ul>
 <li><strong>Easy grading</strong>: Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
 <li><strong>Two kinds of HTML files</strong></li>
 <ol><li>First kind is to preview questions before generating sheets.</li>
 <li>Second kind is the set of sheets.</li></ol>
 <li><strong>Two kinds of questions</strong></li>
 <ol><li>Short answr questions of requiring a number of a word.</li>
-<li>Multiple choice questions whose choices are genterated randomly by one of various methods or by Python coding.</li></ol>
+<li>Multiple choice questions whose choices are genterated randomly by one of various methods or by Python coding.</li>
+<li>A third type of question that can be answered by a <strong>"game" simulation</strong> will be available in the near future.</li></ol>
 <li><strong>Figures</strong> as well as <strong>mathematical expressions</strong> in LaTeX format can be included in both question texts and choices.</li>
 <li><strong>Randomness</strong> is controlled completely by users with Python scripts.</li>
 <li><strong>Easy correction</strong>: When some answers are found incorrect after question sheets are distributed, the answers can be corrected by simply re-generate the sheets with the "work" pickle file (refer to Version 0.0.29). </li></ul>
 
 
 ## Where to get it
 
@@ -48,16 +50,20 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
+<li>Version 0.0.34</li>
+<ul><li>Third kind question is added (refer to Ex005).</li></ul>
+<br>
+
 <li>Version 0.0.33</li>
-<ul><li>A small re-recoding is done.</li></ul>
+<ul><li>A small re-coding is done.</li></ul>
 <br>
 
 <li>Version 0.0.30</li>
 <ul><li>In addition to using a user-defined function for answers, a new way to use resources saved in <a href="https://github.com/generateNscore/html4quiz/tree/main/res">html4quiz/res</a> is added.</li>
 <li>For details, please look at <a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004.py">Ex004.py</a></li>
 <li><a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004/Ex004/index.html">Previews</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.33 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.34 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
 github.com/generateNscore/html4quiz/wiki Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
@@ -13,41 +13,48 @@
 a package that helps you generate question sheets with as many HTML files as
 you want and grade answers from text files submitted by students. ## Features
     * Local: Everything is on your local PC, grows with your creativity, and
       you own everything, unlike the many quiz generators available online.
     * HTML files: Question sheets in HTML files, each named with a
       corresponding identification number, are distributed to students over the
       network.
+          o Each HTML file is complete in itself with everything included.
           o Students use their mobile devices to read, answer questions, save
             answers to a text file for submission within the same HTML page,
             and submit the text file as directed over the network.
-          o Saving answers to a file can be repeated as many times as desired.
+          o Answers can be changed, and saving answers to a text file can be
+            repeated as many times as desired until the file is submitted.
     * Easy grading: Grade answers in text files submitted by all students can
       be achieved with a few keystrokes.
     * Two kinds of HTML files
          1. First kind is to preview questions before generating sheets.
          2. Second kind is the set of sheets.
     * Two kinds of questions
          1. Short answr questions of requiring a number of a word.
          2. Multiple choice questions whose choices are genterated randomly by
             one of various methods or by Python coding.
+         3. A third type of question that can be answered by a "game"
+            simulation will be available in the near future.
     * Figures as well as mathematical expressions in LaTeX format can be
       included in both question texts and choices.
     * Randomness is controlled completely by users with Python scripts.
     * Easy correction: When some answers are found incorrect after question
       sheets are distributed, the answers can be corrected by simply re-
       generate the sheets with the "work" pickle file (refer to Version
       0.0.29).
 ## Where to get it
 pip install html4quiz
 ## Dependencies
     * None
 ## Changes
+    * Version 0.0.34
+          o Third kind question is added (refer to Ex005).
+    *
     * Version 0.0.33
-          o A small re-recoding is done.
+          o A small re-coding is done.
     *
     * Version 0.0.30
           o In addition to using a user-defined function for answers, a new way
             to use resources saved in html4quiz/res is added.
           o For details, please look at Ex004.py
           o Previews
     *
```

