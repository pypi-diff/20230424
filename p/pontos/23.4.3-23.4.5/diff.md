# Comparing `tmp/pontos-23.4.3.tar.gz` & `tmp/pontos-23.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.4.3.tar", max compression
+gzip compressed data, was "pontos-23.4.5.tar", max compression
```

## Comparing `pontos-23.4.3.tar` & `pontos-23.4.5.tar`

### file list

```diff
@@ -1,248 +1,251 @@
--rw-r--r--   0        0        0    35149 2023-04-13 08:30:47.399806 pontos-23.4.3/LICENSE
--rw-r--r--   0        0        0     3349 2023-04-13 08:30:47.399806 pontos-23.4.3/README.md
--rw-r--r--   0        0        0    97724 2023-04-13 08:30:47.403806 pontos-23.4.3/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-13 08:30:47.403806 pontos-23.4.3/poetry.toml
--rw-r--r--   0        0        0      791 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4427 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/git/__init__.py
--rw-r--r--   0        0        0    16117 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13121 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7508 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3400 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/main.py
--rw-r--r--   0        0        0     7491 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/parser.py
--rw-r--r--   0        0        0    14588 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/release.py
--rw-r--r--   0        0        0    12039 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      749 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0      757 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0      737 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0      753 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0      757 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0      757 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      871 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0      737 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0      737 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      747 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0      709 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      741 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      741 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0      733 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0      733 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      793 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0      802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0      781 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0      802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0      802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      915 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0      781 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0      781 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0      791 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0      751 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      783 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      783 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      727 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0      735 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0      715 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0      731 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0      735 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0      735 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      849 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0      715 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0      715 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      725 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0      687 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      720 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      720 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12050 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1416 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     7752 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     7786 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/errors.py
--rw-r--r--   0        0        0     2809 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13419 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2145 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16023 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/version.py
--rw-r--r--   0        0        0     2890 2023-04-13 08:30:47.411806 pontos-23.4.3/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/git/__init__.py
--rw-r--r--   0        0        0    27772 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6098 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/__init__.py
--rw-r--r--   0        0        0     3190 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_helper.py
--rw-r--r--   0        0        0     8223 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_parser.py
--rw-r--r--   0        0        0    65783 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_release.py
--rw-r--r--   0        0        0    21452 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/test_helper.py
--rw-r--r--   0        0        0     1373 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15227 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/__init__.py
--rw-r--r--   0        0        0    11322 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/test_errors.py
--rw-r--r--   0        0        0     5505 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_version.py
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 pontos-23.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 12:47:13.902953 pontos-23.4.5/LICENSE
+-rw-r--r--   0        0        0     3349 2023-04-24 12:47:13.902953 pontos-23.4.5/README.md
+-rw-r--r--   0        0        0    97087 2023-04-24 12:47:13.906953 pontos-23.4.5/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-24 12:47:13.906953 pontos-23.4.5/poetry.toml
+-rw-r--r--   0        0        0      791 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4427 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     6158 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-04-24 12:47:13.906953 pontos-23.4.5/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3400 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/main.py
+-rw-r--r--   0        0        0     8044 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/parser.py
+-rw-r--r--   0        0        0    12786 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1508 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     7786 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-04-24 12:47:13.910953 pontos-23.4.5/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13419 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2145 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16023 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-04-24 12:47:13.914953 pontos-23.4.5/pontos/version/version.py
+-rw-r--r--   0        0        0     2895 2023-04-24 12:47:13.914953 pontos-23.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-04-24 12:47:13.914953 pontos-23.4.5/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     4385 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-04-24 12:47:13.914953 pontos-23.4.5/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_helper.py
+-rw-r--r--   0        0        0     8597 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_parser.py
+-rw-r--r--   0        0        0    76187 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/test_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-04-24 12:47:13.918953 pontos-23.4.5/tests/version/test_version.py
+-rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 pontos-23.4.5/PKG-INFO
```

### Comparing `pontos-23.4.3/LICENSE` & `pontos-23.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/README.md` & `pontos-23.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/poetry.lock` & `pontos-23.4.5/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 [package.extras]
 doc = ["packaging", "sphinx-autodoc-typehints (>=1.2.0)", "sphinx-rtd-theme"]
 test = ["contextlib2", "coverage[toml] (>=4.5)", "hypothesis (>=4.0)", "mock (>=4)", "pytest (>=7.0)", "pytest-mock (>=3.6.1)", "trustme", "uvloop (<0.15)", "uvloop (>=0.15)"]
 trio = ["trio (>=0.16,<0.22)"]
 
 [[package]]
 name = "astroid"
-version = "2.15.2"
+version = "2.15.3"
 description = "An abstract syntax tree for Python with inference support."
 category = "dev"
 optional = false
 python-versions = ">=3.7.2"
 files = [
-    {file = "astroid-2.15.2-py3-none-any.whl", hash = "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"},
-    {file = "astroid-2.15.2.tar.gz", hash = "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd"},
+    {file = "astroid-2.15.3-py3-none-any.whl", hash = "sha256:f11e74658da0f2a14a8d19776a8647900870a63de71db83713a8e77a6af52662"},
+    {file = "astroid-2.15.3.tar.gz", hash = "sha256:44224ad27c54d770233751315fa7f74c46fa3ee0fab7beef1065f99f09897efe"},
 ]
 
 [package.dependencies]
 lazy-object-proxy = ">=1.4.0"
 typing-extensions = {version = ">=4.0.0", markers = "python_version < \"3.11\""}
 wrapt = [
     {version = ">=1.11,<2", markers = "python_version < \"3.11\""},
@@ -68,61 +68,59 @@
 [package.dependencies]
 pontos = ">=22.8.0"
 rich = ">=12.5.1"
 tomlkit = ">=0.5.11"
 
 [[package]]
 name = "autohooks-plugin-black"
-version = "22.11.0"
+version = "23.4.0"
 description = "An autohooks plugin for python code formatting via black"
 category = "dev"
 optional = false
-python-versions = ">=3.7,<4.0"
+python-versions = ">=3.7.2,<4.0.0"
 files = [
-    {file = "autohooks_plugin_black-22.11.0-py3-none-any.whl", hash = "sha256:e2fd93f1b8995c963356114dafa21ededbcb81f9f6273887a82f26bca5342fe7"},
-    {file = "autohooks_plugin_black-22.11.0.tar.gz", hash = "sha256:c67cfe2a5c008b5596d109a5384c48aa9421a00cf0b49a67c1f380c6fe55155b"},
+    {file = "autohooks_plugin_black-23.4.0-py3-none-any.whl", hash = "sha256:1a65814ab573a40799cf52af7aa026e73ef60d784cf14a8eba33aaf245811899"},
+    {file = "autohooks_plugin_black-23.4.0.tar.gz", hash = "sha256:31b0497f8987def02d5387b9eb03c46837621097c9814d19ff6b9da960867a06"},
 ]
 
 [package.dependencies]
 autohooks = ">=21.6.0"
 black = ">=20.8"
 
 [[package]]
 name = "autohooks-plugin-isort"
-version = "22.8.0"
+version = "23.4.0"
 description = "An autohooks plugin for python code formatting via isort"
 category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 files = [
-    {file = "autohooks-plugin-isort-22.8.0.tar.gz", hash = "sha256:ed798f3ff9a2046ca7943cc25cbdd13afde2ddf82935cead3d61da4e210d070b"},
-    {file = "autohooks_plugin_isort-22.8.0-py3-none-any.whl", hash = "sha256:711ba763f962245cecf74b8d5014a5d5a13dcc1e55c775c4d00c85de8291fa90"},
+    {file = "autohooks_plugin_isort-23.4.0-py3-none-any.whl", hash = "sha256:ada2aad42a2c6e12b4b931a524c971968b4f2426bd7bc96f7806867e1237e449"},
+    {file = "autohooks_plugin_isort-23.4.0.tar.gz", hash = "sha256:309188365bfed8f2841545f7484bc9e4872d031ef8d495128a86e409483c5b6a"},
 ]
 
 [package.dependencies]
 autohooks = ">=21.6.0"
-autohooks-plugin-black = ">=22.7.0"
-autohooks-plugin-pylint = ">=21.6.0"
 isort = ">=5.8.0,<6.0.0"
 
 [[package]]
 name = "autohooks-plugin-pylint"
-version = "22.8.1"
+version = "23.4.0"
 description = "An autohooks plugin for python code linting via pylint"
 category = "dev"
 optional = false
-python-versions = ">=3.7,<4.0"
+python-versions = ">=3.7.2,<4.0.0"
 files = [
-    {file = "autohooks-plugin-pylint-22.8.1.tar.gz", hash = "sha256:d348a61b2b027ad51275dace830ec3643cf14416519eb68167a4bdadfe44ac7e"},
-    {file = "autohooks_plugin_pylint-22.8.1-py3-none-any.whl", hash = "sha256:a7195e0f6a568cd8e0e4a964ebcecf2eb4e457a17a8b3dbc6283dfc546a474c2"},
+    {file = "autohooks_plugin_pylint-23.4.0-py3-none-any.whl", hash = "sha256:2dd581c3764949ef9c1041f5a34206cac796a342a900f47e5f42346e80598009"},
+    {file = "autohooks_plugin_pylint-23.4.0.tar.gz", hash = "sha256:746c24a73bb312e9883f531d13db16da4bd05949969e7adeee3e8d1105a9c6c2"},
 ]
 
 [package.dependencies]
 autohooks = ">=2.2.0"
-pylint = ">=2.8.3,<3.0.0"
+pylint = ">=2.8.3"
 
 [[package]]
 name = "babel"
 version = "2.12.1"
 description = "Internationalization utilities"
 category = "dev"
 optional = false
@@ -487,56 +485,56 @@
 files = [
     {file = "hpack-4.0.0-py3-none-any.whl", hash = "sha256:84a076fad3dc9a9f8063ccb8041ef100867b1878b25ef0ee63847a5d53818a6c"},
     {file = "hpack-4.0.0.tar.gz", hash = "sha256:fc41de0c63e687ebffde81187a948221294896f6bdc0ae2312708df339430095"},
 ]
 
 [[package]]
 name = "httpcore"
-version = "0.16.3"
+version = "0.17.0"
 description = "A minimal low-level HTTP client."
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "httpcore-0.16.3-py3-none-any.whl", hash = "sha256:da1fb708784a938aa084bde4feb8317056c55037247c787bd7e19eb2c2949dc0"},
-    {file = "httpcore-0.16.3.tar.gz", hash = "sha256:c5d6f04e2fc530f39e0c077e6a30caa53f1451096120f1f38b954afd0b17c0cb"},
+    {file = "httpcore-0.17.0-py3-none-any.whl", hash = "sha256:0fdfea45e94f0c9fd96eab9286077f9ff788dd186635ae61b312693e4d943599"},
+    {file = "httpcore-0.17.0.tar.gz", hash = "sha256:cc045a3241afbf60ce056202301b4d8b6af08845e3294055eb26b09913ef903c"},
 ]
 
 [package.dependencies]
 anyio = ">=3.0,<5.0"
 certifi = "*"
 h11 = ">=0.13,<0.15"
 sniffio = ">=1.0.0,<2.0.0"
 
 [package.extras]
 http2 = ["h2 (>=3,<5)"]
 socks = ["socksio (>=1.0.0,<2.0.0)"]
 
 [[package]]
 name = "httpx"
-version = "0.23.3"
+version = "0.24.0"
 description = "The next generation HTTP client."
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "httpx-0.23.3-py3-none-any.whl", hash = "sha256:a211fcce9b1254ea24f0cd6af9869b3d29aba40154e947d2a07bb499b3e310d6"},
-    {file = "httpx-0.23.3.tar.gz", hash = "sha256:9818458eb565bb54898ccb9b8b251a28785dd4a55afbc23d0eb410754fe7d0f9"},
+    {file = "httpx-0.24.0-py3-none-any.whl", hash = "sha256:447556b50c1921c351ea54b4fe79d91b724ed2b027462ab9a329465d147d5a4e"},
+    {file = "httpx-0.24.0.tar.gz", hash = "sha256:507d676fc3e26110d41df7d35ebd8b3b8585052450f4097401c9be59d928c63e"},
 ]
 
 [package.dependencies]
 certifi = "*"
 h2 = {version = ">=3,<5", optional = true, markers = "extra == \"http2\""}
-httpcore = ">=0.15.0,<0.17.0"
-rfc3986 = {version = ">=1.3,<2", extras = ["idna2008"]}
+httpcore = ">=0.15.0,<0.18.0"
+idna = "*"
 sniffio = "*"
 
 [package.extras]
 brotli = ["brotli", "brotlicffi"]
-cli = ["click (>=8.0.0,<9.0.0)", "pygments (>=2.0.0,<3.0.0)", "rich (>=10,<13)"]
+cli = ["click (>=8.0.0,<9.0.0)", "pygments (>=2.0.0,<3.0.0)", "rich (>=10,<14)"]
 http2 = ["h2 (>=3,<5)"]
 socks = ["socksio (>=1.0.0,<2.0.0)"]
 
 [[package]]
 name = "hyperframe"
 version = "6.0.1"
 description = "HTTP/2 framing layer for Python"
@@ -570,22 +568,22 @@
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.3.0"
+version = "6.6.0"
 description = "Read metadata from Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "importlib_metadata-6.3.0-py3-none-any.whl", hash = "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"},
-    {file = "importlib_metadata-6.3.0.tar.gz", hash = "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402"},
+    {file = "importlib_metadata-6.6.0-py3-none-any.whl", hash = "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed"},
+    {file = "importlib_metadata-6.6.0.tar.gz", hash = "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"},
 ]
 
 [package.dependencies]
 zipp = ">=0.5"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
@@ -856,22 +854,22 @@
 linkify = ["linkify-it-py (>=1.0,<2.0)"]
 rtd = ["ipython", "pydata-sphinx-theme (==v0.13.0rc4)", "sphinx-autodoc2 (>=0.4.2,<0.5.0)", "sphinx-book-theme (==1.0.0rc2)", "sphinx-copybutton", "sphinx-design2", "sphinx-pyscript", "sphinx-tippy (>=0.3.1)", "sphinx-togglebutton", "sphinxext-opengraph (>=0.7.5,<0.8.0)", "sphinxext-rediraffe (>=0.2.7,<0.3.0)"]
 testing = ["beautifulsoup4", "coverage[toml]", "pytest (>=7,<8)", "pytest-cov", "pytest-param-files (>=0.3.4,<0.4.0)", "pytest-regressions", "sphinx-pytest"]
 testing-docutils = ["pygments", "pytest (>=7,<8)", "pytest-param-files (>=0.3.4,<0.4.0)"]
 
 [[package]]
 name = "packaging"
-version = "23.0"
+version = "23.1"
 description = "Core utilities for Python packages"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
-    {file = "packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
+    {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
+    {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "pathspec"
 version = "0.11.1"
 description = "Utility library for gitignore style pattern matching of file paths."
 category = "dev"
@@ -896,22 +894,22 @@
 
 [package.extras]
 docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pygments"
-version = "2.14.0"
+version = "2.15.1"
 description = "Pygments is a syntax highlighting package written in Python."
 category = "main"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "Pygments-2.14.0-py3-none-any.whl", hash = "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"},
-    {file = "Pygments-2.14.0.tar.gz", hash = "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297"},
+    {file = "Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
+    {file = "Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pylint"
@@ -1050,41 +1048,23 @@
 urllib3 = ">=1.21.1,<1.27"
 
 [package.extras]
 socks = ["PySocks (>=1.5.6,!=1.5.7)"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<6)"]
 
 [[package]]
-name = "rfc3986"
-version = "1.5.0"
-description = "Validating URI References per RFC 3986"
-category = "main"
-optional = false
-python-versions = "*"
-files = [
-    {file = "rfc3986-1.5.0-py2.py3-none-any.whl", hash = "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"},
-    {file = "rfc3986-1.5.0.tar.gz", hash = "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835"},
-]
-
-[package.dependencies]
-idna = {version = "*", optional = true, markers = "extra == \"idna2008\""}
-
-[package.extras]
-idna2008 = ["idna"]
-
-[[package]]
 name = "rich"
-version = "13.3.3"
+version = "13.3.4"
 description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 category = "main"
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "rich-13.3.3-py3-none-any.whl", hash = "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333"},
-    {file = "rich-13.3.3.tar.gz", hash = "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"},
+    {file = "rich-13.3.4-py3-none-any.whl", hash = "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a"},
+    {file = "rich-13.3.4.tar.gz", hash = "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"},
 ]
 
 [package.dependencies]
 markdown-it-py = ">=2.2.0,<3.0.0"
 pygments = ">=2.13.0,<3.0.0"
 
 [package.extras]
@@ -1155,41 +1135,41 @@
 files = [
     {file = "snowballstemmer-2.2.0-py2.py3-none-any.whl", hash = "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"},
     {file = "snowballstemmer-2.2.0.tar.gz", hash = "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1"},
 ]
 
 [[package]]
 name = "soupsieve"
-version = "2.4"
+version = "2.4.1"
 description = "A modern CSS selector implementation for Beautiful Soup."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "soupsieve-2.4-py3-none-any.whl", hash = "sha256:49e5368c2cda80ee7e84da9dbe3e110b70a4575f196efb74e51b94549d921955"},
-    {file = "soupsieve-2.4.tar.gz", hash = "sha256:e28dba9ca6c7c00173e34e4ba57448f0688bb681b7c5e8bf4971daafc093d69a"},
+    {file = "soupsieve-2.4.1-py3-none-any.whl", hash = "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8"},
+    {file = "soupsieve-2.4.1.tar.gz", hash = "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"},
 ]
 
 [[package]]
 name = "sphinx"
