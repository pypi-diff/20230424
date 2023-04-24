# Comparing `tmp/sara_compis1_tools-0.0.6.tar.gz` & `tmp/sara_compis1_tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.6.tar", last modified: Thu Apr 20 00:11:06 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.7.tar", last modified: Mon Apr 24 05:46:04 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.6.tar` & `sara_compis1_tools-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 00:11:06.188101 sara_compis1_tools-0.0.6/
--rw-rw-rw-   0        0        0      215 2023-04-20 00:02:21.000000 sara_compis1_tools-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-04-20 00:11:06.186531 sara_compis1_tools-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/README.txt
--rw-rw-rw-   0        0        0     1441 2023-04-19 23:26:29.000000 sara_compis1_tools-0.0.6/generated.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:11:06.161867 sara_compis1_tools-0.0.6/sara_compis1_tools/
--rw-rw-rw-   0        0        0     6072 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      255 2023-04-19 23:59:19.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0     1167 2023-04-19 20:23:20.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/Visualizer.py
--rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0     1618 2023-04-20 00:00:07.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/generated.py
--rw-rw-rw-   0        0        0    14271 2023-04-20 00:00:00.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/lexGen.py
--rw-rw-rw-   0        0        0     1937 2023-04-20 00:05:56.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/stateafd_objects.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:11:06.181465 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      829 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-04-20 00:11:06.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 00:11:06.188101 sara_compis1_tools-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-04-20 00:02:31.000000 sara_compis1_tools-0.0.6/setup.py
--rw-rw-rw-   0        0        0     1948 2023-04-19 18:13:23.000000 sara_compis1_tools-0.0.6/stateafd_objects.py
+drwxrwxrwx   0        0        0        0 2023-04-24 05:46:04.363636 sara_compis1_tools-0.0.7/
+-rw-rw-rw-   0        0        0      303 2023-04-24 05:36:05.000000 sara_compis1_tools-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      904 2023-04-24 05:46:04.358351 sara_compis1_tools-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 05:46:04.317601 sara_compis1_tools-0.0.7/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     4483 2023-04-24 01:35:25.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/AFD_tools.py
+-rw-rw-rw-   0        0        0      155 2023-04-23 15:56:11.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Error.py
+-rw-rw-rw-   0        0        0     6092 2023-04-24 03:38:02.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      263 2023-04-21 02:28:08.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0     1385 2023-04-23 04:32:41.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Visualizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0     7598 2023-04-24 05:29:24.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/generated.py
+-rw-rw-rw-   0        0        0    10130 2023-04-24 05:10:59.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/lexEval.py
+-rw-rw-rw-   0        0        0    17009 2023-04-24 05:33:59.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/lexGen.py
+drwxrwxrwx   0        0        0        0 2023-04-24 05:46:04.351861 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-04-24 05:46:04.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 05:46:04.363636 sara_compis1_tools-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-04-24 05:36:28.000000 sara_compis1_tools-0.0.7/setup.py
```

### Comparing `sara_compis1_tools-0.0.6/LICENSE.txt` & `sara_compis1_tools-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.6/PKG-INFO` & `sara_compis1_tools-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara_compis1_tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
@@ -25,7 +25,11 @@
 0.0.5 (19/04/2023)
 ------------------
 - Rearranging packages.
 
 0.0.6 (19/04/2023)
 ------------------
 - More fields for the StateAFD class.
+
+0.0.7 (23/04/2023)
+------------------
+- Additions for AFN simulation.
```

### Comparing `sara_compis1_tools-0.0.6/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.7/sara_compis1_tools/Format.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,22 +113,22 @@
                     val = regexx[i + 1]
                     val = str(ord(val))
                     if len(val) == 2:
                         val = '0' + val
                     elif len(val) == 1:
                         val = '00' + val
                     i += 2
-                elif val.isalnum() or val in ["#", '_']:
+                elif val.isalnum() or val in ["#", '_', '^', '"']:
                     val = str(ord(val))
                     if len(val) == 2:
                         val = '0' + val
                     elif len(val) == 1:
                         val = '00' + val
 
