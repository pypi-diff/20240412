# Comparing `tmp/MedRoom.AI.DataEngineer-0.0.1.tar.gz` & `tmp/medroom_ai_dataengineer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedRoom.AI.DataEngineer-0.0.1.tar", last modified: Mon Nov  6 18:55:10 2023, max compression
+gzip compressed data, was "medroom_ai_dataengineer-0.0.2.tar", last modified: Fri Apr 12 18:04:33 2024, max compression
```

## Comparing `MedRoom.AI.DataEngineer-0.0.1.tar` & `medroom_ai_dataengineer-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-11-06 18:55:10.015312 MedRoom.AI.DataEngineer-0.0.1/
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-11-06 18:55:09.975312 MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    11670 2023-11-06 18:55:09.000000 MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      524 2023-11-06 18:55:09.000000 MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      115 2023-11-06 18:55:09.000000 MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        1 2023-08-08 00:56:44.000000 MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      124 2023-11-06 18:55:09.000000 MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/requires.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        8 2023-11-06 18:55:09.000000 MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/top_level.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    11670 2023-11-06 18:55:10.015312 MedRoom.AI.DataEngineer-0.0.1/PKG-INFO
--rwxrwxr-x   0 guilherme  (1000) guilherme  (1000)     2618 2023-10-10 23:27:22.000000 MedRoom.AI.DataEngineer-0.0.1/README.md
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-11-06 18:55:09.963312 MedRoom.AI.DataEngineer-0.0.1/medroom/
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-11-06 18:55:09.963312 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-11-06 18:55:09.995312 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/
--rwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-08-07 17:50:31.000000 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/__init__.py
--rwxrwxr-x   0 guilherme  (1000) guilherme  (1000)      632 2023-10-07 20:34:37.000000 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/config.py
--rwxrwxr-x   0 guilherme  (1000) guilherme  (1000)      582 2023-08-07 17:50:31.000000 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/main.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-11-06 18:55:10.011312 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/utils/
--rwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-08-07 17:50:31.000000 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/utils/__init__.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     2151 2023-10-10 21:15:22.000000 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/utils/evalmetrics.py
--rwxrwxr-x   0 guilherme  (1000) guilherme  (1000)     2292 2023-10-10 21:18:57.000000 MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/utils/textclean.py
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       38 2023-11-06 18:55:10.015312 MedRoom.AI.DataEngineer-0.0.1/setup.cfg
--rwxrwxr-x   0 guilherme  (1000) guilherme  (1000)     1269 2023-10-10 20:28:37.000000 MedRoom.AI.DataEngineer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.533494 medroom_ai_dataengineer-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.531494 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/
+-rw-rw-rw-   0        0        0    13724 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      115 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      124 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13724 2024-04-12 18:04:33.532493 medroom_ai_dataengineer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5758 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.497490 medroom_ai_dataengineer-0.0.2/medroom/
+drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.498490 medroom_ai_dataengineer-0.0.2/medroom/dna/
+drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.528497 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/config.py
+-rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.530493 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/__init__.py
+-rw-rw-rw-   0        0        0     2211 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/evalmetrics.py
+-rw-rw-rw-   0        0        0     1889 2024-04-12 17:16:27.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/textclean.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 18:04:33.533494 medroom_ai_dataengineer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/setup.py
```

### Comparing `MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/PKG-INFO` & `medroom_ai_dataengineer-0.0.2/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,212 +1,201 @@
-Metadata-Version: 1.2
-Name: MedRoom.AI.DataEngineer
-Version: 0.0.1
-Summary: A Natural Language Processing Data Engineer
-Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
-Author: Team IA
-Author-email: medroom@medroom.com.br
-License:                                  Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-Description: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `MedRoom.AI.DataEngineer-0.0.1/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt` & `medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 MedRoom.AI.DataEngineer.egg-info/PKG-INFO
 MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
 MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
 MedRoom.AI.DataEngineer.egg-info/not-zip-safe
 MedRoom.AI.DataEngineer.egg-info/requires.txt
```