-version = "6.1.3"
+version = "6.2.0"
 description = "Python documentation generator"
 category = "dev"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "Sphinx-6.1.3.tar.gz", hash = "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2"},
-    {file = "sphinx-6.1.3-py3-none-any.whl", hash = "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"},
+    {file = "Sphinx-6.2.0.tar.gz", hash = "sha256:9ef22c2941bc3d0ff080d25a797f7521fc317e857395c712ddde97a19d5bb440"},
+    {file = "sphinx-6.2.0-py3-none-any.whl", hash = "sha256:ff1c2a1167bef9cdcd8ec71339e85fe10f26d4e9ef9382ef10b2687c876c936b"},
 ]
 
 [package.dependencies]
 alabaster = ">=0.7,<0.8"
 babel = ">=2.9"
 colorama = {version = ">=0.4.5", markers = "sys_platform == \"win32\""}
-docutils = ">=0.18,<0.20"
+docutils = ">=0.18.1,<0.20"
 imagesize = ">=1.3"
 importlib-metadata = {version = ">=4.8", markers = "python_version < \"3.10\""}
 Jinja2 = ">=3.0"
 packaging = ">=21.0"
 Pygments = ">=2.13"
 requests = ">=2.25.0"
 snowballstemmer = ">=2.0"
@@ -1199,15 +1179,15 @@
 sphinxcontrib-jsmath = "*"
 sphinxcontrib-qthelp = "*"
 sphinxcontrib-serializinghtml = ">=1.1.5"
 
 [package.extras]
 docs = ["sphinxcontrib-websupport"]
 lint = ["docutils-stubs", "flake8 (>=3.5.0)", "flake8-simplify", "isort", "mypy (>=0.990)", "ruff", "sphinx-lint", "types-requests"]
-test = ["cython", "html5lib", "pytest (>=4.6)"]
+test = ["cython", "filelock", "html5lib", "pytest (>=4.6)"]
 
 [[package]]
 name = "sphinx-autobuild"
 version = "2021.3.14"
 description = "Rebuild Sphinx documentation on changes, with live-reload in the browser."
 category = "dev"
 optional = false
@@ -1360,31 +1340,31 @@
 files = [
     {file = "tomlkit-0.11.7-py3-none-any.whl", hash = "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c"},
     {file = "tomlkit-0.11.7.tar.gz", hash = "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"},
 ]
 
 [[package]]
 name = "tornado"
-version = "6.2"
+version = "6.3.1"
 description = "Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed."
 category = "dev"
 optional = false
-python-versions = ">= 3.7"
+python-versions = ">= 3.8"
 files = [
-    {file = "tornado-6.2-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:20f638fd8cc85f3cbae3c732326e96addff0a15e22d80f049e00121651e82e72"},
-    {file = "tornado-6.2-cp37-abi3-macosx_10_9_x86_64.whl", hash = "sha256:87dcafae3e884462f90c90ecc200defe5e580a7fbbb4365eda7c7c1eb809ebc9"},
-    {file = "tornado-6.2-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ba09ef14ca9893954244fd872798b4ccb2367c165946ce2dd7376aebdde8e3ac"},
-    {file = "tornado-6.2-cp37-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b8150f721c101abdef99073bf66d3903e292d851bee51910839831caba341a75"},
-    {file = "tornado-6.2-cp37-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d3a2f5999215a3a06a4fc218026cd84c61b8b2b40ac5296a6db1f1451ef04c1e"},
-    {file = "tornado-6.2-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:5f8c52d219d4995388119af7ccaa0bcec289535747620116a58d830e7c25d8a8"},
-    {file = "tornado-6.2-cp37-abi3-musllinux_1_1_i686.whl", hash = "sha256:6fdfabffd8dfcb6cf887428849d30cf19a3ea34c2c248461e1f7d718ad30b66b"},
-    {file = "tornado-6.2-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:1d54d13ab8414ed44de07efecb97d4ef7c39f7438cf5e976ccd356bebb1b5fca"},
-    {file = "tornado-6.2-cp37-abi3-win32.whl", hash = "sha256:5c87076709343557ef8032934ce5f637dbb552efa7b21d08e89ae7619ed0eb23"},
-    {file = "tornado-6.2-cp37-abi3-win_amd64.whl", hash = "sha256:e5f923aa6a47e133d1cf87d60700889d7eae68988704e20c75fb2d65677a8e4b"},
-    {file = "tornado-6.2.tar.gz", hash = "sha256:9b630419bde84ec666bfd7ea0a4cb2a8a651c2d5cccdbdd1972a0c859dfc3c13"},
+    {file = "tornado-6.3.1-cp38-abi3-macosx_10_9_universal2.whl", hash = "sha256:db181eb3df8738613ff0a26f49e1b394aade05034b01200a63e9662f347d4415"},
+    {file = "tornado-6.3.1-cp38-abi3-macosx_10_9_x86_64.whl", hash = "sha256:b4e7b956f9b5e6f9feb643ea04f07e7c6b49301e03e0023eedb01fa8cf52f579"},
+    {file = "tornado-6.3.1-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9661aa8bc0e9d83d757cd95b6f6d1ece8ca9fd1ccdd34db2de381e25bf818233"},
+    {file = "tornado-6.3.1-cp38-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:81c17e0cc396908a5e25dc8e9c5e4936e6dfd544c9290be48bd054c79bcad51e"},
+    {file = "tornado-6.3.1-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a27a1cfa9997923f80bdd962b3aab048ac486ad8cfb2f237964f8ab7f7eb824b"},
+    {file = "tornado-6.3.1-cp38-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:d7117f3c7ba5d05813b17a1f04efc8e108a1b811ccfddd9134cc68553c414864"},
+    {file = "tornado-6.3.1-cp38-abi3-musllinux_1_1_i686.whl", hash = "sha256:ffdce65a281fd708da5a9def3bfb8f364766847fa7ed806821a69094c9629e8a"},
+    {file = "tornado-6.3.1-cp38-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:90f569a35a8ec19bde53aa596952071f445da678ec8596af763b9b9ce07605e6"},
+    {file = "tornado-6.3.1-cp38-abi3-win32.whl", hash = "sha256:3455133b9ff262fd0a75630af0a8ee13564f25fb4fd3d9ce239b8a7d3d027bf8"},
+    {file = "tornado-6.3.1-cp38-abi3-win_amd64.whl", hash = "sha256:1285f0691143f7ab97150831455d4db17a267b59649f7bd9700282cba3d5e771"},
+    {file = "tornado-6.3.1.tar.gz", hash = "sha256:5e2f49ad371595957c50e42dd7e5c14d64a6843a3cf27352b69c706d1b5918af"},
 ]
 
 [[package]]
 name = "typing-extensions"
 version = "4.5.0"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 category = "main"
@@ -1512,8 +1492,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "2bb914b7a9a6c268d2ff81b9c6eb2d989199aa1b65c558a01ffe782ccda2c545"
+content-hash = "5ed66859a1d2cde2199521fae6e6bd13a66e1417eb9e7ed8ce2d25b5789dd017"
```

### Comparing `pontos-23.4.3/pontos/__init__.py` & `pontos-23.4.5/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/changelog/__init__.py` & `pontos-23.4.5/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/changelog/conventional_commits.py` & `pontos-23.4.5/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/changelog/errors.py` & `pontos-23.4.5/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/changelog/main.py` & `pontos-23.4.5/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/errors.py` & `pontos-23.4.5/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/git/__init__.py` & `pontos-23.4.5/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/git/git.py` & `pontos-23.4.5/pontos/git/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         cmd_args = ["git"]
         cmd_args.extend(args)
         output = subprocess.run(
             cmd_args,
             cwd=fspath(cwd) if cwd else None,
             check=True,
             stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
             encoding="utf8",
             errors="replace",
         )
         return output.stdout
     except subprocess.CalledProcessError as e:
         if ignore_errors:
             return ""
```

### Comparing `pontos-23.4.3/pontos/git/status.py` & `pontos-23.4.5/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/__init__.py` & `pontos-23.4.5/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/__init__.py` & `pontos-23.4.5/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/argparser.py` & `pontos-23.4.5/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/cmds.py` & `pontos-23.4.5/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/core.py` & `pontos-23.4.5/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/env.py` & `pontos-23.4.5/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/errors.py` & `pontos-23.4.5/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/event.py` & `pontos-23.4.5/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/actions/main.py` & `pontos-23.4.5/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/__init__.py` & `pontos-23.4.5/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/api.py` & `pontos-23.4.5/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/artifacts.py` & `pontos-23.4.5/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/branch.py` & `pontos-23.4.5/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/client.py` & `pontos-23.4.5/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/contents.py` & `pontos-23.4.5/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/errors.py` & `pontos-23.4.5/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/helper.py` & `pontos-23.4.5/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/labels.py` & `pontos-23.4.5/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/organizations.py` & `pontos-23.4.5/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/pull_requests.py` & `pontos-23.4.5/pontos/github/api/pull_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,14 @@
         params = {"per_page": "100"}
         api = f"/repos/{repo}/issues/{pull_request}/comments"
 
         async for response in self._client.get_all(api, params=params):
             response.raise_for_status()
 
             for comment in response.json():
-                print(comment)
                 yield Comment.from_dict(comment)
 
     async def files(
         self,
         repo: str,
         pull_request: Union[int, str],
         *,
```

### Comparing `pontos-23.4.3/pontos/github/api/release.py` & `pontos-23.4.5/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/repositories.py` & `pontos-23.4.5/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/search.py` & `pontos-23.4.5/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/tags.py` & `pontos-23.4.5/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/teams.py` & `pontos-23.4.5/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/api/workflows.py` & `pontos-23.4.5/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/argparser.py` & `pontos-23.4.5/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/cmds.py` & `pontos-23.4.5/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/main.py` & `pontos-23.4.5/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/__init__.py` & `pontos-23.4.5/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/artifact.py` & `pontos-23.4.5/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/base.py` & `pontos-23.4.5/pontos/github/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,15 @@
     CHECK_SUITE = "check_suite"
     CREATE = "create"
     DELETE = "delete"
     DEPLOYMENT = "deployment"
     DEPLOYMENT_STATUS = "deployment_status"
     DISCUSSION = "discussion"
     DISCUSSION_COMMENT = "discussion_comment"
+    DYNAMIC = "dynamic"
     FORK = "fork"
     GOLLUM = "gollum"
     ISSUE_COMMENT = "issue_comment"
     ISSUES = "issues"
     LABEL = "label"
     MERGE_GROUP = "merge_group"
     MILESTONE = "milestone"
```

### Comparing `pontos-23.4.3/pontos/github/models/branch.py` & `pontos-23.4.5/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/organization.py` & `pontos-23.4.5/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/pull_request.py` & `pontos-23.4.5/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/release.py` & `pontos-23.4.5/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/search.py` & `pontos-23.4.5/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/tag.py` & `pontos-23.4.5/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/models/workflow.py` & `pontos-23.4.5/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/pr_template.md` & `pontos-23.4.5/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/script/__init__.py` & `pontos-23.4.5/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/script/errors.py` & `pontos-23.4.5/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/script/load.py` & `pontos-23.4.5/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/github/script/parser.py` & `pontos-23.4.5/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/helper.py` & `pontos-23.4.5/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/models/__init__.py` & `pontos-23.4.5/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/__init__.py` & `pontos-23.4.5/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/api.py` & `pontos-23.4.5/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/cpe/__init__.py` & `pontos-23.4.5/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/cpe/api.py` & `pontos-23.4.5/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/cve/__init__.py` & `pontos-23.4.5/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/cve/api.py` & `pontos-23.4.5/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/models/__init__.py` & `pontos-23.4.5/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/models/cpe.py` & `pontos-23.4.5/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/models/cve.py` & `pontos-23.4.5/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/models/cvss_v2.py` & `pontos-23.4.5/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/nvd/models/cvss_v3.py` & `pontos-23.4.5/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/pontos.py` & `pontos-23.4.5/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/release/__init__.py` & `pontos-23.4.5/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/release/helper.py` & `pontos-23.4.5/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/release/main.py` & `pontos-23.4.5/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/release/parser.py` & `pontos-23.4.5/pontos/release/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -103,14 +103,20 @@
         "--release-version",
         help=(
             "Will release changelog as version. "
             "Default: lookup version in project definition."
         ),
         action=ReleaseVersionAction,
     )
