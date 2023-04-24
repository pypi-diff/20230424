# Comparing `tmp/saffier-0.7.3.tar.gz` & `tmp/saffier-0.7.4.tar.gz`

## Comparing `saffier-0.7.3.tar` & `saffier-0.7.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/exceptions.py
--rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/fields.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/metaclass.py
--rw-r--r--   0        0        0     9039 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/models.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/testclient.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/types.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/enums.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/functional.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/base.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/datastructures.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/events.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/formats.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/schemas.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/sync.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/unique.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/base.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/print.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/connection.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/constants.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/datastructures.py
--rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/fields.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/manager.py
--rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/query/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/query/protocols.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/__init__.py
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/base.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/cli.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/constants.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/decorators.py
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/env.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/branches.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/check.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/current.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/downgrade.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/edit.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/heads.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/history.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/init.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/list_templates.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/makemigrations.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/merge.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/migrate.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/revision.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/show.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/stamp.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/__init__.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/enums.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/ipython.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/fields.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/types.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.3/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.3/README.md
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 saffier-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 saffier-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/exceptions.py
+-rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/fields.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/metaclass.py
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/models.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/testclient.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/types.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/enums.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/functional.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/base.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/events.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/formats.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/schemas.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/sync.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/unique.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/print.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/connection.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/constants.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/datastructures.py
+-rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/fields.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/manager.py
+-rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/query/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/db/query/protocols.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/__init__.py
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/base.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/constants.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/decorators.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/env.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/branches.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/check.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/current.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/downgrade.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/edit.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/heads.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/history.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/init.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/list_templates.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/makemigrations.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/merge.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/migrate.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/revision.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/show.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/enums.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/migrations/templates/default/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.4/saffier/sqlalchemy/types.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.4/LICENSE
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.4/README.md
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 saffier-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0    11190 2020-02-02 00:00:00.000000 saffier-0.7.4/PKG-INFO
```

### Comparing `saffier-0.7.3/saffier/__init__.py` & `saffier-0.7.4/saffier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.3"
+__version__ = "0.7.4"
 
 from saffier.conf import settings
 from saffier.conf.global_settings import SaffierSettings
 
 from .core.registry import Registry
 from .db.connection import Database
 from .db.constants import CASCADE, RESTRICT, SET_NULL
```

### Comparing `saffier-0.7.3/saffier/exceptions.py` & `saffier-0.7.4/saffier/exceptions.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/fields.py` & `saffier-0.7.4/saffier/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/metaclass.py` & `saffier-0.7.4/saffier/metaclass.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/models.py` & `saffier-0.7.4/saffier/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import asyncio
 import functools
 import typing
 
-import nest_asyncio
 import sqlalchemy
 from sqlalchemy.engine import Engine
 
 from saffier.core.schemas import Schema
 from saffier.core.utils import ModelUtil
 from saffier.db.datastructures import Index, UniqueConstraint
 from saffier.db.manager import Manager
 from saffier.exceptions import ImproperlyConfigured
 from saffier.metaclass import MetaInfo, ModelMeta, ReflectMeta
 
-nest_asyncio.apply()
-
 
 def async_adapter(wrapped_func):
     """Adapter to run async functions inside the blocking"""
 
     @functools.wraps(wrapped_func)
     def run_sync(*args, **kwargs):
         loop = asyncio.get_event_loop()
```

### Comparing `saffier-0.7.3/saffier/conf/__init__.py` & `saffier-0.7.4/saffier/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/conf/functional.py` & `saffier-0.7.4/saffier/conf/functional.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/conf/global_settings.py` & `saffier-0.7.4/saffier/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/conf/module_import.py` & `saffier-0.7.4/saffier/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/base.py` & `saffier-0.7.4/saffier/core/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/datastructures.py` & `saffier-0.7.4/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/events.py` & `saffier-0.7.4/saffier/core/events.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/formats.py` & `saffier-0.7.4/saffier/core/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/registry.py` & `saffier-0.7.4/saffier/core/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,9 +82,8 @@
 
         await self.engine.dispose()
 
     async def drop_all(self) -> None:
         async with self.database:
             async with self.engine.begin() as conn:
                 await conn.run_sync(self.metadata.drop_all)
-
         await self.engine.dispose()
```

### Comparing `saffier-0.7.3/saffier/core/schemas.py` & `saffier-0.7.4/saffier/core/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/sync.py` & `saffier-0.7.4/saffier/core/sync.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/unique.py` & `saffier-0.7.4/saffier/core/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/utils.py` & `saffier-0.7.4/saffier/core/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/terminal/base.py` & `saffier-0.7.4/saffier/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/terminal/print.py` & `saffier-0.7.4/saffier/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/core/terminal/terminal.py` & `saffier-0.7.4/saffier/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/db/datastructures.py` & `saffier-0.7.4/saffier/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/db/fields.py` & `saffier-0.7.4/saffier/db/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         elif value is None:
             raise self.validation_error("null")
         elif value not in Uniqueness([key for key, value in self.choices]):
             if value == "":
                 if self.null and self.coerce_types:
                     return None
                 raise self.validation_error("required")