-            elif regexx[i].isalnum() or regexx[i] in ['#', '_']:
+            elif regexx[i].isalnum() or regexx[i] in ['#', '_', '^', '"']:
                 val = str(ord(val)) 
                 if len(val) == 2:
                     val = '0' + val
                 elif len(val) == 1:
                     val = '00' + val
                     
             if i + 1 < len(regexx):
```

### Comparing `sara_compis1_tools-0.0.6/sara_compis1_tools/Syntax.py` & `sara_compis1_tools-0.0.7/sara_compis1_tools/Syntax.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.6/sara_compis1_tools/Visualizer.py` & `sara_compis1_tools-0.0.7/sara_compis1_tools/Visualizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,16 +15,23 @@
             if state.accepting:
                 node_attrs.update({'peripheries': '2'})
             G.add_node(str(state.name), **node_attrs)
 
             for transition, final_dest in state.transitions.items():
                 G.add_node(str(final_dest))
                 
-                if int(transition) not in [el for el in range(0, 35)]:
-                    transition = str(chr(int(transition)))
+                if ord(transition) in [el for el in range(0, 35)]:
+                    transition = str(ord(transition))
+
+                    if len(transition) == 1:
+                        transition = '00' + transition
+                    elif len(transition) == 2:
+                        transition = '0' + transition
+
+                
 
                 G.add_edge(str(state.name), str(final_dest), label=transition, dir='forward')    
 
         dot = Digraph()
         for u, v, data in G.edges(data=True):
             dot.edge(u, v, label=data['label'], dir=data['dir'])
         for node in G.nodes:
```

### Comparing `sara_compis1_tools-0.0.6/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.7/sara_compis1_tools/directAFD.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.6/sara_compis1_tools/lexGen.py` & `sara_compis1_tools-0.0.7/sara_compis1_tools/lexGen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,75 @@
 from Format import Format
 from directAFD import AFD
 from StateAFD import StateAFD
-
+from Error import Error
 import sys
 
 
 class Token:
         def __init__(self, name):
             self.name = name
             self.regex = None
             self.line_no = None
             self.value = None
     
         def __str__(self):
             return f"Token({self.name}, {self.regex})"
 
 
+class ruleLine:
+    def __init__(self, line_no, line):
+        self.line_no = line_no
+        self.line = line
+
+
 class Lexer:
     def __init__(self, filename):
         self.filename = filename
         self.tokens = []
         self.tokenizer = None
 
     
     def remove_spaces(self, lines):
         wo_spaces = []
-        # Si hay comillas dobles reemplazar por simples
-        for i in range(len(lines)):
-            lines[i] = lines[i].replace('"', "'")
-
         for line in lines:
             new_line = []
             between_q = False
             for char in line:
                 if char == "'":
                     between_q = not between_q
                 if char != " " or between_q:
                     new_line.append(char)
             wo_spaces.append("".join(new_line))
         return wo_spaces
+    
+
+    def clean_comments(self, joined):
+        for index, line in enumerate(joined):
+            line_wo_comment = ''
+            i = 0
+            while i < len(line):
+                if i < len(line) - 1 and line[i] == '(' and line[i + 1] == '*':
+                    while i < len(line) - 1 and (line[i] != '*' or line[i + 1] != ')'):
+                        i += 1
+                    i += 2
+                else:
+                    line_wo_comment += line[i]
+                    i += 1
+            joined[index] = line_wo_comment
+        return joined
 
 
-    def getLines(self):
+    def getLines(self, tokens_mode):
         f = open(self.filename, "r", encoding="utf-8")
         lines = f.readlines()
         f.close()
-
-        lines = [line.encode('utf-8').decode('unicode_escape') for line in lines]
+        
+        if tokens_mode:
+            lines = [line.encode('utf-8').decode('unicode_escape') for line in lines]
 
         lines_with_n = [n[:-1] for n in lines]
         check_comments = [lll.split(' ') for lll in lines_with_n]  
 
         joined = [' '.join(line) for line in check_comments]
         # Revision de errores en comentarios
         for line_no, lj in enumerate(joined, start=1):
@@ -64,30 +83,17 @@
                     if comments_stack and comments_stack[-1] == '(*':
                         comments_stack.pop()
                     else:
                         raise Exception(f"Error en comentario, linea {line_no}")
             if comments_stack:
                 raise Exception(f"Error en comentario, linea {line_no}")
 
