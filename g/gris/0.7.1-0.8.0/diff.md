# Comparing `tmp/gris-0.7.1.tar.gz` & `tmp/gris-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gris-0.7.1.tar", last modified: Fri Apr 21 05:03:25 2023, max compression
+gzip compressed data, was "gris-0.8.0.tar", last modified: Mon Apr 24 02:34:07 2023, max compression
```

## Comparing `gris-0.7.1.tar` & `gris-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.976763 gris-0.7.1/
--rw-r--r--   0 anglyan    (502) staff       (20)    18092 2023-04-21 00:57:42.000000 gris-0.7.1/LICENSE.txt
--rw-r--r--   0 anglyan    (502) staff       (20)       27 2023-04-21 00:57:42.000000 gris-0.7.1/MANIFEST.in
--rw-r--r--   0 anglyan    (502) staff       (20)     1276 2023-04-21 05:03:25.976544 gris-0.7.1/PKG-INFO
--rw-r--r--   0 anglyan    (502) staff       (20)      648 2023-04-21 01:09:14.000000 gris-0.7.1/README.md
--rw-r--r--   0 anglyan    (502) staff       (20)      689 2023-04-21 05:02:50.000000 gris-0.7.1/pyproject.toml
--rw-r--r--   0 anglyan    (502) staff       (20)       38 2023-04-21 05:03:25.976810 gris-0.7.1/setup.cfg
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.972893 gris-0.7.1/src/
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.974290 gris-0.7.1/src/gris/
--rw-r--r--   0 anglyan    (502) staff       (20)       20 2023-04-21 01:09:48.000000 gris-0.7.1/src/gris/__init__.py
--rw-r--r--   0 anglyan    (502) staff       (20)    10150 2023-04-21 01:09:48.000000 gris-0.7.1/src/gris/gris.py
-drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 05:03:25.975749 gris-0.7.1/src/gris.egg-info/
--rw-r--r--   0 anglyan    (502) staff       (20)     1276 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/PKG-INFO
--rw-r--r--   0 anglyan    (502) staff       (20)      214 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/SOURCES.txt
--rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/dependency_links.txt
--rw-r--r--   0 anglyan    (502) staff       (20)        5 2023-04-21 05:03:25.000000 gris-0.7.1/src/gris.egg-info/top_level.txt
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-24 02:34:07.127277 gris-0.8.0/
+-rw-r--r--   0 anglyan    (502) staff       (20)    18092 2023-04-21 00:57:42.000000 gris-0.8.0/LICENSE.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)       27 2023-04-21 00:57:42.000000 gris-0.8.0/MANIFEST.in
+-rw-r--r--   0 anglyan    (502) staff       (20)     2201 2023-04-24 02:34:07.127145 gris-0.8.0/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)     1505 2023-04-24 02:27:02.000000 gris-0.8.0/README.md
+-rw-r--r--   0 anglyan    (502) staff       (20)      749 2023-04-24 02:30:43.000000 gris-0.8.0/pyproject.toml
+-rw-r--r--   0 anglyan    (502) staff       (20)       38 2023-04-24 02:34:07.127311 gris-0.8.0/setup.cfg
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-24 02:34:07.122553 gris-0.8.0/src/
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-24 02:34:07.125990 gris-0.8.0/src/gris/
+-rw-r--r--   0 anglyan    (502) staff       (20)       68 2023-04-23 15:38:06.000000 gris-0.8.0/src/gris/__init__.py
+-rw-r--r--   0 anglyan    (502) staff       (20)      427 2023-04-22 17:07:20.000000 gris-0.8.0/src/gris/__main__.py
+-rw-r--r--   0 anglyan    (502) staff       (20)        0 2023-04-23 06:14:15.000000 gris-0.8.0/src/gris/bibtex.py
+-rw-r--r--   0 anglyan    (502) staff       (20)     7147 2023-04-23 21:16:11.000000 gris-0.8.0/src/gris/gris.py
+-rw-r--r--   0 anglyan    (502) staff       (20)     7449 2023-04-23 15:37:32.000000 gris-0.8.0/src/gris/io.py
+-rw-r--r--   0 anglyan    (502) staff       (20)      274 2023-04-23 05:52:59.000000 gris-0.8.0/src/gris/wos.py
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-24 02:34:07.126996 gris-0.8.0/src/gris.egg-info/
+-rw-r--r--   0 anglyan    (502) staff       (20)     2201 2023-04-24 02:34:07.000000 gris-0.8.0/src/gris.egg-info/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)      285 2023-04-24 02:34:07.000000 gris-0.8.0/src/gris.egg-info/SOURCES.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-24 02:34:07.000000 gris-0.8.0/src/gris.egg-info/dependency_links.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        5 2023-04-24 02:34:07.000000 gris-0.8.0/src/gris.egg-info/top_level.txt
```

### Comparing `gris-0.7.1/LICENSE.txt` & `gris-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gris-0.7.1/pyproject.toml` & `gris-0.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gris"
 authors = [
 { name="Angel Yanguas-Gil"}]