### Comparing `MedRoom.AI.DataEngineer-0.0.1/PKG-INFO` & `medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,212 +1,219 @@
-Metadata-Version: 1.2
-Name: MedRoom.AI.DataEngineer
-Version: 0.0.1
-Summary: A Natural Language Processing Data Engineer
-Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
-Author: Team IA
-Author-email: medroom@medroom.com.br
-License:                                  Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-Description: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
+Metadata-Version: 2.1
+Name: MedRoom.AI.DataEngineer
+Version: 0.0.2
+Summary: A Natural Language Processing Data Engineer
+Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
+Author: Team IA
+Author-email: medroom@medroom.com.br
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Dist: nltk==3.8.1
+Requires-Dist: spacy==3.7.1
+Requires-Dist: unidecode==1.3.7
+Requires-Dist: matplotlib==3.7.0
+Requires-Dist: pandas==2.1.1
+Requires-Dist: numpy==1.26.0
+Requires-Dist: seaborn==0.13.0
+Requires-Dist: scikit-learn==1.3.1
```

### Comparing `MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/config.py` & `medroom_ai_dataengineer-0.0.2/medroom/dna/processors/config.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import yaml
-import os
-import logging
-from dotenv import load_dotenv
-
-PATH = f'opt/data_engineer/datalake/'
-
-class Config:
-
-    def __init__(self):
-        super().__init__()
-
-        logging.info('Setting up lakes file')
-
-        self.PATH
-
-    @staticmethod
-    def parse_recipe():
-        with open(PATH + 'commands.yml') as f:
-            read_data = yaml.safe_load(f)
-        return read_data
-    
-
-    @staticmethod
-    def parse_recipe_stop():
-        with open(PATH + 'stopWords.yml') as f:
-            read_data = yaml.safe_load(f)
-        return read_data
-    
-    @staticmethod
-    def path_root(self):
+import yaml
+import os
+import logging
+from dotenv import load_dotenv
+
+PATH = f'opt/data_engineer/datalake/'
+
+class Config:
+
+    def __init__(self):
+        super().__init__()
+
+        logging.info('Setting up lakes file')
+
+        self.PATH
+
+    @staticmethod
+    def parse_recipe():
+        with open(PATH + 'commands.yml') as f:
+            read_data = yaml.safe_load(f)
+        return read_data
+    
+
+    @staticmethod
+    def parse_recipe_stop():
+        with open(PATH + 'stopWords.yml') as f:
+            read_data = yaml.safe_load(f)
+        return read_data
+    
+    @staticmethod
+    def path_root(self):
         return PATH
