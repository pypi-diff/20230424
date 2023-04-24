# Comparing `tmp/xtest_sapnwrfc-0.0.12.tar.gz` & `tmp/xtest_sapnwrfc-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtest_sapnwrfc-0.0.12.tar", last modified: Mon Apr 24 11:58:27 2023, max compression
+gzip compressed data, was "xtest_sapnwrfc-0.0.13.tar", last modified: Mon Apr 24 12:49:45 2023, max compression
```

## Comparing `xtest_sapnwrfc-0.0.12.tar` & `xtest_sapnwrfc-0.0.13.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.391621 xtest_sapnwrfc-0.0.12/
--rw-r--r--   0 d037732    (501) wheel        (0)    10273 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/LICENSE
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.378096 xtest_sapnwrfc-0.0.12/LICENSES/
--rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/LICENSES/Apache-2.0.txt
--rw-r--r--   0 d037732    (501) wheel        (0)       79 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/MANIFEST.in
--rw-r--r--   0 d037732    (501) wheel        (0)    23350 2023-04-24 11:58:27.391325 xtest_sapnwrfc-0.0.12/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)    10133 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/README.md
--rw-r--r--   0 d037732    (501) wheel        (0)     1764 2023-04-24 11:57:59.000000 xtest_sapnwrfc-0.0.12/pyproject.toml
--rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-24 11:58:27.391679 xtest_sapnwrfc-0.0.12/setup.cfg
--rw-r--r--   0 d037732    (501) wheel        (0)     6349 2023-04-24 11:57:35.000000 xtest_sapnwrfc-0.0.12/setup.py
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.375329 xtest_sapnwrfc-0.0.12/src/
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.386857 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/
--rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/__init__.py
--rw-r--r--   0 d037732    (501) wheel        (0)  2353011 2023-04-24 11:28:26.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.cpp
--rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.pyx
--rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_exception.py
--rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_utils.py
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.390858 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/
--rw-r--r--   0 d037732    (501) wheel        (0)    23350 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)      398 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/SOURCES.txt
--rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/dependency_links.txt
--rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/top_level.txt
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 12:49:45.855080 xtest_sapnwrfc-0.0.13/
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 12:49:45.831990 xtest_sapnwrfc-0.0.13/LICENSES/
+-rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.13/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)    23473 2023-04-24 12:49:45.854538 xtest_sapnwrfc-0.0.13/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)    10250 2023-04-24 12:10:06.000000 xtest_sapnwrfc-0.0.13/README.md
+-rw-r--r--   0 d037732    (501) wheel        (0)     1892 2023-04-24 12:49:21.000000 xtest_sapnwrfc-0.0.13/pyproject.toml
+-rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-24 12:49:45.855140 xtest_sapnwrfc-0.0.13/setup.cfg
+-rw-r--r--   0 d037732    (501) wheel        (0)     5751 2023-04-24 12:48:25.000000 xtest_sapnwrfc-0.0.13/setup.py
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 12:49:45.830017 xtest_sapnwrfc-0.0.13/src/
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 12:49:45.843392 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/__init__.py
+-rw-r--r--   0 d037732    (501) wheel        (0)  2353011 2023-04-24 11:28:26.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/_cyrfc.cpp
+-rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/_cyrfc.pyx
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/_exception.py
+-rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/_utils.py
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 12:49:45.847445 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc.egg-info/
+-rw-r--r--   0 d037732    (501) wheel        (0)    23473 2023-04-24 12:49:45.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc.egg-info/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)      699 2023-04-24 12:49:45.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 12:49:45.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 12:43:10.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc.egg-info/not-zip-safe
+-rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-24 12:49:45.000000 xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc.egg-info/top_level.txt
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 12:49:45.853942 xtest_sapnwrfc-0.0.13/tests/
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     4386 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_client_config.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     8887 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_connection.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)    26084 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_datatypes.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     3943 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_errors.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     7218 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_errors_abap.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     3471 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_options.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)      690 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_rfcsdk.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     2703 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_server.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)      988 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_table_type.py
+-rw-r--r--   0 d037732    (501) wheel        (0)     4887 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_throughput.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     2227 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_timeout.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     1519 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.13/tests/test_wsrfc.py
```

### Comparing `xtest_sapnwrfc-0.0.12/LICENSE` & `xtest_sapnwrfc-0.0.13/LICENSES/Apache-2.0.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,208 @@
 Apache License