-            raise self.validation_error(("required"))
+            raise self.validation_error("required")
         return value
 
 
 class Text(String):
     def __init__(self, **kwargs: typing.Any) -> None:
         super().__init__(format="text", **kwargs)
 
@@ -389,15 +389,15 @@
         "union": "Did not match any valid type.",
     }
 
     def __init__(self, any_of: typing.List[SaffierField], **kwargs: typing.Any):
         super().__init__(**kwargs)
 
         self.any_of = any_of
-        if any([child.null for child in any_of]):
+        if any(child.null for child in any_of):
             self.allow_null = True
 
     def check(self, value: typing.Any) -> typing.Any:
         if value is None and self.allow_null:
             return None
         elif value is None:
             raise self.validation_error("null")
```

### Comparing `saffier-0.7.3/saffier/db/manager.py` & `saffier-0.7.4/saffier/db/manager.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/db/queryset.py` & `saffier-0.7.4/saffier/db/queryset.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/db/query/protocols.py` & `saffier-0.7.4/saffier/db/query/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/base.py` & `saffier-0.7.4/saffier/migrations/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/cli.py` & `saffier-0.7.4/saffier/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/env.py` & `saffier-0.7.4/saffier/migrations/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/__init__.py` & `saffier-0.7.4/saffier/migrations/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/branches.py` & `saffier-0.7.4/saffier/migrations/operations/branches.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/current.py` & `saffier-0.7.4/saffier/migrations/operations/current.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/downgrade.py` & `saffier-0.7.4/saffier/migrations/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/heads.py` & `saffier-0.7.4/saffier/migrations/operations/heads.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/history.py` & `saffier-0.7.4/saffier/migrations/operations/history.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/init.py` & `saffier-0.7.4/saffier/migrations/operations/init.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/makemigrations.py` & `saffier-0.7.4/saffier/migrations/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/merge.py` & `saffier-0.7.4/saffier/migrations/operations/merge.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/migrate.py` & `saffier-0.7.4/saffier/migrations/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/revision.py` & `saffier-0.7.4/saffier/migrations/operations/revision.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/stamp.py` & `saffier-0.7.4/saffier/migrations/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/shell/base.py` & `saffier-0.7.4/saffier/migrations/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/shell/ipython.py` & `saffier-0.7.4/saffier/migrations/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/shell/ptpython.py` & `saffier-0.7.4/saffier/migrations/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/operations/shell/utils.py` & `saffier-0.7.4/saffier/migrations/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/templates/default/alembic.ini.mako` & `saffier-0.7.4/saffier/migrations/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/migrations/templates/default/env.py` & `saffier-0.7.4/saffier/migrations/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/sqlalchemy/fields.py` & `saffier-0.7.4/saffier/sqlalchemy/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/saffier/sqlalchemy/protocols.py` & `saffier-0.7.4/saffier/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/LICENSE` & `saffier-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/README.md` & `saffier-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `saffier-0.7.3/pyproject.toml` & `saffier-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -39,19 +39,17 @@
 ]
 dependencies = [
     "alembic>=1.9.3,<2.0.0",
     "anyio>=3.6.2,<4",
     "click>=8.1.3,<9.0.0",
     "loguru>=0.6.0,<0.7.0",
     "databasez>=0.2.0",
-    "nest_asyncio>=1.5.6,<2.0.0",
     "orjson >=3.8.5,<4.0.0",
     "pydantic>=1.10.5,<2.0.0",
     "rich>=13.3.1,<14.0.0",
-    "sqlalchemy>=2.0.8,<2.1",
 ]
 keywords = [
     "api",
     "rest",
     "http",
     "asgi",
     "pydantic",
```

### Comparing `saffier-0.7.3/PKG-INFO` & `saffier-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saffier
-Version: 0.7.3
+Version: 0.7.4
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -37,19 +37,17 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: alembic<2.0.0,>=1.9.3
 Requires-Dist: anyio<4,>=3.6.2
 Requires-Dist: click<9.0.0,>=8.1.3
 Requires-Dist: databasez>=0.2.0
 Requires-Dist: loguru<0.7.0,>=0.6.0
-Requires-Dist: nest-asyncio<2.0.0,>=1.5.6
 Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic<2.0.0,>=1.10.5
 Requires-Dist: rich<14.0.0,>=13.3.1
-Requires-Dist: sqlalchemy<2.1,>=2.0.8
 Provides-Extra: all
 Requires-Dist: databasez[mysql,postgresql,sqlite]; extra == 'all'
 Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'all'
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'all'
 Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'all'
 Requires-Dist: pydantic<2.0.0,>=1.10.4; extra == 'all'
 Provides-Extra: dev
```