-
-        for index, line in enumerate(joined):
-            line_wo_comment = ''
-            i = 0
-            while i < len(line):
-                if i < len(line) - 1 and line[i] == '(' and line[i + 1] == '*':
-                    while i < len(line) - 1 and (line[i] != '*' or line[i + 1] != ')'):
-                        i += 1
-                    i += 2
-                else:
-                    line_wo_comment += line[i]
-                    i += 1
-            joined[index] = line_wo_comment
+        joined = self.clean_comments(joined)
             
-
-        return (self.remove_spaces(joined), joined)
+        return joined
     
 
     def special_split(self, text, delimiter):
         result = []
         start = 0
         open_curly_b = 0
 
@@ -112,51 +118,63 @@
                     for element in line:
                         if element == '':
                             line.pop(line.index(element))
         return lines
     
 
     def assign_values(self):
-        splits = [self.special_split(line, ' ') for line in self.getLines()[1]]
+        splits = [self.special_split(line, ' ') for line in self.getLines(tokens_mode=False)]
         splits = self.remove_spaces_list(splits)
         
         start = 0
-        for indx, line in enumerate(splits):
+        rules_lines = []
+        for indx, line in enumerate(splits, start=1):
             if line[0] == 'rule':
                 start = indx + 1
+            if start:
+                rules_lines.append(ruleLine(indx, line))
+
         
-        if start:
-            rules = ''.join([''.join([word.replace('\t', '') for word in line]) for line in splits[start:]]).split('|')
+        if len(rules_lines) > 1:
+
+            rules_lines = rules_lines[1:]
+            for rule in rules_lines:
+                if rule.line[0] == '|':
+                    rule.line.pop(0)
+                if len(rule.line) == 1:
+                    rule.line = rule.line[0]
+
             rules_dict = {}
-            for rule in rules:
+            for rule in rules_lines:
                 name = ''
                 value = ''
                 inside = False
 
-                for i in range(len(rule)):
-                    if rule[i] == '{':
+                for i in range(len(rule.line)):
+                    if rule.line[i] == '{':
                         inside = True
                         continue
 
-                    if rule[i] == '}':
+                    if rule.line[i] == '}':
                         inside = False
                         continue
 
                     if not inside:
-                        name += rule[i]
+                        if rule.line[i] not in ['\t', ' ']:
+                            name += rule.line[i]
                     else:
-                        value += rule[i]
+                        value += rule.line[i]
 
                 if name:
-                    rules_dict[name] = value.strip()
+                    rules_dict[name] = (ruleLine(rule.line_no, value.strip()))
         return rules_dict
 
 
     def getTokens(self):
-        lines = self.getLines()[0]
+        lines = self.remove_spaces(self.getLines(tokens_mode=True))
         for line_no, line in enumerate(lines, start=1):
             # generando tokens
             if line[:3] == 'let':
                 name, regex = line[3:].split('=')
                 token = Token(name)
                 token.regex = regex
                 token.line_no = line_no
@@ -185,14 +203,21 @@
 
     
     def change_range_format(self):
         tokens = self.tokens
         for token in tokens:
             new_regex = ''
             i = 0
+
+            if token.regex[0] == "'" and token.regex[-1] == "'" and token.regex.count("'") == 2:
+                unquoted_token = token.regex[1:-1]
+                token.regex = f'({unquoted_token})'
+                continue
+            
+
             while i < len(token.regex):
 
                 p_left = token.regex.count("(")
                 p_right = token.regex.count(")")
                 if (p_left + p_right) % 2 != 0:
                     raise Exception("Error: Los parentesis no estan balanceados, "+ "linea " + str(token.line_no))
                 
@@ -239,27 +264,29 @@
                             elements = [content[i] for i in range(len(content))]
                             content = '|'.join(elements)
                     new_regex += '(' + content + ')'
                     i = j
                 else:
                     check = ""
                     j = i