+    release_parser.add_argument(
+        "--release-series",
+        help="Create a release for a release series. Setting a release series "
+        "is required if the latest tag version is newer then the to be "
+        'released version. Examples: "1.2", "2", "22.4"',
+    )
 
     release_parser.add_argument(
         "--next-version",
         help=(
             "Sets the next version in project definition "
             "after the release. Default: set to next dev version"
         ),
@@ -169,14 +175,20 @@
         type=versioning_scheme_argument_type,
     )
     sign_parser.add_argument(
         "--release-version",
         help="Will release changelog as version. Must be PEP 440 compliant.",
     )
     sign_parser.add_argument(
+        "--release-series",
+        help="Sign release files for a release series. Setting a release "
+        "series is required if the latest tag version is newer then the to be "
+        'signed version. Examples: "1.2", "2", "22.4"',
+    )
+    sign_parser.add_argument(
         "--git-tag-prefix",
         default="v",
         help="Prefix for git tag versions. Default: %(default)s",
     )
     sign_parser.add_argument(
         "--project",
         help="The github project",
```

### Comparing `pontos-23.4.3/pontos/release/release.py` & `pontos-23.4.5/pontos/release/release.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,96 +16,89 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import asyncio
 from argparse import Namespace
 from enum import IntEnum, auto
 from pathlib import Path
-from typing import Iterable, Optional
+from typing import Optional
 
 import httpx
 
 from pontos.changelog.conventional_commits import ChangelogBuilder
 from pontos.errors import PontosError
 from pontos.git import Git
 from pontos.github.api import GitHubAsyncRESTApi
 from pontos.terminal import Terminal
 from pontos.version import Version, VersionCalculator, VersionError
-from pontos.version.helper import get_last_release_versions
+from pontos.version.helper import get_last_release_version
 from pontos.version.project import Project
 from pontos.version.schemes import VersioningScheme
 
 from .helper import ReleaseType, find_signing_key, get_git_repository_name
 
 
 class ReleaseReturnValue(IntEnum):
     """
     Possible return values of ReleaseCommand
     """
 
     SUCCESS = 0
     PROJECT_SETTINGS_NOT_FOUND = auto()
     TOKEN_MISSING = auto()
+    NO_LAST_RELEASE_VERSION = auto()
     NO_RELEASE_VERSION = auto()
     ALREADY_TAKEN = auto()
     CREATE_RELEASE_ERROR = auto()
     UPDATE_VERSION_ERROR = auto()
     UPDATE_VERSION_AFTER_RELEASE_ERROR = auto()
 
 
-def _get_version(
-    release_version: Version, last_release_versions: Iterable[Version]
-) -> Optional[Version]:
-    for version in last_release_versions:
-        if release_version > version:
-            return version
-
-    return None
-
-
 class ReleaseCommand:
     """
     A CLI command for creating a release
 
     Args:
         terminal: A Terminal for output
     """
 
     def __init__(self, terminal: Terminal) -> None:
         self.git = Git()
         self.terminal = terminal
 
-    def _get_release_version(
+    def _get_next_release_version(
         self,
         *,
-        current_version: Version,
+        last_release_version: Version,
         calculator: VersionCalculator,
         release_type: ReleaseType,
         release_version: Optional[Version],
     ) -> Version:
         if release_type == ReleaseType.CALENDAR:
-            return calculator.next_calendar_version(current_version)
+            return calculator.next_calendar_version(last_release_version)
 
         if release_type == ReleaseType.PATCH:
-            return calculator.next_patch_version(current_version)
+            return calculator.next_patch_version(last_release_version)
 
         if release_type == ReleaseType.MINOR:
-            return calculator.next_minor_version(current_version)
+            return calculator.next_minor_version(last_release_version)
 
         if release_type == ReleaseType.MAJOR:
-            return calculator.next_major_version(current_version)
+            return calculator.next_major_version(last_release_version)
 
         if release_type == ReleaseType.ALPHA:
-            return calculator.next_alpha_version(current_version)
+            return calculator.next_alpha_version(last_release_version)
 
         if release_type == ReleaseType.BETA:
-            return calculator.next_beta_version(current_version)
+            return calculator.next_beta_version(last_release_version)
 
         if release_type == ReleaseType.RELEASE_CANDIDATE:
-            return calculator.next_release_candidate_version(current_version)
+            return calculator.next_release_candidate_version(
+                last_release_version
+            )
 
         if not release_version:
             raise VersionError(
                 "No release version provided. Either use a different release "
                 "strategy or provide a release version."
             )
         return release_version
@@ -141,82 +134,14 @@
             repo,
             git_version,
             name=f"{self.project} {release_version}",
             body=release_text,
             prerelease=release_version.is_pre_release,
         )
 
-    def _get_last_release(
-        self,
-        release_type: ReleaseType,
-        release_version: Version,
-        calculator: VersionCalculator,
-    ) -> Version:
-        # try to get last tag for the matching release series
-        if release_type in [
-            ReleaseType.PATCH,
-            ReleaseType.ALPHA,
-            ReleaseType.BETA,
-            ReleaseType.RELEASE_CANDIDATE,
-        ]:
-            tag_name = (
-                f"{self.git_tag_prefix}"
-                f"{release_version.major}.{release_version.minor}.*"
-            )
-        elif release_type == ReleaseType.MINOR:
-            tag_name = f"{self.git_tag_prefix}{release_version.major}.*"
-        else:
-            tag_name = None
-
-        last_release_versions = get_last_release_versions(
-            calculator.version_from_string,
-            git_tag_prefix=self.git_tag_prefix,
-            ignore_pre_releases=not release_version.is_pre_release,
-            tag_name=tag_name,
-        )
-
-        last_release_version = _get_version(
-            release_version, last_release_versions
-        )
-
-        if tag_name and not last_release_version:
-            if release_type in [
-                ReleaseType.PATCH,
-                ReleaseType.ALPHA,
-                ReleaseType.BETA,
-                ReleaseType.RELEASE_CANDIDATE,
-            ]:
-                tag_name = f"{self.git_tag_prefix}{release_version.major}.*"
-            else:
-                tag_name = None
-
-            last_release_versions = get_last_release_versions(
-                calculator.version_from_string,
-                git_tag_prefix=self.git_tag_prefix,
-                ignore_pre_releases=not release_version.is_pre_release,
-                tag_name=tag_name,
-            )
-
-            last_release_version = _get_version(
-                release_version, last_release_versions
-            )
-
-            if not last_release_version:
-                last_release_versions = get_last_release_versions(
-                    calculator.version_from_string,
-                    git_tag_prefix=self.git_tag_prefix,
-                    ignore_pre_releases=not release_version.is_pre_release,
-                )
-
-                last_release_version = _get_version(
-                    release_version, last_release_versions
-                )
-
-        return last_release_version
-
     async def run(
         self,
         *,
         token: str,
         space: str,
         project: Optional[str],
         versioning_scheme: VersioningScheme,
@@ -224,14 +149,15 @@
         release_version: Optional[Version],
         next_version: Optional[str],
         git_signing_key: str,
         git_remote_name: Optional[str],
         git_tag_prefix: Optional[str],
         cc_config: Optional[Path],
         local: Optional[bool] = False,
+        release_series: Optional[str] = None,
     ) -> ReleaseReturnValue:
         """
         Create a release
 
         Args:
             token: A token for creating a release on GitHub
             space: GitHub username or organization. Required for generating
@@ -241,103 +167,115 @@
             versioning_scheme: The versioning scheme to use for version parsing
                 and calculation
             release_type: Type of the release to prepare. Defines the release
                 version. PATCH increments the bugfix version. CALENDAR creates
                 a new CalVer release version. VERSION uses the provided
                 release_version.
             release_version: Optional release version to use. If not set the
-                current version will be determined from the project.
+                to be released version will be determined from the project.
             next_version: Optional version to set after the release.
+                If not set the next development version will be set.
             git_signing_key: A GPG key ID to use for creating signatures.
             git_remote_name: Name of the git remote to use.
             git_tag_prefix: An optional prefix to use for creating a git tag
                 from the release version.
             cc_config: A path to a settings file for creating conventional
                 commits.
             local: Only create changes locally and don't push changes to
                 remote repository. Also don't create a GitHub release.
+            release_series: Optional release series to use.
+                For example: "1.2", "2", "23".
         """
         git_signing_key = (
             git_signing_key
             if git_signing_key is not None
             else find_signing_key(self.terminal)
         )
         self.git_tag_prefix = git_tag_prefix or ""
         self.project = (
             project if project is not None else get_git_repository_name()
         )
         self.space = space
 
+        self.terminal.info(
+            f"Using versioning scheme {versioning_scheme.__class__.__name__}"
+        )
+
         try:
-            project = Project(versioning_scheme)
+            last_release_version = get_last_release_version(
+                parse_version=versioning_scheme.parse_version,
+                git_tag_prefix=self.git_tag_prefix,
+                tag_name=f"{self.git_tag_prefix}{release_series}.*"
+                if release_series
+                else None,
+            )
         except PontosError as e:
-            self.terminal.error(f"Unable to determine project settings. {e}")
-            return ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
+            self.terminal.error(
+                f"Could not determine last release version. {e}"
+            )
+            return ReleaseReturnValue.NO_LAST_RELEASE_VERSION
 
-        self.terminal.info(f"Using versioning scheme {versioning_scheme}")
+        if not last_release_version:
+            if not release_version:
+                self.terminal.error("Unable to determine last release version.")
+                return ReleaseReturnValue.NO_LAST_RELEASE_VERSION
+            else:
+                self.terminal.info(
+                    f"Creating the initial release {release_version}"
+                )
+
+        else:
+            self.terminal.info(f"Last release was {last_release_version}")
 
         calculator = versioning_scheme.calculator()
 
         try:
-            current_version = project.get_current_version()
-
-            self.terminal.info(f"Current version is {current_version}")
-
-            release_version = self._get_release_version(
-                current_version=current_version,
+            release_version = self._get_next_release_version(
+                last_release_version=last_release_version,
                 calculator=calculator,
                 release_type=release_type,
                 release_version=release_version,
             )
         except VersionError as e:
             self.terminal.error(f"Unable to determine release version. {e}")
             return ReleaseReturnValue.NO_RELEASE_VERSION
 
-        if not release_version:
-            return ReleaseReturnValue.NO_RELEASE_VERSION
-
         self.terminal.info(f"Preparing the release {release_version}")
 
         git_version = f"{self.git_tag_prefix}{release_version}"
 
         if self._has_tag(git_version):
             self.terminal.error(f"Git tag {git_version} already exists.")
             return ReleaseReturnValue.ALREADY_TAKEN
 
         try:
+            project = Project(versioning_scheme)
+        except PontosError as e:
+            self.terminal.error(f"Unable to determine project settings. {e}")
+            return ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
+
+        try:
             updated = project.update_version(release_version)
 
             self.terminal.ok(f"Updated version to {release_version}")
 
             for path in updated.changed_files:
                 self.terminal.info(f"Adding changes of {path}")
                 self.git.add(path)
         except VersionError as e:
             self.terminal.error(
                 f"Unable to update version to {release_version}. {e}"
             )
             return ReleaseReturnValue.UPDATE_VERSION_ERROR
 
-        last_release_version = self._get_last_release(
-            release_type=release_type,
-            release_version=release_version,
-            calculator=calculator,
+        self.terminal.info(
+            f"Creating changelog for {release_version} since "
+            f"{last_release_version}"
         )
 
-        if not last_release_version:
-            self.terminal.info(
-                f"No last release found. Creating changelog for the initial "
-                f"release {release_version}"
-            )
-        else:
-            self.terminal.info(
-                f"Creating changelog for {release_version} since "
-                f"{last_release_version}"
-            )
-
         release_text = self._create_changelog(
             release_version, last_release_version, cc_config
         )
 
         self.terminal.info("Committing changes")
 
         commit_msg = f"Automatic release to {release_version}"
@@ -421,9 +359,10 @@
             release_version=args.release_version,
             next_version=args.next_version,
             git_remote_name=args.git_remote_name,
             git_signing_key=args.git_signing_key,
             git_tag_prefix=args.git_tag_prefix,
             cc_config=args.cc_config,
             local=args.local,
+            release_series=args.release_series,
         )
     )
```

### Comparing `pontos-23.4.3/pontos/release/sign.py` & `pontos-23.4.5/pontos/release/sign.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,22 +178,23 @@
                 f"{stderr.decode(errors='replace')}"
             )
 
     async def run(
         self,
         *,
         token: str,
-        dry_run: Optional[bool] = False,
         space: str,
-        project: Optional[str],
         versioning_scheme: VersioningScheme,
-        git_tag_prefix: Optional[str],
-        release_version: Optional[Version],
         signing_key: str,
         passphrase: str,
+        dry_run: Optional[bool] = False,
+        project: Optional[str],
+        git_tag_prefix: Optional[str],
+        release_version: Optional[Version],
+        release_series: Optional[str] = None,
     ) -> SignReturnValue:
         """
         Sign a release
 
         Args:
             token: A token for creating a release on GitHub
             dry_run: True to not upload the signature files
@@ -205,39 +206,48 @@
                 and calculation
             git_tag_prefix: An optional prefix to use for handling a git tag
                 from the release version.
             release_version: Optional release version to use. If not set the
                 current version will be determined from the project.
             signing_key: A GPG key ID to use for creating signatures.
             passphrase: Passphrase for the signing key
+            release_series: Optional release series to use.
+                For example: "1.2", "2", "23".
         """
         if not token and not dry_run:
             # dry run doesn't upload assets. therefore a token MAY NOT be
             # required # for public repositories.
             self.terminal.error(
                 "Token is missing. The GitHub token is required to upload "
                 "signature files."
             )
             return SignReturnValue.TOKEN_MISSING
 
+        self.terminal.info(
+            f"Using versioning scheme {versioning_scheme.__class__.__name__}"
+        )
+
         try:
             project = (
                 project if project is not None else get_git_repository_name()
             )
-        except GitError:
-            self.terminal.error("Could not determine project. {e}")
+        except GitError as e:
+            self.terminal.error(f"Could not determine project. {e}")
             return SignReturnValue.NO_PROJECT
 
         try:
             release_version = (
                 release_version
                 if release_version is not None
                 else get_last_release_version(
                     versioning_scheme.parse_version,
                     git_tag_prefix=git_tag_prefix,
+                    tag_name=f"{git_tag_prefix}{release_series}.*"
+                    if release_series
+                    else None,
                 )
             )
         except PontosError as e:
             self.terminal.error(f"Could not determine release version. {e}")
             return SignReturnValue.NO_RELEASE_VERSION
 
         if not release_version:
@@ -367,9 +377,10 @@
             project=args.project,
             space=args.space,
             versioning_scheme=args.versioning_scheme,
             git_tag_prefix=args.git_tag_prefix,
             release_version=args.release_version,
             signing_key=args.signing_key,
             passphrase=args.passphrase,
+            release_series=args.release_series,
         )
     )