+
 Version 2.0, January 2004
-http://www.apache.org/licenses/
 
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION,
+AND DISTRIBUTION
+
+   1. Definitions.
+
+
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution
+as defined by Sections 1 through 9 of this document.
+
+
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright
+owner that is granting the License.
+
+
+
+"Legal Entity" shall mean the union of the acting entity and all other entities
+that control, are controlled by, or are under common control with that entity.
+For the purposes of this definition, "control" means (i) the power, direct
+or indirect, to cause the direction or management of such entity, whether
+by contract or otherwise, or (ii) ownership of fifty percent (50%) or more
+of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions
+granted by this License.
+
+
+
+"Source" form shall mean the preferred form for making modifications, including
+but not limited to software source code, documentation source, and configuration
+files.
+
+
+
+"Object" form shall mean any form resulting from mechanical transformation
+or translation of a Source form, including but not limited to compiled object
+code, generated documentation, and conversions to other media types.
+
+
 
-1. Definitions.
+"Work" shall mean the work of authorship, whether in Source or Object form,
+made available under the License, as indicated by a copyright notice that
+is included in or attached to the work (an example is provided in the Appendix
+below).
 
-"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
 
-"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
 
-"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+"Derivative Works" shall mean any work, whether in Source or Object form,
+that is based on (or derived from) the Work and for which the editorial revisions,
+annotations, elaborations, or other modifications represent, as a whole, an
+original work of authorship. For the purposes of this License, Derivative
+Works shall not include works that remain separable from, or merely link (or
+bind by name) to the interfaces of, the Work and Derivative Works thereof.
 
-"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
 
-"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
 
-"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+"Contribution" shall mean any work of authorship, including the original version
+of the Work and any modifications or additions to that Work or Derivative
+Works thereof, that is intentionally submitted to Licensor for inclusion in
+the Work by the copyright owner or by an individual or Legal Entity authorized
+to submit on behalf of the copyright owner. For the purposes of this definition,
+"submitted" means any form of electronic, verbal, or written communication
+sent to the Licensor or its representatives, including but not limited to
+communication on electronic mailing lists, source code control systems, and
+issue tracking systems that are managed by, or on behalf of, the Licensor
+for the purpose of discussing and improving the Work, but excluding communication
+that is conspicuously marked or otherwise designated in writing by the copyright
+owner as "Not a Contribution."
 
-"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
 
-"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
 
-"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf
+of whom a Contribution has been received by Licensor and subsequently incorporated
+within the Work.
 
-"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+2. Grant of Copyright License. Subject to the terms and conditions of this
+License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive,
+no-charge, royalty-free, irrevocable copyright license to reproduce, prepare
+Derivative Works of, publicly display, publicly perform, sublicense, and distribute
+the Work and such Derivative Works in Source or Object form.
 
-2. Grant of Copyright License.
+3. Grant of Patent License. Subject to the terms and conditions of this License,
+each Contributor hereby grants to You a perpetual, worldwide, non-exclusive,
+no-charge, royalty-free, irrevocable (except as stated in this section) patent
+license to make, have made, use, offer to sell, sell, import, and otherwise
+transfer the Work, where such license applies only to those patent claims
+licensable by such Contributor that are necessarily infringed by their Contribution(s)
+alone or by combination of their Contribution(s) with the Work to which such
+Contribution(s) was submitted. If You institute patent litigation against
+any entity (including a cross-claim or counterclaim in a lawsuit) alleging
+that the Work or a Contribution incorporated within the Work constitutes direct
+or contributory patent infringement, then any patent licenses granted to You
+under this License for that Work shall terminate as of the date such litigation
+is filed.
 
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+4. Redistribution. You may reproduce and distribute copies of the Work or
+Derivative Works thereof in any medium, with or without modifications, and
+in Source or Object form, provided that You meet the following conditions:
 
-3. Grant of Patent License.
+(a) You must give any other recipients of the Work or Derivative Works a copy
+of this License; and
 
-Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+(b) You must cause any modified files to carry prominent notices stating that
+You changed the files; and
 
-4. Redistribution.
+(c) You must retain, in the Source form of any Derivative Works that You distribute,
+all copyright, patent, trademark, and attribution notices from the Source
+form of the Work, excluding those notices that do not pertain to any part
+of the Derivative Works; and
 