-version = "0.7.1"
+version = "0.8.0"
 description = "Parser of RIS file format"
 readme = "README.md"
 keywords = ["RIS file format", "RefMan RIS", "bibliography", "parser"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
@@ -19,8 +19,9 @@
     "Environment :: Console",
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/anglyan/gris.git"
+"docs" = "https://gris.readthedocs.io/en/latest/index.html"
```

### Comparing `gris-0.7.1/src/gris/gris.py` & `gris-0.8.0/src/gris/io.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,49 @@
-#Copyright (c) 2013 Angel Yanguas-Gil
-#This program is free software, licensed under GPLv2 or later.
-#A copy of the GPLv2 license is provided in the root directory of
-#the source code.
-
-"""Parse WOK and Refman's RIS files"""
-
+import json
 import re
 import csv
+from .gris import clean_reference
 
 woktag = "^[A-Z][A-Z0-9] |^ER$|^EF$"
-ristag = "^[A-Z][A-Z0-9]  - "
+ristag = "^[A-Z][A-Z0-9]  -"
 
 wokpat = re.compile(woktag)
 rispat = re.compile(ristag)
 
 ris_boundtags = ('TY', 'ER')
 wok_boundtags = ('PT', 'ER')
 
 wok_ignoretags = ['FN', 'VR', 'EF']
 ris_ignoretags = []
 
-ristags = {'TY': "Record kind",
-        'A2': "Secondary Author",
-        'A3': "Tertiary Author",
-        'A4': "Subsidiary Author",
-        'AB': "Abstract",
-        'AD': "Author Address",
-        'AN': "Accession Number",
-        'AU': "Author",
-        'C1': "Custom 1",
-        'CA': "Caption",
-        'CN': "Call Number",
-        'CY': "Place Published",
-        'DA': "Date",
-        'DB': "Name of Database",
-        'DO': "DOI",
-        'DP': "Database Provider",
-        'ET': "Edition",
-        'J2': "Alternate Title",
-        'KW': "Keywords",
-        'L1': "File Attachments",
-        'L4': "Figure",
-        'LA': "Language",
-        'LB': "Label",
-        'IS': "Number",
-        'M3': "Type of Work",
-        'N1': "Notes",
-        'NV': "Number of Volumes",
-        'OP': "Original Publication",
-        'PB': "Publisher",
-        'PY': "Year",
-        'RI': "Reviewed Item",
-        'RN': "Research Notes",
-        'RP': "Reprint Edition",
-        'SE': "Version",
-        'SN': "ISBN",
-        'SP': "Pages",
-        'ST': "Short Title",
-        'T2': "Dictionary Title",
-        'TA': "Translated Author",
-        'TI': "Title",
-        'TT': "Translated Title",
-        'UR': "URL",
-        'VL': "Volume",
-        'Y2': "Access Date",
-        'ER': "[End of Reference]"
-        }
-
-missing_string = 'NA'
-
-def read_ris(filename, wok=True):
+def read_ris(filename, wok=False):
     """Parse a ris file and return a list of entries.
 
     Entries are codified as dictionaries whose keys are the
     different tags. For single line and singly ocurring tags,
     the content is codified as a string. In the case of multiline
     or multiple key ocurrences, the content is returned as a list
     of strings.
 
-    Keyword arguments:
-    filename -- input ris file
-    wok -- flag, Web of Knowledge format is used if True, otherwise
-           Refman's RIS specifications are used.
+    Args:
+        filename (str) : input ris file
+        wok (:obj:`bool`, optional) : old WebofKnowledge's other document
+            format is used if True. Defaults False.
 
     """
 
     if wok:
         gettag = lambda line: line[0:2]
-        getcontent = lambda line: line[2:]
+        getcontent = lambda line: line[2:].strip()
         istag = lambda line: (wokpat.match(line) != None )
         starttag, endtag = wok_boundtags
         ignoretags = wok_ignoretags
     else:
         gettag = lambda line: line[0:2]
-        getcontent = lambda line: line[6:]
+        getcontent = lambda line: line[6:].strip()
         istag = lambda line: (rispat.match(line) != None )
         starttag, endtag = ris_boundtags
         ignoretags = ris_ignoretags
 
     filelines = open(filename, encoding='utf-8-sig', mode='r').readlines()
     #WOK saves text files as utf8 with BOM, BOM is not handled automatically
     #by python 3, so we have to use utf-8-sig to deal with it.
@@ -117,29 +63,29 @@
                 continue
             if inref:
                 #Active reference
                 if tag == None:
                     text = "Expected tag in line %d:\n %s" %(ln, line)
                     raise IOError(text)
                 else:
-                    #Active tag
-                    if hasattr(current[tag], "append"):
-                        current[tag].append(line.strip())
+                    #Dealing with multiline records
+                    if isinstance(current[tag], list):
+                        current[tag][-1] += "\n" + line.strip()
                     else:
-                        current[tag] = [current[tag], line.strip()]
+                        current[tag] += "\n" + line.strip()
             else:
                 text = "Expected start tag in line %d:\n %s" %(ln, line)
                 raise IOError(text)
         else:
             #Get the new tag
             tag = gettag(line)
             if tag in ignoretags:
                 continue
             elif tag == endtag:
-                #Close the active entry and append it to the entry list
+                #Close the active entry and append it to the entry list                    
                 refs.append(current)
                 current = {}
                 inref = False
             elif tag == starttag:
                 #New entry
                 if inref:
                     text = "Missing end of record tag in line %d:\n %s" % (
@@ -147,207 +93,151 @@
                     raise IOError(text)
                 current[tag] = getcontent(line)
                 inref = True
             else:
                 if not inref:
                     text = "Invalid start tag in line %d:\n %s" %(ln, line)
                     raise IOError(text)
-                current[tag] = getcontent(line)
+                if tag in current:
+                    if not isinstance(current[tag], list):
+                        current[tag] = [current[tag]]
+                    current[tag].append(getcontent(line))
+                else:
+                    current[tag] = getcontent(line)
 
     refs = [clean_reference(r) for r in refs]
 
     return refs
 
-def clean_reference(ref):
-    """Remove trailing spaces and line breaks from the entries"""
-    for k,v in ref.items():
-        try:
-            nv = v.strip()
-        except AttributeError:
-            nv = [el.strip() for el in v]
-        ref[k] = nv
-    return ref
-
-
-def tag2string(ref, t):
-    """Return the content of tag t as a string, 'NA' if the tag is not
-    present"""
-
-    if t in ref:
-        if isinstance(ref[t], list):
-            return " ".join(ref[t])
-        else:
-            return ref[t]
-    else:
-        return missing_string
 
-def tag2list(ref, t):
-    """Return the content of tag t as a list, [] if the tag is not present
-    """
-    if t in ref:
-        if isinstance(ref[t], list):
-            return ref[t]
-        else:
-            return [ref[t]]
-    else:
-        return []
 
-def get_authors(ref):
-    """Return a list of the authors"""
-    if 'AF' in ref:
-        return tag2list(ref, 'AF')
-    else:
-        return tag2list(ref, 'AU')
+def write_key(key):
+    return "{}  -".format(key)
 
-def get_abstract(ref):
-    """Return the abstract"""
-    return tag2string(ref, 'AB')
-
-def get_pubyear(ref):
-    """Return the publication year"""
-    return tag2string(ref, 'PY')
-
-def get_title(ref):
-    """Return the pubication title"""
-    return tag2string(ref, 'TI')
-
-def get_volume(ref):
-    """Return the publication volume"""
-    return tag2string(ref, 'VL')
-
-def get_issue(ref):
-    """Return the publication issue"""
-    return tag2string(ref, 'IS')
-
-def get_page(ref):
-    """Return the page and, if not present, the article number"""
-    if 'BP' in ref:
-        return tag2string(ref, 'BP')
-    else:
-        return tag2string(ref, 'AR')
 
-def write_key(key, value):
-    """Return a string with the key, value in the WOK RIS format
+def write_entry(key, value):
+    """Return a string with the key, value
     """
 
-    if isinstance(value, list):
-        lines = [key + " " + value[0].strip()]
-        for val in value[1:]:
-            lines.append("   " + val.strip())
-        return lines
-    else:
-        return [key + " " + value.strip()]
+    if not isinstance(value, list):
+        value = [value]
+    
+    lines = []
+    key_str = write_key(key)
+    lines = [key_str + " " + val.strip() for val in value]
+    return lines
+
 
 def write_ref(entry):
     """Return a string with the content of the reference
-    in WOK RIS format.
+    in RIS format.
 
     entry is a dictionary where tags are keys and the values are
     either lists or strings containing the corresponding bibliographic
     data
     """
 
-    entrylines = write_key('PT', entry['PT'])
+#    entrylines = write_key('PT', entry['PT'])
+    starttag, endtag = ris_boundtags
+
+    entrylines = write_entry(starttag, entry[starttag])
     for k, v in entry.items():
-        if k != 'PT':
-            entrylines.extend(write_key(k, v))
-    entrylines.append('ER')
+        if k != starttag:
+            entrylines.extend(write_entry(k, v))
+    entrylines.append(write_key(endtag))
     return entrylines
 
-def write_ris(entrylist):
-    """Write a list of entries in the wok ris file format
+
+def write_json(file_name, refs):
+    with open(file_name, 'w') as f:
+        json.dump(refs, f, indent=4)
+        f.close()
+
+
+def load_json(file_name):
+    with open(file_name, 'r') as f:
+        refs = json.load(f)
+        f.close()
+        if not isinstance(refs, list):
+            refs = [refs]
+        return refs
+    
+
+def write_ris(file_name, entrylist):
+    """Write a list of entries in the RIS file format
 
     write_ris uses as an input a list of entries as codified
-    using read_ris, returning a list of strings. The current version
-    returns a wok-compatible ris format.
+    using read_ris, returning a list of strings.
 
     """
-    header = ['FN Thompsom Reuters Web of Knowledge',
-             'VR 1.0']
-    filelines = header
-    for entry in entrylist:
-        filelines.extend(write_ref(entry))
-        filelines.append("")
-    filelines.append('EF')
+    with open(file_name, 'w') as f:
+        filelines = []
+        for entry in entrylist:
+            filelines.extend(write_ref(entry))
+            filelines.append("")
+        f.write("\n".join(filelines))
+        f.close()
     return filelines
 
-
 def get_country(add):
     """Extract the country from a ris address field
     """
 
     rpc = add.split(',')[-1][:-1].strip().upper()
     if ' USA' in rpc:
         rpc = 'USA'
     elif len(rpc.split()[0]) == 2:
         rpc = 'USA'
     return rpc
 
-def recordtolist(i, ref):
-    """Transform a single record into a 2D list"""
-
-    title = tag2string(ref, 'TI')
-    authors = [au.upper() for au in tag2list(ref, 'AU')]
-    categories = [c.strip() for c in tag2string(ref, 'WC').split(';')]
-    source = tag2string(ref, 'SO')
-    dt = tag2string(ref, 'DT')
-    tc = tag2string(ref, 'TC')
-    pubyear = tag2string(ref, 'PY')
-    aff = tag2list(ref, 'C1')
-    reprint = tag2string(ref, 'RP')
-    rpc = get_country(reprint)
-    affc = [get_country(ai) for ai in aff]
-    doi = tag2string(ref, 'DI')
-    if len(aff) == 0:
-        aff = ['NA']
-        affc = ['NA']
-    if len(categories) == 0:
-        categories = ['NA']
-    names = [an.split(',')[0].strip() if ',' in an else an for an in authors]
-    lines = [[str(i), dt, source,
-            pubyear, title, doi, tc, reprint, rpc, au, name,
-            aff[0], affc[0], categories[0]]
-            for (au, name) in zip(authors, names)]
-    lines2 = [[str(i), dt, source, pubyear,
-            title, doi, tc, reprint, rpc, authors[0],
-            names[0], ai, aci, categories[0]] for ai,aci in zip(aff[1:], affc[1:])]
-    lines3 = [[str(i), dt, source, pubyear,
-            title, doi, tc, reprint, rpc, authors[0],
-            names[0], aff[0], affc[0], c] for c in categories[1:]]
 
-    return lines + lines2 + lines3
+# def recordtolist(i, ref):
+#     """Transform a single record into a 2D list"""
 
+#     title = tag2string(ref, 'TI')
+#     authors = [au.upper() for au in tag2list(ref, 'AU')]
+#     categories = [c.strip() for c in tag2string(ref, 'WC').split(';')]
+#     source = tag2string(ref, 'SO')
+#     dt = tag2string(ref, 'DT')
+#     tc = tag2string(ref, 'TC')
+#     pubyear = tag2string(ref, 'PY')
+#     aff = tag2list(ref, 'C1')
+#     reprint = tag2string(ref, 'RP')
+#     rpc = get_country(reprint)
+#     affc = [get_country(ai) for ai in aff]
+#     doi = tag2string(ref, 'DI')
+#     if len(aff) == 0:
+#         aff = ['NA']
+#         affc = ['NA']
+#     if len(categories) == 0:
+#         categories = ['NA']
+#     names = [an.split(',')[0].strip() if ',' in an else an for an in authors]
+#     lines = [[str(i), dt, source,
+#             pubyear, title, doi, tc, reprint, rpc, au, name,
+#             aff[0], affc[0], categories[0]]
+#             for (au, name) in zip(authors, names)]
+#     lines2 = [[str(i), dt, source, pubyear,
+#             title, doi, tc, reprint, rpc, authors[0],
+#             names[0], ai, aci, categories[0]] for ai,aci in zip(aff[1:], affc[1:])]
+#     lines3 = [[str(i), dt, source, pubyear,
+#             title, doi, tc, reprint, rpc, authors[0],
+#             names[0], aff[0], affc[0], c] for c in categories[1:]]
+
+#     return lines + lines2 + lines3
+
+
+# def refs2csv(refs, filename):
+#     """Save a list of references to a csv file
+#     """
+
+#     table = [["Ref #", "Document type", "Source", "Year", "Title",
+#             "DOI", "Times cited", "Reprint Author", "Reprint country",
+#             "Author, complete",
+#             "Author name", "Affiliation", "Affiliation country",
+#             "Category"]]
+#     for i, ref in enumerate(refs):
+#         r = ristocsv(i, ref)
+#         table.extend(r)
+#     out = csv.writer(open(csvname, 'w'))
+#     out.writerows(table)
+#     return table
 
-def refs2csv(refs, filename):
-    """Save a list of references to a csv file
-    """
-
-    table = [["Ref #", "Document type", "Source", "Year", "Title",
-            "DOI", "Times cited", "Reprint Author", "Reprint country",
-            "Author, complete",
-            "Author name", "Affiliation", "Affiliation country",
-            "Category"]]
-    for i, ref in enumerate(refs):
-        r = ristocsv(i, ref)
-        table.extend(r)
-    out = csv.writer(open(csvname, 'w'))
-    out.writerows(table)
-    return table
-
-
-
-if __name__ == '__main__':
-
-    import sys
-
-    if len(sys.argv) > 2:
-        if sys.argv[2] == 'ris':
-            wok=False
-        else:
-            wok=True
-    else:
-        wok=True
-    refs = read_ris(sys.argv[1], wok)
-    print(len(refs))
-    authors = [r['AU'] for r in refs]
-    for a in authors:
-        print(a)
```