```

### Comparing `pontos-23.4.3/pontos/terminal/__init__.py` & `pontos-23.4.5/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/terminal/null.py` & `pontos-23.4.5/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/terminal/rich.py` & `pontos-23.4.5/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/terminal/terminal.py` & `pontos-23.4.5/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/testing/__init__.py` & `pontos-23.4.5/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/updateheader/__init__.py` & `pontos-23.4.5/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/updateheader/__main__.py` & `pontos-23.4.5/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash` & `pontos-23.4.5/tests/git/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-#!/bin/bash
-# Copyright (C) <year> <company>
+# Copyright (C) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
+# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Affero General Public License
+# You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.c` & `pontos-23.4.5/tests/github/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-/* Copyright (C) <year> <company>
- *
- * SPDX-License-Identifier: AGPL-3.0-or-later
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU Affero General Public License as
- * published by the Free Software Foundation, either version 3 of the
- * License, or (at your option) any later version.
- *
- * This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU Affero General Public License for more details.
- *
- * You should have received a copy of the GNU Affero General Public License
- * along with this program.  If not, see <http://www.gnu.org/licenses/>.
- */
+# Copyright (C) 2022 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake` & `pontos-23.4.5/tests/github/actions/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright (C) <year> <company>
+# Copyright (C) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
+# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Affero General Public License
+# You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.go` & `pontos-23.4.5/tests/github/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-// Copyright (C) <year> <company>
-//
-// SPDX-License-Identifier: AGPL-3.0-or-later
-//
-// This program is free software: you can redistribute it and/or modify
-// it under the terms of the GNU Affero General Public License as
-// published by the Free Software Foundation, either version 3 of the
-// License, or (at your option) any later version.
-//
-// This program is distributed in the hope that it will be useful,
-// but WITHOUT ANY WARRANTY; without even the implied warranty of
-// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-// GNU Affero General Public License for more details.
-//
-// You should have received a copy of the GNU Affero General Public License
-// along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# Copyright (C) 2022 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.h` & `pontos-23.4.5/tests/github/script/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-/* Copyright (C) <year> <company>
- *
- * SPDX-License-Identifier: AGPL-3.0-or-later
- *
- * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU Affero General Public License as
- * published by the Free Software Foundation, either version 3 of the
- * License, or (at your option) any later version.
- *
- * This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU Affero General Public License for more details.
- *
- * You should have received a copy of the GNU Affero General Public License
- * along with this program.  If not, see <http://www.gnu.org/licenses/>.
- */
+# Copyright (C) 2022 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.js` & `pontos-23.4.5/tests/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-00000000: 2f2a 2043 6f70 7972 6967 6874 2028 4329  /* Copyright (C)
-00000010: 203c 7965 6172 3e20 3c63 6f6d 7061 6e79   <year> <company
-00000020: 3e0a 202a 0a20 2a20 5350 4458 2d4c 6963  >. *. * SPDX-Lic
-00000030: 656e 7365 2d49 6465 6e74 6966 6965 723a  ense-Identifier:
-00000040: 2041 4750 4c2d 332e 302d 6f72 2d6c 6174   AGPL-3.0-or-lat
-00000050: 6572 0a20 2a0a 202a 2054 6869 7320 7072  er. *. * This pr
-00000060: 6f67 7261 6d20 6973 2066 7265 6520 736f  ogram is free so
-00000070: 6674 7761 7265 3a20 796f 7520 6361 6e20  ftware: you can 
-00000080: 7265 6469 7374 7269 6275 7465 2069 7420  redistribute it 
-00000090: 616e 642f 6f72 206d 6f64 6966 790a 202a  and/or modify. *
-000000a0: 2069 7420 756e 6465 7220 7468 6520 7465   it under the te
-000000b0: 726d 7320 6f66 2074 6865 2047 4e55 2041  rms of the GNU A
-000000c0: 6666 6572 6f20 4765 6e65 7261 6c20 5075  ffero General Pu
-000000d0: 626c 6963 204c 6963 656e 7365 2061 730a  blic License as.
-000000e0: 202a 2070 7562 6c69 7368 6564 2062 7920   * published by 
-000000f0: 7468 6520 4672 6565 2053 6f66 7477 6172  the Free Softwar
-00000100: 6520 466f 756e 6461 7469 6f6e 2c20 6569  e Foundation, ei
-00000110: 7468 6572 2076 6572 7369 6f6e 2033 206f  ther version 3 o
-00000120: 6620 7468 650a 202a 204c 6963 656e 7365  f the. * License
-00000130: 2c20 6f72 2028 6174 2079 6f75 7220 6f70  , or (at your op
-00000140: 7469 6f6e 2920 616e 7920 6c61 7465 7220  tion) any later 
-00000150: 7665 7273 696f 6e2e 0a20 2a0a 202a 2054  version.. *. * T
-00000160: 6869 7320 7072 6f67 7261 6d20 6973 2064  his program is d
-00000170: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
-00000180: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
-00000190: 696c 6c20 6265 2075 7365 6675 6c2c 0a20  ill be useful,. 
-000001a0: 2a20 6275 7420 5749 5448 4f55 5420 414e  * but WITHOUT AN
-000001b0: 5920 5741 5252 414e 5459 3b20 7769 7468  Y WARRANTY; with
-000001c0: 6f75 7420 6576 656e 2074 6865 2069 6d70  out even the imp
-000001d0: 6c69 6564 2077 6172 7261 6e74 7920 6f66  lied warranty of
-000001e0: 0a20 2a20 4d45 5243 4841 4e54 4142 494c  . * MERCHANTABIL
-000001f0: 4954 5920 6f72 2046 4954 4e45 5353 2046  ITY or FITNESS F
-00000200: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
-00000210: 5055 5250 4f53 452e 2020 5365 6520 7468  PURPOSE.  See th
-00000220: 650a 202a 2047 4e55 2041 6666 6572 6f20  e. * GNU Affero 
-00000230: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00000240: 6963 656e 7365 2066 6f72 206d 6f72 6520  icense for more 
-00000250: 6465 7461 696c 732e 0a20 2a0a 202a 2059  details.. *. * Y
-00000260: 6f75 2073 686f 756c 6420 6861 7665 2072  ou should have r
-00000270: 6563 6569 7665 6420 6120 636f 7079 206f  eceived a copy o
-00000280: 6620 7468 6520 474e 5520 4166 6665 726f  f the GNU Affero
-00000290: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-000002a0: 4c69 6365 6e73 650a 202a 2061 6c6f 6e67  License. * along
-000002b0: 2077 6974 6820 7468 6973 2070 726f 6772   with this progr
-000002c0: 616d 2e20 2049 6620 6e6f 742c 2073 6565  am.  If not, see
-000002d0: 203c 6874 7470 3a2f 2f77 7777 2e67 6e75   <http://www.gnu
-000002e0: 2e6f 7267 2f6c 6963 656e 7365 732f 3e2e  .org/licenses/>.
-000002f0: 0a20 2a2f 0a                             . */.
+00000000: 2320 436f 7079 7269 6768 7420 2843 2920  # Copyright (C) 
+00000010: 3230 3232 2047 7265 656e 626f 6e65 2041  2022 Greenbone A
+00000020: 470a 230a 2320 5350 4458 2d4c 6963 656e  G.#.# SPDX-Licen
+00000030: 7365 2d49 6465 6e74 6966 6965 723a 2047  se-Identifier: G
+00000040: 504c 2d33 2e30 2d6f 722d 6c61 7465 720a  PL-3.0-or-later.
+00000050: 230a 2320 5468 6973 2070 726f 6772 616d  #.# This program
+00000060: 2069 7320 6672 6565 2073 6f66 7477 6172   is free softwar
+00000070: 653a 2079 6f75 2063 616e 2072 6564 6973  e: you can redis
+00000080: 7472 6962 7574 6520 6974 2061 6e64 2f6f  tribute it and/o
+00000090: 7220 6d6f 6469 6679 0a23 2069 7420 756e  r modify.# it un
+000000a0: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
+000000b0: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
+000000c0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000000d0: 6173 2070 7562 6c69 7368 6564 2062 790a  as published by.
+000000e0: 2320 7468 6520 4672 6565 2053 6f66 7477  # the Free Softw
+000000f0: 6172 6520 466f 756e 6461 7469 6f6e 2c20  are Foundation, 
+00000100: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
+00000110: 206f 6620 7468 6520 4c69 6365 6e73 652c   of the License,
+00000120: 206f 720a 2320 2861 7420 796f 7572 206f   or.# (at your o
+00000130: 7074 696f 6e29 2061 6e79 206c 6174 6572  ption) any later
+00000140: 2076 6572 7369 6f6e 2e0a 230a 2320 5468   version..#.# Th
+00000150: 6973 2070 726f 6772 616d 2069 7320 6469  is program is di
+00000160: 7374 7269 6275 7465 6420 696e 2074 6865  stributed in the
+00000170: 2068 6f70 6520 7468 6174 2069 7420 7769   hope that it wi
+00000180: 6c6c 2062 6520 7573 6566 756c 2c0a 2320  ll be useful,.# 
+00000190: 6275 7420 5749 5448 4f55 5420 414e 5920  but WITHOUT ANY 
+000001a0: 5741 5252 414e 5459 3b20 7769 7468 6f75  WARRANTY; withou
+000001b0: 7420 6576 656e 2074 6865 2069 6d70 6c69  t even the impli
+000001c0: 6564 2077 6172 7261 6e74 7920 6f66 0a23  ed warranty of.#
+000001d0: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
+000001e0: 206f 7220 4649 544e 4553 5320 464f 5220   or FITNESS FOR 
+000001f0: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
+00000200: 504f 5345 2e20 2053 6565 2074 6865 0a23  POSE.  See the.#
+00000210: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
+00000220: 6c69 6320 4c69 6365 6e73 6520 666f 7220  lic License for 
+00000230: 6d6f 7265 2064 6574 6169 6c73 2e0a 230a  more details..#.
+00000240: 2320 596f 7520 7368 6f75 6c64 2068 6176  # You should hav
+00000250: 6520 7265 6365 6976 6564 2061 2063 6f70  e received a cop
+00000260: 7920 6f66 2074 6865 2047 4e55 2047 656e  y of the GNU Gen
+00000270: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
+00000280: 6e73 650a 2320 616c 6f6e 6720 7769 7468  nse.# along with
+00000290: 2074 6869 7320 7072 6f67 7261 6d2e 2020   this program.  
+000002a0: 4966 206e 6f74 2c20 7365 6520 3c68 7474  If not, see <htt
+000002b0: 703a 2f2f 7777 772e 676e 752e 6f72 672f  p://www.gnu.org/
+000002c0: 6c69 6365 6e73 6573 2f3e 2e0a            licenses/>..
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl` & `pontos-23.4.5/tests/terminal/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# Copyright (C) <year> <company>
-# Some text descriptions might be excerpted from (a) referenced
-# source(s), and are Copyright (C) by the respective right holder(s).
+# -*- coding: utf-8 -*-
+# Copyright (C) 2020-2022 Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
+# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Affero General Public License
+# You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.po` & `pontos-23.4.5/tests/nvd/cpe/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright (C) <year> <company>
+# Copyright (C) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
+# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Affero General Public License
+# You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.py` & `pontos-23.4.5/tests/nvd/cve/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright (C) <year> <company>
+# Copyright (C) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
+# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Affero General Public License
+# You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh` & `pontos-23.4.5/tests/nvd/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-#!/bin/sh
-# Copyright (C) <year> <company>
+# Copyright (C) 2022 Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
+# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU Affero General Public License
+# You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt` & `pontos-23.4.5/tests/release/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Copyright (C) <year> <company>
-
-SPDX-License-Identifier: AGPL-3.0-or-later
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# Copyright (C) 2020-2022 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml` & `pontos-23.4.5/tests/testing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-<?xml version="1.0"?>
-
-<!--
-Copyright (C) <year> <company>
-
-SPDX-License-Identifier: AGPL-3.0-or-later
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
--->
+# Copyright (C) 2022 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl` & `pontos-23.4.5/tests/version/commands/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-<?xml version="1.0"?>
-
-<!--
-Copyright (C) <year> <company>
-
-SPDX-License-Identifier: AGPL-3.0-or-later
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
--->
+# Copyright (C) 2023 Greenbone Networks GmbH
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.c` & `pontos-23.4.5/tests/updateheader/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-/* Copyright (C) <year> <company>
- *
- * SPDX-License-Identifier: GPL-2.0-only
- *
- * This program is free software; you can redistribute it and/or
- * modify it under the terms of the GNU General Public License
- * version 2 as published by the Free Software Foundation.
- *
- * This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program; if not, write to the Free Software
- * Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA.
- */
+# Copyright (C) 2020-2022 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.h` & `pontos-23.4.5/tests/version/test_commands.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-/* Copyright (C) <year> <company>
- *
- * SPDX-License-Identifier: GPL-2.0-only
- *
- * This program is free software; you can redistribute it and/or
- * modify it under the terms of the GNU General Public License
- * version 2 as published by the Free Software Foundation.
- *
- * This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program; if not, write to the Free Software
- * Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA.
- */
+# Copyright (C) 2023 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+import unittest
+
+from pontos.version.commands import get_commands
+
+
+class GetCommandsTestCase(unittest.TestCase):
+    def test_available_commands(self):
+        self.assertEqual(len(get_commands()), 5)
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.bash` & `pontos-23.4.5/tests/changelog/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,34 @@
-#!/bin/bash
-# Copyright (C) <year> <company>
+# Copyright (C) 2020-2022 Greenbone AG
 #
-# SPDX-License-Identifier: GPL-2.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
-# This program is free software; you can redistribute it and/or
-# modify it under the terms of the GNU General Public License
-# as published by the Free Software Foundation; either version 2
-# of the License, or (at your option) any later version.
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA.
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+import os
+from contextlib import contextmanager
+from pathlib import Path
+
+
+@contextmanager
+def use_cwd(path: Path) -> None:
+    """
+    Context Manager to change the current working directory temporaryly
+    """
+    current_cwd = Path.cwd()
+
+    os.chdir(str(path))
+
+    yield
+
+    os.chdir(str(current_cwd))
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.c` & `pontos-23.4.5/tests/version/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,34 @@
-/* Copyright (C) <year> <company>
- *
- * SPDX-License-Identifier: GPL-2.0-or-later
- *
- * This program is free software; you can redistribute it and/or
- * modify it under the terms of the GNU General Public License
- * as published by the Free Software Foundation; either version 2
- * of the License, or (at your option) any later version.
- *
- * This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program; if not, write to the Free Software
- * Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA.
- */
+# Copyright (C) 2020-2022 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+import os
+from contextlib import contextmanager
+from pathlib import Path
+
+
+@contextmanager
+def use_cwd(path: Path) -> None:
+    """
+    Context Manager to change the current working directory temporaryly
+    """
+    current_cwd = Path.cwd()
+
+    os.chdir(str(path))
+
+    yield
+
+    os.chdir(str(current_cwd))
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake` & `pontos-23.4.5/pontos/version/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-# Copyright (C) <year> <company>
+# Copyright (C) 2020-2022 Greenbone AG
 #
-# SPDX-License-Identifier: GPL-2.0-or-later
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
-# This program is free software; you can redistribute it and/or
-# modify it under the terms of the GNU General Public License
-# as published by the Free Software Foundation; either version 2
-# of the License, or (at your option) any later version.
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program; if not, write to the Free Software
-# Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA.
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+# pylint: disable=invalid-name
+
+from .main import main
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.txt` & `pontos-23.4.5/tests/version/test_errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,31 @@
-Copyright (C) <year> <company>
+# Copyright (C) 2023 Greenbone AG
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-SPDX-License-Identifier: GPL-2.0-or-later
 
-This program is free software; you can redistribute it and/or
-modify it under the terms of the GNU General Public License
-as published by the Free Software Foundation; either version 2
-of the License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program; if not, write to the Free Software
-Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA.
+import unittest
+
+from pontos.version.errors import VersionError
+
+
+class VersionErrorTestCase(unittest.TestCase):
+    def test_should_print_message(self):
+        err = VersionError("foo bar")
+        self.assertEqual(str(err), "foo bar")
+
+    def test_should_raise(self):
+        with self.assertRaisesRegex(VersionError, "^foo bar$"):
+            raise VersionError("foo bar")
```

### Comparing `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.bash` & `pontos-23.4.5/tests/version/schemes/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#!/bin/bash
-# Copyright (C) <year> <company>
+# Copyright (C) 2023 Greenbone Networks GmbH
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `pontos-23.4.3/pontos/updateheader/updateheader.py` & `pontos-23.4.5/pontos/updateheader/updateheader.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,36 +77,36 @@
 ) -> Tuple[bool, Union[Dict[str, Union[str, None]], None]]:
     """Match the line for the regex"""
     copyright_match = re.search(regex, line)
     if copyright_match:
         return (
             True,
             {
-                "creation_year": copyright_match.group(1),
-                "modification_year": copyright_match.group(2),
-                "company": copyright_match.group(3),
+                "creation_year": copyright_match.group(2),
+                "modification_year": copyright_match.group(3),
+                "company": copyright_match.group(4),
             },
         )
     return False, None
 
 
 def _add_header(
-    suffix: str, licence: str, company: str, year: str
+    suffix: str, license_id: str, company: str, year: str
 ) -> Union[str, None]:
     """Tries to add the header to the file.
     Requirements:
       - file type must be supported
-      - licence file must exist
+      - license file must exist
     """
     if suffix in SUPPORTED_FILE_TYPES:
         root = Path(__file__).parent
-        licence_file = root / "templates" / licence / f"template{suffix}"
+        license_file = root / "templates" / license_id / f"template{suffix}"
         try:
             return (
-                licence_file.read_text(encoding="utf-8")
+                license_file.read_text(encoding="utf-8")
                 .replace("<company>", company)
                 .replace("<year>", year)
             )
         except FileNotFoundError as e:
             raise e
     else:
         raise ValueError
@@ -145,68 +145,69 @@
                 found, copyright_match = _find_copyright(line=line, regex=regex)
                 i = i - 1
             # header not found, add header
             if i == 0 and not found:
                 try:
                     header = _add_header(
                         file.suffix,
-                        parsed_args.licence,
+                        parsed_args.license_id,
                         parsed_args.company,
                         parsed_args.year,
                     )
                     if header:
                         fp.seek(0)  # back to beginning of file
                         rest_of_file = fp.read()
                         fp.seek(0)
                         fp.write(header)
                         fp.write("\n")
                         fp.write(rest_of_file)
-                        print(f"{file}: Added licence header.")
+                        print(f"{file}: Added license header.")
                         return 0
                 except ValueError:
                     print(
-                        f"{file}: No licence header for the"
+                        f"{file}: No license header for the"
                         f" format {file.suffix} found.",
                     )
                 except FileNotFoundError:
                     print(
-                        f"{file}: Licence file for {parsed_args.licence} "
+                        f"{file}: License file for {parsed_args.license_id} "
                         "is not existing."
                     )
                 return 1
             # replace found header and write it to file
             if copyright_match and (
                 not copyright_match["modification_year"]
                 and copyright_match["creation_year"] < parsed_args.year
                 or copyright_match["modification_year"]
                 and copyright_match["modification_year"] < parsed_args.year
             ):
                 copyright_term = (
-                    f'Copyright (C) {copyright_match["creation_year"]}'
+                    f"SPDX-FileCopyrightText: "
+                    f'{copyright_match["creation_year"]}'
                     f'-{parsed_args.year} {copyright_match["company"]}'
                 )
                 new_line = re.sub(regex, copyright_term, line)
                 fp_write = fp.tell() - len(line)  # save position to insert
                 rest_of_file = fp.read()
                 fp.seek(fp_write)
                 fp.write(new_line)
                 fp.write(rest_of_file)
                 # in some cases we replace "YYYY - YYYY" with "YYYY-YYYY"
                 # resulting in 2 characters left at the end of the file
                 # so we truncate the file, just in case!
                 fp.truncate()
                 print(
-                    f"{file}: Changed Licence Header Copyright Year "
+                    f"{file}: Changed License Header Copyright Year "
                     f'{copyright_match["modification_year"]} -> '
                     f"{parsed_args.year}"
                 )
 
                 return 0
             else:
-                print(f"{file}: Licence Header is ok.")
+                print(f"{file}: License Header is ok.")
                 return 0
     except FileNotFoundError as e:
         print(f"{file}: File is not existing.")
         raise e
     except UnicodeDecodeError as e:
         print(f"{file}: Ignoring binary file.")
         raise e
@@ -290,26 +291,26 @@
             "If year is set, modified year will be "
             "set to the specified year."
         ),
     )
 
     parser.add_argument(
         "-l",
-        "--licence",
+        "--license",
         choices=SUPPORTED_LICENCES,
         default="GPL-3.0-or-later",
-        help=("Use the passed licence type"),
+        help=("Use the passed license type"),
     )
 
     parser.add_argument(
         "--company",
         default="Greenbone AG",
         help=(
             "If a header will be added to file, "
-            "it will be licenced by company."
+            "it will be licensed by company."
         ),
     )
 
     files_group = parser.add_mutually_exclusive_group(required=True)
     files_group.add_argument(
         "-f", "--files", nargs="+", help="Files to update."
     )
@@ -371,15 +372,15 @@
 
     else:
         # should never happen
         term.error("Specify files to update!")
         sys.exit(1)
 
     regex = re.compile(
-        "[Cc]opyright.*?(19[0-9]{2}|20[0-9]{2}) "
+        "(SPDX-FileCopyrightText:|[Cc]opyright).*?(19[0-9]{2}|20[0-9]{2}) "
         f"?-? ?(19[0-9]{{2}}|20[0-9]{{2}})? ({parsed_args.company})"
     )
 
     for file in files:
         try:
             if file.absolute() in exclude_list:
                 term.warning(f"{file}: Ignoring file from exclusion list.")
```

### Comparing `pontos-23.4.3/pontos/version/__init__.py` & `pontos-23.4.5/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/__main__.py` & `pontos-23.4.5/tests/version/test_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2022 Greenbone AG
+# Copyright (C) 2023 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,13 +11,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# pylint: disable=invalid-name
+import unittest
+from contextlib import redirect_stderr
+from io import StringIO
 
-from .main import main
+from pontos.version.parser import parse_args
 
-if __name__ == "__main__":
-    main()
+
+class ParserTestCase(unittest.TestCase):
+    def test_error_while_parsing(self):
+        with redirect_stderr(StringIO()), self.assertRaises(SystemExit) as cm:
+            parse_args(["update", "foo"])
+
+        # exception code in argparse
+        self.assertEqual(cm.exception.code, 2)
```

### Comparing `pontos-23.4.3/pontos/version/_calculator.py` & `pontos-23.4.5/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/commands/__init__.py` & `pontos-23.4.5/pontos/version/commands/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,29 +18,32 @@
 from typing import Iterable, Tuple, Type
 
 from ._cmake import CMakeVersionCommand
 from ._command import VersionCommand
 from ._go import GoVersionCommand
 from ._javascript import JavaScriptVersionCommand
 from ._python import PythonVersionCommand