-                    while token.regex[j] not in ['+', '*', '?']:
+                    while token.regex[j] not in ['+', '*', '?', '(', ')', '[', ']']:
                         check += token.regex[j]
                         j += 1
                     keys = [tk.name for tk in tokens]
                     if check in keys:
                         i = j - 1
                         new_regex += check
                     else:
                         new_regex += token.regex[i]
                 i += 1
 
             count_all = int((new_regex.count('(') + new_regex.count(')')) /2)
             if not count_all or new_regex[-1] in ['+', '*', '?']:
+                if  new_regex[0] == "'" and new_regex[-1] == "'":
+                    new_regex = new_regex[1:-1]
                 new_regex = f'({new_regex})'
 
             token.regex = new_regex
 
 
     def replace_tokens(self):
         for tk in self.tokens:
@@ -313,44 +340,58 @@
 
     
     def generate_automatas(self):
         mega_content = []
         count = 0
         return_values = self.assign_values()
         done = []
+        errors = set()
         for token in self.tokens:
             if token.name in return_values:
                 ff = Format(token.regex)
                 token.regex = ff.positiveId(token.regex + '#')
                 token.regex = ff.zeroOrOneId(token.regex)
                 token.regex = self.remove_double_parentheses(token.regex)
                 token.regex = ff.concat(token.regex)
                 token.value = return_values[token.name]
                 done.append(token.name)
                 
                 afdd = AFD(token)
                 new_afd = afdd.generateAFD(count)
+                for elem in new_afd:
+                    if elem.accepting:
+                        elem.value = token.value
+
                 mega_content.append(new_afd)
                 count += len(new_afd)
 
+        for rt, rt_val in return_values.items():
+            if rt not in [tk.name for tk in self.tokens]:
+                if rt[0] != "'" and rt[-1] != "'":
+                    errors.add(Error(line=rt_val.line_no, error="Error: Token no definido: " + rt))
+
         for value in return_values:
-            if len(value) == 3 and value[0] == "'" and value[2] == "'" and value not in done:
+            if value[0] == "'" and value[-1] == "'" and value not in done:
                 lenn = len(value)
                 token = Token(name=value[1:-1])
                 token.regex = value + '#'
                 token.value = return_values[value]
                 ff = Format(token.regex)
                 token.regex = ff.concat(token.regex)
                 done.append(token.name)
                 
                 afdd = AFD(token)
                 new_afd = afdd.generateAFD(count)
+                for elem in new_afd:
+                    if elem.accepting:
+                        elem.value = token.value
+
                 mega_content.append(new_afd)
                 count += len(new_afd)
-        return mega_content
+        return mega_content, errors
     
 
     def unify(self, mega_content):
         stack = []    
         for element in mega_content:
             for state in element:
                 if state.start:
@@ -366,37 +407,65 @@
         self.assign_values()
         self.getTokens()
         self.change_range_format()
         self.surround_dot()
         self.replace_tokens()
     
 
+    def change_values(self, mega_automata):
+        for state in mega_automata:
+            updates = {str(chr(int(key))): state.transitions.pop(key) for key in list(state.transitions.keys())}
+            state.transitions.update(updates)
+
 
     
 if __name__ == '__main__':
 
-    # if len(sys.argv) < 2:
-    #     print("Por favor ingrese el archivo .yal")
-    #     sys.exit(1)
+    if len(sys.argv) < 2:
+        print("Por favor ingrese el archivo .yal")
+        sys.exit(1)
 
-    # yal_file = sys.argv[1]
-    yal_file = "p1.yal"
+    yal_file = sys.argv[1]
     lexer = Lexer(yal_file)
     
     lexer.read()
-    mega_content = lexer.generate_automatas()
+    mega_content, errors = lexer.generate_automatas()
     mega_automata = lexer.unify(mega_content)
+    lexer.change_values(mega_automata)
 
-    with open('generated.py', 'w') as file:
+    with open('generated.py', 'w', encoding="utf-8") as file:
         file.write("from sara_compis1_tools.StateAFD import StateAFD\n")
-        file.write("from sara_compis1_tools.Visualizer import Visualizer\n\n")
+        file.write("from lexEval import LexEval\n")
+        file.write("from Error import Error\n")
+        file.write("import sys\n\n")
         file.write("mega = [")
         for i, obj in enumerate(mega_automata):
