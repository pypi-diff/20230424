# Comparing `tmp/spccpkg-0.0.7.tar.gz` & `tmp/spccpkg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spccpkg-0.0.7.tar", last modified: Sun Apr 23 19:29:51 2023, max compression
+gzip compressed data, was "spccpkg-0.0.8.tar", last modified: Mon Apr 24 17:14:25 2023, max compression
```

## Comparing `spccpkg-0.0.7.tar` & `spccpkg-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 19:29:51.598322 spccpkg-0.0.7/
--rw-rw-rw-   0        0        0      451 2023-04-23 19:29:51.596326 spccpkg-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 19:29:51.599387 spccpkg-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-23 19:27:08.000000 spccpkg-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 19:29:51.505311 spccpkg-0.0.7/spcc/
--rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.7/spcc/__init__.py
--rw-rw-rw-   0        0        0    38396 2023-04-23 19:26:44.000000 spccpkg-0.0.7/spcc/code.py
-drwxrwxrwx   0        0        0        0 2023-04-23 19:29:51.588359 spccpkg-0.0.7/spccpkg.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-23 19:29:50.000000 spccpkg-0.0.7/spccpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-23 19:29:51.000000 spccpkg-0.0.7/spccpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 19:29:50.000000 spccpkg-0.0.7/spccpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 19:29:50.000000 spccpkg-0.0.7/spccpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:14:25.474378 spccpkg-0.0.8/
+-rw-rw-rw-   0        0        0      451 2023-04-24 17:14:25.473377 spccpkg-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:14:25.475377 spccpkg-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-24 17:12:43.000000 spccpkg-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:14:25.453380 spccpkg-0.0.8/spcc/
+-rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.8/spcc/__init__.py
+-rw-rw-rw-   0        0        0    43578 2023-04-24 17:12:36.000000 spccpkg-0.0.8/spcc/code.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:14:25.472375 spccpkg-0.0.8/spccpkg.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-24 17:14:25.000000 spccpkg-0.0.8/spccpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-24 17:14:25.000000 spccpkg-0.0.8/spccpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:14:25.000000 spccpkg-0.0.8/spccpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-24 17:14:25.000000 spccpkg-0.0.8/spccpkg.egg-info/top_level.txt
```

### Comparing `spccpkg-0.0.7/setup.py` & `spccpkg-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A basic hello package'
 
 # Setting up
 setup(
     name="spccpkg",
     version=VERSION,
     author="yashbrid03",
```

### Comparing `spccpkg-0.0.7/spcc/code.py` & `spccpkg-0.0.8/spcc/code.py`

 * *Files 5% similar despite different names*

```diff
@@ -1268,26 +1268,276 @@
                         card[j] = card[j]
                 print('\t'.join(card))
         else:  # Non-macro instruction
             print(line)
         '''
         print(string)
 
+    def nested():
+        strings = '''
+        nestedif.l
+        %{
+#include "y.tab.h"
+%}
+
+%%
+"if" {return IF;}
+[sS][0-9]* {return S;}
+"<"|">"|"=="|"<="|">="|"!=" {return RELOP;}
+[0-9]+ {return NUMBER;}
+[a-z][a-zA-Z0-9_]* {return ID;}
+\n {return NL;}
+. {return yytext[0];}
+%%
+
+
+nestedif.y
+
+%{
+#include<stdio.h>
+#include<stdlib.h>
+int count=0;
+%}
+
+%token IF RELOP S NUMBER ID NL
+
+%%
+stmt: if_stmt NL {printf("No. of nested if statements=%d\n",count);exit(0);}
+;
+if_stmt : IF'('cond')''{'if_stmt'}' {count++;}
+          |S
+;
+cond: x RELOP x 
+;
+x:ID | NUMBER
+;
+%%
+
+int yyerror(char *msg)
+{
+printf("the statement is invalid\n");
+exit(0);
+}
+main()
+{
+printf("enter the statement\n");
+yyparse();
+}
+int yywrap(){return(1);}
+        '''
+        print(strings)
+
+    def quad():
+        string = '''
+        Quadruples.y
+
+%{
+#include<stdio.h>
+#include<stdlib.h>
+#include<string.h>
+char * createT(); // Declaration for creating the temporary variables
+int tempcount=0; // Global variable to track the number of temporary variables
+%}
+%union { char str[30]; }
+// Redefining the datatype of yylval using union declaration, which is int by default
+%left '+'
+%left '-'
+%left '*'
+%left '/'
+%token <str> Var // Defining the datatype of Tokens as str
+%token <str> Num
+%type <str> s // Defining the datatypes of Non-Terminals
+%type <str> exp
+%%
+s : Var '=' exp {printf("\n \t%s \t\t%s\n",$1,$3);}
+exp : '(' exp ')' {strcpy($$,$2);}
+| exp '+' exp {strcpy($$,createT()); printf("\n+\t%s\t%s\t%s",$1,$3,$$);}
+| exp '-' exp {strcpy($$,createT()); printf("\n-\t%s\t%s\t%s",$1,$3,$$);}
+| exp '' exp {strcpy($$,createT()); printf("\n\t%s\t%s\t%s",$1,$3,$$);}
+| exp '/' exp {strcpy($$,createT()); printf("\n/\t%s\t%s\t%s",$1,$3,$$);}
+| Num {strcpy($$,$1);}
+| Var {strcpy($$,$1);}
+;
+%%
+char * createT()
+{
+char snum[30],*ptr; // Declaring the string array and pointer variable
+sprintf(snum,"t%d",tempcount); // Returning a formatted String
+ptr=snum; // Intializing the pointer with formatted string address
+tempcount++; // Temporary count
+return ptr; // Returning the pointer
+}
+int main()
+{
+yyparse();
+return 0;
+}
+int yyerror(char *err)
+{
+printf("\nInvlaid");
+exit(0);
+}
+
+
+Quadruples.l
+
+%{
+#include"y.tab.h"
+%}
+%%
+[a-zA-Z]+ {strcpy(yylval.str,yytext); return Var;}
+[0-9]+ {strcpy(yylval.str,yytext); return Num;}
+\n {return 0;}
+[ \t] {}
+. {return yytext[0];}
+%%
+int yywrap()
+{
+return 1;
+}Quadruples.l
+
+%{
+#include"y.tab.h"
+%}
+%%
+[a-zA-Z]+ {strcpy(yylval.str,yytext); return Var;}
+[0-9]+ {strcpy(yylval.str,yytext); return Num;}
+\n {return 0;}
+[ \t] {}
+. {return yytext[0];}
+%%
+int yywrap()
+{
+return 1;
+}
+        '''
+        print(string)
+
+    def adverb():
+        string = '''
+        Adverb.l
+
+%{
+#include <stdio.h>
+#include <string.h>
+int verb_count = 0;
+int adverb_count = 0;
+int adjective_count = 0;
+int noun_count = 0;
+%}
+
+%x verb_token
+%x adverb_token
+%x adjective_token
+%x noun_token
+
+%%
+
+"run"|"walk"|"jump"|"swim"|"fly"|"eat"|"drink"|"sleep"|"play"|"work" {
+    verb_count++;
+    BEGIN(verb_token);
+}
+
+"quickly"|"slowly"|"happily"|"angrily"|"carefully"|"loudly"|"softly"|"well"|"badly"|"hard" {
+    adverb_count++;
+    BEGIN(adverb_token);
+}
+"happy"|"sad"|"angry"|"excited"|"tired"|"strong"|"weak"|"big"|"small"|"fast" {
+    adjective_count++;
+    BEGIN(adjective_token);
+}
+"dog"|"cat"|"bird"|"car"|"house"|"tree"|"flower"|"book"|"pencil"|"computer" {
+    noun_count++;
+    BEGIN(noun_token);
+}
+<verb_token>.|\n { BEGIN(INITIAL); }
+<adverb_token>.|\n { BEGIN(INITIAL); }
+<adjective_token>.|\n { BEGIN(INITIAL); }
+<noun_token>.|\n { BEGIN(INITIAL); }
+%%
+int yywrap(){
+    return 1;
+}
+int main(int argc, char *argv[])
+{
+    yylex();
+    printf("Number of verbs: %d\nNumber of adverbs: %d\nNumber of adjectives: %d\nNumber of nouns: %d\n", verb_count, adverb_count,adjective_count,noun_count);
+    return 0;
+}
+        '''
+        print(string)
+
+    def identifierlex():
+        string = '''
+        identifier.l
+
+%{
+    #include<stdio.h>
+    #include<stdlib.h>
+    int keywords=0; 
+    int identifiers=0; 
+    int operators=0;
+%}
+
+%%
+if|else|while|do|for|int|printf|return|main     {keywords++;}
+[a-zA-Z][a-zA-Z0-9]*     {identifiers++;}
+\+|\-|\*|\/|\%|\=|\!=    {operators++;}
+.                        ;
+
+%%
+int yywrap(void) {
+    return 1;
+}
+int main(int argc, char** argv) {
+    if (argc > 1) {
+        FILE *file;
+        file = fopen(argv[1], "r");
+        if (!file) {
+            fprintf(stderr, "Could not open %s\n", argv[1]);
+            exit(1);
+        }
+        yyin = file;
+    }   
+    yylex();
+    printf("Keywords: %d\nIdentifiers: %d\nOperators: %d\n",keywords, identifiers, operators);
+    return 0;
+}
+        '''
+        print(string)
+
+    def wordcount():
+        string = '''
+        logic for wordcount
+
+%%
+\n {charCount++; lineCount++;}
+[^ \t\n]+ {wordCount++; charCount+=yyleng;}
+. {charCount++;}
+%%
+        '''
+        print(string)
+
     def main():
         string = '''
+        wordcount()
         lexical()
         flex()
         ff()
         generatePT()
         PP()
         OP()
         yacc()
+        nested()
         ICG()
         ICG2()
         commands()
         DSP1()
         P2()
         macro()
         P1macro()
         P2macro()
+        quad()
+        identifierlex()
+        adverb()
         '''
         print(string)
```