+from ._cargo import CargoVersionCommand
 
 __all__ = (
     "VersionCommand",
     "CMakeVersionCommand",
     "GoVersionCommand",
     "JavaScriptVersionCommand",
     "PythonVersionCommand",
+    "CargoVersionCommand",
     "get_commands",
 )
 
 __COMMANDS: Tuple[Type[VersionCommand]] = (
     CMakeVersionCommand,
     GoVersionCommand,
     JavaScriptVersionCommand,
     PythonVersionCommand,
+    CargoVersionCommand,
 )
 
 
 def get_commands() -> Iterable[Type[VersionCommand]]:
     """
     Returns the available VersionCommands
     """
```

### Comparing `pontos-23.4.3/pontos/version/commands/_cmake.py` & `pontos-23.4.5/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/commands/_command.py` & `pontos-23.4.5/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/commands/_go.py` & `pontos-23.4.5/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/commands/_javascript.py` & `pontos-23.4.5/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/commands/_python.py` & `pontos-23.4.5/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/errors.py` & `pontos-23.4.5/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/helper.py` & `pontos-23.4.5/pontos/version/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-from typing import Optional
+from typing import Iterator, Optional
 
 from pontos.git import Git, TagSort
 from pontos.git.git import DEFAULT_TAG_SORT_SUFFIX
 
 from .version import ParseVersionFuncType, Version
 
 
 def get_last_release_versions(
     parse_version: ParseVersionFuncType,
     *,
     git_tag_prefix: Optional[str] = "",
     ignore_pre_releases: Optional[bool] = False,
     tag_name: Optional[str] = None,
-) -> list[Version]:
+) -> Iterator[Version]:
     """Get the last released Versions from git.
 
     Args:
         git_tag_prefix: Git tag prefix to consider
         ignore_pre_release: Ignore pre releases and only consider non pre
             releases. Default is False.
         tag_name: A pattern for filtering the tags. For example: "1.2.*"
@@ -47,26 +47,22 @@
     tag_list = Git().list_tags(
         sort=TagSort.VERSION,
         sort_suffix=DEFAULT_TAG_SORT_SUFFIX,
         tag_name=tag_name,
     )
     tag_list.reverse()
 
-    tags = []
-
     for tag in tag_list:
         last_release_version = tag.strip(git_tag_prefix)
 
         version = parse_version(last_release_version)
         if version.is_pre_release and ignore_pre_releases:
             continue
 
-        tags.append(version)
-
-    return tags
+        yield version
 
 
 def get_last_release_version(
     parse_version: ParseVersionFuncType,
     *,
     git_tag_prefix: Optional[str] = "",
     ignore_pre_releases: Optional[bool] = False,
@@ -81,15 +77,18 @@
         tag_name: A pattern for filtering the tags. For example: "1.2.*"
 
     Returns:
         Last released git tag as Version if tags were found
         or None
     """
 