-            file.write(f"StateAFD(name='{obj.name}',transitions={obj.transitions},accepting={obj.accepting},start={obj.start}, value={obj.value})")
+            if obj.value:
+                value_str = repr(obj.value.line) if isinstance(obj.value.line, str) else str(obj.value.line)
+            else:
+                value_str = None
+            file.write(f"StateAFD(name='{obj.name}',transitions={obj.transitions},accepting={obj.accepting},start={obj.start}, value={value_str})")
             if i != len(mega_automata) - 1:
-                file.write(",") 
-        file.write("]\n\n")
+                file.write(",")
+        file.write("]\n")
 
-        file.write("visual = Visualizer()\n")
-        file.write("visual.draw_mega_afd(mega)")
-        
+        if errors:
+            file.write("errors = set([")
+            for i, error in enumerate(errors):
+                file.write(f"Error(line={error.line}, error='{error.error}')")
+                if i != len(errors) - 1:
+                    file.write(",")
+            file.write("])\n\n")
+        else:
+            file.write("errors = set()\n\n")
+
+        file.write("if len(sys.argv) < 2:\n\tprint('Por favor ingrese el archivo plano')\n\tsys.exit(1)\n")
+        file.write("txt_file = sys.argv[1]\n\n")
+        file.write("lex = LexEval(txt_file)\n")
+
+        file.write("results = lex.evaluate(mega, errors)\n")
+        file.write("lex.print_tokens(results)\n\n")
+
+        file.write("from Visualizer import Visualizer\n")
+        file.write("v = Visualizer()\n")
+        file.write("v.draw_mega_afd(mega)\n")
```

### Comparing `sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/PKG-INFO` & `sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara-compis1-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
@@ -25,7 +25,11 @@
 0.0.5 (19/04/2023)
 ------------------
 - Rearranging packages.
 
 0.0.6 (19/04/2023)
 ------------------
 - More fields for the StateAFD class.
+
+0.0.7 (23/04/2023)
+------------------
+- Additions for AFN simulation.
```

### Comparing `sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/SOURCES.txt` & `sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 CHANGELOG.txt
 LICENSE.txt
 MANIFEST.in
 README.txt
-generated.py
 setup.py
-stateafd_objects.py
+sara_compis1_tools/AFD_tools.py
+sara_compis1_tools/Error.py
 sara_compis1_tools/Format.py
 sara_compis1_tools/StateAFD.py
 sara_compis1_tools/Syntax.py
 sara_compis1_tools/Visualizer.py
 sara_compis1_tools/__init__.py
 sara_compis1_tools/directAFD.py
 sara_compis1_tools/generated.py
+sara_compis1_tools/lexEval.py
 sara_compis1_tools/lexGen.py
-sara_compis1_tools/stateafd_objects.py
 sara_compis1_tools.egg-info/PKG-INFO
 sara_compis1_tools.egg-info/SOURCES.txt
 sara_compis1_tools.egg-info/dependency_links.txt
 sara_compis1_tools.egg-info/requires.txt
 sara_compis1_tools.egg-info/top_level.txt
```

### Comparing `sara_compis1_tools-0.0.6/setup.py` & `sara_compis1_tools-0.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='sara_compis1_tools',
-    version='0.0.6',
-    description='A collection of tools for the Language Design course',
-    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
-    url='https://github.com/MGonza20/Compis_Lab4',
-    author='Sara Paguaga',
-    author_email='sara.paguaga@gmail.com',
-    license='MIT',
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3'
-    ],
-    keywords='Compiler',
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=[
-        'networkx',
-        'graphviz'
-    ]
+from setuptools import setup, find_packages
+
+setup(
+    name='sara_compis1_tools',
+    version='0.0.7',
+    description='A collection of tools for the Language Design course',
+    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
+    url='https://github.com/MGonza20/Compis_Lab4',
+    author='Sara Paguaga',
+    author_email='sara.paguaga@gmail.com',
+    license='MIT',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3'
+    ],
+    keywords='Compiler',
+    packages=find_packages(),
+    include_package_data=True,
+    install_requires=[
+        'networkx',
+        'graphviz'
+    ]
 )
```