```

### Comparing `MedRoom.AI.DataEngineer-0.0.1/medroom/dna/processors/utils/evalmetrics.py` & `medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/evalmetrics.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import seaborn as sns
-from sklearn import preprocessing
-from sklearn.metrics import accuracy_score, classification_report, confusion_matrix, roc_auc_score
-
-
-class ModelEvaluator:
-    @staticmethod
-    def accuracy(y_true, y_pred):
-        acc = accuracy_score(y_true, y_pred)
-        print("Acurácia do modelo = %2.f%%" % (acc * 100.00))
-
-    @staticmethod
-    def classification_report(y_true, y_pred):
-        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).T
-        report_df = report_df.drop(columns=["support"])
-        plt.subplots(figsize=(4, 3))
-        sns.heatmap(report_df, cmap="Greens", linewidths=0.5, annot=True)
-        plt.title("Classification Report")
-        plt.show()
-
-    @staticmethod
-    def confusion_matrix(y_true, y_pred):
-        # Criando a matriz de confusão
-        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).T
-        report_df = report_df.drop(columns=["support"])
-
-        cnf_report_df = report_df.index[:-3]
-        cnf_matrix = confusion_matrix(y_true, y_pred)
-        cnf_matrix = pd.DataFrame(cnf_matrix, index=cnf_report_df.values, columns=cnf_report_df.values)
-        cnf_matrix = cnf_matrix / cnf_matrix.sum(axis=1).values[:, np.newaxis]  # Normalização em linha (recall)
-
-        # Plotagem da matriz de confusão
-        sns.heatmap(
-            cnf_matrix,
-            cmap="Greens",
-            linecolor="white",
-            linewidths=0.5,
-            annot=True,
-            fmt=".0%",
-            cbar=False,
-            square=True,
-        )
-        plt.title("Confusion Matrix")
-        plt.show()
-
-    @staticmethod
-    def roc_auc(y_true, y_pred):
-        # Converter rótulos para formato binário
-        lb = preprocessing.LabelBinarizer()
-        lb.fit(y_true)
-
-        y_test = lb.transform(y_true)
-        y_pred = lb.transform(y_pred)
-
-        # Calcular a área sob a curva (AUC-ROC)
-        auc_roc = roc_auc_score(y_test, y_pred, average="weighted", multi_class="ovr")
-        print("ROC_AUC do modelo = %2.f%%" % (auc_roc * 100.00))
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import seaborn as sns
+from sklearn import preprocessing
+from sklearn.metrics import accuracy_score, classification_report, confusion_matrix, roc_auc_score
+
+
+class ModelEvaluator:
+    @staticmethod
+    def accuracy(y_true, y_pred):
+        acc = accuracy_score(y_true, y_pred)
+        print("Acurácia do modelo = %2.f%%" % (acc * 100.00))
+
+    @staticmethod
+    def classification_report(y_true, y_pred):
+        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).T
+        report_df = report_df.drop(columns=["support"])
+        plt.subplots(figsize=(4, 3))
+        sns.heatmap(report_df, cmap="Greens", linewidths=0.5, annot=True)
+        plt.title("Classification Report")
+        plt.show()
+
+    @staticmethod
+    def confusion_matrix(y_true, y_pred):
+        # Criando a matriz de confusão
+        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).T
+        report_df = report_df.drop(columns=["support"])
+
+        cnf_report_df = report_df.index[:-3]
+        cnf_matrix = confusion_matrix(y_true, y_pred)
+        cnf_matrix = pd.DataFrame(cnf_matrix, index=cnf_report_df.values, columns=cnf_report_df.values)
+        cnf_matrix = cnf_matrix / cnf_matrix.sum(axis=1).values[:, np.newaxis]  # Normalização em linha (recall)
+
+        # Plotagem da matriz de confusão
+        sns.heatmap(
+            cnf_matrix,
+            cmap="Greens",
+            linecolor="white",
+            linewidths=0.5,
+            annot=True,
+            fmt=".0%",
+            cbar=False,
+            square=True,
+        )
+        plt.title("Confusion Matrix")
+        plt.show()
+
+    @staticmethod
+    def roc_auc(y_true, y_pred):
+        # Converter rótulos para formato binário
+        lb = preprocessing.LabelBinarizer()
+        lb.fit(y_true)
+
+        y_test = lb.transform(y_true)
+        y_pred = lb.transform(y_pred)
+
+        # Calcular a área sob a curva (AUC-ROC)
+        auc_roc = roc_auc_score(y_test, y_pred, average="weighted", multi_class="ovr")
+        print("ROC_AUC do modelo = %2.f%%" % (auc_roc * 100.00))
```

### Comparing `MedRoom.AI.DataEngineer-0.0.1/setup.py` & `medroom_ai_dataengineer-0.0.2/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import find_namespace_packages, setup
-from setuptools.command.install import install
-from setuptools import setup, find_packages
-from distutils.command.install import install as _install
-
-import os
-
-
-PROJECT_DIR = os.path.dirname(__file__)
-INFO = open(os.path.join(PROJECT_DIR, 'INFO')).readlines()
-INFO = dict((line.strip().split('=') for line in INFO))
-
-DEPENDENCIES = open(os.path.join(PROJECT_DIR, 'requirements.txt')).readlines()
-
-setup(
-    name='MedRoom.AI.DataEngineer',
-    description='A Natural Language Processing Data Engineer',
-    version=INFO['version'],
-    author=INFO['author'],
-    author_email=INFO['author_email'],
-    url=INFO['url'],    
-    license=open(os.path.join(PROJECT_DIR, 'LICENSE')).read(),
-    packages=find_namespace_packages(include=['medroom','medroom.dna', 'medroom.dna.processors', 'medroom.dna.processors.*', 'medroom.dna.processors.utils']),
-    install_requires=[d for d in DEPENDENCIES if '://' not in d],
-    python_requires='>=3.8',
-    #TO-DO: Fix dependency links : not working with bdist_wheel
-    dependency_links = ["git+https://github.com/explosion/spacy-models/releases/download/pt_core_news_sm-3.2.0/pt_core_news_sm-3.2.0.tar.gz"],
-    tests_require=['pytest', 'parameterized'],
-    zip_safe=False
+from setuptools import find_namespace_packages, setup
+from setuptools.command.install import install
+from setuptools import setup, find_packages
+from distutils.command.install import install as _install
+
+import os
+
+
+PROJECT_DIR = os.path.dirname(__file__)
+INFO = open(os.path.join(PROJECT_DIR, 'INFO')).readlines()
+INFO = dict((line.strip().split('=') for line in INFO))
+
+DEPENDENCIES = open(os.path.join(PROJECT_DIR, 'requirements.txt')).readlines()
+
+setup(
+    name='MedRoom.AI.DataEngineer',
+    description='A Natural Language Processing Data Engineer',
+    version=INFO['version'],
+    author=INFO['author'],
+    author_email=INFO['author_email'],
+    url=INFO['url'],    
+    license=open(os.path.join(PROJECT_DIR, 'LICENSE')).read(),
+    packages=find_namespace_packages(include=['medroom','medroom.dna', 'medroom.dna.processors', 'medroom.dna.processors.*', 'medroom.dna.processors.utils']),
+    install_requires=[d for d in DEPENDENCIES if '://' not in d],
+    python_requires='>=3.8',
+    #TO-DO: Fix dependency links : not working with bdist_wheel
+    dependency_links = ["git+https://github.com/explosion/spacy-models/releases/download/pt_core_news_sm-3.2.0/pt_core_news_sm-3.2.0.tar.gz"],
+    tests_require=['pytest', 'parameterized'],
+    zip_safe=False
 )
```