-    versions = get_last_release_versions(
+    it = get_last_release_versions(
         parse_version=parse_version,
         git_tag_prefix=git_tag_prefix,
         ignore_pre_releases=ignore_pre_releases,
         tag_name=tag_name,
     )
 
-    return versions[0] if versions else None
+    try:
+        return next(it)
+    except StopIteration:
+        return None
```

### Comparing `pontos-23.4.3/pontos/version/main.py` & `pontos-23.4.5/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/parser.py` & `pontos-23.4.5/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/project.py` & `pontos-23.4.5/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/schemes/__init__.py` & `pontos-23.4.5/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/schemes/_pep440.py` & `pontos-23.4.5/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/schemes/_scheme.py` & `pontos-23.4.5/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/schemes/_semantic.py` & `pontos-23.4.5/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pontos/version/version.py` & `pontos-23.4.5/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/pyproject.toml` & `pontos-23.4.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.4.3"
+version = "23.4.5"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
@@ -35,29 +35,29 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 colorful = "^0.5.4"
 tomlkit = ">=0.5.11"
 packaging = ">=20.3"
-httpx = {extras = ["http2"], version = "^0.23.0"}
+httpx = {extras = ["http2"], version = ">=0.23,<0.25"}
 rich = ">=12.4.4"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
 python-dateutil = "^2.8.2"
 semver = ">=2.13,<4.0"
 
 [tool.poetry.dev-dependencies]
 autohooks = ">=22.7.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 autohooks-plugin-isort = ">=22.3.0"
 rope = "^1.7.0"
 coverage = "^7.2"
 myst-parser = ">=0.19.1"
-Sphinx = "^6.1.3"
+Sphinx = "^6.2.0"
 furo = "^2023.3.27"
 sphinx-autobuild = "^2021.3.14"
 
 [tool.black]
 line-length = 80
 target-version = ['py39', 'py310', 'py311']
 exclude = '''
```

### Comparing `pontos-23.4.3/scripts/github/artifacts-download.py` & `pontos-23.4.5/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/artifacts.py` & `pontos-23.4.5/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/branchprotection.py` & `pontos-23.4.5/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/create-repository.py` & `pontos-23.4.5/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/enforce-admins.py` & `pontos-23.4.5/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/lock-branch.py` & `pontos-23.4.5/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/members.py` & `pontos-23.4.5/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/release-assets-download.py` & `pontos-23.4.5/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/repositories.py` & `pontos-23.4.5/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/search-repositories.py` & `pontos-23.4.5/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/team-repositories.py` & `pontos-23.4.5/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/teams.py` & `pontos-23.4.5/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/scripts/github/workflow-runs.py` & `pontos-23.4.5/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/__init__.py` & `pontos-23.4.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/changelog/__init__.py` & `pontos-23.4.5/tests/github/api/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2022 Greenbone AG
+# Copyright (C) 2022 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,24 +11,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import os
-from contextlib import contextmanager
-from pathlib import Path
+from unittest.mock import MagicMock
 
+import httpx
 
-@contextmanager
-def use_cwd(path: Path) -> None:
-    """
-    Context Manager to change the current working directory temporaryly
-    """
-    current_cwd = Path.cwd()
+from pontos.github.api.client import GitHubAsyncREST, GitHubAsyncRESTClient
+from tests import AsyncMock, IsolatedAsyncioTestCase
 
-    os.chdir(str(path))
 
-    yield
+def create_response(*args, **kwargs) -> MagicMock:
+    return MagicMock(spec=httpx.Response, *args, **kwargs)
 
-    os.chdir(str(current_cwd))
+
+class GitHubAsyncRESTTestCase(IsolatedAsyncioTestCase):
+    api_cls = GitHubAsyncREST
+
+    def setUp(self) -> None:
+        self.client = AsyncMock(spec=GitHubAsyncRESTClient)
+        self.api = self.api_cls(self.client)
```

### Comparing `pontos-23.4.3/tests/changelog/test_conventional_commits.py` & `pontos-23.4.5/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/changelog/test_parser.py` & `pontos-23.4.5/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/git/test_git.py` & `pontos-23.4.5/tests/git/test_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 from pathlib import Path
 from unittest.mock import patch
 
 from pontos.git import Git
 from pontos.git.git import (
     DEFAULT_TAG_SORT_SUFFIX,
     ConfigScope,
+    GitError,
     MergeStrategy,
     TagSort,
 )
 from pontos.git.status import Status
-from pontos.testing import temp_git_repository
+from pontos.testing import temp_directory, temp_git_repository
 
 
 class GitTestCase(unittest.TestCase):
     @patch("pontos.git.git.exec_git")
     def test_exec(self, exec_git_mock):
         git = Git()
         git.exec("foo", "bar", "baz")
@@ -904,7 +905,22 @@
             status = next(it)
             self.assertEqual(status.index, Status.DELETED)
             self.assertEqual(status.working_tree, Status.UNMODIFIED)
             self.assertEqual(status.path, Path("lorem.json"))
 
             with self.assertRaises(StopIteration):
                 next(it)
+
+    def test_git_error(self):
+        with temp_directory(change_into=True), self.assertRaises(
+            GitError
+        ) as cm:
+            Git().log()
+
+        self.assertEqual(cm.exception.returncode, 128)
+        self.assertEqual(
+            cm.exception.stderr,
+            "fatal: not a git repository (or any of the parent directories): "
+            ".git\n",
+        )
+        self.assertEqual(cm.exception.stdout, "")
+        self.assertEqual(cm.exception.cmd, ["git", "log"])
```

### Comparing `pontos-23.4.3/tests/git/test_status.py` & `pontos-23.4.5/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/actions/test-pull-request-event.json` & `pontos-23.4.5/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/actions/test_core.py` & `pontos-23.4.5/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/actions/test_env.py` & `pontos-23.4.5/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/actions/test_event.py` & `pontos-23.4.5/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/pr-files.json` & `pontos-23.4.5/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/release-response.json` & `pontos-23.4.5/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_artifacts.py` & `pontos-23.4.5/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_branch.py` & `pontos-23.4.5/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_client.py` & `pontos-23.4.5/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_contents.py` & `pontos-23.4.5/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_labels.py` & `pontos-23.4.5/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_organizations.py` & `pontos-23.4.5/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_pull_requests.py` & `pontos-23.4.5/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_release.py` & `pontos-23.4.5/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_repositories.py` & `pontos-23.4.5/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_search.py` & `pontos-23.4.5/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_tags.py` & `pontos-23.4.5/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_teams.py` & `pontos-23.4.5/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/api/test_workflows.py` & `pontos-23.4.5/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_artifact.py` & `pontos-23.4.5/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_base.py` & `pontos-23.4.5/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_branch.py` & `pontos-23.4.5/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_organization.py` & `pontos-23.4.5/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_pull_request.py` & `pontos-23.4.5/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_release.py` & `pontos-23.4.5/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_search.py` & `pontos-23.4.5/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_tag.py` & `pontos-23.4.5/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/models/test_workflow.py` & `pontos-23.4.5/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/script/test_load.py` & `pontos-23.4.5/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/script/test_parser.py` & `pontos-23.4.5/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/github/test_argparser.py` & `pontos-23.4.5/tests/github/test_argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     create_pull_request,
     create_release,
     create_tag,
     file_status,
     update_pull_request,
 )
 from pontos.github.models.base import FileStatus
+from pontos.testing import temp_directory
 
 
 class TestArgparsing(unittest.TestCase):
     def setUp(self):
         self.term = Mock()
 
     def test_create_pr_parse_args(self):
@@ -101,47 +102,52 @@
     def test_update_pr_parse_args_fail(self):
         argv = ["pr", "update", "foo/bar"]
 
         with self.assertRaises(SystemExit), redirect_stderr(io.StringIO()):
             parse_args(argv)
 
     def test_fs_parse_args(self):
-        argv = [
-            "FS",
-            "foo/bar",
-            "8",
-            "-o",
-            "some.file",
-        ]
-
-        with patch.dict("os.environ", {}, clear=True):
-            parsed_args = parse_args(argv)
-
-        output = io.open(Path("some.file"), mode="w", encoding="utf-8")
-
-        expected_args = Namespace(
-            command="FS",
-            func=file_status,
-            repo="foo/bar",
-            pull_request=8,
-            output=output,
-            status=[FileStatus.ADDED, FileStatus.MODIFIED],
-            token="GITHUB_TOKEN",
-        )
-
-        self.assertEqual(type(parsed_args.output), type(expected_args.output))
-        self.assertEqual(parsed_args.command, expected_args.command)
-        self.assertEqual(parsed_args.func, expected_args.func)
-        self.assertEqual(parsed_args.repo, expected_args.repo)
-        self.assertEqual(parsed_args.pull_request, expected_args.pull_request)
-        self.assertEqual(parsed_args.status, expected_args.status)
-        self.assertEqual(parsed_args.token, expected_args.token)
+        with temp_directory(change_into=True) as tmp_dir:
+            argv = [
+                "FS",
+                "foo/bar",
+                "8",
+                "-o",
+                "some.file",
+            ]
+
+            with patch.dict("os.environ", {}, clear=True):
+                parsed_args = parse_args(argv)
+
+            output = open(tmp_dir / "some.file", mode="w", encoding="utf-8")
+
+            expected_args = Namespace(
+                command="FS",
+                func=file_status,
+                repo="foo/bar",
+                pull_request=8,
+                output=output,
+                status=[FileStatus.ADDED, FileStatus.MODIFIED],
+                token="GITHUB_TOKEN",
+            )
+
+            self.assertEqual(
+                type(parsed_args.output), type(expected_args.output)
+            )
+            self.assertEqual(parsed_args.command, expected_args.command)
+            self.assertEqual(parsed_args.func, expected_args.func)
+            self.assertEqual(parsed_args.repo, expected_args.repo)
+            self.assertEqual(
+                parsed_args.pull_request, expected_args.pull_request
+            )
+            self.assertEqual(parsed_args.status, expected_args.status)
+            self.assertEqual(parsed_args.token, expected_args.token)
 
-        output.close()
-        parsed_args.output.close()
+            output.close()
+            parsed_args.output.close()
 
     def test_create_release_parse_args(self):
         argv = [
             "re",
             "create",
             "foo/bar",
             "123",
```

### Comparing `pontos-23.4.3/tests/github/test_cmds.py` & `pontos-23.4.5/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/models/test_models.py` & `pontos-23.4.5/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/nvd/__init__.py` & `pontos-23.4.5/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/nvd/cpe/test_api.py` & `pontos-23.4.5/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/nvd/cve/test_api.py` & `pontos-23.4.5/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/nvd/models/test_cpe.py` & `pontos-23.4.5/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/nvd/models/test_cve.py` & `pontos-23.4.5/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/nvd/test_api.py` & `pontos-23.4.5/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/release/test_helper.py` & `pontos-23.4.5/tests/release/test_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import contextlib
+import os
 import subprocess
 import unittest
 from pathlib import Path
 from typing import Generator
 from unittest.mock import MagicMock
 
 from pontos.git.git import ConfigScope, Git, GitError, exec_git
@@ -57,14 +58,15 @@
                 scope=ConfigScope.LOCAL,
             )
             signing_key = find_signing_key(terminal)
             self.assertEqual(
                 signing_key, "1234567890ABCEDEF1234567890ABCEDEF123456"
             )
 
+    @unittest.skipUnless(os.environ.get("CI"), "only run on CI")
     def test_find_no_signing_key(self):
         terminal = MagicMock()
         saved_key = None
 
         git = Git()
         try:
             # save possibly set git signing key from user temporarily
```

### Comparing `pontos-23.4.3/tests/release/test_parser.py` & `pontos-23.4.5/tests/release/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,21 @@
                 "--release-type",
                 "patch",
             ]
         )
 
         self.assertEqual(args.cc_config, Path("foo.toml"))
 
+    def test_release_series(self):
+        _, _, args = parse_args(
+            ["release", "--release-type", "patch", "--release-series", "22.4"]
+        )
+
+        self.assertEqual(args.release_series, "22.4")
+
 
 class SignParseArgsTestCase(unittest.TestCase):
     def test_sign_func(self):
         _, _, args = parse_args(["sign"])
 
         self.assertEqual(args.func, sign)
 
@@ -251,7 +258,12 @@
 
         self.assertEqual(args.signing_key, "123")
 
     def test_passphrase(self):
         _, _, args = parse_args(["sign", "--passphrase", "123"])
 
         self.assertEqual(args.passphrase, "123")
+
+    def test_release_series(self):
+        _, _, args = parse_args(["sign", "--release-series", "22.4"])
+
+        self.assertEqual(args.release_series, "22.4")
```

### Comparing `pontos-23.4.3/tests/release/test_release.py` & `pontos-23.4.5/tests/release/test_release.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # pylint: disable=too-many-lines, line-too-long, invalid-name
 
 import unittest
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
-from typing import Optional
+from typing import Iterable, Optional, Union
 from unittest.mock import AsyncMock, MagicMock, call, patch
 
 from httpx import HTTPStatusError, Request, Response
 
 from pontos.git.git import ConfigScope, Git
 from pontos.release.main import parse_args
 from pontos.release.release import ReleaseReturnValue, release
@@ -37,16 +37,24 @@
 from pontos.version.schemes._pep440 import PEP440Version, PEP440VersioningScheme
 
 
 def mock_terminal() -> MagicMock:
     return MagicMock(spec=Terminal)
 
 
+def str_or_list(values: Union[str, Iterable[str]]) -> Iterable[str]:
+    if values and isinstance(values, str):
+        return [values]
+    return values
+
+
 @contextmanager
-def setup_go_project(*, current_version: str, tags: list[str] = None) -> Path:
+def setup_go_project(
+    *, current_version: str, tags: Union[str, Iterable[str]] = None
+) -> Path:
     with temp_git_repository() as tmp_git:
         git = Git(tmp_git)
 
         git.config("commit.gpgSign", "false", scope=ConfigScope.LOCAL)
         git.config("tag.gpgSign", "false", scope=ConfigScope.LOCAL)
         git.config("tag.sort", "refname", scope=ConfigScope.LOCAL)
 
@@ -57,15 +65,15 @@
         update = go.update_version(new_version=PEP440Version(current_version))
 
         git.add(update.changed_files)
         git.add(go.project_file_path)
         git.commit("Create initial release")
 
         if tags:
-            for tag in tags:
+            for tag in str_or_list(tags):
                 git.tag(f"v{tag}")
 
         yield tmp_git
 
 
 @patch.dict(
     "os.environ",
@@ -73,35 +81,38 @@
         "GITHUB_TOKEN": "foo",
         "GITHUB_USER": "user",
         "GPG_SIGNING_KEY": "1234",
     },
 )
 class ReleaseTestCase(unittest.TestCase):
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_version(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2")
         next_version = PEP440Version("1.0.0.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
@@ -112,16 +123,14 @@
         ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-version",
                 "0.0.2",
                 "--next-version",
                 "1.0.0.dev1",
             ]
         )
 
@@ -155,73 +164,171 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.0.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
+                ),
+            ]
+        )
+        git_mock.return_value.tag.assert_called_once_with(
+            "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
+        )
+
+        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+
+    @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch(
+        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+    )
+    @patch(
+        "pontos.release.release.ReleaseCommand._create_changelog",
+        autospec=True,
+    )
+    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    def test_initial_release_version(
+        self,
+        gather_commands_mock: MagicMock,
+        create_changelog_mock: MagicMock,
+        create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
+        git_mock: MagicMock,
+    ):
+        current_version = PEP440Version("0.0.1")
+        release_version = PEP440Version("1.0.0")
+        next_version = PEP440Version("1.0.1.dev1")
+        command_mock = MagicMock(spec=GoVersionCommand)
+        gather_commands_mock.return_value = [command_mock]
+        create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = None
+        command_mock.update_version.side_effect = [
+            VersionUpdate(
+                previous=current_version,
+                new=release_version,
+                changed_files=["MyProject.conf"],
+            ),
+            VersionUpdate(
+                previous=release_version,
+                new=next_version,
+                changed_files=["MyProject.conf"],
+            ),
+        ]
+
+        _, token, args = parse_args(
+            [
+                "release",
+                "--project",
+                "foo",
+                "--release-version",
+                "1.0.0",
+            ]
+        )
+
+        with temp_git_repository():
+            released = release(
+                terminal=mock_terminal(),
+                args=args,
+                token=token,
+            )
+
+        git_mock.return_value.push.assert_has_calls(
+            [
+                call(follow_tags=True, remote=None),
+                call(follow_tags=True, remote=None),
+            ],
+        )
+
+        command_mock.update_version.assert_has_calls(
+            [
+                call(release_version, force=False),
+                call(next_version, force=False),
+            ]
+        )
+
+        self.assertEqual(
+            create_release_mock.await_args.args[1:],
+            (release_version, "foo", "A Changelog"),
+        )
+
+        git_mock.return_value.add.assert_has_calls(
+            [call("MyProject.conf"), call("MyProject.conf")]
+        )
+        git_mock.return_value.commit.assert_has_calls(
+            [
+                call(
+                    "Automatic release to 1.0.0",
+                    verify=False,
+                    gpg_signing_key="1234",
+                ),
+                call(
+                    "Automatic adjustments after release\n\n"
+                    "* Update to version 1.0.1.dev1\n",
+                    verify=False,
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.0.2", gpg_key_id="123", message="Automatic release to 0.0.2"
+            "v1.0.0", gpg_key_id="1234", message="Automatic release to 1.0.0"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_patch(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2")
         next_version = PEP440Version("1.0.0.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
-        command_mock.get_current_version.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
                 "patch",
                 "--next-version",
                 "1.0.0.dev1",
             ]
         )
 
@@ -254,74 +361,74 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.0.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.0.2", gpg_key_id="123", message="Automatic release to 0.0.2"
+            "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_calendar(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         today = datetime.today()
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version(f"{today.year % 100}.{today.month}.0")
         next_version = PEP440Version(f"{today.year % 100}.{today.month}.1.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
-        command_mock.get_current_version.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
                 "calendar",
             ]
         )
 
         with temp_git_repository():
             released = release(
@@ -353,75 +460,75 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     f"Automatic release to {release_version}",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     f"* Update to version {next_version}\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
             f"v{release_version}",
-            gpg_key_id="123",
+            gpg_key_id="1234",
             message=f"Automatic release to {release_version}",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_minor(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.1.0")
         next_version = PEP440Version("0.1.1.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
-        command_mock.get_current_version.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
                 "minor",
                 "--next-version",
                 "0.1.1.dev1",
             ]
         )
 
@@ -454,73 +561,73 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.1.0",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.1.1.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.1.0", gpg_key_id="123", message="Automatic release to 0.1.0"
+            "v0.1.0", gpg_key_id="1234", message="Automatic release to 0.1.0"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_major(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("1.0.0")
         next_version = PEP440Version("1.0.1.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
-        command_mock.get_current_version.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
                 "major",
                 "--next-version",
                 "1.0.1.dev1",
             ]
         )
 
@@ -553,73 +660,73 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 1.0.0",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.1.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v1.0.0", gpg_key_id="123", message="Automatic release to 1.0.0"
+            "v1.0.0", gpg_key_id="1234", message="Automatic release to 1.0.0"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_alpha(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2a1")
         next_version = PEP440Version("0.0.2a2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
-        command_mock.get_current_version.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
                 "alpha",
             ]
         )
 
         with temp_git_repository():
             released = release(
@@ -650,73 +757,75 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2a1",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.0.2a2.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.0.2a1", gpg_key_id="123", message="Automatic release to 0.0.2a1"
+            "v0.0.2a1",
+            gpg_key_id="1234",
+            message="Automatic release to 0.0.2a1",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_beta(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2b1")
         next_version = PEP440Version("0.0.2b2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
-        command_mock.get_current_version.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
                 "beta",
             ]
         )
 
         with temp_git_repository():
             released = release(
@@ -747,73 +856,75 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2b1",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.0.2b2.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.0.2b1", gpg_key_id="123", message="Automatic release to 0.0.2b1"
+            "v0.0.2b1",
+            gpg_key_id="1234",
+            message="Automatic release to 0.0.2b1",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
         autospec=True,
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_release_candidate(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2rc1")
         next_version = PEP440Version("0.0.2rc2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["MyProject.conf"],
             ),
         ]
-        command_mock.get_current_version.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
                 "release-candidate",
             ]
         )
 
         with temp_git_repository():
             released = release(
@@ -844,33 +955,35 @@
             [call("MyProject.conf"), call("MyProject.conf")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2rc1",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 0.0.2rc2.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
         git_mock.return_value.tag.assert_called_once_with(
             "v0.0.2rc1",
-            gpg_key_id="123",
+            gpg_key_id="1234",
             message="Automatic release to 0.0.2rc1",
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
-    def test_no_token(self):
+    def test_no_token(
+        self,
+    ):
         _, _, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
                 "0.0.1",
@@ -881,72 +994,98 @@
             terminal=mock_terminal(),
             args=args,
             token=None,
         )
 
         self.assertEqual(released, ReleaseReturnValue.TOKEN_MISSING)
 
-    def test_no_project_settings(self):
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    def test_no_project_settings(
+        self,
+        get_last_release_version_mock: MagicMock,
+    ):
+        current_version = PEP440Version("0.0.1")
+        get_last_release_version_mock.return_value = current_version
+
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
                 "0.0.1",
-                "--git-signing-key",
-                "123",
             ]
         )
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         self.assertEqual(
             released, ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
         )
 
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
-    def test_no_release_error(self, gather_commands_mock: MagicMock):
-        command_mock = MagicMock(spec=GoVersionCommand)
-        gather_commands_mock.return_value = [command_mock]
-        command_mock.get_current_version.side_effect = VersionError("An error")
-
+    def test_last_release_version_error(self):
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-type",
-                "patch",
+                "major",
             ]
         )
+        with temp_git_repository():
+            released = release(
+                terminal=mock_terminal(),
+                args=args,
+                token=token,
+            )
 
+        self.assertEqual(released, ReleaseReturnValue.NO_LAST_RELEASE_VERSION)
+
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    def test_no_last_release_version(
+        self,
+        get_last_release_version_mock: MagicMock,
+    ):
+        get_last_release_version_mock.return_value = None
+        _, token, args = parse_args(
+            [
+                "release",
+                "--project",
+                "foo",
+                "--release-type",
+                "minor",
+            ]
+        )
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        self.assertEqual(released, ReleaseReturnValue.NO_RELEASE_VERSION)
+        self.assertEqual(released, ReleaseReturnValue.NO_LAST_RELEASE_VERSION)
 
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
-    def test_no_release(
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch(
+        "pontos.release.release.ReleaseCommand._get_next_release_version",
+        autospec=True,
+    )
+    def test_no_release_error(
         self,
-        gather_commands_mock: MagicMock,
+        get_next_release_version_mock: MagicMock,
+        get_last_release_version_mock: MagicMock,
     ):
-        command_mock = MagicMock(spec=GoVersionCommand)
-        gather_commands_mock.return_value = [command_mock]
-        command_mock.get_current_version.return_value = None
+        current_version = PEP440Version("0.0.1")
+        get_next_release_version_mock.side_effect = VersionError("An error")
+        get_last_release_version_mock.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--git-signing-key",
@@ -962,69 +1101,70 @@
                 args=args,
                 token=token,
             )
 
         self.assertEqual(released, ReleaseReturnValue.NO_RELEASE_VERSION)
 
     @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.version.helper.Git", autospec=True)
     def test_has_tag(
         self,
-        gather_commands_mock: MagicMock,
-        git_mock: MagicMock,
+        git_mock1: MagicMock,
+        git_mock2: MagicMock,
     ):
-        command_mock = MagicMock(spec=GoVersionCommand)
-        gather_commands_mock.return_value = [command_mock]
-        git_mock.return_value.list_tags.return_value = ["v0.0.1"]
+        tags = ["v1.0.0", "v1.0.1"]
+        git_mock1.return_value.list_tags.return_value = tags
+        git_mock2.return_value.list_tags.return_value = tags
 
         _, token, args = parse_args(
             [
                 "release",
                 "--release-version",
-                "0.0.1",
+                "1.0.1",
                 "--project",
                 "bla",
-                "--git-signing-key",
-                "1337",
             ]
         )
 
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 token=token,
                 args=args,
             )
 
             self.assertEqual(released, ReleaseReturnValue.ALREADY_TAKEN)
 
-        git_mock.return_value.list_tags.assert_called_once()
+        git_mock1.return_value.list_tags.assert_called_once()
+        git_mock2.return_value.list_tags.assert_called_once()
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_update_version_error(
         self,
         gather_commands_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         command_mock.update_version.side_effect = VersionError("An error")
+        current_version = PEP440Version("0.0.1rc1")
+        get_last_release_version_mock.return_value = current_version
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-version",
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
             ]
         )
 
@@ -1046,33 +1186,36 @@
         git_mock.return_value.add.assert_not_called()
         git_mock.return_value.commit.assert_not_called()
         git_mock.return_value.tag.assert_not_called()
 
         self.assertEqual(released, ReleaseReturnValue.UPDATE_VERSION_ERROR)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_github_create_release_failure(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.0")
         release_version = PEP440Version("0.0.1")
         next_version = PEP440Version("0.0.2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
@@ -1093,16 +1236,14 @@
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
-                "--git-signing-key",
-                "123",
             ]
         )
 
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
@@ -1112,62 +1253,63 @@
         self.assertEqual(released, ReleaseReturnValue.CREATE_RELEASE_ERROR)
 
         git_mock.return_value.push.assert_called_once_with(
             follow_tags=True, remote=None
         )
         git_mock.return_value.add.assert_called_once_with("MyProject.conf")
         git_mock.return_value.commit.assert_called_once_with(
-            "Automatic release to 0.0.1", verify=False, gpg_signing_key="123"
+            "Automatic release to 0.0.1", verify=False, gpg_signing_key="1234"
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.0.1", gpg_key_id="123", message="Automatic release to 0.0.1"
+            "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_update_version_after_release_error(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.0")
         release_version = PEP440Version("0.0.1")
         next_version = PEP440Version("0.0.2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
         create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionError("An error"),
         ]
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-version",
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
             ]
         )
 
@@ -1192,44 +1334,47 @@
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
         git_mock.return_value.add.assert_called_once_with("MyProject.conf")
         git_mock.return_value.commit.assert_called_once_with(
-            "Automatic release to 0.0.1", verify=False, gpg_signing_key="123"
+            "Automatic release to 0.0.1", verify=False, gpg_signing_key="1234"
         )
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.0.1", gpg_key_id="123", message="Automatic release to 0.0.1"
+            "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(
             released, ReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
         )
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_to_specific_git_remote(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock,
     ):
         current_version = PEP440Version("0.0.0")
         release_version = PEP440Version("0.0.1")
         next_version = PEP440Version("0.0.2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
@@ -1292,33 +1437,36 @@
         git_mock.return_value.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_without_git_prefix(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock,
     ):
         current_version = PEP440Version("0.0.0")
         release_version = PEP440Version("0.0.1")
         next_version = PEP440Version("0.0.2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
@@ -1334,16 +1482,14 @@
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
-                "--git-signing-key",
-                "1234",
                 "--git-tag-prefix",
                 "",
             ]
         )
 
         with temp_git_repository():
             released = release(
@@ -1381,31 +1527,34 @@
         git_mock.return_value.tag.assert_called_once_with(
             "0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch("pontos.release.release.GitHubAsyncRESTApi", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_github_api(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         github_api_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock,
     ):
         current_version = PEP440Version("0.0.0")
         release_version = PEP440Version("0.0.1")
         next_version = PEP440Version("0.0.2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
@@ -1427,16 +1576,14 @@
                 "foo",
                 "--release-version",
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
                 "--git-remote-name",
                 "upstream",
-                "--git-signing-key",
-                "1234",
             ]
         )
 
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
@@ -1475,31 +1622,34 @@
         git_mock.return_value.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch("pontos.release.release.GitHubAsyncRESTApi", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_github_api_pre_release(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         github_api_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock,
     ):
         current_version = PEP440Version("0.0.0")
         release_version = PEP440Version("0.0.1a1")
         next_version = PEP440Version("0.0.1a1+dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
@@ -1521,16 +1671,14 @@
                 "foo",
                 "--release-version",
                 "0.0.1a1",
                 "--next-version",
                 "0.0.1a1+dev1",
                 "--git-remote-name",
                 "upstream",
-                "--git-signing-key",
-                "1234",
             ]
         )
 
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
@@ -1589,15 +1737,15 @@
         git_mock,
     ):
         release_version = PEP440Version("0.0.2")
 
         create_changelog_mock.return_value = "A Changelog"
         _, token, args = parse_args(["release", "--release-type", "patch"])
 
-        with setup_go_project(current_version="0.0.1"):
+        with setup_go_project(current_version="0.0.1", tags=["0.0.1"]):
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
@@ -1622,46 +1770,46 @@
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch("pontos.changelog.conventional_commits.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_versions", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_with_changelog(
         self,
         gather_commands_mock: MagicMock,
         create_release_mock: AsyncMock,
-        get_last_release_versions_mock: MagicMock,
         cc_git_mock: MagicMock,
+        get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2")
         next_version = PEP440Version("1.0.0.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["project.conf"],
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["project.conf", "version.lang"],
             ),
         ]
-        get_last_release_versions_mock.return_value = [current_version]
         cc_git_mock.return_value.log.return_value = [
             "1234567 Add: foo bar",
             "8abcdef Add: bar baz",
             "8abcd3f Add bar baz",
             "8abcd3d Adding bar baz",
             "1337abc Change: bar to baz",
             "42a42a4 Remove: foo bar again",
@@ -1689,16 +1837,14 @@
 [0.0.2]: https://github.com/greenbone/foo/compare/v0.0.1...v0.0.2"""
 
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
-                "--git-signing-key",
-                "123",
                 "--release-version",
                 "0.0.2",
                 "--next-version",
                 "1.0.0.dev1",
             ]
         )
 
@@ -1731,57 +1877,60 @@
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", expected_changelog),
         )
 
         git_mock.return_value.tag.assert_called_once_with(
-            "v0.0.2", gpg_key_id="123", message="Automatic release to 0.0.2"
+            "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
         git_mock.return_value.add.assert_has_calls(
             [call("project.conf"), call("project.conf"), call("version.lang")]
         )
         git_mock.return_value.commit.assert_has_calls(
             [
                 call(
                     "Automatic release to 0.0.2",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
                 call(
                     "Automatic adjustments after release\n\n"
                     "* Update to version 1.0.0.dev1\n",
                     verify=False,
-                    gpg_signing_key="123",
+                    gpg_signing_key="1234",
                 ),
             ]
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_local(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
         git_mock,
     ):
         current_version = PEP440Version("0.0.0")
         release_version = PEP440Version("0.0.1")
         next_version = PEP440Version("0.0.2.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
         gather_commands_mock.return_value = [command_mock]
+        get_last_release_version_mock.return_value = current_version
         command_mock.update_version.side_effect = [
             VersionUpdate(
                 previous=current_version,
                 new=release_version,
                 changed_files=["MyProject.conf"],
             ),
             VersionUpdate(
@@ -1797,16 +1946,14 @@
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
-                "--git-signing-key",
-                "1234",
                 "--local",
             ]
         )
 
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
@@ -1838,18 +1985,19 @@
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
 
 @dataclass
 class Release:
     release_type: str
-    current_version: str
     expected_release_version: str
-    expected_last_release_version: Optional[str] = None
     tags: list[str] = field(default_factory=list)
+    expected_last_release_version: Optional[str] = None
+    current_version: Optional[str] = None
+    release_series: Optional[str] = None
 
 
 @patch.dict(
     "os.environ",
     {"GITHUB_TOKEN": "foo", "GITHUB_USER": "user", "GPG_SIGNING_KEY": ""},
 )
 class ReleaseGoProjectTestCase(unittest.TestCase):
@@ -1861,38 +2009,94 @@
     def test_release(
         self, github_api_mock: AsyncMock, _git_push_mock: MagicMock
     ):
         create_api_mock = AsyncMock()
         github_api_mock.return_value.releases.create = create_api_mock
 
         releases = [
-            Release("major", "1.0.0", "2.0.0"),
-            Release("minor", "1.0.0", "1.1.0"),
-            Release("patch", "1.0.0", "1.0.1"),
-            Release("patch", "1.0.5", "1.0.6"),
-            Release("alpha", "1.0.0", "1.0.1a1"),
-            Release("alpha", "1.0.0a3", "1.0.0a4"),
-            Release("beta", "1.0.0", "1.0.1b1"),
-            Release("beta", "1.0.0b2", "1.0.0b3"),
-            Release("release-candidate", "1.0.0", "1.0.1rc1"),
-            Release("release-candidate", "1.0.0rc1", "1.0.0rc2"),
+            Release(
+                release_type="major",
+                current_version="1.0.0",
+                expected_release_version="2.0.0",
+                tags="1.0.0",
+            ),
+            Release(
+                release_type="minor",
+                current_version="1.0.0",
+                expected_release_version="1.1.0",
+                tags="1.0.0",
+            ),
+            Release(
+                release_type="patch",
+                current_version="1.0.0",
+                expected_release_version="1.0.1",
+                tags="1.0.0",
+            ),
+            Release(
+                release_type="patch",
+                current_version="1.0.5",
+                expected_release_version="1.0.6",
+                tags="1.0.5",
+            ),
+            Release(
+                release_type="alpha",
+                current_version="1.0.0",
+                expected_release_version="1.0.1a1",
+                tags="1.0.0",
+            ),
+            Release(
+                release_type="alpha",
+                current_version="1.0.0a3",
+                expected_release_version="1.0.0a4",
+                tags="1.0.0a3",
+            ),
+            Release(
+                release_type="beta",
+                current_version="1.0.0",
+                expected_release_version="1.0.1b1",
+                tags="1.0.0",
+            ),
+            Release(
+                release_type="beta",
+                current_version="1.0.0b2",
+                expected_release_version="1.0.0b3",
+                tags="1.0.0b2",
+            ),
+            Release(
+                release_type="release-candidate",
+                current_version="1.0.0",
+                expected_release_version="1.0.1rc1",
+                tags="1.0.0",
+            ),
+            Release(
+                release_type="release-candidate",
+                current_version="1.0.0rc1",
+                expected_release_version="1.0.0rc2",
+                tags="1.0.0rc1",
+            ),
         ]
 
         for r in releases:
-            with setup_go_project(current_version=r.current_version):
+            with setup_go_project(
+                current_version=r.current_version, tags=r.tags
+            ):
                 _, token, args = parse_args(
                     ["release", "--release-type", r.release_type]
                 )
                 released = release(
                     terminal=mock_terminal(),
                     args=args,
                     token=token,
                 )
 
-            self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+            self.assertEqual(
+                released,
+                ReleaseReturnValue.SUCCESS,
+                f"v{r.expected_release_version}",
+            )
             self.assertEqual(
                 create_api_mock.call_args.args[1],
                 f"v{r.expected_release_version}",
             )
 
             create_api_mock.reset_mock()
 
@@ -1913,97 +2117,154 @@
     ):
         create_api_mock = AsyncMock()
         github_api_mock.return_value.releases.create = create_api_mock
 
         create_changelog_mock.return_value = "A Changelog"
 
         releases = [
-            Release("major", "1.0.0", "2.0.0", "1.0.0", ["1.0.0", "3.0.0"]),
-            Release("major", "1.0.0rc1", "1.0.0", None, ["3.0.0"]),
-            Release("minor", "1.0.0", "1.1.0", "1.0.0", ["1.0.0", "2.0.0"]),
             Release(
-                "minor", "1.1.0", "1.2.0", "1.1.0", ["1.0.0", "1.1.0", "2.0.0"]
+                release_type="major",
+                current_version="1.0.0",
+                expected_release_version="2.0.0",
+                expected_last_release_version="1.0.0",
+                tags=["1.0.0", "3.0.0"],
+                release_series="1",
             ),
             Release(
-                "patch", "1.0.0", "1.0.1", "1.0.0", ["1.0.0", "1.1.0", "2.0.0"]
+                release_type="major",
+                current_version="1.0.0rc1",
+                expected_release_version="1.0.0",
+                expected_last_release_version="0.9.0",
+                tags=["0.9.0", "0.8.1", "0.5.0"],
             ),
             Release(
-                "patch", "1.0.5", "1.0.6", "1.0.5", ["1.0.5", "1.1.0", "2.0.0"]
+                release_type="minor",
+                current_version="1.0.0",
+                expected_release_version="2.1.0",
+                expected_last_release_version="2.0.0",
+                tags=["1.0.0", "2.0.0"],
             ),
             Release(
-                "patch", "1.0.5", "1.0.6", "1.0.3", ["1.0.3", "1.1.0", "2.0.0"]
+                release_type="minor",
+                current_version="1.0.0",
+                expected_release_version="1.1.0",
+                expected_last_release_version="1.0.0",
+                tags=["1.0.0", "2.0.0"],
+                release_series="1",
             ),
             Release(
-                "patch",
-                "1.1.0rc1",
-                "1.1.0",
-                "1.0.0",
-                ["1.0.0", "1.2.0", "2.0.0"],
+                release_type="minor",
+                current_version="1.1.0",
+                expected_release_version="1.2.0",
+                expected_last_release_version="1.1.0",
+                tags=["1.0.0", "1.1.0", "2.0.0"],
+                release_series="1.1",
             ),
             Release(
-                "alpha",
-                "1.0.0",
-                "1.0.1a1",
-                "1.0.0",
-                ["1.0.0", "2.0.0", "1.1.0"],
+                release_type="patch",
+                current_version="1.0.0",
+                expected_release_version="1.0.1",
+                expected_last_release_version="1.0.0",
+                tags=["1.0.0", "1.1.0", "2.0.0"],
+                release_series="1.0",
             ),
             Release(
-                "alpha",
-                "1.0.0a3",
-                "1.0.0a4",
-                "1.0.0a3",
-                ["1.0.0a3", "2.0.0", "1.1.0"],
+                release_type="patch",
+                current_version="1.0.5",
+                expected_release_version="1.0.6",
+                expected_last_release_version="1.0.5",
+                tags=["1.0.5", "1.1.0", "2.0.0"],
+                release_series="1.0",
             ),
             Release(
-                "beta",
-                "1.0.0",
-                "1.0.1b1",
-                "1.0.0",
-                ["1.0.0", "2.0.0", "1.1.0"],
+                release_type="patch",
+                current_version="1.0.5",
+                expected_release_version="1.1.1",
+                expected_last_release_version="1.1.0",
+                tags=["1.0.5", "1.1.0", "2.0.0"],
+                release_series="1.1",
             ),
             Release(
-                "beta",
-                "1.0.0b2",
-                "1.0.0b3",
-                "1.0.0b2",
-                ["1.0.0b2", "2.0.0", "1.1.0"],
+                release_type="patch",
+                current_version="1.1.0rc1",
+                expected_release_version="1.1.0",
+                expected_last_release_version="1.1.0b1",
+                tags=["1.0.0", "1.1.0b1", "1.2.0", "2.0.0"],
+                release_series="1.1",
             ),
             Release(
-                "release-candidate",
-                "1.0.0",
-                "1.0.1rc1",
-                "1.0.0",
-                ["1.0.0", "2.0.0", "1.1.0"],
+                release_type="alpha",
+                current_version="1.0.0",
+                expected_release_version="1.0.1a1",
+                expected_last_release_version="1.0.0",
+                tags=["1.0.0", "2.0.0", "1.1.0"],
+                release_series="1.0",
             ),
             Release(
-                "release-candidate",
-                "1.0.0rc1",
-                "1.0.0rc2",
-                "1.0.0rc1",
-                ["1.0.0rc1", "2.0.0", "1.1.0"],
+                release_type="alpha",
+                current_version="1.0.0a3",
+                expected_release_version="1.0.0a4",
+                expected_last_release_version="1.0.0a3",
+                tags=["1.0.0a3", "2.0.0", "1.1.0"],
+                release_series="1.0",
+            ),
+            Release(
+                release_type="beta",
+                current_version="1.0.0",
+                expected_release_version="1.0.1b1",
+                expected_last_release_version="1.0.0",
+                tags=["1.0.0", "2.0.0", "1.1.0"],
+                release_series="1.0",
+            ),
+            Release(
+                release_type="beta",
+                current_version="1.0.0b2",
+                expected_release_version="1.0.0b3",
+                expected_last_release_version="1.0.0b2",
+                tags=["1.0.0b2", "2.0.0", "1.1.0"],
+                release_series="1.0",
+            ),
+            Release(
+                release_type="release-candidate",
+                current_version="1.0.0",
+                expected_release_version="1.0.1rc1",
+                expected_last_release_version="1.0.0",
+                tags=["1.0.0", "2.0.0", "1.1.0"],
+                release_series="1.0",
+            ),
+            Release(
+                release_type="release-candidate",
+                current_version="1.0.0rc1",
+                expected_release_version="1.0.0rc2",
+                expected_last_release_version="1.0.0rc1",
+                tags=["1.0.0rc1", "2.0.0", "1.1.0"],
+                release_series="1.0",
             ),
         ]
 
         for r in releases:
             with setup_go_project(
                 current_version=r.current_version, tags=r.tags
             ):
-                _, token, args = parse_args(
-                    ["release", "--release-type", r.release_type]
-                )
+                input_args = ["release", "--release-type", r.release_type]
+                if r.release_series:
+                    input_args.extend(["--release-series", r.release_series])
+
+                _, token, args = parse_args(input_args)
                 released = release(
                     terminal=mock_terminal(),
                     args=args,
                     token=token,
                 )
 
             self.assertEqual(released, ReleaseReturnValue.SUCCESS)
             self.assertEqual(
                 create_api_mock.call_args.args[1],
                 f"v{r.expected_release_version}",
+                f"Unexpected current release version {r}",
             )
 
             self.assertEqual(
                 create_changelog_mock.call_args.args[1],
                 PEP440Version.from_string(r.expected_release_version),
                 f"Unexpected current release version {r}",
             )
```

### Comparing `pontos-23.4.3/tests/release/test_sign.py` & `pontos-23.4.5/tests/release/test_sign.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
         with temp_directory(change_into=True):
             _, token, args = parse_args(
                 [
                     "sign",
                     "--project",
                     "foo",
-                    "--release",
+                    "--release-version",
                     "1.2.3",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
                 args=args,
@@ -343,14 +343,120 @@
                 [
                     (Path("file.zip.asc"), "application/pgp-signature"),
                     (Path("file.tar.asc"), "application/pgp-signature"),
                     (Path("file1.asc"), "application/pgp-signature"),
                     (Path("file2.asc"), "application/pgp-signature"),
                 ],
             )
+
+    @patch("pontos.version.helper.Git", autospec=True)
+    @patch("pontos.release.sign.cmd_runner", autospec=True)
+    @patch("pontos.release.sign.SignCommand.download_asset", autospec=True)
+    @patch("pontos.release.sign.SignCommand.download_tar", autospec=True)
+    @patch("pontos.release.sign.SignCommand.download_zip", autospec=True)
+    @patch("pontos.release.sign.GitHubAsyncRESTApi.releases", autospec=True)
+    def test_sign_success_determine_release_version_with_release_series(
+        self,
+        github_releases_mock: AsyncMock,
+        download_zip_mock: AsyncMock,
+        download_tar_mock: AsyncMock,
+        download_asset_mock: AsyncMock,
+        cmd_runner_mock: AsyncMock,
+        git_mock: MagicMock,
+    ):
+        tar_file = Path("file.tar")
+        zip_file = Path("file.zip")
+        some_asset = Path("file1")
+        other_asset = Path("file2")
+        download_tar_mock.return_value = tar_file
+        download_zip_mock.return_value = zip_file
+        download_asset_mock.side_effect = [some_asset, other_asset]
+        github_releases_mock.exists = AsyncMock(return_value=True)
+        github_releases_mock.download_release_assets.return_value = (
+            AsyncIteratorMock(
+                [
+                    (
+                        "foo",
+                        MagicMock(),
+                    ),
+                    ("bar", MagicMock()),
+                ]
+            )
+        )
+        process = AsyncMock(spec=Process, returncode=0)
+        process.communicate.return_value = ("", "")
+        cmd_runner_mock.return_value = process
+        git_mock.return_value.list_tags.return_value = [
+            "v2.0.1",
+        ]
+
+        with temp_directory(change_into=True):
+            _, token, args = parse_args(
+                ["sign", "--project", "foo", "--release-series", "2"]
+            )
+
+            result = sign(
+                terminal=mock_terminal(),
+                args=args,
+                token=token,
+            )
+
+            self.assertEqual(result, SignReturnValue.SUCCESS)
+
+            cmd_runner_mock.assert_has_calls(
+                [
+                    call(
+                        "gpg",
+                        "--default-key",
+                        "0ED1E580",
+                        "--yes",
+                        "--detach-sign",
+                        "--armor",
+                        zip_file,
+                    ),
+                    call(
+                        "gpg",
+                        "--default-key",
+                        "0ED1E580",
+                        "--yes",
+                        "--detach-sign",
+                        "--armor",
+                        tar_file,
+                    ),
+                    call(
+                        "gpg",
+                        "--default-key",
+                        "0ED1E580",
+                        "--yes",
+                        "--detach-sign",
+                        "--armor",
+                        some_asset,
+                    ),
+                    call(
+                        "gpg",
+                        "--default-key",
+                        "0ED1E580",
+                        "--yes",
+                        "--detach-sign",
+                        "--armor",
+                        other_asset,
+                    ),
+                ]
+            )
+
+            github_releases_mock.upload_release_assets.assert_called_once_with(
+                "greenbone/foo",
+                "v2.0.1",
+                [
+                    (Path("file.zip.asc"), "application/pgp-signature"),
+                    (Path("file.tar.asc"), "application/pgp-signature"),
+                    (Path("file1.asc"), "application/pgp-signature"),
+                    (Path("file2.asc"), "application/pgp-signature"),
+                ],
+            )
 
     @patch("pontos.release.sign.cmd_runner", autospec=True)
     @patch("pontos.release.sign.SignCommand.download_asset", autospec=True)
     @patch("pontos.release.sign.SignCommand.download_tar", autospec=True)
     @patch("pontos.release.sign.SignCommand.download_zip", autospec=True)
     @patch("pontos.release.sign.GitHubAsyncRESTApi.releases", autospec=True)
     def test_sign_success_dry_run(
```

### Comparing `pontos-23.4.3/tests/terminal/test_terminal.py` & `pontos-23.4.5/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/test_helper.py` & `pontos-23.4.5/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/test_pontos.py` & `pontos-23.4.5/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/testing/test_testing.py` & `pontos-23.4.5/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/updateheader/test_header.py` & `pontos-23.4.5/tests/updateheader/test_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,30 +35,17 @@
 from pontos.updateheader.updateheader import (
     _get_modified_year as get_modified_year,
 )
 from pontos.updateheader.updateheader import _parse_args as parse_args
 from pontos.updateheader.updateheader import _update_file as update_file
 from pontos.updateheader.updateheader import main
 
-HEADER = """# Copyright (C) {date} Greenbone AG
+HEADER = """# SPDX-FileCopyrightText: {date} Greenbone AG
 #
-# SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>."""
+# SPDX-License-Identifier: AGPL-3.0-or-later"""
 
 
 class Terminal(ConsoleTerminal):
     @staticmethod
     def get_width() -> int:
         return 999
 
@@ -67,15 +54,15 @@
     def setUp(self):
         self.args = Namespace()
         self.args.company = "Greenbone AG"
 
         self.path = Path(__file__).parent
 
         self.regex = re.compile(
-            "[Cc]opyright.*?(19[0-9]{2}|20[0-9]{2}) "
+            "(SPDX-FileCopyrightText:|[Cc]opyright).*?(19[0-9]{2}|20[0-9]{2}) "
             f"?-? ?(19[0-9]{{2}}|20[0-9]{{2}})? ({self.args.company})"
         )
 
     @patch("pontos.updateheader.updateheader.run")
     def test_get_modified_year(self, run_mock):
         test_file = self.path / "test.py"
         test_file.touch(exist_ok=True)
@@ -132,49 +119,78 @@
         self.assertEqual(match["company"], self.args.company)
 
         # No match
         found, match = find_copyright(regex=self.regex, line=invalid_line)
         self.assertFalse(found)
         self.assertIsNone(match)
 
+    def test_find_spdx_copyright(self):
+        test_line = "# SPDX-FileCopyrightText: 1995-2021 Greenbone AG"
+        test2_line = "# SPDX-FileCopyrightText: 1995 Greenbone AG"
+        invalid_line = (
+            "# This program is free software: "
+            "you can redistribute it and/or modify"
+        )
+
+        # Full match
+        found, match = find_copyright(regex=self.regex, line=test_line)
+        self.assertTrue(found)
+        self.assertIsNotNone(match)
+        self.assertEqual(match["creation_year"], "1995")
+        self.assertEqual(match["modification_year"], "2021")
+        self.assertEqual(match["company"], self.args.company)
+
+        # No modification Date
+        found, match = find_copyright(regex=self.regex, line=test2_line)
+        self.assertTrue(found)
+        self.assertIsNotNone(match)
+        self.assertEqual(match["creation_year"], "1995")
+        self.assertEqual(match["modification_year"], None)
+        self.assertEqual(match["company"], self.args.company)
+
+        # No match
+        found, match = find_copyright(regex=self.regex, line=invalid_line)
+        self.assertFalse(found)
+        self.assertIsNone(match)
+
     def test_add_header(self):
         expected_header = HEADER.format(date="2021") + "\n"
 
         header = add_header(
             suffix=".py",
-            licence="AGPL-3.0-or-later",
+            license_id="AGPL-3.0-or-later",
             company=self.args.company,
             year="2021",
         )
 
         self.assertEqual(header, expected_header)
 
     def test_add_header_wrong_file_suffix(self):
         with self.assertRaises(ValueError):
             add_header(
                 suffix=".prr",
-                licence="AGPL-3.0-or-later",
+                license_id="AGPL-3.0-or-later",
                 company=self.args.company,
                 year="2021",
             )
 
-    def test_add_header_licence_not_found(self):
+    def test_add_header_license_not_found(self):
         with self.assertRaises(FileNotFoundError):
             add_header(
                 suffix=".py",
-                licence="AAAGPL-3.0-or-later",
+                license_id="AAAGPL-3.0-or-later",
                 company=self.args.company,
                 year="2021",
             )
 
     @patch("sys.stdout", new_callable=StringIO)
     def test_update_file_not_existing(self, mock_stdout):
         self.args.year = "2020"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         term = Terminal()
 
         test_file = self.path / "test.py"
         if test_file.exists():
             test_file.unlink()
 
@@ -189,67 +205,67 @@
         ret = mock_stdout.getvalue()
         self.assertEqual(
             ret,
             f"{test_file}: File is not existing.\n",
         )
 
     @patch("sys.stdout", new_callable=StringIO)
-    def test_update_file_wrong_licence(self, mock_stdout):
+    def test_update_file_wrong_license(self, mock_stdout):
         self.args.year = "2020"
         self.args.changed = False
-        self.args.licence = "AAAGPL-3.0-or-later"
+        self.args.license_id = "AAAGPL-3.0-or-later"
 
         term = Terminal()
 
         test_file = self.path / "test.py"
         test_file.touch()
 
         code = update_file(
             file=test_file, regex=self.regex, parsed_args=self.args, term=term
         )
         self.assertEqual(code, 1)
 
         ret = mock_stdout.getvalue()
         self.assertEqual(
             ret,
-            f"{test_file}: Licence file for "
+            f"{test_file}: License file for "
             "AAAGPL-3.0-or-later is not existing.\n",
         )
 
         test_file.unlink()
 
     @patch("sys.stdout", new_callable=StringIO)
     def test_update_file_suffix_invalid(self, mock_stdout):
         self.args.year = "2020"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         term = Terminal()
 
         test_file = self.path / "test.pppy"
         test_file.touch()
 
         code = update_file(
             file=test_file, regex=self.regex, parsed_args=self.args, term=term
         )
         self.assertEqual(code, 1)
 
         ret = mock_stdout.getvalue()
         self.assertEqual(
             ret,
-            f"{test_file}: No licence header for the format .pppy found.\n",
+            f"{test_file}: No license header for the format .pppy found.\n",
         )
 
         test_file.unlink()
 
     @patch("sys.stdout", new_callable=StringIO)
     def test_update_file_binary_file(self, mock_stdout):
         self.args.year = "2020"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         term = Terminal()
 
         test_file = self.path / "test.py"
         if test_file.exists():
             test_file.unlink()
 
@@ -275,15 +291,15 @@
 
         test_file.unlink()
 
     @patch("sys.stdout", new_callable=StringIO)
     def test_update_file_changed(self, mock_stdout):
         self.args.year = "1995"
         self.args.changed = True
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         term = Terminal()
 
         test_file = self.path / "test.py"
         if test_file.exists():
             test_file.unlink()
 
@@ -304,41 +320,41 @@
         self.assertIn(f"using {self.args.year} instead.", ret)
         self.assertIn("File is not existing.", ret)
 
     @patch("sys.stdout", new_callable=StringIO)
     def test_update_create_header(self, mock_stdout):
         self.args.year = "1995"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         term = Terminal()
 
         expected_header = HEADER.format(date="1995") + "\n\n"
 
         test_file = self.path / "test.py"
         test_file.touch()
 
         code = update_file(
             file=test_file, regex=self.regex, parsed_args=self.args, term=term
         )
 
         ret = mock_stdout.getvalue()
         self.assertEqual(
-            f"{test_file}: Added licence header.\n",
+            f"{test_file}: Added license header.\n",
             ret,
         )
         self.assertEqual(code, 0)
         self.assertEqual(expected_header, test_file.read_text(encoding="utf-8"))
         test_file.unlink()
 
     @patch("sys.stdout", new_callable=StringIO)
     def test_update_header_in_file(self, mock_stdout):
         self.args.year = "2021"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         term = Terminal()
 
         header = HEADER.format(date="2020")
 
         test_file = self.path / "test.py"
         if test_file.exists():
@@ -350,29 +366,29 @@
             file=test_file, regex=self.regex, parsed_args=self.args, term=term
         )
 
         self.assertEqual(code, 0)
         ret = mock_stdout.getvalue()
         self.assertEqual(
             ret,
-            f"{test_file}: Changed Licence Header "
+            f"{test_file}: Changed License Header "
             "Copyright Year None -> 2021\n",
         )
         self.assertIn(
-            "# Copyright (C) 2020-2021 Greenbone AG",
+            "# SPDX-FileCopyrightText: 2020-2021 Greenbone AG",
             test_file.read_text(encoding="utf-8"),
         )
 
         test_file.unlink()
 
     @patch("sys.stdout", new_callable=StringIO)
     def test_update_header_ok_in_file(self, mock_stdout):
         self.args.year = "2021"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         term = Terminal()
 
         header = HEADER.format(date="2021")
 
         test_file = self.path / "test.py"
         if test_file.exists():
@@ -384,51 +400,51 @@
             file=test_file, regex=self.regex, parsed_args=self.args, term=term
         )
 
         self.assertEqual(code, 0)
         ret = mock_stdout.getvalue()
         self.assertEqual(
             ret,
-            f"{test_file}: Licence Header is ok.\n",
+            f"{test_file}: License Header is ok.\n",
         )
         self.assertIn(
-            "# Copyright (C) 2021 Greenbone AG",
+            "# SPDX-FileCopyrightText: 2021 Greenbone AG",
             test_file.read_text(encoding="utf-8"),
         )
 
         test_file.unlink()
 
     def test_argparser_files(self):
         self.args.year = "2021"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         args = ["-f", "test.py", "-y", "2021", "-l", "AGPL-3.0-or-later"]
 
         args = parse_args(args)
         self.assertIsNotNone(args)
         self.assertEqual(args.company, self.args.company)
         self.assertEqual(args.files, ["test.py"])
         self.assertEqual(args.year, self.args.year)
-        self.assertEqual(args.licence, self.args.licence)
+        self.assertEqual(args.license, self.args.license_id)
 
     def test_argparser_dir(self):
         self.args.year = "2020"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
 
         args = ["-d", ".", "-c", "-l", "AGPL-3.0-or-later"]
 
         args = parse_args(args)
         self.assertIsNotNone(args)
         self.assertEqual(args.company, self.args.company)
         self.assertEqual(args.directories, ["."])
         self.assertTrue(args.changed)
         self.assertEqual(args.year, str(datetime.datetime.now().year))
-        self.assertEqual(args.licence, self.args.licence)
+        self.assertEqual(args.license, self.args.license_id)
 
     def test_get_exclude_list(self):
         # Try to find the current file from two directories up...
         test_dirname = Path(__file__) / "../.."
         # with a relative glob
         test_ignore_file = Path("ignore.file")
         test_ignore_file.write_text("*.py\n", encoding="utf-8")
@@ -441,15 +457,15 @@
 
         test_ignore_file.unlink()
 
     @patch("pontos.updateheader.updateheader._parse_args")
     def test_main(self, argparser_mock):
         self.args.year = "2021"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
         self.args.files = ["test.py"]
         self.args.directories = None
         self.args.verbose = 0
         self.args.log_file = None
         self.args.quiet = False
 
         argparser_mock.return_value = self.args
@@ -461,15 +477,15 @@
         self.assertTrue(code)
 
     @patch("sys.stdout", new_callable=StringIO)
     @patch("pontos.updateheader.updateheader._parse_args")
     def test_main_never_happen(self, argparser_mock, mock_stdout):
         self.args.year = "2021"
         self.args.changed = False
-        self.args.licence = "AGPL-3.0-or-later"
+        self.args.license_id = "AGPL-3.0-or-later"
         self.args.files = None
         self.args.directories = None
         self.args.verbose = 0
         self.args.log_file = None
         self.args.quiet = False
 
         argparser_mock.return_value = self.args
```

### Comparing `pontos-23.4.3/tests/version/commands/test_cmake.py` & `pontos-23.4.5/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/commands/test_go.py` & `pontos-23.4.5/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/commands/test_javascript.py` & `pontos-23.4.5/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/commands/test_python.py` & `pontos-23.4.5/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/schemes/test_pep440.py` & `pontos-23.4.5/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/schemes/test_semantic.py` & `pontos-23.4.5/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/test_helper.py` & `pontos-23.4.5/tests/version/test_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,78 +15,129 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import unittest
 from unittest.mock import patch
 
 from pontos.git.git import Git
+from pontos.version.errors import VersionError
 from pontos.version.helper import (
     get_last_release_version,
     get_last_release_versions,
 )
-from pontos.version.schemes import PEP440VersioningScheme
+from pontos.version.schemes import (
+    PEP440VersioningScheme,
+    SemanticVersioningScheme,
+)
 
 parse_version = PEP440VersioningScheme.parse_version
 Version = PEP440VersioningScheme.version_cls
 
 
 class GetLastReleaseVersionsTestCase(unittest.TestCase):
     @patch("pontos.version.helper.Git", spec=Git)
     def test_get_last_release_versions(self, git_mock):
         git_interface = git_mock.return_value
         git_interface.list_tags.return_value = ["1", "2", "3.55"]
-        self.assertEqual(
-            get_last_release_versions(parse_version),
-            [Version("3.55"), Version("2"), Version("1")],
-        )
+
+        it = get_last_release_versions(parse_version)
+
+        version = next(it)
+        self.assertEqual(version, Version("3.55"))
+
+        version = next(it)
+        self.assertEqual(version, Version("2"))
+
+        version = next(it)
+        self.assertEqual(version, Version("1"))
+
+        with self.assertRaises(StopIteration):
+            next(it)
 
     @patch("pontos.version.helper.Git", spec=Git)
     def test_get_no_release_versions(self, git_mock):
         git_interface = git_mock.return_value
         git_interface.list_tags.return_value = []
-        self.assertEqual(get_last_release_versions(parse_version), [])
+
+        it = get_last_release_versions(parse_version)
+        with self.assertRaises(StopIteration):
+            next(it)
 
     @patch("pontos.version.helper.Git", spec=Git)
     def test_get_last_release_versions_with_git_prefix(self, git_mock):
         git_interface = git_mock.return_value
         git_interface.list_tags.return_value = ["v1", "v2", "v3.55"]
-        self.assertEqual(
-            get_last_release_versions(parse_version, git_tag_prefix="v"),
-            [Version("3.55"), Version("2"), Version("1")],
-        )
+
+        it = get_last_release_versions(parse_version, git_tag_prefix="v")
+
+        version = next(it)
+        self.assertEqual(version, Version("3.55"))
+
+        version = next(it)
+        self.assertEqual(version, Version("2"))
+
+        version = next(it)
+        self.assertEqual(version, Version("1"))
+
+        with self.assertRaises(StopIteration):
+            next(it)
 
     @patch("pontos.version.helper.Git", spec=Git)
     def test_get_last_release_versions_ignore_pre_releases(self, git_mock):
         git_interface = git_mock.return_value
         git_interface.list_tags.return_value = [
             "1",
             "2",
             "3.55a1",
             "3.56.dev1",
             "4.0.0rc1",
             "4.0.1b1",
         ]
-        self.assertEqual(
-            get_last_release_versions(parse_version, ignore_pre_releases=True),
-            [Version("2"), Version("1")],
-        )
+        it = get_last_release_versions(parse_version, ignore_pre_releases=True)
+
+        version = next(it)
+        self.assertEqual(version, Version("2"))
+
+        version = next(it)
+        self.assertEqual(version, Version("1"))
+
+        with self.assertRaises(StopIteration):
+            next(it)
 
     @patch("pontos.version.helper.Git", spec=Git)
     def test_get_last_release_versions_no_non_pre_release(self, git_mock):
         git_interface = git_mock.return_value
         git_interface.list_tags.return_value = [
             "3.55a1",
             "3.56.dev1",
             "4.0.0rc1",
             "4.0.1b1",
         ]
-        self.assertEqual(
-            get_last_release_versions(parse_version, ignore_pre_releases=True),
-            [],
-        )
+
+        it = get_last_release_versions(parse_version, ignore_pre_releases=True)
+
+        with self.assertRaises(StopIteration):
+            next(it)
+
+    @patch("pontos.version.helper.Git", spec=Git)
+    def test_invalid_version(self, git_mock):
+        git_interface = git_mock.return_value
+        git_interface.list_tags.return_value = [
+            "1.0.0",
+            "3.55a1",
+            "2.0.0",
+        ]
+
+        it = get_last_release_versions(SemanticVersioningScheme.parse_version)
+        next(it)
+
+        with self.assertRaisesRegex(
+            VersionError, "3.55a1 is not valid SemVer string"
+        ):
+            next(it)
 
 
 class GetLastReleaseVersionTestCase(unittest.TestCase):
     @patch("pontos.version.helper.Git", spec=Git)
     def test_get_last_release_version(self, git_mock):
         git_interface = git_mock.return_value
         git_interface.list_tags.return_value = ["1", "2", "3.55"]
@@ -145,7 +196,34 @@
             "4.0.0rc1",
             "4.0.1b1",
         ]
         self.assertEqual(
             get_last_release_version(parse_version, tag_name="4.0.*"),
             Version("4.0.1b1"),
         )
+
+    @patch("pontos.version.helper.Git", spec=Git)
+    def test_invalid_version(self, git_mock):
+        git_interface = git_mock.return_value
+        git_interface.list_tags.return_value = ["1", "2", "3.55a1"]
+
+        with self.assertRaisesRegex(
+            VersionError, "3.55a1 is not valid SemVer string"
+        ):
+            get_last_release_version(SemanticVersioningScheme.parse_version)
+
+    @patch("pontos.version.helper.Git", spec=Git)
+    def test_success_with_invalid_version(self, git_mock):
+        git_interface = git_mock.return_value
+        git_interface.list_tags.return_value = [
+            "1.0.0",
+            "2.0.0",
+            "3.55a1",
+            "4.0.0",
+        ]
+
+        version = get_last_release_version(
+            SemanticVersioningScheme.parse_version
+        )
+        self.assertEqual(
+            version, SemanticVersioningScheme.parse_version("4.0.0")
+        )
```

### Comparing `pontos-23.4.3/tests/version/test_main.py` & `pontos-23.4.5/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/test_project.py` & `pontos-23.4.5/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/tests/version/test_version.py` & `pontos-23.4.5/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.3/PKG-INFO` & `pontos-23.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.4.3
+Version: 23.4.5
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: colorful (>=0.5.4,<0.6.0)
-Requires-Dist: httpx[http2] (>=0.23.0,<0.24.0)
+Requires-Dist: httpx[http2] (>=0.23,<0.25)
 Requires-Dist: packaging (>=20.3)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: rich (>=12.4.4)
 Requires-Dist: semver (>=2.13,<4.0)
 Requires-Dist: tomlkit (>=0.5.11)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Project-URL: Documentation, https://greenbone.github.io/pontos/
```