-You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+(d) If the Work includes a "NOTICE" text file as part of its distribution,
+then any Derivative Works that You distribute must include a readable copy
+of the attribution notices contained within such NOTICE file, excluding those
+notices that do not pertain to any part of the Derivative Works, in at least
+one of the following places: within a NOTICE text file distributed as part
+of the Derivative Works; within the Source form or documentation, if provided
+along with the Derivative Works; or, within a display generated by the Derivative
+Works, if and wherever such third-party notices normally appear. The contents
+of the NOTICE file are for informational purposes only and do not modify the
+License. You may add Your own attribution notices within Derivative Works
+that You distribute, alongside or as an addendum to the NOTICE text from the
+Work, provided that such additional attribution notices cannot be construed
+as modifying the License.
 
-You must give any other recipients of the Work or Derivative Works a copy of this License; and
-You must cause any modified files to carry prominent notices stating that You changed the files; and
-You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
-If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
-You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+You may add Your own copyright statement to Your modifications and may provide
+additional or different license terms and conditions for use, reproduction,
+or distribution of Your modifications, or for any such Derivative Works as
+a whole, provided Your use, reproduction, and distribution of the Work otherwise
+complies with the conditions stated in this License.
 
-5. Submission of Contributions.
+5. Submission of Contributions. Unless You explicitly state otherwise, any
+Contribution intentionally submitted for inclusion in the Work by You to the
+Licensor shall be under the terms and conditions of this License, without
+any additional terms or conditions. Notwithstanding the above, nothing herein
+shall supersede or modify the terms of any separate license agreement you
+may have executed with Licensor regarding such Contributions.
 
-Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+6. Trademarks. This License does not grant permission to use the trade names,
+trademarks, service marks, or product names of the Licensor, except as required
+for reasonable and customary use in describing the origin of the Work and
+reproducing the content of the NOTICE file.
 
-6. Trademarks.
+7. Disclaimer of Warranty. Unless required by applicable law or agreed to
+in writing, Licensor provides the Work (and each Contributor provides its
+Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied, including, without limitation, any warranties
+or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR
+A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness
+of using or redistributing the Work and assume any risks associated with Your
+exercise of permissions under this License.
 
-This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+8. Limitation of Liability. In no event and under no legal theory, whether
+in tort (including negligence), contract, or otherwise, unless required by
+applicable law (such as deliberate and grossly negligent acts) or agreed to
+in writing, shall any Contributor be liable to You for damages, including
+any direct, indirect, special, incidental, or consequential damages of any
+character arising as a result of this License or out of the use or inability
+to use the Work (including but not limited to damages for loss of goodwill,
+work stoppage, computer failure or malfunction, or any and all other commercial
+damages or losses), even if such Contributor has been advised of the possibility
+of such damages.
 
-7. Disclaimer of Warranty.
+9. Accepting Warranty or Additional Liability. While redistributing the Work
+or Derivative Works thereof, You may choose to offer, and charge a fee for,
+acceptance of support, warranty, indemnity, or other liability obligations
+and/or rights consistent with this License. However, in accepting such obligations,
+You may act only on Your own behalf and on Your sole responsibility, not on
+behalf of any other Contributor, and only if You agree to indemnify, defend,
+and hold each Contributor harmless for any liability incurred by, or claims
+asserted against, such Contributor by reason of your accepting any such warranty
+or additional liability. END OF TERMS AND CONDITIONS
 
-Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+APPENDIX: How to apply the Apache License to your work.
 
-8. Limitation of Liability.
+To apply the Apache License to your work, attach the following boilerplate
+notice, with the fields enclosed by brackets "[]" replaced with your own identifying
+information. (Don't include the brackets!) The text should be enclosed in
+the appropriate comment syntax for the file format. We also recommend that
+a file or class name and description of purpose be included on the same "printed
+page" as the copyright notice for easier identification within third-party
+archives.
 
-In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+Copyright [yyyy] [name of copyright owner]
 
-9. Accepting Warranty or Additional Liability.
+Licensed under the Apache License, Version 2.0 (the "License");
 
-While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+you may not use this file except in compliance with the License.
 
-END OF TERMS AND CONDITIONS
+You may obtain a copy of the License at
 
-APPENDIX: How to apply the Apache License to your work
+http://www.apache.org/licenses/LICENSE-2.0
 
-To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!) The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
+Unless required by applicable law or agreed to in writing, software
 
-   Copyright [yyyy] [name of copyright owner]
+distributed under the License is distributed on an "AS IS" BASIS,
 
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 
-     http://www.apache.org/licenses/LICENSE-2.0
+See the License for the specific language governing permissions and
 
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+limitations under the License.
```

### Comparing `xtest_sapnwrfc-0.0.12/PKG-INFO` & `xtest_sapnwrfc-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: xtest_sapnwrfc
-Version: 0.0.12
+Version: 0.0.13
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
-Maintainer: Srdjan Boskovic
-Maintainer-email: srdjan.boskovic@sap.com
+Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
         
         http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION,
         AND DISTRIBUTION
         
@@ -231,15 +230,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSES/Apache-2.0.txt
 
 <h1>PyRFC</h1>
 
 Asynchronous, non-blocking [SAP NetWeawer RFC SDK](https://support.sap.com/en/product/connectors/nwrfcsdk.html) bindings for Python.
 
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyrfc)](https://pypi.org/project/pyrfc/)
@@ -253,14 +252,15 @@
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
   - [macOS](#macos)
 - [Download and installation](#download-and-installation)
+  - [Linux](#linux)
 - [Getting started](#getting-started)
   - [Call ABAP Function Module from Python](#call-abap-function-module-from-python)
   - [Call Python function from ABAP](#call-python-function-from-abap)
 - [SPJ articles](#spj-articles)
 - [How to obtain support](#how-to-obtain-support)
 - [Contributing](#contributing)
 - [License](#license)
@@ -319,14 +319,20 @@
 
 ## Download and installation
 
 ```shell
 pip install pyrfc
 ```
 
+### Linux
+
+```shell
+pip install --no-build-isolation pyrfc
+```
+
 Cython is required on Linux platforms, for the the default build from source installation method.
 
 Build from source can be also requested on Windows and Darwin platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
 # or
@@ -334,15 +340,15 @@
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
-python setup.py bdist_wheel
+python -m build --no-isolation --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
 
 ## Getting started
```

### Comparing `xtest_sapnwrfc-0.0.12/README.md` & `xtest_sapnwrfc-0.0.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
   - [macOS](#macos)
 - [Download and installation](#download-and-installation)
+  - [Linux](#linux)
 - [Getting started](#getting-started)
   - [Call ABAP Function Module from Python](#call-abap-function-module-from-python)
   - [Call Python function from ABAP](#call-python-function-from-abap)
 - [SPJ articles](#spj-articles)
 - [How to obtain support](#how-to-obtain-support)
 - [Contributing](#contributing)
 - [License](#license)
@@ -80,14 +81,20 @@
 
 ## Download and installation
 
 ```shell
 pip install pyrfc
 ```
 
+### Linux
+
+```shell
+pip install --no-build-isolation pyrfc
+```
+
 Cython is required on Linux platforms, for the the default build from source installation method.
 
 Build from source can be also requested on Windows and Darwin platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
 # or
@@ -95,15 +102,15 @@
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
-python setup.py bdist_wheel
+python -m build --no-isolation --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
 
 ## Getting started
```

### Comparing `xtest_sapnwrfc-0.0.12/pyproject.toml` & `xtest_sapnwrfc-0.0.13/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["Cython ~= 0.29.0", "setuptools ~= 67.7.0", "wheel ~= 0.40.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "xtest_sapnwrfc"
-version = "0.0.12"
+version = "0.0.13"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
 authors = [ { name = "SAP SE"} ]
-maintainers = [ { name = "Srdjan Boskovic" } ]
+maintainers = [ { name = "Srdjan Boskovic", email = "srdjan.boskovic@sap.com" } ]
 requires-python = ">=3.7"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -37,18 +37,19 @@
 documentation = "http://sap.github.io/PyRFC"
 repository = "https://github.com/SAP/PyRFC.git"
 
 [tool.cython-lint]
 max-line-length = 148
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
-# [tool.setuptools]
-# package-dir = { "" = "src" }
-# license-files = ["LICENSES", "Apache-2.0.txt"]
+[tool.setuptools]
+zip-safe = false
+include-package-data = false
+exclude-package-data = {"*" = ["*.cpp", "*.html", "*.pyx", "*.pxd"]}
+license-files=["LICENSES/*.txt"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
+include = ["xtest_sapnwrfc"]
 
 [tool.setuptools.dynamic]
 readme = {file = "README.md"}
-
-
```

### Comparing `xtest_sapnwrfc-0.0.12/setup.py` & `xtest_sapnwrfc-0.0.13/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -179,27 +179,14 @@
     extra_link_args=LINK_ARGS,
     libraries=LIBS,
 )
 
 # cf. http://docs.python.org/distutils/setupscript.html#additional-meta-data
 setup(
     name=PACKAGE_NAME,
-    #version="2.8.3", # __version__,
-    #description=("Python bindings for SAP NetWeaver RFC SDK"),
-    #long_description="readme_md",
-    #long_description_content_type="text/markdown",
-    #download_url="https://github.com/SAP/PyRFC/tarball/main",
-    packages=find_packages(where="src", exclude=["*.cpp", "*.html"]),
-    package_dir={"": "src"},
-    #keywords=f"pyrfc sap rfc nwrfc sapnwrfc",
-    #author="SAP SE",
-    #url="https://github.com/SAP/pyrfc",
-    #license="OSI Approved :: Apache Software License",
-    maintainer="Srdjan Boskovic",
-    maintainer_email="srdjan.boskovic@sap.com",
     # install_requires=["setuptools"],
     cmdclass=CMDCLASS,  # type: ignore
     ext_modules=cythonize(PYRFC_EXT, annotate=True, compiler_directives={'language_level' : "3"})  # type: ignore
     if BUILD_CYTHON
     else [PYRFC_EXT],  # type: ignore
     test_suite=MODULE_NAME,
 )
```

### Comparing `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/__init__.py` & `xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/__init__.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.cpp` & `xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/_cyrfc.cpp`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.pyx` & `xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/_cyrfc.pyx`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_exception.py` & `xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc/_exception.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/PKG-INFO` & `xtest_sapnwrfc-0.0.13/src/xtest_sapnwrfc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: xtest-sapnwrfc
-Version: 0.0.12
+Version: 0.0.13
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
-Maintainer: Srdjan Boskovic
-Maintainer-email: srdjan.boskovic@sap.com
+Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
         
         http://www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION,
         AND DISTRIBUTION
         
@@ -231,15 +230,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSES/Apache-2.0.txt
 
 <h1>PyRFC</h1>
 
 Asynchronous, non-blocking [SAP NetWeawer RFC SDK](https://support.sap.com/en/product/connectors/nwrfcsdk.html) bindings for Python.
 
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyrfc)](https://pypi.org/project/pyrfc/)
@@ -253,14 +252,15 @@
 - [Supported platforms](#supported-platforms)
 - [Requirements](#requirements)
   - [SAP NW RFC SDK 7.50.11](#sap-nw-rfc-sdk-75011)
   - [Docker](#docker)
   - [Windows](#windows)
   - [macOS](#macos)
 - [Download and installation](#download-and-installation)
+  - [Linux](#linux)
 - [Getting started](#getting-started)
   - [Call ABAP Function Module from Python](#call-abap-function-module-from-python)
   - [Call Python function from ABAP](#call-python-function-from-abap)
 - [SPJ articles](#spj-articles)
 - [How to obtain support](#how-to-obtain-support)
 - [Contributing](#contributing)
 - [License](#license)
@@ -319,14 +319,20 @@
 
 ## Download and installation
 
 ```shell
 pip install pyrfc
 ```
 
+### Linux
+
+```shell
+pip install --no-build-isolation pyrfc
+```
+
 Cython is required on Linux platforms, for the the default build from source installation method.
 
 Build from source can be also requested on Windows and Darwin platforms:
 
 ```shell
 pip install pyrfc --no-binary :all:
 # or
@@ -334,15 +340,15 @@
 ```
 
 Alternative build from source installation:
 
 ```shell
 git clone https://github.com/SAP/PyRFC.git
 cd PyRFC
-python setup.py bdist_wheel
+python -m build --no-isolation --wheel --sdist --outdir dist
 pip install --upgrade --no-index --find-links=dist pyrfc
 ```
 
 See also the [pyrfc documentation](http://sap.github.io/PyRFC),
 complementing _SAP NWRFC SDK_[documentation](https://support.sap.com/nwrfcsdk), especially [SAP NWRFC SDK 7.50 Programming Guide](https://support.sap.com/content/dam/support/en_us/library/ssp/products/connectors/nwrfcsdk/NW_RFC_750_ProgrammingGuide.pdf).
 
 ## Getting started
```

