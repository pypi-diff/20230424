# Comparing `tmp/jupyter_collaboration-1.0.0a7.tar.gz` & `tmp/jupyter_collaboration-1.0.0a8.tar.gz`

## Comparing `jupyter_collaboration-1.0.0a7.tar` & `jupyter_collaboration-1.0.0a8.tar`

### file list

```diff
@@ -1,99 +1,103 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.eslintrc.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.gitconfig
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.npmignore
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.prettierrc
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.readthedocs.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.stylelintrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.yarnrc.yml
--rw-r--r--   0        0        0    36954 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/CHANGELOG.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/CONTRIBUTING.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/RELEASE.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/codecov.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/install.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/lerna.json
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/setup.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/tsconfig.json
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/tsconfig.test.json
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/typedoc.json
--rw-r--r--   0        0        0   466278 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/yarn.lock
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/Makefile
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/make.bat
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/conf.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/configuration.md
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/index.md
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/_static/jupyter_logo.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/developer/architecture.md
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/developer/contributing.rst
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/developer/javascript_api.rst
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/developer/python_api.rst
--rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/docs/source/images/rtc_shared_cursors.png
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter-config/jupyter_collaboration.json
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/_version.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/app.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/handlers.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/package.json
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/413.ed870732b79e27f9bc6d.js
--rw-r--r--   0        0        0    11080 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/493.186e89468d33ae2f1acb.js
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/497.53bcecf29101af297e6d.js
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/8.e96092f47976d91f296d.js
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/839.b379ccb87adf98b344b9.js
--rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/9.1a44b656eb74a0222c38.js
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/933.6dbefb158f22077b6dbf.js
--rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/remoteEntry.ed732341b4b6f42ac23d.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/style.js
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/scripts/bump_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/tests/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/tests/test_ydoc.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/README.md
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/babel.config.js
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/src/utils.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/packages/docprovider/test/yprovider.spec.ts
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/LICENSE
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/README.md
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/pyproject.toml
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a7/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.eslintrc.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.flake8
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.gitconfig
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.npmignore
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.prettierrc
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.readthedocs.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.stylelintrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.yarnrc.yml
+-rw-r--r--   0        0        0    38959 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/CHANGELOG.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/RELEASE.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/codecov.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/install.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/lerna.json
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/setup.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tsconfig.json
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tsconfig.test.json
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/typedoc.json
+-rw-r--r--   0        0        0   488941 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/yarn.lock
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/Makefile
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/make.bat
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/conf.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/configuration.md
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/index.md
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/_static/jupyter_logo.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/architecture.md
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/contributing.rst
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/javascript_api.rst
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/developer/python_api.rst
+-rw-r--r--   0        0        0    61242 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/docs/source/images/rtc_shared_cursors.png
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter-config/jupyter_collaboration.json
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/_version.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/app.py
+-rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/handlers.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/loaders.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/rooms.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/stores.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/utils.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/package.json
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/413.cf154c48ecaa08648e56.js
+-rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/493.0975334cbddac1bcf819.js
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/497.ab1a0ee570b8e4f31289.js
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/8.6b2a09634af3599cbddb.js
+-rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/839.2efa17f8ec8b5c6c87a6.js
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/9.f46ff2dd7fa86c1246e8.js
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/933.f161fc3dcf0d2c141b27.js
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/remoteEntry.c7ae49e75d2022d8409a.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/style.js
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/scripts/bump_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tests/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/tests/test_ydoc.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/README.md
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/babel.config.js
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/tsconfig.json
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/collaboratorspanel.tsx
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/components.tsx
+-rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/cursors.ts
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/index.ts
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/menu.ts
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/tokens.ts
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/userinfopanel.tsx
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/src/utils.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/base.css
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/index.js
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/menu.css
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration/style/sidepanel.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/README.md
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/tsconfig.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/schema/user-menu-bar.json
+-rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/collaboration.ts
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/index.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/collaboration-extension/style/index.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/packages/docprovider/test/yprovider.spec.ts
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/LICENSE
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/README.md
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/pyproject.toml
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 jupyter_collaboration-1.0.0a8/PKG-INFO
```

### Comparing `jupyter_collaboration-1.0.0a7/.eslintrc.js` & `jupyter_collaboration-1.0.0a8/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/.pre-commit-config.yaml` & `jupyter_collaboration-1.0.0a8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/CHANGELOG.md` & `jupyter_collaboration-1.0.0a8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,42 @@
-## Changelog
+# Changelog
 
 All notable changes to this project will be documented in this file.
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.0.0alpha8
+
+([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.7...2e5a6cc66961a5552e8a89c0850c7483c1e1acb2))
+
+### Enhancements made
+
+- Follow up #133 [#136](https://github.com/jupyterlab/jupyter_collaboration/pull/136) ([@hbcarlos](https://github.com/hbcarlos))
+- Creates a new FileLoader class to separate the logic of watching files [#121](https://github.com/jupyterlab/jupyter_collaboration/pull/121) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Bugs fixed
+
+- Fix metadata [#138](https://github.com/jupyterlab/jupyter_collaboration/pull/138) ([@hbcarlos](https://github.com/hbcarlos))
+
+### Maintenance and upkeep improvements
+
+- Upgrade jupyter ydoc [#135](https://github.com/jupyterlab/jupyter_collaboration/pull/135) ([@fcollonval](https://github.com/fcollonval))
+
+### Documentation improvements
+
+- Upgrade jupyter ydoc [#135](https://github.com/jupyterlab/jupyter_collaboration/pull/135) ([@fcollonval](https://github.com/fcollonval))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter_collaboration/graphs/contributors?from=2023-03-29&to=2023-04-24&type=c))
+
+[@codecov-commenter](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Acodecov-commenter+updated%3A2023-03-29..2023-04-24&type=Issues) | [@davidbrochart](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Adavidbrochart+updated%3A2023-03-29..2023-04-24&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Afcollonval+updated%3A2023-03-29..2023-04-24&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Agithub-actions+updated%3A2023-03-29..2023-04-24&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Ahbcarlos+updated%3A2023-03-29..2023-04-24&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.0.0alpha7
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.6...9d8475f5cc333e22b50160ec32e508a4e8c75c06))
 
 ### Enhancements made
 
 - Allow other extensions to register shared models [#133](https://github.com/jupyterlab/jupyter_collaboration/pull/133) ([@hbcarlos](https://github.com/hbcarlos))
@@ -18,16 +47,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/jupyter_collaboration/graphs/contributors?from=2023-03-27&to=2023-03-29&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Agithub-actions+updated%3A2023-03-27..2023-03-29&type=Issues) | [@hbcarlos](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Ahbcarlos+updated%3A2023-03-27..2023-03-29&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Ajupyterlab%2Fjupyter_collaboration+involves%3Atrungleduc+updated%3A2023-03-27..2023-03-29&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.0alpha6
 
 ([Full Changelog](https://github.com/jupyterlab/jupyter_collaboration/compare/@jupyter/collaboration-extension@1.0.0-alpha.5...01836212bc693eae5404453785a591d15770880e))
 
 ### Bugs fixed
 
 - Justify content in side panel [#131](https://github.com/jupyterlab/jupyter_collaboration/pull/131) ([@martinRenou](https://github.com/martinRenou))
```

### Comparing `jupyter_collaboration-1.0.0a7/package.json` & `jupyter_collaboration-1.0.0a8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'1.0.0-alpha.8'"}*

```diff
@@ -59,14 +59,14 @@
         "stylelint:check": "stylelint --cache \"packages/**/style/**/*.css\"",
         "test": "lerna run test",
         "test:cov": "lerna run test:cov",
         "test:debug": "lerna run test:debug",
         "test:debug:watch": "lerna run test:debug:watch",
         "watch": "lerna run watch"
     },
-    "version": "1.0.0-alpha.7",
+    "version": "1.0.0-alpha.8",
     "workspaces": {
         "packages": [
             "packages/*"
         ]
     }
 }
```

### Comparing `jupyter_collaboration-1.0.0a7/yarn.lock` & `jupyter_collaboration-1.0.0a8/yarn.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is generated by running "yarn install" inside your project.
 # Manual changes might be lost - proceed with caution!
 
 __metadata:
   version: 6
   cacheKey: 8
 
-"@ampproject/remapping@npm:^2.1.0":
+"@ampproject/remapping@npm:^2.2.0":
   version: 2.2.0
   resolution: "@ampproject/remapping@npm:2.2.0"
   dependencies:
     "@jridgewell/gen-mapping": ^0.1.0
     "@jridgewell/trace-mapping": ^0.3.9
   checksum: d74d170d06468913921d72430259424b7e4c826b5a7d39ff839a29d547efb97dc577caa8ba3fb5cf023624e9af9d09651afc3d4112a45e2050328abc9b3a2292
   languageName: node
@@ -21,51 +21,52 @@
   dependencies:
     "@babel/highlight": ^7.18.6
   checksum: 195e2be3172d7684bf95cff69ae3b7a15a9841ea9d27d3c843662d50cdd7d6470fd9c8e64be84d031117e4a4083486effba39f9aef6bbb2c89f7f21bcfba33ba
   languageName: node
   linkType: hard
 
 "@babel/compat-data@npm:^7.17.7, @babel/compat-data@npm:^7.20.1, @babel/compat-data@npm:^7.20.5":
-  version: 7.20.14
-  resolution: "@babel/compat-data@npm:7.20.14"
-  checksum: 6c9efe36232094e4ad0b70d165587f21ca718e5d011f7a52a77a18502a7524e90e2855aa5a2e086395bcfd21bd2c7c99128dcd8d9fdffe94316b72acf5c66f2c
+  version: 7.21.0
+  resolution: "@babel/compat-data@npm:7.21.0"
+  checksum: dbf632c532f9c75ba0be7d1dc9f6cd3582501af52f10a6b90415d634ec5878735bd46064c91673b10317af94d4cc99c4da5bd9d955978cdccb7905fc33291e4d
   languageName: node
   linkType: hard
 
 "@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3":
-  version: 7.20.12
-  resolution: "@babel/core@npm:7.20.12"
+  version: 7.21.3
+  resolution: "@babel/core@npm:7.21.3"
   dependencies:
-    "@ampproject/remapping": ^2.1.0
+    "@ampproject/remapping": ^2.2.0
     "@babel/code-frame": ^7.18.6
-    "@babel/generator": ^7.20.7
+    "@babel/generator": ^7.21.3
     "@babel/helper-compilation-targets": ^7.20.7
-    "@babel/helper-module-transforms": ^7.20.11
-    "@babel/helpers": ^7.20.7
-    "@babel/parser": ^7.20.7
+    "@babel/helper-module-transforms": ^7.21.2
+    "@babel/helpers": ^7.21.0
+    "@babel/parser": ^7.21.3
     "@babel/template": ^7.20.7
-    "@babel/traverse": ^7.20.12
-    "@babel/types": ^7.20.7
+    "@babel/traverse": ^7.21.3
+    "@babel/types": ^7.21.3
     convert-source-map: ^1.7.0
     debug: ^4.1.0
     gensync: ^1.0.0-beta.2
     json5: ^2.2.2
     semver: ^6.3.0
-  checksum: 62e6c3e2149a70b5c9729ef5f0d3e2e97e9dcde89fc039c8d8e3463d5d7ba9b29ee84d10faf79b61532ac1645aa62f2bd42338320617e6e3a8a4d8e2a27076e7
+  checksum: bef25fbea96f461bf79bd1d0e4f0cdce679fd5ada464a89c1141ddba59ae1adfdbb23e04440c266ed525712d33d5ffd818cd8b0c25b1dee0e648d5559516153a
   languageName: node
   linkType: hard
 
-"@babel/generator@npm:^7.20.7, @babel/generator@npm:^7.7.2":
-  version: 7.20.14
-  resolution: "@babel/generator@npm:7.20.14"
+"@babel/generator@npm:^7.21.3, @babel/generator@npm:^7.7.2":
+  version: 7.21.3
+  resolution: "@babel/generator@npm:7.21.3"
   dependencies:
-    "@babel/types": ^7.20.7
+    "@babel/types": ^7.21.3
     "@jridgewell/gen-mapping": ^0.3.2
+    "@jridgewell/trace-mapping": ^0.3.17
     jsesc: ^2.5.1
-  checksum: 5f6aa2d86af26e76d276923a5c34191124a119b16ee9ccc34aef654a7dec84fbd7d2daed2e6458a6a06bf87f3661deb77c9fea59b8f67faff5c90793c96d76d6
+  checksum: be6bb5a32a0273260b91210d4137b7b5da148a2db8dd324654275cb0af865ae59de5e1536e93ac83423b2586415059e1c24cf94293026755cf995757238da749
   languageName: node
   linkType: hard
 
 "@babel/helper-annotate-as-pure@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/helper-annotate-as-pure@npm:7.18.6"
   dependencies:
@@ -95,41 +96,41 @@
     semver: ^6.3.0
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 8c32c873ba86e2e1805b30e0807abd07188acbe00ebb97576f0b09061cc65007f1312b589eccb4349c5a8c7f8bb9f2ab199d41da7030bf103d9f347dcd3a3cf4
   languageName: node
   linkType: hard
 
-"@babel/helper-create-class-features-plugin@npm:^7.18.6, @babel/helper-create-class-features-plugin@npm:^7.20.5, @babel/helper-create-class-features-plugin@npm:^7.20.7":
-  version: 7.20.12
-  resolution: "@babel/helper-create-class-features-plugin@npm:7.20.12"
+"@babel/helper-create-class-features-plugin@npm:^7.18.6, @babel/helper-create-class-features-plugin@npm:^7.21.0":
+  version: 7.21.0
+  resolution: "@babel/helper-create-class-features-plugin@npm:7.21.0"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.18.6
     "@babel/helper-environment-visitor": ^7.18.9
-    "@babel/helper-function-name": ^7.19.0
-    "@babel/helper-member-expression-to-functions": ^7.20.7
+    "@babel/helper-function-name": ^7.21.0
+    "@babel/helper-member-expression-to-functions": ^7.21.0
     "@babel/helper-optimise-call-expression": ^7.18.6
     "@babel/helper-replace-supers": ^7.20.7
     "@babel/helper-skip-transparent-expression-wrappers": ^7.20.0
     "@babel/helper-split-export-declaration": ^7.18.6
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 1e9ed4243b75278fa24deb40dc62bf537b79307987223a2d2d2ae5abf7ba6dc8435d6e3bb55d52ceb30d3e1eba88e7eb6a1885a8bb519e5cfc3e9dedb97d43e6
+  checksum: 3e781d91d1056ea9b3a0395f3017492594a8b86899119b4a1645227c31727b8bec9bc8f6b72e86b1c5cf2dd6690893d2e8c5baff4974c429e616ead089552a21
   languageName: node
   linkType: hard
 
 "@babel/helper-create-regexp-features-plugin@npm:^7.18.6, @babel/helper-create-regexp-features-plugin@npm:^7.20.5":
-  version: 7.20.5
-  resolution: "@babel/helper-create-regexp-features-plugin@npm:7.20.5"
+  version: 7.21.0
+  resolution: "@babel/helper-create-regexp-features-plugin@npm:7.21.0"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.18.6
-    regexpu-core: ^5.2.1
+    regexpu-core: ^5.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 7f29c3cb7447cca047b0d394f8ab98e4923d00e86a7afa56e5df9770c48ec107891505d2d1f06b720ecc94ed24bf58d90986cc35fe4a43b549eb7b7a5077b693
+  checksum: 63a6396a4e9444edc7e97617845583ea5cf059573d0b4cc566869f38576d543e37fde0edfcc21d6dfb7962ed241e909561714dc41c5213198bac04e0983b04f2
   languageName: node
   linkType: hard
 
 "@babel/helper-define-polyfill-provider@npm:^0.3.3":
   version: 0.3.3
   resolution: "@babel/helper-define-polyfill-provider@npm:0.3.3"
   dependencies:
@@ -157,64 +158,64 @@
   resolution: "@babel/helper-explode-assignable-expression@npm:7.18.6"
   dependencies:
     "@babel/types": ^7.18.6
   checksum: 225cfcc3376a8799023d15dc95000609e9d4e7547b29528c7f7111a0e05493ffb12c15d70d379a0bb32d42752f340233c4115bded6d299bc0c3ab7a12be3d30f
   languageName: node
   linkType: hard
 
-"@babel/helper-function-name@npm:^7.18.9, @babel/helper-function-name@npm:^7.19.0":
-  version: 7.19.0
-  resolution: "@babel/helper-function-name@npm:7.19.0"
+"@babel/helper-function-name@npm:^7.18.9, @babel/helper-function-name@npm:^7.19.0, @babel/helper-function-name@npm:^7.21.0":
+  version: 7.21.0
+  resolution: "@babel/helper-function-name@npm:7.21.0"
   dependencies:
-    "@babel/template": ^7.18.10
-    "@babel/types": ^7.19.0
-  checksum: eac1f5db428ba546270c2b8d750c24eb528b8fcfe50c81de2e0bdebf0e20f24bec688d4331533b782e4a907fad435244621ca2193cfcf80a86731299840e0f6e
+    "@babel/template": ^7.20.7
+    "@babel/types": ^7.21.0
+  checksum: d63e63c3e0e3e8b3138fa47b0cd321148a300ef12b8ee951196994dcd2a492cc708aeda94c2c53759a5c9177fffaac0fd8778791286746f72a000976968daf4e
   languageName: node
   linkType: hard
 
 "@babel/helper-hoist-variables@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/helper-hoist-variables@npm:7.18.6"
   dependencies:
     "@babel/types": ^7.18.6
   checksum: fd9c35bb435fda802bf9ff7b6f2df06308a21277c6dec2120a35b09f9de68f68a33972e2c15505c1a1a04b36ec64c9ace97d4a9e26d6097b76b4396b7c5fa20f
   languageName: node
   linkType: hard
 
-"@babel/helper-member-expression-to-functions@npm:^7.20.7":
-  version: 7.20.7
-  resolution: "@babel/helper-member-expression-to-functions@npm:7.20.7"
+"@babel/helper-member-expression-to-functions@npm:^7.20.7, @babel/helper-member-expression-to-functions@npm:^7.21.0":
+  version: 7.21.0
+  resolution: "@babel/helper-member-expression-to-functions@npm:7.21.0"
   dependencies:
-    "@babel/types": ^7.20.7
-  checksum: cec17aab7e964830b0146e575bd141127032319f26ed864a65b35abd75ad618d264d3e11449b9b4e29cfd95bb1a7e774afddd4884fdcc29c36ac9cbd2b66359f
+    "@babel/types": ^7.21.0
+  checksum: 49cbb865098195fe82ba22da3a8fe630cde30dcd8ebf8ad5f9a24a2b685150c6711419879cf9d99b94dad24cff9244d8c2a890d3d7ec75502cd01fe58cff5b5d
   languageName: node
   linkType: hard
 
 "@babel/helper-module-imports@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/helper-module-imports@npm:7.18.6"
   dependencies:
     "@babel/types": ^7.18.6
   checksum: f393f8a3b3304b1b7a288a38c10989de754f01d29caf62ce7c4e5835daf0a27b81f3ac687d9d2780d39685aae7b55267324b512150e7b2be967b0c493b6a1def
   languageName: node
   linkType: hard
 
-"@babel/helper-module-transforms@npm:^7.18.6, @babel/helper-module-transforms@npm:^7.20.11":
-  version: 7.20.11
-  resolution: "@babel/helper-module-transforms@npm:7.20.11"
+"@babel/helper-module-transforms@npm:^7.18.6, @babel/helper-module-transforms@npm:^7.20.11, @babel/helper-module-transforms@npm:^7.21.2":
+  version: 7.21.2
+  resolution: "@babel/helper-module-transforms@npm:7.21.2"
   dependencies:
     "@babel/helper-environment-visitor": ^7.18.9
     "@babel/helper-module-imports": ^7.18.6
     "@babel/helper-simple-access": ^7.20.2
     "@babel/helper-split-export-declaration": ^7.18.6
     "@babel/helper-validator-identifier": ^7.19.1
     "@babel/template": ^7.20.7
-    "@babel/traverse": ^7.20.10
-    "@babel/types": ^7.20.7
-  checksum: 29319ebafa693d48756c6ba0d871677bb0037e0da084fbe221a17c38d57093fc8aa38543c07d76e788266a937976e37ab4901971ca7f237c5ab45f524b9ecca0
+    "@babel/traverse": ^7.21.2
+    "@babel/types": ^7.21.2
+  checksum: 8a1c129a4f90bdf97d8b6e7861732c9580f48f877aaaafbc376ce2482febebcb8daaa1de8bc91676d12886487603f8c62a44f9e90ee76d6cac7f9225b26a49e1
   languageName: node
   linkType: hard
 
 "@babel/helper-optimise-call-expression@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/helper-optimise-call-expression@npm:7.18.6"
   dependencies:
@@ -296,17 +297,17 @@
   version: 7.19.1
   resolution: "@babel/helper-validator-identifier@npm:7.19.1"
   checksum: 0eca5e86a729162af569b46c6c41a63e18b43dbe09fda1d2a3c8924f7d617116af39cac5e4cd5d431bb760b4dca3c0970e0c444789b1db42bcf1fa41fbad0a3a
   languageName: node
   linkType: hard
 
 "@babel/helper-validator-option@npm:^7.18.6":
-  version: 7.18.6
-  resolution: "@babel/helper-validator-option@npm:7.18.6"
-  checksum: f9cc6eb7cc5d759c5abf006402180f8d5e4251e9198197428a97e05d65eb2f8ae5a0ce73b1dfd2d35af41d0eb780627a64edf98a4e71f064eeeacef8de58f2cf
+  version: 7.21.0
+  resolution: "@babel/helper-validator-option@npm:7.21.0"
+  checksum: 8ece4c78ffa5461fd8ab6b6e57cc51afad59df08192ed5d84b475af4a7193fc1cb794b59e3e7be64f3cdc4df7ac78bf3dbb20c129d7757ae078e6279ff8c2f07
   languageName: node
   linkType: hard
 
 "@babel/helper-wrap-function@npm:^7.18.9":
   version: 7.20.5
   resolution: "@babel/helper-wrap-function@npm:7.20.5"
   dependencies:
@@ -314,42 +315,42 @@
     "@babel/template": ^7.18.10
     "@babel/traverse": ^7.20.5
     "@babel/types": ^7.20.5
   checksum: 11a6fc28334368a193a9cb3ad16f29cd7603bab958433efc82ebe59fa6556c227faa24f07ce43983f7a85df826f71d441638442c4315e90a554fe0a70ca5005b
   languageName: node
   linkType: hard
 
-"@babel/helpers@npm:^7.20.7":
-  version: 7.20.13
-  resolution: "@babel/helpers@npm:7.20.13"
+"@babel/helpers@npm:^7.21.0":
+  version: 7.21.0
+  resolution: "@babel/helpers@npm:7.21.0"
   dependencies:
     "@babel/template": ^7.20.7
-    "@babel/traverse": ^7.20.13
-    "@babel/types": ^7.20.7
-  checksum: d62076fa834f342798f8c3fd7aec0870cc1725d273d99e540cbaa8d6c3ed10258228dd14601c8e66bfeabbb9424c3b31090ecc467fe855f7bd72c4734df7fb09
+    "@babel/traverse": ^7.21.0
+    "@babel/types": ^7.21.0
+  checksum: 9370dad2bb665c551869a08ac87c8bdafad53dbcdce1f5c5d498f51811456a3c005d9857562715151a0f00b2e912ac8d89f56574f837b5689f5f5072221cdf54
   languageName: node
   linkType: hard
 
 "@babel/highlight@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/highlight@npm:7.18.6"
   dependencies:
     "@babel/helper-validator-identifier": ^7.18.6
     chalk: ^2.0.0
     js-tokens: ^4.0.0
   checksum: 92d8ee61549de5ff5120e945e774728e5ccd57fd3b2ed6eace020ec744823d4a98e242be1453d21764a30a14769ecd62170fba28539b211799bbaf232bbb2789
   languageName: node
   linkType: hard
 
-"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.13, @babel/parser@npm:^7.20.7":
-  version: 7.20.15
-  resolution: "@babel/parser@npm:7.20.15"
+"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.21.3":
+  version: 7.21.3
+  resolution: "@babel/parser@npm:7.21.3"
   bin:
     parser: ./bin/babel-parser.js
-  checksum: 1d0f47ca67ff2652f1c0ff1570bed8deccbc4b53509e7cd73476af9cc7ed23480c99f1179bd6d0be01612368b92b39e206d330ad6054009d699934848a89298b
+  checksum: a71e6456a1260c2a943736b56cc0acdf5f2a53c6c79e545f56618967e51f9b710d1d3359264e7c979313a7153741b1d95ad8860834cc2ab4ce4f428b13cc07be
   languageName: node
   linkType: hard
 
 "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.18.6"
   dependencies:
@@ -396,23 +397,23 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 49a78a2773ec0db56e915d9797e44fd079ab8a9b2e1716e0df07c92532f2c65d76aeda9543883916b8e0ff13606afeffa67c5b93d05b607bc87653ad18a91422
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-class-static-block@npm:^7.18.6":
-  version: 7.20.7
-  resolution: "@babel/plugin-proposal-class-static-block@npm:7.20.7"
+  version: 7.21.0
+  resolution: "@babel/plugin-proposal-class-static-block@npm:7.21.0"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.20.7
+    "@babel/helper-create-class-features-plugin": ^7.21.0
     "@babel/helper-plugin-utils": ^7.20.2
     "@babel/plugin-syntax-class-static-block": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.12.0
-  checksum: ce1f3e8fd96437d820aa36323b7b3a0cb65b5f2600612665129880d5a4eb7194ce6a298ed2a5a4d3a9ea49bd33089ab95503c4c5b3ba9cea251a07d1706453d9
+  checksum: 236c0ad089e7a7acab776cc1d355330193314bfcd62e94e78f2df35817c6144d7e0e0368976778afd6b7c13e70b5068fa84d7abbf967d4f182e60d03f9ef802b
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-dynamic-import@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/plugin-proposal-dynamic-import@npm:7.18.6"
   dependencies:
@@ -508,23 +509,23 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 7b5b39fb5d8d6d14faad6cb68ece5eeb2fd550fb66b5af7d7582402f974f5bc3684641f7c192a5a57e0f59acfae4aada6786be1eba030881ddc590666eff4d1e
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-optional-chaining@npm:^7.18.9, @babel/plugin-proposal-optional-chaining@npm:^7.20.7":
-  version: 7.20.7
-  resolution: "@babel/plugin-proposal-optional-chaining@npm:7.20.7"
+  version: 7.21.0
+  resolution: "@babel/plugin-proposal-optional-chaining@npm:7.21.0"
   dependencies:
     "@babel/helper-plugin-utils": ^7.20.2
     "@babel/helper-skip-transparent-expression-wrappers": ^7.20.0
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 274b8932335bd064ca24cf1a4da2b2c20c92726d4bfa8b0cb5023857479b8481feef33505c16650c7b9239334e5c6959babc924816324c4cf223dd91c7ca79bc
+  checksum: 11c5449e01b18bb8881e8e005a577fa7be2fe5688e2382c8822d51f8f7005342a301a46af7b273b1f5645f9a7b894c428eee8526342038a275ef6ba4c8d8d746
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-private-methods@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/plugin-proposal-private-methods@npm:7.18.6"
   dependencies:
@@ -533,24 +534,24 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 22d8502ee96bca99ad2c8393e8493e2b8d4507576dd054490fd8201a36824373440106f5b098b6d821b026c7e72b0424ff4aeca69ed5f42e48f029d3a156d5ad
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-private-property-in-object@npm:^7.18.6":
-  version: 7.20.5
-  resolution: "@babel/plugin-proposal-private-property-in-object@npm:7.20.5"
+  version: 7.21.0
+  resolution: "@babel/plugin-proposal-private-property-in-object@npm:7.21.0"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.18.6
-    "@babel/helper-create-class-features-plugin": ^7.20.5
+    "@babel/helper-create-class-features-plugin": ^7.21.0
     "@babel/helper-plugin-utils": ^7.20.2
     "@babel/plugin-syntax-private-property-in-object": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 513b5e0e2c1b2846be5336cf680e932ae17924ef885aa1429e1a4f7924724bdd99b15f28d67187d0a006d5f18a0c4b61d96c3ecb4902fed3c8fe2f0abfc9753a
+  checksum: add881a6a836635c41d2710551fdf777e2c07c0b691bf2baacc5d658dd64107479df1038680d6e67c468bfc6f36fb8920025d6bac2a1df0a81b867537d40ae78
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-unicode-property-regex@npm:^7.18.6, @babel/plugin-proposal-unicode-property-regex@npm:^7.4.4":
   version: 7.18.6
   resolution: "@babel/plugin-proposal-unicode-property-regex@npm:7.18.6"
   dependencies:
@@ -803,40 +804,40 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 0a0df61f94601e3666bf39f2cc26f5f7b22a94450fb93081edbed967bd752ce3f81d1227fefd3799f5ee2722171b5e28db61379234d1bb85b6ec689589f99d7e
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-block-scoping@npm:^7.20.2":
-  version: 7.20.15
-  resolution: "@babel/plugin-transform-block-scoping@npm:7.20.15"
+  version: 7.21.0
+  resolution: "@babel/plugin-transform-block-scoping@npm:7.21.0"
   dependencies:
     "@babel/helper-plugin-utils": ^7.20.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 1dddf7be578306837074cb5059f8408af0b1c0bfcf922ed920d4aa65d08fb7c6e6129ca254e9879c4c6d2a6be4937111551f51922e8b0e071ed16eb6564a4dbb
+  checksum: 15aacaadbecf96b53a750db1be4990b0d89c7f5bc3e1794b63b49fb219638c1fd25d452d15566d7e5ddf5b5f4e1a0a0055c35c1c7aee323c7b114bf49f66f4b0
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-classes@npm:^7.20.2":
-  version: 7.20.7
-  resolution: "@babel/plugin-transform-classes@npm:7.20.7"
+  version: 7.21.0
+  resolution: "@babel/plugin-transform-classes@npm:7.21.0"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.18.6
     "@babel/helper-compilation-targets": ^7.20.7
     "@babel/helper-environment-visitor": ^7.18.9
-    "@babel/helper-function-name": ^7.19.0
+    "@babel/helper-function-name": ^7.21.0
     "@babel/helper-optimise-call-expression": ^7.18.6
     "@babel/helper-plugin-utils": ^7.20.2
     "@babel/helper-replace-supers": ^7.20.7
     "@babel/helper-split-export-declaration": ^7.18.6
     globals: ^11.1.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 4cf55ad88e52c7c66a991add4c8e1c3324384bd52df7085962d396879561456a44352e5ab1725cc80f4e83737a2931e847c4a96c7aa4a549357f23631ff31799
+  checksum: 088ae152074bd0e90f64659169255bfe50393e637ec8765cb2a518848b11b0299e66b91003728fd0a41563a6fdc6b8d548ece698a314fd5447f5489c22e466b7
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-computed-properties@npm:^7.18.9":
   version: 7.20.7
   resolution: "@babel/plugin-transform-computed-properties@npm:7.20.7"
   dependencies:
@@ -845,21 +846,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: be70e54bda8b469146459f429e5f2bd415023b87b2d5af8b10e48f465ffb02847a3ed162ca60378c004b82db848e4d62e90010d41ded7e7176b6d8d1c2911139
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-destructuring@npm:^7.20.2":
-  version: 7.20.7
-  resolution: "@babel/plugin-transform-destructuring@npm:7.20.7"
+  version: 7.21.3
+  resolution: "@babel/plugin-transform-destructuring@npm:7.21.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.20.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: bd8affdb142c77662037215e37128b2110a786c92a67e1f00b38223c438c1610bd84cbc0386e9cd3479245ea811c5ca6c9838f49be4729b592159a30ce79add2
+  checksum: 43ebbe0bfa20287e34427be7c2200ce096c20913775ea75268fb47fe0e55f9510800587e6052c42fe6dffa0daaad95dd465c3e312fd1ef9785648384c45417ac
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-dotall-regex@npm:^7.18.6, @babel/plugin-transform-dotall-regex@npm:^7.4.4":
   version: 7.18.6
   resolution: "@babel/plugin-transform-dotall-regex@npm:7.18.6"
   dependencies:
@@ -891,21 +892,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 7f70222f6829c82a36005508d34ddbe6fd0974ae190683a8670dd6ff08669aaf51fef2209d7403f9bd543cb2d12b18458016c99a6ed0332ccedb3ea127b01229
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-for-of@npm:^7.18.8":
-  version: 7.18.8
-  resolution: "@babel/plugin-transform-for-of@npm:7.18.8"
+  version: 7.21.0
+  resolution: "@babel/plugin-transform-for-of@npm:7.21.0"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.18.6
+    "@babel/helper-plugin-utils": ^7.20.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: ca64c623cf0c7a80ab6f07ebd3e6e4ade95e2ae806696f70b43eafe6394fa8ce21f2b1ffdd15df2067f7363d2ecfe26472a97c6c774403d2163fa05f50c98f17
+  checksum: 2f3f86ca1fab2929fcda6a87e4303d5c635b5f96dc9a45fd4ca083308a3020c79ac33b9543eb4640ef2b79f3586a00ab2d002a7081adb9e9d7440dce30781034
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-function-name@npm:^7.18.9":
   version: 7.18.9
   resolution: "@babel/plugin-transform-function-name@npm:7.18.9"
   dependencies:
@@ -949,23 +950,23 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 23665c1c20c8f11c89382b588fb9651c0756d130737a7625baeaadbd3b973bc5bfba1303bedffa8fb99db1e6d848afb01016e1df2b69b18303e946890c790001
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-modules-commonjs@npm:^7.19.6":
-  version: 7.20.11
-  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.20.11"
+  version: 7.21.2
+  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.21.2"
   dependencies:
-    "@babel/helper-module-transforms": ^7.20.11
+    "@babel/helper-module-transforms": ^7.21.2
     "@babel/helper-plugin-utils": ^7.20.2
     "@babel/helper-simple-access": ^7.20.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: ddd0623e2ad4b5c0faaa0ae30d3407a3fa484d911c968ed33cfb1b339ac3691321c959db60b66dc136dbd67770fff586f7e48a7ce0d7d357f92d6ef6fb7ed1a7
+  checksum: 65aa06e3e3792f39b99eb5f807034693ff0ecf80438580f7ae504f4c4448ef04147b1889ea5e6f60f3ad4a12ebbb57c6f1f979a249dadbd8d11fe22f4441918b
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-modules-systemjs@npm:^7.19.6":
   version: 7.20.11
   resolution: "@babel/plugin-transform-modules-systemjs@npm:7.20.11"
   dependencies:
@@ -1023,21 +1024,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 0fcb04e15deea96ae047c21cb403607d49f06b23b4589055993365ebd7a7d7541334f06bf9642e90075e66efce6ebaf1eb0ef066fbbab802d21d714f1aac3aef
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-parameters@npm:^7.20.1, @babel/plugin-transform-parameters@npm:^7.20.7":
-  version: 7.20.7
-  resolution: "@babel/plugin-transform-parameters@npm:7.20.7"
+  version: 7.21.3
+  resolution: "@babel/plugin-transform-parameters@npm:7.21.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.20.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 6ffe0dd9afb2d2b9bc247381aa2e95dd9997ff5568a0a11900528919a4e073ac68f46409431455badb8809644d47cff180045bc2b9700e3f36e3b23554978947
+  checksum: c92128d7b1fcf54e2cab186c196bbbf55a9a6de11a83328dc2602649c9dc6d16ef73712beecd776cd49bfdc624b5f56740f4a53568d3deb9505ec666bc869da3
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-property-literals@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/plugin-transform-property-literals@npm:7.18.6"
   dependencies:
@@ -1254,63 +1255,52 @@
   version: 0.8.0
   resolution: "@babel/regjsgen@npm:0.8.0"
   checksum: 89c338fee774770e5a487382170711014d49a68eb281e74f2b5eac88f38300a4ad545516a7786a8dd5702e9cf009c94c2f582d200f077ac5decd74c56b973730
   languageName: node
   linkType: hard
 
 "@babel/runtime@npm:^7.8.4":
-  version: 7.20.13
-  resolution: "@babel/runtime@npm:7.20.13"
+  version: 7.21.0
+  resolution: "@babel/runtime@npm:7.21.0"
   dependencies:
     regenerator-runtime: ^0.13.11
-  checksum: 09b7a97a05c80540db6c9e4ddf8c5d2ebb06cae5caf3a87e33c33f27f8c4d49d9c67a2d72f1570e796045288fad569f98a26ceba0c4f5fad2af84b6ad855c4fb
+  checksum: 7b33e25bfa9e0e1b9e8828bb61b2d32bdd46b41b07ba7cb43319ad08efc6fda8eb89445193e67d6541814627df0ca59122c0ea795e412b99c5183a0540d338ab
   languageName: node
   linkType: hard
 
 "@babel/template@npm:^7.18.10, @babel/template@npm:^7.20.7, @babel/template@npm:^7.3.3":
   version: 7.20.7
   resolution: "@babel/template@npm:7.20.7"
   dependencies:
     "@babel/code-frame": ^7.18.6
     "@babel/parser": ^7.20.7
     "@babel/types": ^7.20.7
   checksum: 2eb1a0ab8d415078776bceb3473d07ab746e6bb4c2f6ca46ee70efb284d75c4a32bb0cd6f4f4946dec9711f9c0780e8e5d64b743208deac6f8e9858afadc349e
   languageName: node
   linkType: hard
 
-"@babel/traverse@npm:^7.20.10, @babel/traverse@npm:^7.20.12, @babel/traverse@npm:^7.20.13, @babel/traverse@npm:^7.20.5, @babel/traverse@npm:^7.20.7, @babel/traverse@npm:^7.7.2":
-  version: 7.20.13
-  resolution: "@babel/traverse@npm:7.20.13"
+"@babel/traverse@npm:^7.20.5, @babel/traverse@npm:^7.20.7, @babel/traverse@npm:^7.21.0, @babel/traverse@npm:^7.21.2, @babel/traverse@npm:^7.21.3, @babel/traverse@npm:^7.7.2":
+  version: 7.21.3
+  resolution: "@babel/traverse@npm:7.21.3"
   dependencies:
     "@babel/code-frame": ^7.18.6
-    "@babel/generator": ^7.20.7
+    "@babel/generator": ^7.21.3
     "@babel/helper-environment-visitor": ^7.18.9
-    "@babel/helper-function-name": ^7.19.0
+    "@babel/helper-function-name": ^7.21.0
     "@babel/helper-hoist-variables": ^7.18.6
     "@babel/helper-split-export-declaration": ^7.18.6
-    "@babel/parser": ^7.20.13
-    "@babel/types": ^7.20.7
+    "@babel/parser": ^7.21.3
+    "@babel/types": ^7.21.3
     debug: ^4.1.0
     globals: ^11.1.0
-  checksum: 30ca6e0bd18233fda48fa09315efd14dfc61dcf5b8fa3712b343bfc61b32bc63b5e85ea1773cc9576c9b293b96f46b4589aaeb0a52e1f3eeac4edc076d049fc7
+  checksum: 0af5bcd47a2fc501592b90ac1feae9d449afb9ab0772a4f6e68230f4cd3a475795d538c1de3f880fe3414b6c2820bac84d02c6549eea796f39d74a603717447b
   languageName: node
   linkType: hard
 
-"@babel/types@npm:^7.0.0, @babel/types@npm:^7.18.6, @babel/types@npm:^7.18.9, @babel/types@npm:^7.19.0, @babel/types@npm:^7.20.0, @babel/types@npm:^7.20.2, @babel/types@npm:^7.20.5, @babel/types@npm:^7.20.7, @babel/types@npm:^7.3.0, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4":
-  version: 7.20.7
-  resolution: "@babel/types@npm:7.20.7"
-  dependencies:
-    "@babel/helper-string-parser": ^7.19.4
-    "@babel/helper-validator-identifier": ^7.19.1
-    to-fast-properties: ^2.0.0
-  checksum: b39af241f0b72bba67fd6d0d23914f6faec8c0eba8015c181cbd5ea92e59fc91a52a1ab490d3520c7dbd19ddb9ebb76c476308f6388764f16d8201e37fae6811
-  languageName: node
-  linkType: hard
-
-"@babel/types@npm:^7.8.3":
+"@babel/types@npm:^7.0.0, @babel/types@npm:^7.18.6, @babel/types@npm:^7.18.9, @babel/types@npm:^7.20.0, @babel/types@npm:^7.20.2, @babel/types@npm:^7.20.5, @babel/types@npm:^7.20.7, @babel/types@npm:^7.21.0, @babel/types@npm:^7.21.2, @babel/types@npm:^7.21.3, @babel/types@npm:^7.3.0, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
   version: 7.21.3
   resolution: "@babel/types@npm:7.21.3"
   dependencies:
     "@babel/helper-string-parser": ^7.19.4
     "@babel/helper-validator-identifier": ^7.19.1
     to-fast-properties: ^2.0.0
   checksum: b750274718ba9cefd0b81836c464009bb6ba339fccce51b9baff497a0a2d96c044c61dc90cf203cec0adc770454b53a9681c3f7716883c802b85ab84c365ba35
@@ -1372,27 +1362,27 @@
     "@codemirror/state": ^6.0.0
     "@lezer/css": ^1.0.0
   checksum: 9b0bf7c7544fb604b67325689d783981e4099560f577bc1f10c52cb18e9d275ebdbdbd3f335a1dbb9c4910c36320f74ca015fc92ef99f930ecb9d481a2bf3511
   languageName: node
   linkType: hard
 
 "@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.0":
-  version: 6.4.2
-  resolution: "@codemirror/lang-html@npm:6.4.2"
+  version: 6.4.3
+  resolution: "@codemirror/lang-html@npm:6.4.3"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/lang-css": ^6.0.0
     "@codemirror/lang-javascript": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.2.2
     "@lezer/common": ^1.0.0
     "@lezer/css": ^1.1.0
     "@lezer/html": ^1.3.0
-  checksum: 10eebf44f275867c9916639f55610214c305d27a8a8545c3fa2d9495cbac33eb9f8751fc6b78e83d957c49a4b446bbee959bdf3eb497e88a05796aca02ed773b
+  checksum: 6177d19147580964ecd6910ae951201929a96e63f4f0e624c3138e2805fa87ec6d6d952a3a888c5a52af78b6dd6d04d7d8c76c6a9cd65b1921dc467b5dbaea72
   languageName: node
   linkType: hard
 
 "@codemirror/lang-java@npm:^6.0.0":
   version: 6.0.1
   resolution: "@codemirror/lang-java@npm:6.0.1"
   dependencies:
@@ -1572,88 +1562,87 @@
     style-mod: ^4.0.0
     w3c-keyname: ^2.2.4
   checksum: 718ecbb021ca75eb89003f73c846a07d36a708dcfec8345f0f0dbcfc0d0df5ea6f114918694b2730a6d49e5e50502bcce79ce7ff94ce55748e068e5a35073755
   languageName: node
   linkType: hard
 
 "@csstools/css-parser-algorithms@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@csstools/css-parser-algorithms@npm:2.0.1"
+  version: 2.1.0
+  resolution: "@csstools/css-parser-algorithms@npm:2.1.0"
   peerDependencies:
     "@csstools/css-tokenizer": ^2.0.0
-  checksum: 9f168cfc8fa30ba19fcbe7632d947b74beea494db60cf0eb250f7b77fe72239fb5e6d292b035144dbc52977fb4768f157064f8358530701fe56e5ef2993174c7
+  checksum: 197c8b0db9e721974d3850a44c73a7c1c0ebdddf981ddbc5f0a56d60c09c332bcd9f63ae391811ba3b11b9939faa50ada15c5cc38490861ba48f8933b599f660
   languageName: node
   linkType: hard
 
-"@csstools/css-tokenizer@npm:^2.0.1":
-  version: 2.0.2
-  resolution: "@csstools/css-tokenizer@npm:2.0.2"
-  checksum: 49bd0a191954b56e9fa50d4a3e2d04059196f04efe398c0cb3c2cbcc18549313d984cd0b8c3faa161d81768256014461d1b4d0f40a67764c9c7a6c0e14a97fea
+"@csstools/css-tokenizer@npm:^2.1.0":
+  version: 2.1.0
+  resolution: "@csstools/css-tokenizer@npm:2.1.0"
+  checksum: af3619557e18cd348810cfb41b3b7177b36d216df8dd4cac3979f241c15416baf8cdd55fb764ecc78fab5985b085363cfc8e8b8a18aaa361d00c9b9300b7c0f3
   languageName: node
   linkType: hard
 
 "@csstools/media-query-list-parser@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@csstools/media-query-list-parser@npm:2.0.1"
+  version: 2.0.2
+  resolution: "@csstools/media-query-list-parser@npm:2.0.2"
   peerDependencies:
     "@csstools/css-parser-algorithms": ^2.0.0
     "@csstools/css-tokenizer": ^2.0.0
-  checksum: f30b2a9e1aa3c2d8e98d3ac79463ab514ba4c4577c4cc6120a69d9f4562e521766adb62fc44ffee2226a967bdcfcf86a46bdaf625d21af8f21caa99553994d60
+  checksum: 44bf464a8e79d062549353f276ac6100db600558b006b9407bc179d46b2070b855da5ca8617b964005ab03a7a9c3432a0493d0e4fd6f2b5249244a5c15f420ff
   languageName: node
   linkType: hard
 
 "@csstools/selector-specificity@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@csstools/selector-specificity@npm:2.1.1"
+  version: 2.2.0
+  resolution: "@csstools/selector-specificity@npm:2.2.0"
   peerDependencies:
-    postcss: ^8.4
     postcss-selector-parser: ^6.0.10
-  checksum: 392ab62732e93aa8cbea445bf3485c1acbbecc8ec087b200e06c9ddd2acf740fd1fe46abdacf813e7a50a95a60346377ee3eecb4e1fe3709582e2851430b376a
+  checksum: 97c89f23b3b527d7bd51ed299969ed2b9fbb219a367948b44aefec228b8eda6ae0ad74fe8a82f9aac8ff32cfd00bb6d0c98d1daeab2e8fc6d5c4af25e5be5673
   languageName: node
   linkType: hard
 
 "@discoveryjs/json-ext@npm:^0.5.0":
   version: 0.5.7
   resolution: "@discoveryjs/json-ext@npm:0.5.7"
   checksum: 2176d301cc258ea5c2324402997cf8134ebb212469c0d397591636cea8d3c02f2b3cf9fd58dcb748c7a0dade77ebdc1b10284fa63e608c033a1db52fddc69918
   languageName: node
   linkType: hard
 
 "@eslint-community/eslint-utils@npm:^4.2.0":
-  version: 4.3.0
-  resolution: "@eslint-community/eslint-utils@npm:4.3.0"
+  version: 4.4.0
+  resolution: "@eslint-community/eslint-utils@npm:4.4.0"
   dependencies:
     eslint-visitor-keys: ^3.3.0
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
-  checksum: f487760a692f0f1fef76e248ad72976919576ba57edc2b1b1dc1d182553bae6b5bf7b078e654da85d04f0af8a485d20bd26280002768f4fbcd2e330078340cb0
+  checksum: cdfe3ae42b4f572cbfb46d20edafe6f36fc5fb52bf2d90875c58aefe226892b9677fef60820e2832caf864a326fe4fc225714c46e8389ccca04d5f9288aabd22
   languageName: node
   linkType: hard
 
 "@eslint-community/regexpp@npm:^4.4.0":
-  version: 4.4.0
-  resolution: "@eslint-community/regexpp@npm:4.4.0"
-  checksum: 2d127af0c752b80e8a782eacfe996a86925d21de92da3ffc6f9e615e701145e44a62e26bdd88bfac2cd76779c39ba8d9875a91046ec5e7e5f23cb647c247ea6a
+  version: 4.5.0
+  resolution: "@eslint-community/regexpp@npm:4.5.0"
+  checksum: 99c01335947dbd7f2129e954413067e217ccaa4e219fe0917b7d2bd96135789384b8fedbfb8eb09584d5130b27a7b876a7150ab7376f51b3a0c377d5ce026a10
   languageName: node
   linkType: hard
 
 "@eslint/eslintrc@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@eslint/eslintrc@npm:2.0.1"
+  version: 2.0.2
+  resolution: "@eslint/eslintrc@npm:2.0.2"
   dependencies:
     ajv: ^6.12.4
     debug: ^4.3.2
-    espree: ^9.5.0
+    espree: ^9.5.1
     globals: ^13.19.0
     ignore: ^5.2.0
     import-fresh: ^3.2.1
     js-yaml: ^4.1.0
     minimatch: ^3.1.2
     strip-json-comments: ^3.1.1
-  checksum: 56b9192a687a450db53a7b883daf9f0f447c43b3510189cf88808a7a2467c2a302a42a50f184cc6d5a9faf3d1df890a2ef0fd0d60b751f32a3e9dfea717c6b48
+  checksum: cfcf5e12c7b2c4476482e7f12434e76eae16fcd163ee627309adb10b761e5caa4a4e52ed7be464423320ff3d11eca5b50de5bf8be3e25834222470835dd5c801
   languageName: node
   linkType: hard
 
 "@eslint/js@npm:8.36.0":
   version: 8.36.0
   resolution: "@eslint/js@npm:8.36.0"
   checksum: b7d6b84b823c8c7784be390741196617565527b1f7c0977fde9455bfb57fd88f81c074a03dd878757d2c33fa29f24291e9ecbc1425710f067917324b55e1bf3a
@@ -1729,160 +1718,160 @@
 "@istanbuljs/schema@npm:^0.1.2":
   version: 0.1.3
   resolution: "@istanbuljs/schema@npm:0.1.3"
   checksum: 5282759d961d61350f33d9118d16bcaed914ebf8061a52f4fa474b2cb08720c9c81d165e13b82f2e5a8a212cc5af482f0c6fc1ac27b9e067e5394c9a6ed186c9
   languageName: node
   linkType: hard
 
-"@jest/console@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/console@npm:29.4.3"
+"@jest/console@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/console@npm:29.5.0"
   dependencies:
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     "@types/node": "*"
     chalk: ^4.0.0
-    jest-message-util: ^29.4.3
-    jest-util: ^29.4.3
+    jest-message-util: ^29.5.0
+    jest-util: ^29.5.0
     slash: ^3.0.0
-  checksum: 8d9b163febe735153b523db527742309f4d598eda22f17f04e030060329bd3da4de7420fc1f7812f7a16f08273654a7de094c4b4e8b81a99dbfc17cfb1629008
+  checksum: 9f4f4b8fabd1221361b7f2e92d4a90f5f8c2e2b29077249996ab3c8b7f765175ffee795368f8d6b5b2bb3adb32dc09319f7270c7c787b0d259e624e00e0f64a5
   languageName: node
   linkType: hard
 
-"@jest/core@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/core@npm:29.4.3"
+"@jest/core@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/core@npm:29.5.0"
   dependencies:
-    "@jest/console": ^29.4.3
-    "@jest/reporters": ^29.4.3
-    "@jest/test-result": ^29.4.3
-    "@jest/transform": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/console": ^29.5.0
+    "@jest/reporters": ^29.5.0
+    "@jest/test-result": ^29.5.0
+    "@jest/transform": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/node": "*"
     ansi-escapes: ^4.2.1
     chalk: ^4.0.0
     ci-info: ^3.2.0
     exit: ^0.1.2
     graceful-fs: ^4.2.9
-    jest-changed-files: ^29.4.3
-    jest-config: ^29.4.3
-    jest-haste-map: ^29.4.3
-    jest-message-util: ^29.4.3
+    jest-changed-files: ^29.5.0
+    jest-config: ^29.5.0
+    jest-haste-map: ^29.5.0
+    jest-message-util: ^29.5.0
     jest-regex-util: ^29.4.3
-    jest-resolve: ^29.4.3
-    jest-resolve-dependencies: ^29.4.3
-    jest-runner: ^29.4.3
-    jest-runtime: ^29.4.3
-    jest-snapshot: ^29.4.3
-    jest-util: ^29.4.3
-    jest-validate: ^29.4.3
-    jest-watcher: ^29.4.3
+    jest-resolve: ^29.5.0
+    jest-resolve-dependencies: ^29.5.0
+    jest-runner: ^29.5.0
+    jest-runtime: ^29.5.0
+    jest-snapshot: ^29.5.0
+    jest-util: ^29.5.0
+    jest-validate: ^29.5.0
+    jest-watcher: ^29.5.0
     micromatch: ^4.0.4
-    pretty-format: ^29.4.3
+    pretty-format: ^29.5.0
     slash: ^3.0.0
     strip-ansi: ^6.0.0
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
-  checksum: 4aa10644d66f44f051d5dd9cdcedce27acc71216dbcc5e7adebdea458e27aefe27c78f457d7efd49f58b968c35f42de5a521590876e2013593e675120b9e6ab1
+  checksum: 9e8f5243fe82d5a57f3971e1b96f320058df7c315328a3a827263f3b17f64be10c80f4a9c1b1773628b64d2de6d607c70b5b2d5bf13e7f5ad04223e9ef6aac06
   languageName: node
   linkType: hard
 
-"@jest/environment@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/environment@npm:29.4.3"
+"@jest/environment@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/environment@npm:29.5.0"
   dependencies:
-    "@jest/fake-timers": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/fake-timers": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/node": "*"
-    jest-mock: ^29.4.3
-  checksum: 7c1b0cc4e84b90f8a3bbeca9bbf088882c88aee70a81b3b8e24265dcb1cbc302cd1eee3319089cf65bfd39adbaea344903c712afea106cb8da6c86088d99c5fb
+    jest-mock: ^29.5.0
+  checksum: 921de6325cd4817dec6685e5ff299b499b6379f3f9cf489b4b13588ee1f3820a0c77b49e6a087996b6de8f629f6f5251e636cba08d1bdb97d8071cc7d033c88a
   languageName: node
   linkType: hard
 
-"@jest/expect-utils@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/expect-utils@npm:29.4.3"
+"@jest/expect-utils@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/expect-utils@npm:29.5.0"
   dependencies:
     jest-get-type: ^29.4.3
-  checksum: 2bbed39ff2fb59f5acac465a1ce7303e3b4b62b479e4f386261986c9827f7f799ea912761e22629c5daf10addf8513f16733c14a29c2647bb66d4ee625e9ff92
+  checksum: c46fb677c88535cf83cf29f0a5b1f376c6a1109ddda266ad7da1a9cbc53cb441fa402dd61fc7b111ffc99603c11a9b3357ee41a1c0e035a58830bcb360871476
   languageName: node
   linkType: hard
 
-"@jest/expect@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/expect@npm:29.4.3"
+"@jest/expect@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/expect@npm:29.5.0"
   dependencies:
-    expect: ^29.4.3
-    jest-snapshot: ^29.4.3
-  checksum: 08d0d40077ec99a7491fe59d05821dbd31126cfba70875855d8a063698b7126b5f6c309c50811caacc6ae2f727c6e44f51bdcf1d6c1ea832b4f020045ef22d45
+    expect: ^29.5.0
+    jest-snapshot: ^29.5.0
+  checksum: bd10e295111547e6339137107d83986ab48d46561525393834d7d2d8b2ae9d5626653f3f5e48e5c3fa742ac982e97bdf1f541b53b9e1d117a247b08e938527f6
   languageName: node
   linkType: hard
 
-"@jest/fake-timers@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/fake-timers@npm:29.4.3"
+"@jest/fake-timers@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/fake-timers@npm:29.5.0"
   dependencies:
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     "@sinonjs/fake-timers": ^10.0.2
     "@types/node": "*"
-    jest-message-util: ^29.4.3
-    jest-mock: ^29.4.3
-    jest-util: ^29.4.3
-  checksum: adaceb9143c395cccf3d7baa0e49b7042c3092a554e8283146df19926247e34c21b5bde5688bb90e9e87b4a02e4587926c5d858ee0a38d397a63175d0a127874
+    jest-message-util: ^29.5.0
+    jest-mock: ^29.5.0
+    jest-util: ^29.5.0
+  checksum: 69930c6922341f244151ec0d27640852ec96237f730fc024da1f53143d31b43cde75d92f9d8e5937981cdce3b31416abc3a7090a0d22c2377512c4a6613244ee
   languageName: node
   linkType: hard
 
-"@jest/globals@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/globals@npm:29.4.3"
+"@jest/globals@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/globals@npm:29.5.0"
   dependencies:
-    "@jest/environment": ^29.4.3
-    "@jest/expect": ^29.4.3
-    "@jest/types": ^29.4.3
-    jest-mock: ^29.4.3
-  checksum: ea76b546ceb4aa5ce2bb3726df12f989b23150b51c9f7664790caa81b943012a657cf3a8525498af1c3518cdb387f54b816cfba1b0ddd22c7b20f03b1d7290b4
+    "@jest/environment": ^29.5.0
+    "@jest/expect": ^29.5.0
+    "@jest/types": ^29.5.0
+    jest-mock: ^29.5.0
+  checksum: b309ab8f21b571a7c672608682e84bbdd3d2b554ddf81e4e32617fec0a69094a290ab42e3c8b2c66ba891882bfb1b8b2736720ea1285b3ad646d55c2abefedd9
   languageName: node
   linkType: hard
 
-"@jest/reporters@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/reporters@npm:29.4.3"
+"@jest/reporters@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/reporters@npm:29.5.0"
   dependencies:
     "@bcoe/v8-coverage": ^0.2.3
-    "@jest/console": ^29.4.3
-    "@jest/test-result": ^29.4.3
-    "@jest/transform": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/console": ^29.5.0
+    "@jest/test-result": ^29.5.0
+    "@jest/transform": ^29.5.0
+    "@jest/types": ^29.5.0
     "@jridgewell/trace-mapping": ^0.3.15
     "@types/node": "*"
     chalk: ^4.0.0
     collect-v8-coverage: ^1.0.0
     exit: ^0.1.2
     glob: ^7.1.3
     graceful-fs: ^4.2.9
     istanbul-lib-coverage: ^3.0.0
     istanbul-lib-instrument: ^5.1.0
     istanbul-lib-report: ^3.0.0
     istanbul-lib-source-maps: ^4.0.0
     istanbul-reports: ^3.1.3
-    jest-message-util: ^29.4.3
-    jest-util: ^29.4.3
-    jest-worker: ^29.4.3
+    jest-message-util: ^29.5.0
+    jest-util: ^29.5.0
+    jest-worker: ^29.5.0
     slash: ^3.0.0
     string-length: ^4.0.1
     strip-ansi: ^6.0.0
     v8-to-istanbul: ^9.0.1
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
-  checksum: 7aa2e429c915bd96c3334962addd69d2bbf52065725757ddde26b293f8c4420a1e8c65363cc3e1e5ec89100a5273ccd3771bec58325a2cc0d97afdc81995073a
+  checksum: 481268aac9a4a75cc49c4df1273d6b111808dec815e9d009dad717c32383ebb0cebac76e820ad1ab44e207540e1c2fe1e640d44c4f262de92ab1933e057fdeeb
   languageName: node
   linkType: hard
 
 "@jest/schemas@npm:^29.4.3":
   version: 29.4.3
   resolution: "@jest/schemas@npm:29.4.3"
   dependencies:
@@ -1898,72 +1887,72 @@
     "@jridgewell/trace-mapping": ^0.3.15
     callsites: ^3.0.0
     graceful-fs: ^4.2.9
   checksum: 2301d225145f8123540c0be073f35a80fd26a2f5e59550fd68525d8cea580fb896d12bf65106591ffb7366a8a19790076dbebc70e0f5e6ceb51f81827ed1f89c
   languageName: node
   linkType: hard
 
-"@jest/test-result@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/test-result@npm:29.4.3"
+"@jest/test-result@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/test-result@npm:29.5.0"
   dependencies:
-    "@jest/console": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/console": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/istanbul-lib-coverage": ^2.0.0
     collect-v8-coverage: ^1.0.0
-  checksum: 164f102b96619ec283c2c39e208b8048e4674f75bf3c3a4f2e95048ae0f9226105add684b25f10d286d91c221625f877e2c1cfc3da46c42d7e1804da239318cb
+  checksum: 2e8ff5242227ab960c520c3ea0f6544c595cc1c42fa3873c158e9f4f685f4ec9670ec08a4af94ae3885c0005a43550a9595191ffbc27a0965df27d9d98bbf901
   languageName: node
   linkType: hard
 
-"@jest/test-sequencer@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/test-sequencer@npm:29.4.3"
+"@jest/test-sequencer@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/test-sequencer@npm:29.5.0"
   dependencies:
-    "@jest/test-result": ^29.4.3
+    "@jest/test-result": ^29.5.0
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.4.3
+    jest-haste-map: ^29.5.0
     slash: ^3.0.0
-  checksum: 145e1fa9379e5be3587bde6d585b8aee5cf4442b06926928a87e9aec7de5be91b581711d627c6ca13144d244fe05e5d248c13b366b51bedc404f9dcfbfd79e9e
+  checksum: eca34b4aeb2fda6dfb7f9f4b064c858a7adf64ec5c6091b6f4ed9d3c19549177cbadcf1c615c4c182688fa1cf085c8c55c3ca6eea40719a34554b0bf071d842e
   languageName: node
   linkType: hard
 
-"@jest/transform@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/transform@npm:29.4.3"
+"@jest/transform@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/transform@npm:29.5.0"
   dependencies:
     "@babel/core": ^7.11.6
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     "@jridgewell/trace-mapping": ^0.3.15
     babel-plugin-istanbul: ^6.1.1
     chalk: ^4.0.0
     convert-source-map: ^2.0.0
     fast-json-stable-stringify: ^2.1.0
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.4.3
+    jest-haste-map: ^29.5.0
     jest-regex-util: ^29.4.3
-    jest-util: ^29.4.3
+    jest-util: ^29.5.0
     micromatch: ^4.0.4
     pirates: ^4.0.4
     slash: ^3.0.0
     write-file-atomic: ^4.0.2
-  checksum: 082d74e04044213aa7baa8de29f8383e5010034f867969c8602a2447a4ef2f484cfaf2491eba3179ce42f369f7a0af419cbd087910f7e5caf7aa5d1fe03f2ff9
+  checksum: d55d604085c157cf5112e165ff5ac1fa788873b3b31265fb4734ca59892ee24e44119964cc47eb6d178dd9512bbb6c576d1e20e51a201ff4e24d31e818a1c92d
   languageName: node
   linkType: hard
 
-"@jest/types@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "@jest/types@npm:29.4.3"
+"@jest/types@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "@jest/types@npm:29.5.0"
   dependencies:
     "@jest/schemas": ^29.4.3
     "@types/istanbul-lib-coverage": ^2.0.0
     "@types/istanbul-reports": ^3.0.0
     "@types/node": "*"
     "@types/yargs": ^17.0.8
     chalk: ^4.0.0
-  checksum: 1756f4149d360f98567f56f434144f7af23ed49a2c42889261a314df6b6654c2de70af618fb2ee0ee39cadaf10835b885845557184509503646c9cb9dcc02bac
+  checksum: 1811f94b19cf8a9460a289c4f056796cfc373480e0492692a6125a553cd1a63824bd846d7bb78820b7b6f758f6dd3c2d4558293bb676d541b2fa59c70fdf9d39
   languageName: node
   linkType: hard
 
 "@jridgewell/gen-mapping@npm:^0.1.0":
   version: 0.1.1
   resolution: "@jridgewell/gen-mapping@npm:0.1.1"
   dependencies:
@@ -2011,30 +2000,30 @@
 "@jridgewell/sourcemap-codec@npm:1.4.14, @jridgewell/sourcemap-codec@npm:^1.4.10":
   version: 1.4.14
   resolution: "@jridgewell/sourcemap-codec@npm:1.4.14"
   checksum: 61100637b6d173d3ba786a5dff019e1a74b1f394f323c1fee337ff390239f053b87266c7a948777f4b1ee68c01a8ad0ab61e5ff4abb5a012a0b091bec391ab97
   languageName: node
   linkType: hard
 
-"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.14, @jridgewell/trace-mapping@npm:^0.3.15, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.9":
+"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.15, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.9":
   version: 0.3.17
   resolution: "@jridgewell/trace-mapping@npm:0.3.17"
   dependencies:
     "@jridgewell/resolve-uri": 3.1.0
     "@jridgewell/sourcemap-codec": 1.4.14
   checksum: 9d703b859cff5cd83b7308fd457a431387db5db96bd781a63bf48e183418dd9d3d44e76b9e4ae13237f6abeeb25d739ec9215c1d5bfdd08f66f750a50074a339
   languageName: node
   linkType: hard
 
 "@jupyter/collaboration-extension@workspace:packages/collaboration-extension":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration-extension@workspace:packages/collaboration-extension"
   dependencies:
-    "@jupyter/collaboration": ^1.0.0-alpha.7
-    "@jupyter/docprovider": ^1.0.0-alpha.7
+    "@jupyter/collaboration": ^1.0.0-alpha.8
+    "@jupyter/docprovider": ^1.0.0-alpha.8
     "@jupyterlab/application": ^4.0.0-beta.0
     "@jupyterlab/apputils": ^4.0.0-beta.0
     "@jupyterlab/builder": ^4.0.0-beta.0
     "@jupyterlab/codemirror": ^4.0.0-beta.0
     "@jupyterlab/coreutils": ^6.0.0-beta.0
     "@jupyterlab/filebrowser": ^4.0.0-beta.0
     "@jupyterlab/services": ^7.0.0-beta.0
@@ -2050,15 +2039,15 @@
     typescript: ~5.0.2
     y-protocols: ^1.0.5
     y-websocket: ^1.3.15
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/collaboration@^1.0.0-alpha.7, @jupyter/collaboration@workspace:packages/collaboration":
+"@jupyter/collaboration@^1.0.0-alpha.8, @jupyter/collaboration@workspace:packages/collaboration":
   version: 0.0.0-use.local
   resolution: "@jupyter/collaboration@workspace:packages/collaboration"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.7.0
     "@jupyterlab/apputils": ^4.0.0-beta.0
     "@jupyterlab/coreutils": ^6.0.0-beta.0
@@ -2072,19 +2061,19 @@
     rimraf: ^4.1.2
     typescript: ~5.0.2
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupyter/docprovider@^1.0.0-alpha.7, @jupyter/docprovider@workspace:packages/docprovider":
+"@jupyter/docprovider@^1.0.0-alpha.8, @jupyter/docprovider@workspace:packages/docprovider":
   version: 0.0.0-use.local
   resolution: "@jupyter/docprovider@workspace:packages/docprovider"
   dependencies:
-    "@jupyter/ydoc": ^0.3.4
+    "@jupyter/ydoc": ^1.0.0
     "@jupyterlab/coreutils": ^6.0.0-beta.0
     "@jupyterlab/services": ^7.0.0-beta.0
     "@jupyterlab/testing": ^4.0.0-beta.0
     "@lumino/coreutils": ^2.0.0
     "@lumino/disposable": ^2.0.0
     "@lumino/signaling": ^2.0.0
     "@types/jest": ^29.2.0
@@ -2129,14 +2118,28 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0-alpha.6
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: edd14a01be6ceac437d3ebfb5f7a2d2c8eac60fec91e48d8d2ef2bef9f1423b4350c57dba25b3b043759ffb61b601a3815c1ea56532d1d707e3fbeb5df86b7e6
   languageName: node
   linkType: hard
 
+"@jupyter/ydoc@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "@jupyter/ydoc@npm:1.0.0"
+  dependencies:
+    "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
+    "@lumino/coreutils": ^1.11.0 || ^2.0.0
+    "@lumino/disposable": ^1.10.0 || ^2.0.0
+    "@lumino/signaling": ^1.10.0 || ^2.0.0
+    y-protocols: ^1.0.5
+    yjs: ^13.5.40
+  checksum: 482f97b7e1e71736a3598dec41659696453821f056ecfaa8e67215b3766b7770cb6d718982069124698e1a824cb9aee20835a248d1d393d2229e7920a2b69f5c
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/application@npm:^4.0.0-beta.0":
   version: 4.0.0-beta.0
   resolution: "@jupyterlab/application@npm:4.0.0-beta.0"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
     "@jupyterlab/apputils": ^4.0.0-beta.0
     "@jupyterlab/coreutils": ^6.0.0-beta.0
@@ -2399,15 +2402,24 @@
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.0.0
     react: ^18.2.0
   checksum: ff4c5ac57f7e8eb08d2a820a63222248c369ea06e63b9423eb299a3aad07d147ae153569eee73771a21f662b13f10b44d832b6bee29a8968bc50d7668b9233f8
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.15, @jupyterlab/nbformat@npm:^4.0.0-beta.0":
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.15, @jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0":
+  version: 3.6.2
+  resolution: "@jupyterlab/nbformat@npm:3.6.2"
+  dependencies:
+    "@lumino/coreutils": ^1.11.0
+  checksum: 9da3c71ca8a8c72d77a941fd527ce1e83f9f0978c3f35106f70f40bab929d261d8a91464303da38cca52450a5cbea0375049b2883795cec457f2673138d3e953
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/nbformat@npm:^4.0.0-beta.0":
   version: 4.0.0-beta.0
   resolution: "@jupyterlab/nbformat@npm:4.0.0-beta.0"
   dependencies:
     "@lumino/coreutils": ^2.0.0
   checksum: 7d6a56d665af349f7e60e0464ce2e4ebc03b25090561aececd23b3e8fe0042af458abb6234523f9a45080f78ac21c5c5bc306a54f74f4b4545e56faf251a9331
   languageName: node
   linkType: hard
@@ -2581,43 +2593,113 @@
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
   checksum: f4de4594a4c7301dc1fa055119284a119fbf0d16e6fb5f4e371f855f02a5b47ea148cec0bee4e5217a1c09bda4ad07542554bd6fcaa073e68d6d9409ceb346ad
   languageName: node
   linkType: hard
 
-"@lerna/child-process@npm:6.5.1":
-  version: 6.5.1
-  resolution: "@lerna/child-process@npm:6.5.1"
+"@lerna/child-process@npm:6.6.1":
+  version: 6.6.1
+  resolution: "@lerna/child-process@npm:6.6.1"
   dependencies:
     chalk: ^4.1.0
     execa: ^5.0.0
     strong-log-transformer: ^2.1.0
-  checksum: 78629ce48ce4b9464c3a51f30ed304915591fd2755398a3adc41a66140e34f1408ce41ac9cf96203c0be68930e39e3347ce92d677e5047ec94103576f68a26ea
+  checksum: 075f872e43b462e07fe3ab690384138f7bfc8313306981e4f2251f3bf8ecc7bae37b35b404cd8cd33e403a7d81975f92bf78c6a1fc1d3140d2b6d3cc38eae555
   languageName: node
   linkType: hard
 
-"@lerna/create@npm:6.5.1":
-  version: 6.5.1
-  resolution: "@lerna/create@npm:6.5.1"
+"@lerna/create@npm:6.6.1":
+  version: 6.6.1
+  resolution: "@lerna/create@npm:6.6.1"
   dependencies:
-    "@lerna/child-process": 6.5.1
+    "@lerna/child-process": 6.6.1
     dedent: ^0.7.0
     fs-extra: ^9.1.0
     init-package-json: ^3.0.2
     npm-package-arg: 8.1.1
     p-reduce: ^2.1.0
     pacote: ^13.6.1
     pify: ^5.0.0
     semver: ^7.3.4
     slash: ^3.0.0
     validate-npm-package-license: ^3.0.4
     validate-npm-package-name: ^4.0.0
     yargs-parser: 20.2.4
-  checksum: dd2c7ffd555468b7e11302de5f2a4da65fa944769c6962be1742db144ee8cf415adf240cfc3a7eca20b8749d7e0f77e716f92359a19431356fce0e2d103e32a5
+  checksum: be8273644d6f156c3c81a89a370e13451ee92c7aeff5dba126be6a909479f2364031a327bd0f43a7beddc03c196c3effff9516201966cc903de3a2e3230dc4d1
+  languageName: node
+  linkType: hard
+
+"@lerna/legacy-package-management@npm:6.6.1":
+  version: 6.6.1
+  resolution: "@lerna/legacy-package-management@npm:6.6.1"
+  dependencies:
+    "@npmcli/arborist": 6.2.3
+    "@npmcli/run-script": 4.1.7
+    "@nrwl/devkit": ">=15.5.2 < 16"
+    "@octokit/rest": 19.0.3
+    byte-size: 7.0.0
+    chalk: 4.1.0
+    clone-deep: 4.0.1
+    cmd-shim: 5.0.0
+    columnify: 1.6.0
+    config-chain: 1.1.12
+    conventional-changelog-core: 4.2.4
+    conventional-recommended-bump: 6.1.0
+    cosmiconfig: 7.0.0
+    dedent: 0.7.0
+    dot-prop: 6.0.1
+    execa: 5.0.0
+    file-url: 3.0.0
+    find-up: 5.0.0
+    fs-extra: 9.1.0
+    get-port: 5.1.1
+    get-stream: 6.0.0
+    git-url-parse: 13.1.0
+    glob-parent: 5.1.2
+    globby: 11.1.0
+    graceful-fs: 4.2.10
+    has-unicode: 2.0.1
+    inquirer: 8.2.4
+    is-ci: 2.0.0
+    is-stream: 2.0.0
+    libnpmpublish: 6.0.4
+    load-json-file: 6.2.0
+    make-dir: 3.1.0
+    minimatch: 3.0.5
+    multimatch: 5.0.0
+    node-fetch: 2.6.7
+    npm-package-arg: 8.1.1
+    npm-packlist: 5.1.1
+    npm-registry-fetch: 14.0.3
+    npmlog: 6.0.2
+    p-map: 4.0.0
+    p-map-series: 2.1.0
+    p-queue: 6.6.2
+    p-waterfall: 2.1.1
+    pacote: 13.6.2
+    pify: 5.0.0
+    pretty-format: 29.4.3
+    read-cmd-shim: 3.0.0
+    read-package-json: 5.0.1
+    resolve-from: 5.0.0
+    semver: 7.3.8
+    signal-exit: 3.0.7
+    slash: 3.0.0
+    ssri: 9.0.1
+    strong-log-transformer: 2.1.0
+    tar: 6.1.11
+    temp-dir: 1.0.0
+    tempy: 1.0.0
+    upath: 2.0.1
+    uuid: 8.3.2
+    write-file-atomic: 4.0.1
+    write-pkg: 4.0.0
+    yargs: 16.2.0
+  checksum: 198cad91376e16edcb66b77cab58217f04ea97a27ccbd811842c9886330c66b2898fe3972ba91231f54c520f208a52207db7060651b2ff290d3702cfc1daaf77
   languageName: node
   linkType: hard
 
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2":
   version: 1.0.2
   resolution: "@lezer/common@npm:1.0.2"
   checksum: bbcc58e07be02652bf0700d2856042ec089d5be0b95893d628b3e18192ade864fac83b61b19653e10b9f1472261a178b12318d934e9004edd5483a577c0db56b
@@ -2653,50 +2735,50 @@
   bin:
     lezer-generator: dist/lezer-generator.cjs
   checksum: 62f93704d7b0b53bbd842c65552b9089f354edbf5f50f05d65a214a5dba05c0a63c898ca448a93ecc803d5b8b05d5eb593a5e5509c478c8dfa3b49ff28dcafb3
   languageName: node
   linkType: hard
 
 "@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3":
-  version: 1.1.3
-  resolution: "@lezer/highlight@npm:1.1.3"
+  version: 1.1.4
+  resolution: "@lezer/highlight@npm:1.1.4"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 90ec143ce46b32f6779c3b245f1b5a540d66686939816d3daed8318821acc4bc719466dc222336cfd483bf04a8de4fdc6f279e904cf114d4d9f786f9feccbbd8
+  checksum: 30e848c02839bfcd9472fcd6e74d71cba12379cef38f27d0c6cab0e6831f92150cfc629d267a40cc31f84cf46ac0a935400163fdf931b2672c516bec29417485
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.3
-  resolution: "@lezer/html@npm:1.3.3"
+  version: 1.3.4
+  resolution: "@lezer/html@npm:1.3.4"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: ad74a5a751daead9d5979a4e1dc55faf94e623672d6b835e4d84d7a1174f326fa6b511a354f6dd5ec4c0b375242614966607ecf07cc92e5c13afe882178fe01d
+  checksum: 81dd134ac094edf7c40bae4c3b7126d336ce4c3c87756344bf604eff64d89b06fcb55f91618a4622eb0dae6d6015722f5bab58e2252d86e81fca8c3ced1a0c4d
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
   version: 1.0.3
   resolution: "@lezer/java@npm:1.0.3"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 2fffea6627d130413ffad4e61040267974cca3167d98881b9e5b5e2455530de74a82c234d93603e92a4972fad314671453c49c0a76b0f4547c4617d671fd7b99
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.1
-  resolution: "@lezer/javascript@npm:1.4.1"
+  version: 1.4.2
+  resolution: "@lezer/javascript@npm:1.4.2"
   dependencies:
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: 634270116d5f1c278e2949d397845f41cac388dec7f0db593a3dc23e0fd4a1b73b9bf08f96fcf109fcd3d38c4b374d48676dce3261ff8ff83a85f5d6a37989f7
+  checksum: 542261c297709babfe450de1233c13fe2f5b111678d280cb0f8304f12bcdae294cb43c0ac64bbd647e5039de3286f6f0715d120fb132bd5af778363d1f612a1f
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
   version: 1.0.0
   resolution: "@lezer/json@npm:1.0.0"
   dependencies:
@@ -2732,20 +2814,20 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
   checksum: a847c255c030b4d38913ddf1d5bd7324d83be7ef8d1d244542870be03b9bf7dc71283afeb2415c40dfd188cb99f0cc44bad760b5f3b7c35c3b8e5e00253848fc
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.0.0":
-  version: 1.1.3
-  resolution: "@lezer/python@npm:1.1.3"
+  version: 1.1.4
+  resolution: "@lezer/python@npm:1.1.4"
   dependencies:
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 6c621b8970a27ccc7f74a4cabf38de4f25904497448c6fd4416e0e613355d12565f722cdddb513a05c76e6ab64cef9060acefb19e4d39d7b0a47589c6f81e2bc
+  checksum: d525e15c75493d4a47eccb72cbdaf942fbc35e8eb2b2a998f12ec869b56a6a5be0a1065ec250ab228b2fdcf8d4b02115b06b0edcbfe72558f2ad8ad161f4d241
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
   version: 1.0.0
   resolution: "@lezer/rust@npm:1.0.0"
   dependencies:
@@ -2768,80 +2850,66 @@
 "@lumino/algorithm@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/algorithm@npm:2.0.0"
   checksum: 663edf536e94397b449c6a2643a735e602fbb396dec86b56ad1193a768dce27c6e7da5ad0384aa90086ea44cbb64dde3f9d565e9fd81858f1eb0c6b4253f3b94
   languageName: node
   linkType: hard
 
-"@lumino/algorithm@npm:^2.0.0-beta.0":
-  version: 2.0.0-beta.0
-  resolution: "@lumino/algorithm@npm:2.0.0-beta.0"
-  checksum: dbb42db24393de3be8e6f50b83728235154fb4d134cdf5fde07f7fe1dcbcdeaa23912729136a8c75e8a05ad31a8114946479785744e84c04636ac8d26a598816
-  languageName: node
-  linkType: hard
-
 "@lumino/application@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/application@npm:2.0.0"
+  version: 2.0.1
+  resolution: "@lumino/application@npm:2.0.1"
   dependencies:
-    "@lumino/commands": ^2.0.0
+    "@lumino/commands": ^2.0.1
     "@lumino/coreutils": ^2.0.0
-    "@lumino/widgets": ^2.0.0
-  checksum: 0c33343e0bbfb3908c92eda90e88ad3c94dba9b7ddc2a5c653d3182497b546ddf2cb6ca1c8b7ed83d83a273a5889bf541f5e92d982ed3323d6835aaa5ad3f244
+    "@lumino/widgets": ^2.0.1
+  checksum: c389b6e35b614c14551963f864a50383ca3a51192adbbef8c208d9ed7d8cd526d5c498743f5e6ca0b7de362027b68324e1cde0c735b314326d21ced15edf8e7b
   languageName: node
   linkType: hard
 
 "@lumino/collections@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/collections@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
   checksum: 4a7fc3571e92a1368a1ef01300ad7b6e0d4ff13cb78b89533d5962eea66d4a7550e15d8b80fa3ab1816b1a89382f35015f9dddf72ab04654c17e5b516b845d8f
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/commands@npm:2.0.0"
+"@lumino/commands@npm:^2.0.0, @lumino/commands@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/commands@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.0.0
     "@lumino/disposable": ^2.0.0
     "@lumino/domutils": ^2.0.0
     "@lumino/keyboard": ^2.0.0
     "@lumino/signaling": ^2.0.0
     "@lumino/virtualdom": ^2.0.0
-  checksum: add40b1460260dc536ec6383514b0328ae091bb77739a4bc0c164e1adf2688b000da93a3947517c4f54bb0f20d596805b526e12d06742efe5f81aa60bad7b762
+  checksum: cefc9bb4b7b61054f199b5bf35501765688eb2922af2610087f43e4bb5f6663ee8579fcf02e12d6083697456423ada67cae5b2d020daa0856c646d050b30d420
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^1.11.0 || ^2.0.0-alpha.6, @lumino/coreutils@npm:^2.0.0-beta.0":
-  version: 2.0.0-beta.0
-  resolution: "@lumino/coreutils@npm:2.0.0-beta.0"
-  checksum: ac490f895fd2fbbf86ee7c51258581830238d4dd8c5491f9ac4bcc55ee3ae779de00bb91aba5a714d5838d364595465f3b014bca2459306de1e37ef2b50434a3
+"@lumino/coreutils@npm:^1.11.0":
+  version: 1.12.1
+  resolution: "@lumino/coreutils@npm:1.12.1"
+  peerDependencies:
+    crypto: 1.0.1
+  checksum: 55f1b87997f8dd0af28ff23c2d4b3aa252e515b9d3bc91b350a5c6c8526ceae61b14b55dc0d8d01691c69d42974b3d559f2b49bc7ced0f474b8f5dc52b3e83ed
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^2.0.0":
+"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.0.0-alpha.6, @lumino/coreutils@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/coreutils@npm:2.0.0"
   checksum: 341b5f569b2804e9651ecec6a441a0a0a9153656cc9dc0480eff8bb1d667df92ee4d64421fbb1469f0f503cd2ce3428c61dd3e5d2eb163e2e21748c318fd7b9e
   languageName: node
   linkType: hard
 
-"@lumino/disposable@npm:^1.10.0 || ^2.0.0-alpha.6":
-  version: 2.0.0-beta.1
-  resolution: "@lumino/disposable@npm:2.0.0-beta.1"
-  dependencies:
-    "@lumino/signaling": ^2.0.0-beta.1
-  checksum: f9df869eaf1f0dde2ea553e83b5a84e35769b89578b48f411cad8574c832e8bf72f9243213d117a75d7f14beed76980dfa8560270e1af9b623228f83351f5098
-  languageName: node
-  linkType: hard
-
-"@lumino/disposable@npm:^2.0.0":
+"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^1.10.0 || ^2.0.0-alpha.6, @lumino/disposable@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/disposable@npm:2.0.0"
   dependencies:
     "@lumino/signaling": ^2.0.0
   checksum: d12ad6e3c72fdb869566374a89250678951a4138ed0e80478976a035ca5c48e0de06300fb6ad5cb9d3fc9694058e3b3367653dc63829ee3e67503a03e2252ccc
   languageName: node
   linkType: hard
@@ -2894,25 +2962,15 @@
 "@lumino/properties@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/properties@npm:2.0.0"
   checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
   languageName: node
   linkType: hard
 
-"@lumino/signaling@npm:^1.10.0 || ^2.0.0-alpha.6, @lumino/signaling@npm:^2.0.0-beta.1":
-  version: 2.0.0-beta.1
-  resolution: "@lumino/signaling@npm:2.0.0-beta.1"
-  dependencies:
-    "@lumino/algorithm": ^2.0.0-beta.0
-    "@lumino/coreutils": ^2.0.0-beta.0
-  checksum: c1bfd554243e77e6f542695eceb659da1eb1d6ae58714e5f24350c11e448a4e1f24241ca7a25da620082250ae0e63053c71916ad4c1d0645bd7545fb3fbebd6b
-  languageName: node
-  linkType: hard
-
-"@lumino/signaling@npm:^2.0.0":
+"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^1.10.0 || ^2.0.0-alpha.6, @lumino/signaling@npm:^2.0.0":
   version: 2.0.0
   resolution: "@lumino/signaling@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.0.0
   checksum: fb46a1b33c4a0cec723e8c6f1a9b6e89544ee1a3b94731437639c0e9a1a29c07ff225179081846ee16c5001bf11bcaace646d1307bbb76ea6ae04006f442cd28
   languageName: node
@@ -2923,30 +2981,30 @@
   resolution: "@lumino/virtualdom@npm:2.0.0"
   dependencies:
     "@lumino/algorithm": ^2.0.0
   checksum: 6fc1d88e7d4a656be7664ccfc5745eb1d4e3d2034db0b11ad6abefcc642f22d265003eef0e1d02bca2e42b6da127123118c631369006f78e88a08885a6f36c25
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/widgets@npm:2.0.0"
+"@lumino/widgets@npm:^2.0.0, @lumino/widgets@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/widgets@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.0.0
+    "@lumino/commands": ^2.0.1
     "@lumino/coreutils": ^2.0.0
     "@lumino/disposable": ^2.0.0
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.0.0
     "@lumino/keyboard": ^2.0.0
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.0.0
     "@lumino/virtualdom": ^2.0.0
-  checksum: 5bb1e03264aa6341b4437bbc4108d9ed3fd64c4feb0549f12703171f16a60caca7b162e14aa3bca39b26c4ce7c88f01a39200c9102aecb6d4f44d2d8afc16c04
+  checksum: 5cb54991f269a3ac3517aea20d960cf9340739067a8c11ce3c601d725fe1db841a576a84e316b73f2b35c243f0fa6da98f4cdfe397ce49e05ae886ca38a037e0
   languageName: node
   linkType: hard
 
 "@nodelib/fs.scandir@npm:2.1.5":
   version: 2.1.5
   resolution: "@nodelib/fs.scandir@npm:2.1.5"
   dependencies:
@@ -2969,68 +3027,76 @@
   dependencies:
     "@nodelib/fs.scandir": 2.1.5
     fastq: ^1.6.0
   checksum: 190c643f156d8f8f277bf2a6078af1ffde1fd43f498f187c2db24d35b4b4b5785c02c7dc52e356497b9a1b65b13edc996de08de0b961c32844364da02986dc53
   languageName: node
   linkType: hard
 
-"@npmcli/arborist@npm:5.3.0":
-  version: 5.3.0
-  resolution: "@npmcli/arborist@npm:5.3.0"
+"@npmcli/arborist@npm:6.2.3":
+  version: 6.2.3
+  resolution: "@npmcli/arborist@npm:6.2.3"
   dependencies:
     "@isaacs/string-locale-compare": ^1.1.0
-    "@npmcli/installed-package-contents": ^1.0.7
-    "@npmcli/map-workspaces": ^2.0.3
-    "@npmcli/metavuln-calculator": ^3.0.1
-    "@npmcli/move-file": ^2.0.0
-    "@npmcli/name-from-folder": ^1.0.1
-    "@npmcli/node-gyp": ^2.0.0
-    "@npmcli/package-json": ^2.0.0
-    "@npmcli/run-script": ^4.1.3
-    bin-links: ^3.0.0
-    cacache: ^16.0.6
+    "@npmcli/fs": ^3.1.0
+    "@npmcli/installed-package-contents": ^2.0.0
+    "@npmcli/map-workspaces": ^3.0.2
+    "@npmcli/metavuln-calculator": ^5.0.0
+    "@npmcli/name-from-folder": ^2.0.0
+    "@npmcli/node-gyp": ^3.0.0
+    "@npmcli/package-json": ^3.0.0
+    "@npmcli/query": ^3.0.0
+    "@npmcli/run-script": ^6.0.0
+    bin-links: ^4.0.1
+    cacache: ^17.0.4
     common-ancestor-path: ^1.0.1
-    json-parse-even-better-errors: ^2.3.1
+    hosted-git-info: ^6.1.1
+    json-parse-even-better-errors: ^3.0.0
     json-stringify-nice: ^1.1.4
-    mkdirp: ^1.0.4
-    mkdirp-infer-owner: ^2.0.0
-    nopt: ^5.0.0
-    npm-install-checks: ^5.0.0
-    npm-package-arg: ^9.0.0
-    npm-pick-manifest: ^7.0.0
-    npm-registry-fetch: ^13.0.0
-    npmlog: ^6.0.2
-    pacote: ^13.6.1
-    parse-conflict-json: ^2.0.1
-    proc-log: ^2.0.0
+    minimatch: ^6.1.6
+    nopt: ^7.0.0
+    npm-install-checks: ^6.0.0
+    npm-package-arg: ^10.1.0
+    npm-pick-manifest: ^8.0.1
+    npm-registry-fetch: ^14.0.3
+    npmlog: ^7.0.1
+    pacote: ^15.0.8
+    parse-conflict-json: ^3.0.0
+    proc-log: ^3.0.0
     promise-all-reject-late: ^1.0.0
     promise-call-limit: ^1.0.1
-    read-package-json-fast: ^2.0.2
-    readdir-scoped-modules: ^1.1.0
-    rimraf: ^3.0.2
+    read-package-json-fast: ^3.0.2
     semver: ^7.3.7
-    ssri: ^9.0.0
-    treeverse: ^2.0.0
+    ssri: ^10.0.1
+    treeverse: ^3.0.0
     walk-up-path: ^1.0.0
   bin:
     arborist: bin/index.js
-  checksum: 7f99f451ba625dd3532e7a69b27cc399cab1e7ef2a069bbc04cf22ef9d16a0076f8f5fb92c4cd146c256cd8a41963b2e417684f063a108e96939c440bad0e95e
+  checksum: f52261745fdcdb95813ec47d0fbe375e6448f3d62f805601a7afe447540f3ffb741834a1c2275707c17a4322e723915c1bb8abb3400dd3a3476ab281b64954bc
   languageName: node
   linkType: hard
 
 "@npmcli/fs@npm:^2.1.0":
   version: 2.1.2
   resolution: "@npmcli/fs@npm:2.1.2"
   dependencies:
     "@gar/promisify": ^1.1.3
     semver: ^7.3.5
   checksum: 405074965e72d4c9d728931b64d2d38e6ea12066d4fad651ac253d175e413c06fe4350970c783db0d749181da8fe49c42d3880bd1cbc12cd68e3a7964d820225
   languageName: node
   linkType: hard
 
+"@npmcli/fs@npm:^3.1.0":
+  version: 3.1.0
+  resolution: "@npmcli/fs@npm:3.1.0"
+  dependencies:
+    semver: ^7.3.5
+  checksum: a50a6818de5fc557d0b0e6f50ec780a7a02ab8ad07e5ac8b16bf519e0ad60a144ac64f97d05c443c3367235d337182e1d012bbac0eb8dbae8dc7b40b193efd0e
+  languageName: node
+  linkType: hard
+
 "@npmcli/git@npm:^3.0.0":
   version: 3.0.2
   resolution: "@npmcli/git@npm:3.0.2"
   dependencies:
     "@npmcli/promise-spawn": ^3.0.0
     lru-cache: ^7.4.4
     mkdirp: ^1.0.4
@@ -3040,213 +3106,280 @@
     promise-retry: ^2.0.1
     semver: ^7.3.5
     which: ^2.0.2
   checksum: bdfd1229bb1113ad4883ef89b74b5dc442a2c96225d830491dd0dec4fa83d083b93cde92b6978d4956a8365521e61bc8dc1891fb905c7c693d5d6aa178f2ab44
   languageName: node
   linkType: hard
 
+"@npmcli/git@npm:^4.0.0":
+  version: 4.0.4
+  resolution: "@npmcli/git@npm:4.0.4"
+  dependencies:
+    "@npmcli/promise-spawn": ^6.0.0
+    lru-cache: ^7.4.4
+    npm-pick-manifest: ^8.0.0
+    proc-log: ^3.0.0
+    promise-inflight: ^1.0.1
+    promise-retry: ^2.0.1
+    semver: ^7.3.5
+    which: ^3.0.0
+  checksum: fd8ad331138c906e090a0f0d3c1662be140fbb39f0dcf4259ee69e8dcb1a939385996dd003d7abb9ce61739e4119e2ea26b2be7ad396988ec1c1ed83179af032
+  languageName: node
+  linkType: hard
+
 "@npmcli/installed-package-contents@npm:^1.0.7":
   version: 1.0.7
   resolution: "@npmcli/installed-package-contents@npm:1.0.7"
   dependencies:
     npm-bundled: ^1.1.1
     npm-normalize-package-bin: ^1.0.1
   bin:
     installed-package-contents: index.js
   checksum: a4a29b99d439827ce2e7817c1f61b56be160e640696e31dc513a2c8a37c792f75cdb6258ec15a1e22904f20df0a8a3019dd3766de5e6619f259834cf64233538
   languageName: node
   linkType: hard
 
-"@npmcli/map-workspaces@npm:^2.0.3":
-  version: 2.0.4
-  resolution: "@npmcli/map-workspaces@npm:2.0.4"
+"@npmcli/installed-package-contents@npm:^2.0.0, @npmcli/installed-package-contents@npm:^2.0.1":
+  version: 2.0.2
+  resolution: "@npmcli/installed-package-contents@npm:2.0.2"
   dependencies:
-    "@npmcli/name-from-folder": ^1.0.1
-    glob: ^8.0.1
-    minimatch: ^5.0.1
-    read-package-json-fast: ^2.0.3
-  checksum: cc8d662ac5115ad9822742a11e11d2d32eda74214bd0f4efec30c9cd833975b5b4c8409fe54ddbb451b040b17a943f770976506cba0f26cfccd58d99b5880d6f
+    npm-bundled: ^3.0.0
+    npm-normalize-package-bin: ^3.0.0
+  bin:
+    installed-package-contents: lib/index.js
+  checksum: 60789d5ed209ee5df479232f62d9d38ecec36e95701cae88320b828b8651351b32d7b47d16d4c36cc7ce5000db4bf1f3e6981bed6381bdc5687ff4bc0795682d
   languageName: node
   linkType: hard
 
-"@npmcli/metavuln-calculator@npm:^3.0.1":
-  version: 3.1.1
-  resolution: "@npmcli/metavuln-calculator@npm:3.1.1"
+"@npmcli/map-workspaces@npm:^3.0.2":
+  version: 3.0.3
+  resolution: "@npmcli/map-workspaces@npm:3.0.3"
   dependencies:
-    cacache: ^16.0.0
-    json-parse-even-better-errors: ^2.3.1
-    pacote: ^13.0.3
+    "@npmcli/name-from-folder": ^2.0.0
+    glob: ^9.3.1
+    minimatch: ^7.4.2
+    read-package-json-fast: ^3.0.0
+  checksum: d61d152b5c3fbe56c467d447877220be4ee147a64904300adbbdfe33074b37bcb15d96d395a1292e46392766e6d1c6eae43d9daa81ae03c84561eadf333f0bc8
+  languageName: node
+  linkType: hard
+
+"@npmcli/metavuln-calculator@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "@npmcli/metavuln-calculator@npm:5.0.0"
+  dependencies:
+    cacache: ^17.0.0
+    json-parse-even-better-errors: ^3.0.0
+    pacote: ^15.0.0
     semver: ^7.3.5
-  checksum: dc9846fdb82a1f4274ff8943f81452c75615bd9bca523c862956ea2c32e18c5a4be5572e169104d3a0eb262b7ede72c8dbbc202a4ab3b3f4946fa55f226dcc64
+  checksum: 82a64c055b260cdc2a57b0177993d026c3b370a57dab8d83fc87319533e5adeceeeb72feafb36a3381d4090e7ca8a34169e83e6167d1f63dbe1f91bf5e6d89f0
   languageName: node
   linkType: hard
 
 "@npmcli/move-file@npm:^2.0.0":
   version: 2.0.1
   resolution: "@npmcli/move-file@npm:2.0.1"
   dependencies:
     mkdirp: ^1.0.4
     rimraf: ^3.0.2
   checksum: 52dc02259d98da517fae4cb3a0a3850227bdae4939dda1980b788a7670636ca2b4a01b58df03dd5f65c1e3cb70c50fa8ce5762b582b3f499ec30ee5ce1fd9380
   languageName: node
   linkType: hard
 
-"@npmcli/name-from-folder@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "@npmcli/name-from-folder@npm:1.0.1"
-  checksum: 67339f4096e32b712d2df0250cc95c087569f09e657d7f81a1760fa2cc5123e29c3c3e1524388832310ba2d96ec4679985b643b44627f6a51f4a00c3b0075de9
+"@npmcli/name-from-folder@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "@npmcli/name-from-folder@npm:2.0.0"
+  checksum: fb3ef891aa57315fb6171866847f298577c8bda98a028e93e458048477133e142b4eb45ce9f3b80454f7c257612cb01754ee782d608507698dd712164436f5bd
   languageName: node
   linkType: hard
 
 "@npmcli/node-gyp@npm:^2.0.0":
   version: 2.0.0
   resolution: "@npmcli/node-gyp@npm:2.0.0"
   checksum: b6bbf0015000f9b64d31aefdc30f244b0348c57adb64017667e0304e96c38644d83da46a4581252652f5d606268df49118f9c9993b41d8020f62b7b15dd2c8d8
   languageName: node
   linkType: hard
 
-"@npmcli/package-json@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@npmcli/package-json@npm:2.0.0"
+"@npmcli/node-gyp@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "@npmcli/node-gyp@npm:3.0.0"
+  checksum: fe3802b813eecb4ade7ad77c9396cb56721664275faab027e3bd8a5e15adfbbe39e2ecc19f7885feb3cfa009b96632741cc81caf7850ba74440c6a2eee7b4ffc
+  languageName: node
+  linkType: hard
+
+"@npmcli/package-json@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "@npmcli/package-json@npm:3.0.0"
   dependencies:
-    json-parse-even-better-errors: ^2.3.1
-  checksum: 7a598e42d2778654ec87438ebfafbcbafbe5a5f5e89ed2ca1db6ca3f94ef14655e304aa41f77632a2a3f5c66b6bd5960bd9370e0ceb4902ea09346720364f9e4
+    json-parse-even-better-errors: ^3.0.0
+  checksum: d7603ec771c365346e39e24a9dda8fdb3918a55f01011d27bf377468c44991092a1fbdaaa580cfd1ff37456a933630b9a99bf3bb08438e1333c2ce559e86398d
   languageName: node
   linkType: hard
 
 "@npmcli/promise-spawn@npm:^3.0.0":
   version: 3.0.0
   resolution: "@npmcli/promise-spawn@npm:3.0.0"
   dependencies:
     infer-owner: ^1.0.4
   checksum: 3454465a2731cea5875ba51f80873e2205e5bd878c31517286b0ede4ea931c7bf3de895382287e906d03710fff6f9e44186bd0eee068ce578901c5d3b58e7692
   languageName: node
   linkType: hard
 
+"@npmcli/promise-spawn@npm:^6.0.0, @npmcli/promise-spawn@npm:^6.0.1":
+  version: 6.0.2
+  resolution: "@npmcli/promise-spawn@npm:6.0.2"
+  dependencies:
+    which: ^3.0.0
+  checksum: aa725780c13e1f97ab32ed7bcb5a207a3fb988e1d7ecdc3d22a549a22c8034740366b351c4dde4b011bcffcd8c4a7be6083d9cf7bc7e897b88837150de018528
+  languageName: node
+  linkType: hard
+
+"@npmcli/query@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "@npmcli/query@npm:3.0.0"
+  dependencies:
+    postcss-selector-parser: ^6.0.10
+  checksum: 90fca7edd5f3e59e875dd8729e6c3aa174292e5b66caa0d7db85841cc5eeb414c7eb7d7637d30f638605d05e1238e718d09b8c1a251f43cfc21d9ac6835c7b39
+  languageName: node
+  linkType: hard
+
 "@npmcli/run-script@npm:4.1.7":
   version: 4.1.7
   resolution: "@npmcli/run-script@npm:4.1.7"
   dependencies:
     "@npmcli/node-gyp": ^2.0.0
     "@npmcli/promise-spawn": ^3.0.0
     node-gyp: ^9.0.0
     read-package-json-fast: ^2.0.3
     which: ^2.0.2
   checksum: 87c32b12fed981fe8a48de985dd1ae0350bcda2830ca4a35efe4b2b96932905cccd04e6e2de5bfea8ed4e2bf3b6f8315630ff9a09c72f80ff3c49f19a9fc80ff
   languageName: node
   linkType: hard
 
-"@npmcli/run-script@npm:^4.1.0, @npmcli/run-script@npm:^4.1.3":
+"@npmcli/run-script@npm:^4.1.0":
   version: 4.2.1
   resolution: "@npmcli/run-script@npm:4.2.1"
   dependencies:
     "@npmcli/node-gyp": ^2.0.0
     "@npmcli/promise-spawn": ^3.0.0
     node-gyp: ^9.0.0
     read-package-json-fast: ^2.0.3
     which: ^2.0.2
   checksum: 7b8d6676353f157e68b26baf848e01e5d887bcf90ce81a52f23fc9a5d93e6ffb60057532d664cfd7aeeb76d464d0c8b0d314ee6cccb56943acb3b6c570b756c8
   languageName: node
   linkType: hard
 
-"@nrwl/cli@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/cli@npm:15.7.2"
+"@npmcli/run-script@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "@npmcli/run-script@npm:6.0.0"
   dependencies:
-    nx: 15.7.2
-  checksum: c59130679458e1572181d8b49ff3a755bba4e07f8fe9a4c0b20330a16105548381467c557a4f3dd09051cf6ae8bcea15c3f2ccd2dba9ad6d0dfec79de0b61b49
+    "@npmcli/node-gyp": ^3.0.0
+    "@npmcli/promise-spawn": ^6.0.0
+    node-gyp: ^9.0.0
+    read-package-json-fast: ^3.0.0
+    which: ^3.0.0
+  checksum: 9fc387f7c405ae4948921764b8b970c12ae07df22bacc242b0f68709c99a83b9d12f411ebd7e60c85a933e2d7be42c70e243ebd71a8d3f6e783e1aab5ccbb2f5
+  languageName: node
+  linkType: hard
+
+"@nrwl/cli@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/cli@npm:15.8.9"
+  dependencies:
+    nx: 15.8.9
+  checksum: e870f8493b132ef2205c37e432decd5c8da2dd337e5f17038736843e9be200fe3b267b1e8b052975cd4eaa7ea370d91a2427cfe983a9458a97f92b89075b8867
   languageName: node
   linkType: hard
 
 "@nrwl/devkit@npm:>=15.5.2 < 16":
-  version: 15.7.2
-  resolution: "@nrwl/devkit@npm:15.7.2"
+  version: 15.8.9
+  resolution: "@nrwl/devkit@npm:15.8.9"
   dependencies:
     "@phenomnomnominal/tsquery": 4.1.1
     ejs: ^3.1.7
     ignore: ^5.0.4
     semver: 7.3.4
+    tmp: ~0.2.1
     tslib: ^2.3.0
   peerDependencies:
     nx: ">= 14.1 <= 16"
-  checksum: a6f78a1374e91c183a71fb3cb81bfc8fe0d21e18d2bd7b20d01777fd31d155c16dce5944ed2146514761a3960683842f137fc5a22975403d515c32fc753c0a1f
+  checksum: fbf495d62a4e465224d8b85c4af57c0b1c9fa5b344e3e8313d0c7a2f47930a52c749ca4d1df4851312d1c46d1be03d606af50b28c06f149f20fc430f5f86474c
   languageName: node
   linkType: hard
 
-"@nrwl/nx-darwin-arm64@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-darwin-arm64@npm:15.7.2"
+"@nrwl/nx-darwin-arm64@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-darwin-arm64@npm:15.8.9"
   conditions: os=darwin & cpu=arm64
   languageName: node
   linkType: hard
 
-"@nrwl/nx-darwin-x64@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-darwin-x64@npm:15.7.2"
+"@nrwl/nx-darwin-x64@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-darwin-x64@npm:15.8.9"
   conditions: os=darwin & cpu=x64
   languageName: node
   linkType: hard
 
-"@nrwl/nx-linux-arm-gnueabihf@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-linux-arm-gnueabihf@npm:15.7.2"
+"@nrwl/nx-linux-arm-gnueabihf@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-linux-arm-gnueabihf@npm:15.8.9"
   conditions: os=linux & cpu=arm
   languageName: node
   linkType: hard
 
-"@nrwl/nx-linux-arm64-gnu@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-linux-arm64-gnu@npm:15.7.2"
+"@nrwl/nx-linux-arm64-gnu@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-linux-arm64-gnu@npm:15.8.9"
   conditions: os=linux & cpu=arm64 & libc=glibc
   languageName: node
   linkType: hard
 
-"@nrwl/nx-linux-arm64-musl@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-linux-arm64-musl@npm:15.7.2"
+"@nrwl/nx-linux-arm64-musl@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-linux-arm64-musl@npm:15.8.9"
   conditions: os=linux & cpu=arm64 & libc=musl
   languageName: node
   linkType: hard
 
-"@nrwl/nx-linux-x64-gnu@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-linux-x64-gnu@npm:15.7.2"
+"@nrwl/nx-linux-x64-gnu@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-linux-x64-gnu@npm:15.8.9"
   conditions: os=linux & cpu=x64 & libc=glibc
   languageName: node
   linkType: hard
 
-"@nrwl/nx-linux-x64-musl@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-linux-x64-musl@npm:15.7.2"
+"@nrwl/nx-linux-x64-musl@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-linux-x64-musl@npm:15.8.9"
   conditions: os=linux & cpu=x64 & libc=musl
   languageName: node
   linkType: hard
 
-"@nrwl/nx-win32-arm64-msvc@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-win32-arm64-msvc@npm:15.7.2"
+"@nrwl/nx-win32-arm64-msvc@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-win32-arm64-msvc@npm:15.8.9"
   conditions: os=win32 & cpu=arm64
   languageName: node
   linkType: hard
 
-"@nrwl/nx-win32-x64-msvc@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/nx-win32-x64-msvc@npm:15.7.2"
+"@nrwl/nx-win32-x64-msvc@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/nx-win32-x64-msvc@npm:15.8.9"
   conditions: os=win32 & cpu=x64
   languageName: node
   linkType: hard
 
-"@nrwl/tao@npm:15.7.2":
-  version: 15.7.2
-  resolution: "@nrwl/tao@npm:15.7.2"
+"@nrwl/tao@npm:15.8.9":
+  version: 15.8.9
+  resolution: "@nrwl/tao@npm:15.8.9"
   dependencies:
-    nx: 15.7.2
+    nx: 15.8.9
   bin:
     tao: index.js
-  checksum: cbf76f385bffb1bf1bde52d4ad950a8abd1ba9865f47afb67a58bb5dc5d7be0d21c5021a3332d2ab665d99b36ec1f08ee260c1289bb7e69783e69712145d2709
+  checksum: dbf0b187d41110211233ce4fc78f49933d52459a09dbf8c807ad58a02466424503c565b49081067a750aa42fdb4ea1090883dab9f2aa91ce968da434303dadf0
   languageName: node
   linkType: hard
 
 "@octokit/auth-token@npm:^3.0.0":
   version: 3.0.3
   resolution: "@octokit/auth-token@npm:3.0.3"
   dependencies:
@@ -3435,47 +3568,55 @@
   peerDependencies:
     typescript: ^3 || ^4
   checksum: 64eb6d90aafa889f62fe73d128b7be2b3295dffde4d5dff63bad75d512b6bc1d8419d8fc784a1a60b45aba4cda2eaf6e233bf59797a1d91b26fac27d99dae047
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.1.0":
-  version: 5.1.0
-  resolution: "@rjsf/core@npm:5.1.0"
+  version: 5.4.0
+  resolution: "@rjsf/core@npm:5.4.0"
   dependencies:
     lodash: ^4.17.15
     lodash-es: ^4.17.15
+    markdown-to-jsx: ^7.2.0
     nanoid: ^3.3.4
     prop-types: ^15.7.2
   peerDependencies:
     "@rjsf/utils": ^5.0.0
     react: ^16.14.0 || >=17
-  checksum: ff38046bb25de86b57e404c5d1ccea84b0485e916caf33a3cb25b030a38ed930a9b89a411671a7c29b047da38e0c682e20b43b13e61d77df770299385ba3c67a
+  checksum: 3d0a2bd0814c8aae3ffb524a0d53ba9141475bcf63975b9a5409602ab9d3ce60f0bdc49c86cff7e30b0d1468562e74a8d5ec2a61b9e5329cf9ef57dcdf227167
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.1.0":
-  version: 5.1.0
-  resolution: "@rjsf/utils@npm:5.1.0"
+  version: 5.4.0
+  resolution: "@rjsf/utils@npm:5.4.0"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.15
     lodash-es: ^4.17.15
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 76d7caf144f98b1547067bfdc2b1baecf452c63bd9d6f2cae6c162a99154bb4d2f5033f6abc0e26ab767dca9ea743f1f5a9d796696e90dd5ed1fdca5ee3c5280
+  checksum: 096283446b100dec731d06abc0a758588138321c930194cc6bb5c4d2def7be28e058eba3ab2741b30421d1c095c3f700a349d3f6d69d2c0b903f2695b855afe6
+  languageName: node
+  linkType: hard
+
+"@sigstore/protobuf-specs@npm:^0.1.0":
+  version: 0.1.0
+  resolution: "@sigstore/protobuf-specs@npm:0.1.0"
+  checksum: 9959bc5176906609dda6ad2a1f5226fac1e49fcb4d29f38969d2a2e3a05cba8e2479721ba78c46a507513abacb63f25a991e5e8856c300204cded455f34ba8c5
   languageName: node
   linkType: hard
 
 "@sinclair/typebox@npm:^0.25.16":
-  version: 0.25.23
-  resolution: "@sinclair/typebox@npm:0.25.23"
-  checksum: 5720daec6e604be9ac849e6361cfa30d19f4d01934c9b79a3a5f5290dfcefaa300192ea0d384bb5dd0104432d88447bbad27adfacdf0b0f042b510bf15fbd5db
+  version: 0.25.24
+  resolution: "@sinclair/typebox@npm:0.25.24"
+  checksum: 10219c58f40b8414c50b483b0550445e9710d4fe7b2c4dccb9b66533dd90ba8e024acc776026cebe81e87f06fa24b07fdd7bc30dd277eb9cc386ec50151a3026
   languageName: node
   linkType: hard
 
 "@sinonjs/commons@npm:^2.0.0":
   version: 2.0.0
   resolution: "@sinonjs/commons@npm:2.0.0"
   dependencies:
@@ -3496,14 +3637,23 @@
 "@tootallnate/once@npm:2":
   version: 2.0.0
   resolution: "@tootallnate/once@npm:2.0.0"
   checksum: ad87447820dd3f24825d2d947ebc03072b20a42bfc96cbafec16bff8bbda6c1a81fcb0be56d5b21968560c5359a0af4038a68ba150c3e1694fe4c109a063bed8
   languageName: node
   linkType: hard
 
+"@tufjs/models@npm:1.0.1":
+  version: 1.0.1
+  resolution: "@tufjs/models@npm:1.0.1"
+  dependencies:
+    minimatch: ^7.4.2
+  checksum: 2f8ebc8e8ef56be67051077b09c7611f50e04d89f8277e3ab518565fbbdf5c81e725c66ae3793cdcc9ec443eb1229dccc3af5d96ec71a134e4c00ea749733bcd
+  languageName: node
+  linkType: hard
+
 "@types/babel__core@npm:^7.1.14":
   version: 7.20.0
   resolution: "@types/babel__core@npm:7.20.0"
   dependencies:
     "@babel/parser": ^7.20.7
     "@babel/types": ^7.20.7
     "@types/babel__generator": "*"
@@ -3548,20 +3698,20 @@
     "@types/eslint": "*"
     "@types/estree": "*"
   checksum: ea6a9363e92f301cd3888194469f9ec9d0021fe0a397a97a6dd689e7545c75de0bd2153dfb13d3ab532853a278b6572c6f678ce846980669e41029d205653460
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.21.1
-  resolution: "@types/eslint@npm:8.21.1"
+  version: 8.37.0
+  resolution: "@types/eslint@npm:8.37.0"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 584068441e4000c7b41c8928274fdcc737bc62f564928c30eb64ec41bbdbac31612f9fedaf490bceab31ec8305e99615166428188ea345d58878394683086fae
+  checksum: 06d3b3fba12004294591b5c7a52e3cec439472195da54e096076b1f2ddfbb8a445973b9681046dd530a6ac31eca502f635abc1e3ce37d03513089358e6f822ee
   languageName: node
   linkType: hard
 
 "@types/estree@npm:*":
   version: 1.0.0
   resolution: "@types/estree@npm:1.0.0"
   checksum: 910d97fb7092c6738d30a7430ae4786a38542023c6302b95d46f49420b797f21619cdde11fa92b338366268795884111c2eb10356e4bd2c8ad5b92941e9e6443
@@ -3606,20 +3756,20 @@
   dependencies:
     "@types/istanbul-lib-report": "*"
   checksum: f1ad54bc68f37f60b30c7915886b92f86b847033e597f9b34f2415acdbe5ed742fa559a0a40050d74cdba3b6a63c342cac1f3a64dba5b68b66a6941f4abd7903
   languageName: node
   linkType: hard
 
 "@types/jest@npm:^29.2.0":
-  version: 29.4.0
-  resolution: "@types/jest@npm:29.4.0"
+  version: 29.5.0
+  resolution: "@types/jest@npm:29.5.0"
   dependencies:
     expect: ^29.0.0
     pretty-format: ^29.0.0
-  checksum: 23760282362a252e6690314584d83a47512d4cd61663e957ed3398ecf98195fe931c45606ee2f9def12f8ed7d8aa102d492ec42d26facdaf8b78094a31e6568e
+  checksum: cd877e5c56d299cceb8bfdcbb1a77723c706750dd3c3bc47403bc3599b8faff590a3b009c68bb5b11bf7a8c77d1fb01de5e124329b4a08e65f1cdda28b0ecdb8
   languageName: node
   linkType: hard
 
 "@types/jsdom@npm:^20.0.0":
   version: 20.0.1
   resolution: "@types/jsdom@npm:20.0.1"
   dependencies:
@@ -3648,17 +3798,17 @@
   version: 1.2.2
   resolution: "@types/minimist@npm:1.2.2"
   checksum: b8da83c66eb4aac0440e64674b19564d9d86c80ae273144db9681e5eeff66f238ade9515f5006ffbfa955ceff8b89ad2bd8ec577d7caee74ba101431fb07045d
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 18.14.0
-  resolution: "@types/node@npm:18.14.0"
-  checksum: d83fcf5e4ed544755dd9028f5cbb6b9d46235043159111bb2ad62223729aee581c0144a9f6df8ba73d74011db9ed4ebd7af2fd5e0996714e3beb508a5da8ac5c
+  version: 18.15.11
+  resolution: "@types/node@npm:18.15.11"
+  checksum: 977b4ad04708897ff0eb049ecf82246d210939c82461922d20f7d2dcfd81bbc661582ba3af28869210f7e8b1934529dcd46bff7d448551400f9d48b9d3bddec3
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.1
   resolution: "@types/normalize-package-data@npm:2.4.1"
   checksum: e87bccbf11f95035c89a132b52b79ce69a1e3652fe55962363063c9c0dae0fe2477ebc585e03a9652adc6f381d24ba5589cc5e51849df4ced3d3e004a7d40ed5
@@ -3683,28 +3833,28 @@
   version: 15.7.5
   resolution: "@types/prop-types@npm:15.7.5"
   checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26, @types/react@npm:^18.0.27":
-  version: 18.0.28
-  resolution: "@types/react@npm:18.0.28"
+  version: 18.0.31
+  resolution: "@types/react@npm:18.0.31"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: e752df961105e5127652460504785897ca6e77259e0da8f233f694f9e8f451cde7fa0709d4456ade0ff600c8ce909cfe29f9b08b9c247fa9b734e126ec53edd7
+  checksum: 6befbd5587e266905b50fd6bbd7c1cacd557bddf99e6a9862ca2f1d06df3dca71b9d485a37d010479730f021aab93b852d417c714de5efc2f41be0ff4c09b4db
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
-  version: 0.16.2
-  resolution: "@types/scheduler@npm:0.16.2"
-  checksum: b6b4dcfeae6deba2e06a70941860fb1435730576d3689225a421280b7742318d1548b3d22c1f66ab68e414f346a9542f29240bc955b6332c5b11e561077583bc
+  version: 0.16.3
+  resolution: "@types/scheduler@npm:0.16.3"
+  checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
   languageName: node
   linkType: hard
 
 "@types/semver@npm:^7.3.12":
   version: 7.3.13
   resolution: "@types/semver@npm:7.3.13"
   checksum: 00c0724d54757c2f4bc60b5032fe91cda6410e48689633d5f35ece8a0a66445e3e57fa1d6e07eb780f792e82ac542948ec4d0b76eb3484297b79bd18b8cf1cb0
@@ -3747,19 +3897,19 @@
   version: 21.0.0
   resolution: "@types/yargs-parser@npm:21.0.0"
   checksum: b2f4c8d12ac18a567440379909127cf2cec393daffb73f246d0a25df36ea983b93b7e9e824251f959e9f928cbc7c1aab6728d0a0ff15d6145f66cec2be67d9a2
   languageName: node
   linkType: hard
 
 "@types/yargs@npm:^17.0.8":
-  version: 17.0.22
-  resolution: "@types/yargs@npm:17.0.22"
+  version: 17.0.24
+  resolution: "@types/yargs@npm:17.0.24"
   dependencies:
     "@types/yargs-parser": "*"
-  checksum: 0773523fda71bafdc52f13f5970039e535a353665a60ba9261149a5c9c2b908242e6e77fbb7a8c06931ec78ce889d64d09673c68ba23eb5f5742d5385d0d1982
+  checksum: 5f3ac4dc4f6e211c1627340160fbe2fd247ceba002190da6cf9155af1798450501d628c9165a183f30a224fc68fa5e700490d740ff4c73e2cdef95bc4e8ba7bf
   languageName: node
   linkType: hard
 
 "@typescript-eslint/eslint-plugin@npm:~5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/eslint-plugin@npm:5.55.0"
   dependencies:
@@ -3806,14 +3956,24 @@
   dependencies:
     "@typescript-eslint/types": 5.55.0
     "@typescript-eslint/visitor-keys": 5.55.0
   checksum: f253db88f69a29e4abe2f567d0a611cc3e7fb1a911a2cc54a2f6baf16e3de4d1883b3f8e45ee61b3db9fa5543dda0fd7b608de9d28ba6173ab49bfd17ff90cad
   languageName: node
   linkType: hard
 
+"@typescript-eslint/scope-manager@npm:5.57.0":
+  version: 5.57.0
+  resolution: "@typescript-eslint/scope-manager@npm:5.57.0"
+  dependencies:
+    "@typescript-eslint/types": 5.57.0
+    "@typescript-eslint/visitor-keys": 5.57.0
+  checksum: 4a851f23da2adbf6341b04c1e3f19fcb66415683f26805d3123725d18845bd4a150bd182de0a91279d5682f2568bb5dd831d4ad0bdb70f49d9ca7381cec4dd17
+  languageName: node
+  linkType: hard
+
 "@typescript-eslint/type-utils@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/type-utils@npm:5.55.0"
   dependencies:
     "@typescript-eslint/typescript-estree": 5.55.0
     "@typescript-eslint/utils": 5.55.0
     debug: ^4.3.4
@@ -3830,14 +3990,21 @@
 "@typescript-eslint/types@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/types@npm:5.55.0"
   checksum: 7d851f09a2106514d3a9c7164d34758f30abfe554e3c7a02be75cdc7e16644e23ca32840a8f39a0321bc509927fb4d98ce91b22b21e8544ac56cef33b815a864
   languageName: node
   linkType: hard
 
+"@typescript-eslint/types@npm:5.57.0":
+  version: 5.57.0
+  resolution: "@typescript-eslint/types@npm:5.57.0"
+  checksum: 79a100fb650965f63c01c20e6abd79ca0d2043c3a329b9fef89917d6b9ba3c0f946dca3f14f2975ee6349daadd6ce0e98fde3aafe4b710e5a27abe1adc590c85
+  languageName: node
+  linkType: hard
+
 "@typescript-eslint/typescript-estree@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/typescript-estree@npm:5.55.0"
   dependencies:
     "@typescript-eslint/types": 5.55.0
     "@typescript-eslint/visitor-keys": 5.55.0
     debug: ^4.3.4
@@ -3848,15 +4015,33 @@
   peerDependenciesMeta:
     typescript:
       optional: true
   checksum: d24a11aee3d01067018d99804f420aecb8af88e43bf170d5d14f6480bd378c0a81ce49a37f5d6c36e5f0f319e3fa8b099720f295f2767338be1a4f7e9a5323e1
   languageName: node
   linkType: hard
 
-"@typescript-eslint/utils@npm:5.55.0, @typescript-eslint/utils@npm:^5.10.0":
+"@typescript-eslint/typescript-estree@npm:5.57.0":
+  version: 5.57.0
+  resolution: "@typescript-eslint/typescript-estree@npm:5.57.0"
+  dependencies:
+    "@typescript-eslint/types": 5.57.0
+    "@typescript-eslint/visitor-keys": 5.57.0
+    debug: ^4.3.4
+    globby: ^11.1.0
+    is-glob: ^4.0.3
+    semver: ^7.3.7
+    tsutils: ^3.21.0
+  peerDependenciesMeta:
+    typescript:
+      optional: true
+  checksum: 648b88f88ea6cc293ec67b4c0f4f3c2bf733be7e0f2eee08aadbaec6939fd724a6c287decc336abbf67b9e366cc2c48f2e0e48d8302b533e783f798332a06e83
+  languageName: node
+  linkType: hard
+
+"@typescript-eslint/utils@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/utils@npm:5.55.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@types/json-schema": ^7.0.9
     "@types/semver": ^7.3.12
     "@typescript-eslint/scope-manager": 5.55.0
@@ -3866,24 +4051,52 @@
     semver: ^7.3.7
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
   checksum: 368cfc3fb9d6af6901e739e2e41c3f7f1c1244576607445f4f59d95eccb237f73e1a75e7f0816ec9a32a0f1ec6bb4a3602a99e17e70fe184e62f7c69dcbe4b8d
   languageName: node
   linkType: hard
 
+"@typescript-eslint/utils@npm:^5.10.0":
+  version: 5.57.0
+  resolution: "@typescript-eslint/utils@npm:5.57.0"
+  dependencies:
+    "@eslint-community/eslint-utils": ^4.2.0
+    "@types/json-schema": ^7.0.9
+    "@types/semver": ^7.3.12
+    "@typescript-eslint/scope-manager": 5.57.0
+    "@typescript-eslint/types": 5.57.0
+    "@typescript-eslint/typescript-estree": 5.57.0
+    eslint-scope: ^5.1.1
+    semver: ^7.3.7
+  peerDependencies:
+    eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
+  checksum: 461258e1194d24c5e642c65ba1afd612712fa8e617ac85cfbbe3dde2557fe4abadedbce19a6954ae0cccbfb92b8a09f38d65a3eedca0394861a5d1c4c893c5ed
+  languageName: node
+  linkType: hard
+
 "@typescript-eslint/visitor-keys@npm:5.55.0":
   version: 5.55.0
   resolution: "@typescript-eslint/visitor-keys@npm:5.55.0"
   dependencies:
     "@typescript-eslint/types": 5.55.0
     eslint-visitor-keys: ^3.3.0
   checksum: 0b24c72dff99dd2cf41c19d20067f8ab20a38aa2e82c79c5530bec7cf651031e95c80702fc21c813c9b94e5f3d4cd210f13967b2966ef38abe548cb5f05848a3
   languageName: node
   linkType: hard
 
+"@typescript-eslint/visitor-keys@npm:5.57.0":
+  version: 5.57.0
+  resolution: "@typescript-eslint/visitor-keys@npm:5.57.0"
+  dependencies:
+    "@typescript-eslint/types": 5.57.0
+    eslint-visitor-keys: ^3.3.0
+  checksum: 77d53f74648e48bf1c6313cd60568c2b1539157ac13945f26204a54beb156666c24f3d033dd0db8ed5d1d4595ee63c072732b17132e4488b46763bf8fdcefa49
+  languageName: node
+  linkType: hard
+
 "@webassemblyjs/ast@npm:1.11.1":
   version: 1.11.1
   resolution: "@webassemblyjs/ast@npm:1.11.1"
   dependencies:
     "@webassemblyjs/helper-numbers": 1.11.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.1
   checksum: 1eee1534adebeece635362f8e834ae03e389281972611408d64be7895fc49f48f98fddbbb5339bf8a72cb101bcb066e8bca3ca1bf1ef47dadf89def0395a8d87
@@ -4082,20 +4295,20 @@
   version: 1.1.0
   resolution: "@yarnpkg/lockfile@npm:1.1.0"
   checksum: 05b881b4866a3546861fee756e6d3812776ea47fa6eb7098f983d6d0eefa02e12b66c3fff931574120f196286a7ad4879ce02743c8bb2be36c6a576c7852083a
   languageName: node
   linkType: hard
 
 "@yarnpkg/parsers@npm:^3.0.0-rc.18":
-  version: 3.0.0-rc.39
-  resolution: "@yarnpkg/parsers@npm:3.0.0-rc.39"
+  version: 3.0.0-rc.42
+  resolution: "@yarnpkg/parsers@npm:3.0.0-rc.42"
   dependencies:
     js-yaml: ^3.10.0
     tslib: ^2.4.0
-  checksum: b54fb3694bd09e09142d5a8d607240a8389ce3ccf44a70808ac770c178bb527948c3805a230b6fa55753f95574c93773a853a37ece978e323c9f2d229fd82252
+  checksum: 147216f53d683ac2b0b4a68e6cda77b7194d70db5ad3b0b6863129b6f1e36054de5cd5c707707fc36921e110d3ac1cb6a0f51fc9e8d74a4a4123ec3b93d3951e
   languageName: node
   linkType: hard
 
 "@zkochan/js-yaml@npm:0.0.6":
   version: 0.0.6
   resolution: "@zkochan/js-yaml@npm:0.0.6"
   dependencies:
@@ -4121,21 +4334,37 @@
 "abab@npm:^2.0.3, abab@npm:^2.0.6":
   version: 2.0.6
   resolution: "abab@npm:2.0.6"
   checksum: 6ffc1af4ff315066c62600123990d87551ceb0aafa01e6539da77b0f5987ac7019466780bf480f1787576d4385e3690c81ccc37cfda12819bf510b8ab47e5a3e
   languageName: node
   linkType: hard
 
-"abbrev@npm:1, abbrev@npm:^1.0.0":
+"abbrev@npm:^1.0.0":
   version: 1.1.1
   resolution: "abbrev@npm:1.1.1"
   checksum: a4a97ec07d7ea112c517036882b2ac22f3109b7b19077dc656316d07d308438aac28e4d9746dc4d84bf6b1e75b4a7b0a5f3cb30592419f128ca9a8cee3bcfa17
   languageName: node
   linkType: hard
 
+"abbrev@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "abbrev@npm:2.0.0"
+  checksum: 0e994ad2aa6575f94670d8a2149afe94465de9cedaaaac364e7fb43a40c3691c980ff74899f682f4ca58fa96b4cbd7421a015d3a6defe43a442117d7821a2f36
+  languageName: node
+  linkType: hard
+
+"abort-controller@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "abort-controller@npm:3.0.0"
+  dependencies:
+    event-target-shim: ^5.0.0
+  checksum: 170bdba9b47b7e65906a28c8ce4f38a7a369d78e2271706f020849c1bfe0ee2067d4261df8bbb66eb84f79208fd5b710df759d64191db58cfba7ce8ef9c54b75
+  languageName: node
+  linkType: hard
+
 "abstract-leveldown@npm:^6.2.1":
   version: 6.3.0
   resolution: "abstract-leveldown@npm:6.3.0"
   dependencies:
     buffer: ^5.5.0
     immediate: ^3.2.3
     level-concat-iterator: ~2.0.0
@@ -4215,21 +4444,21 @@
   dependencies:
     debug: 4
   checksum: f52b6872cc96fd5f622071b71ef200e01c7c4c454ee68bc9accca90c98cfb39f2810e3e9aa330435835eedc8c23f4f8a15267f67c6e245d2b33757575bdac49d
   languageName: node
   linkType: hard
 
 "agentkeepalive@npm:^4.2.1":
-  version: 4.2.1
-  resolution: "agentkeepalive@npm:4.2.1"
+  version: 4.3.0
+  resolution: "agentkeepalive@npm:4.3.0"
   dependencies:
     debug: ^4.1.0
-    depd: ^1.1.2
+    depd: ^2.0.0
     humanize-ms: ^1.2.1
-  checksum: 39cb49ed8cf217fd6da058a92828a0a84e0b74c35550f82ee0a10e1ee403c4b78ade7948be2279b188b7a7303f5d396ea2738b134731e464bf28de00a4f72a18
+  checksum: 982453aa44c11a06826c836025e5162c846e1200adb56f2d075400da7d32d87021b3b0a58768d949d824811f5654223d5a8a3dad120921a2439625eb847c6260
   languageName: node
   linkType: hard
 
 "aggregate-error@npm:^3.0.0":
   version: 3.1.0
   resolution: "aggregate-error@npm:3.1.0"
   dependencies:
@@ -4375,14 +4604,24 @@
   dependencies:
     delegates: ^1.0.0
     readable-stream: ^3.6.0
   checksum: 52590c24860fa7173bedeb69a4c05fb573473e860197f618b9a28432ee4379049336727ae3a1f9c4cb083114601c1140cee578376164d0e651217a9843f9fe83
   languageName: node
   linkType: hard
 
+"are-we-there-yet@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "are-we-there-yet@npm:4.0.0"
+  dependencies:
+    delegates: ^1.0.0
+    readable-stream: ^4.1.0
+  checksum: 35d6a65ce9a0c53d8d8eeef8805528c483c5c3512f2050b32c07e61becc440c4ec8178d6ee6cedc1e5a81b819eb55d9c0a9fc7d9f862cae4c7dc30ec393f0a58
+  languageName: node
+  linkType: hard
+
 "argparse@npm:^1.0.7":
   version: 1.0.10
   resolution: "argparse@npm:1.0.10"
   dependencies:
     sprintf-js: ~1.0.2
   checksum: 7ca6e45583a28de7258e39e13d81e925cfa25d7d4aacbf806a382d3c02fcb13403a07fb8aeef949f10a7cfe4a62da0e2e807b348a5980554cc28ee573ef95945
   languageName: node
@@ -4391,14 +4630,24 @@
 "argparse@npm:^2.0.1":
   version: 2.0.1
   resolution: "argparse@npm:2.0.1"
   checksum: 83644b56493e89a254bae05702abf3a1101b4fa4d0ca31df1c9985275a5a5bd47b3c27b7fa0b71098d41114d8ca000e6ed90cad764b306f8a503665e4d517ced
   languageName: node
   linkType: hard
 
+"array-buffer-byte-length@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "array-buffer-byte-length@npm:1.0.0"
+  dependencies:
+    call-bind: ^1.0.2
+    is-array-buffer: ^3.0.1
+  checksum: 044e101ce150f4804ad19c51d6c4d4cfa505c5b2577bd179256e4aa3f3f6a0a5e9874c78cd428ee566ac574c8a04d7ce21af9fe52e844abfdccb82b33035a7c3
+  languageName: node
+  linkType: hard
+
 "array-differ@npm:^3.0.0":
   version: 3.0.0
   resolution: "array-differ@npm:3.0.0"
   checksum: 117edd9df5c1530bd116c6e8eea891d4bd02850fd89b1b36e532b6540e47ca620a373b81feca1c62d1395d9ae601516ba538abe5e8172d41091da2c546b05fb7
   languageName: node
   linkType: hard
 
@@ -4464,21 +4713,14 @@
 "arrify@npm:^2.0.1":
   version: 2.0.1
   resolution: "arrify@npm:2.0.1"
   checksum: 067c4c1afd182806a82e4c1cb8acee16ab8b5284fbca1ce29408e6e91281c36bb5b612f6ddfbd40a0f7a7e0c75bf2696eb94c027f6e328d6e9c52465c98e4209
   languageName: node
   linkType: hard
 
-"asap@npm:^2.0.0":
-  version: 2.0.6
-  resolution: "asap@npm:2.0.6"
-  checksum: b296c92c4b969e973260e47523207cd5769abd27c245a68c26dc7a0fe8053c55bb04360237cb51cab1df52be939da77150ace99ad331fb7fb13b3423ed73ff3d
-  languageName: node
-  linkType: hard
-
 "astral-regex@npm:^2.0.0":
   version: 2.0.0
   resolution: "astral-regex@npm:2.0.0"
   checksum: 876231688c66400473ba505731df37ea436e574dd524520294cc3bbc54ea40334865e01fa0d074d74d036ee874ee7e62f486ea38bc421ee8e6a871c06f011766
   languageName: node
   linkType: hard
 
@@ -4514,38 +4756,38 @@
   version: 1.0.5
   resolution: "available-typed-arrays@npm:1.0.5"
   checksum: 20eb47b3cefd7db027b9bbb993c658abd36d4edd3fe1060e83699a03ee275b0c9b216cc076ff3f2db29073225fb70e7613987af14269ac1fe2a19803ccc97f1a
   languageName: node
   linkType: hard
 
 "axios@npm:^1.0.0":
-  version: 1.3.3
-  resolution: "axios@npm:1.3.3"
+  version: 1.3.4
+  resolution: "axios@npm:1.3.4"
   dependencies:
     follow-redirects: ^1.15.0
     form-data: ^4.0.0
     proxy-from-env: ^1.1.0
-  checksum: b734a4bc348e2fa27150a7d4289d783fa405feb3f79f8daf28fd05813a12c8525ae9d3854aafe7ba041b005a4a751a0ba3b923331ceed41296ae14c7e54e2f26
+  checksum: 7440edefcf8498bc3cdf39de00443e8101f249972c83b739c6e880d9d669fea9486372dbe8739e88b3bf8bb1ad15f6106693f206f078f4516fe8fd47b1c3093c
   languageName: node
   linkType: hard
 
-"babel-jest@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "babel-jest@npm:29.4.3"
+"babel-jest@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "babel-jest@npm:29.5.0"
   dependencies:
-    "@jest/transform": ^29.4.3
+    "@jest/transform": ^29.5.0
     "@types/babel__core": ^7.1.14
     babel-plugin-istanbul: ^6.1.1
-    babel-preset-jest: ^29.4.3
+    babel-preset-jest: ^29.5.0
     chalk: ^4.0.0
     graceful-fs: ^4.2.9
     slash: ^3.0.0
   peerDependencies:
     "@babel/core": ^7.8.0
-  checksum: a1a95937adb5e717dbffc2eb9e583fa6d26c7e5d5b07bb492a2d7f68631510a363e9ff097eafb642ad642dfac9dc2b13872b584f680e166a4f0922c98ea95853
+  checksum: eafb6d37deb71f0c80bf3c80215aa46732153e5e8bcd73f6ff47d92e5c0c98c8f7f75995d0efec6289c371edad3693cd8fa2367b0661c4deb71a3a7117267ede
   languageName: node
   linkType: hard
 
 "babel-plugin-istanbul@npm:^6.1.1":
   version: 6.1.1
   resolution: "babel-plugin-istanbul@npm:6.1.1"
   dependencies:
@@ -4554,23 +4796,23 @@
     "@istanbuljs/schema": ^0.1.2
     istanbul-lib-instrument: ^5.0.4
     test-exclude: ^6.0.0
   checksum: cb4fd95738219f232f0aece1116628cccff16db891713c4ccb501cddbbf9272951a5df81f2f2658dfdf4b3e7b236a9d5cbcf04d5d8c07dd5077297339598061a
   languageName: node
   linkType: hard
 
-"babel-plugin-jest-hoist@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "babel-plugin-jest-hoist@npm:29.4.3"
+"babel-plugin-jest-hoist@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "babel-plugin-jest-hoist@npm:29.5.0"
   dependencies:
     "@babel/template": ^7.3.3
     "@babel/types": ^7.3.3
     "@types/babel__core": ^7.1.14
     "@types/babel__traverse": ^7.0.6
-  checksum: c8702a6db6b30ec39dfb9f8e72b501c13895231ed80b15ed2648448f9f0c7b7cc4b1529beac31802ae655f63479a05110ca612815aa25fb1b0e6c874e1589137
+  checksum: 099b5254073b6bc985b6d2d045ad26fb8ed30ff8ae6404c4fe8ee7cd0e98a820f69e3dfb871c7c65aae0f4b65af77046244c07bb92d49ef9005c90eedf681539
   languageName: node
   linkType: hard
 
 "babel-plugin-polyfill-corejs2@npm:^0.3.3":
   version: 0.3.3
   resolution: "babel-plugin-polyfill-corejs2@npm:0.3.3"
   dependencies:
@@ -4624,23 +4866,23 @@
     "@babel/plugin-syntax-top-level-await": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: d118c2742498c5492c095bc8541f4076b253e705b5f1ad9a2e7d302d81a84866f0070346662355c8e25fc02caa28dc2da8d69bcd67794a0d60c4d6fab6913cc8
   languageName: node
   linkType: hard
 
-"babel-preset-jest@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "babel-preset-jest@npm:29.4.3"
+"babel-preset-jest@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "babel-preset-jest@npm:29.5.0"
   dependencies:
-    babel-plugin-jest-hoist: ^29.4.3
+    babel-plugin-jest-hoist: ^29.5.0
     babel-preset-current-node-syntax: ^1.0.0
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: a091721861ea2f8d969ace8fe06570cff8f2e847dbc6e4800abacbe63f72131abde615ce0a3b6648472c97e55a5be7f8bf7ae381e2b194ad2fa1737096febcf5
+  checksum: 5566ca2762766c9319b4973d018d2fa08c0fcf6415c72cc54f4c8e7199e851ea8f5e6c6730f03ed7ed44fc8beefa959dd15911f2647dee47c615ff4faeddb1ad
   languageName: node
   linkType: hard
 
 "balanced-match@npm:^1.0.0":
   version: 1.0.2
   resolution: "balanced-match@npm:1.0.2"
   checksum: 9706c088a283058a8a99e0bf91b0a2f75497f185980d9ffa8b304de1d9e58ebda7c72c07ebf01dadedaac5b2907b2c6f566f660d62bd336c3468e960403b9d65
@@ -4671,25 +4913,23 @@
 "big.js@npm:^5.2.2":
   version: 5.2.2
   resolution: "big.js@npm:5.2.2"
   checksum: b89b6e8419b097a8fb4ed2399a1931a68c612bce3cfd5ca8c214b2d017531191070f990598de2fc6f3f993d91c0f08aa82697717f6b3b8732c9731866d233c9e
   languageName: node
   linkType: hard
 
-"bin-links@npm:^3.0.0":
-  version: 3.0.3
-  resolution: "bin-links@npm:3.0.3"
+"bin-links@npm:^4.0.1":
+  version: 4.0.1
+  resolution: "bin-links@npm:4.0.1"
   dependencies:
-    cmd-shim: ^5.0.0
-    mkdirp-infer-owner: ^2.0.0
-    npm-normalize-package-bin: ^2.0.0
-    read-cmd-shim: ^3.0.0
-    rimraf: ^3.0.0
-    write-file-atomic: ^4.0.0
-  checksum: ea2dc6f91a6ef8b3840ceb48530bbeb8d6d1c6f7985fe1409b16d7e7db39432f0cb5ce15cc2788bb86d989abad6e2c7fba3500996a210a682eec18fb26a66e72
+    cmd-shim: ^6.0.0
+    npm-normalize-package-bin: ^3.0.0
+    read-cmd-shim: ^4.0.0
+    write-file-atomic: ^5.0.0
+  checksum: a806561750039bcd7d4234efe5c0b8b7ba0ea8495086740b0da6395abe311e2cdb75f8324787354193f652d2ac5ab038c4ca926ed7bcc6ce9bc2001607741104
   languageName: node
   linkType: hard
 
 "bl@npm:^4.0.3, bl@npm:^4.1.0":
   version: 4.1.0
   resolution: "bl@npm:4.1.0"
   dependencies:
@@ -4773,14 +5013,24 @@
   dependencies:
     base64-js: ^1.3.1
     ieee754: ^1.1.13
   checksum: e2cf8429e1c4c7b8cbd30834ac09bd61da46ce35f5c22a78e6c2f04497d6d25541b16881e30a019c6fd3154150650ccee27a308eff3e26229d788bbdeb08ab84
   languageName: node
   linkType: hard
 
+"buffer@npm:^6.0.3":
+  version: 6.0.3
+  resolution: "buffer@npm:6.0.3"
+  dependencies:
+    base64-js: ^1.3.1
+    ieee754: ^1.2.1
+  checksum: 5ad23293d9a731e4318e420025800b42bf0d264004c0286c8cc010af7a270c7a0f6522e84f54b9ad65cbd6db20b8badbfd8d2ebf4f80fa03dab093b89e68c3f9
+  languageName: node
+  linkType: hard
+
 "builtins@npm:^1.0.3":
   version: 1.0.3
   resolution: "builtins@npm:1.0.3"
   checksum: 47ce94f7eee0e644969da1f1a28e5f29bd2e48b25b2bbb61164c345881086e29464ccb1fb88dbc155ea26e8b1f5fc8a923b26c8c1ed0935b67b644d410674513
   languageName: node
   linkType: hard
 
@@ -4796,15 +5046,15 @@
 "byte-size@npm:7.0.0":
   version: 7.0.0
   resolution: "byte-size@npm:7.0.0"
   checksum: 6cdd45fb64ac3f80d5cbbc01df7974a4613b3e64bd792b6b8211c8669ca3d1f7efd9379ba24cebfc371ce3e890817dcdaf0bd7ed99571fe2de4b946e6c31a138
   languageName: node
   linkType: hard
 
-"cacache@npm:^16.0.0, cacache@npm:^16.0.6, cacache@npm:^16.1.0":
+"cacache@npm:^16.0.0, cacache@npm:^16.1.0":
   version: 16.1.3
   resolution: "cacache@npm:16.1.3"
   dependencies:
     "@npmcli/fs": ^2.1.0
     "@npmcli/move-file": ^2.0.0
     chownr: ^2.0.0
     fs-minipass: ^2.1.0
@@ -4822,14 +5072,35 @@
     ssri: ^9.0.0
     tar: ^6.1.11
     unique-filename: ^2.0.0
   checksum: d91409e6e57d7d9a3a25e5dcc589c84e75b178ae8ea7de05cbf6b783f77a5fae938f6e8fda6f5257ed70000be27a681e1e44829251bfffe4c10216002f8f14e6
   languageName: node
   linkType: hard
 
+"cacache@npm:^17.0.0, cacache@npm:^17.0.4":
+  version: 17.0.5
+  resolution: "cacache@npm:17.0.5"
+  dependencies:
+    "@npmcli/fs": ^3.1.0
+    fs-minipass: ^3.0.0
+    glob: ^9.3.1
+    lru-cache: ^7.7.1
+    minipass: ^4.0.0
+    minipass-collect: ^1.0.2
+    minipass-flush: ^1.0.5
+    minipass-pipeline: ^1.2.4
+    p-map: ^4.0.0
+    promise-inflight: ^1.0.1
+    ssri: ^10.0.0
+    tar: ^6.1.11
+    unique-filename: ^3.0.0
+  checksum: 83312d74acf4d17e378fc1f09ace1dedcb0a1b1033a0e9e22246052b8715cda7bdc8b7ab6dcadd3cb3f2965266def476835488cad5aea810159d452749757fbd
+  languageName: node
+  linkType: hard
+
 "call-bind@npm:^1.0.0, call-bind@npm:^1.0.2":
   version: 1.0.2
   resolution: "call-bind@npm:1.0.2"
   dependencies:
     function-bind: ^1.1.1
     get-intrinsic: ^1.0.2
   checksum: f8e31de9d19988a4b80f3e704788c4a2d6b6f3d17cfec4f57dc29ced450c53a49270dc66bf0fbd693329ee948dd33e6c90a329519aef17474a4d961e8d6426b0
@@ -4865,17 +5136,17 @@
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001449":
-  version: 1.0.30001457
-  resolution: "caniuse-lite@npm:1.0.30001457"
-  checksum: f311a7c5098681962402a86a0a367014ee91c3135395ee68bbfaf45caf0e36d581e42d7c5b1526ce99484a228e6cf5cf0e400678292c65f5a21512a3fc7a5fb6
+  version: 1.0.30001473
+  resolution: "caniuse-lite@npm:1.0.30001473"
+  checksum: 007ad17463612d38080fc59b5fa115ccb1016a1aff8daab92199a7cf8eb91cf987e85e7015cb0bca830ee2ef45f252a016c29a98a6497b334cceb038526b73f1
   languageName: node
   linkType: hard
 
 "chalk@npm:4.1.0":
   version: 4.1.0
   resolution: "chalk@npm:4.1.0"
   dependencies:
@@ -5035,23 +5306,30 @@
 "clone@npm:^1.0.2":
   version: 1.0.4
   resolution: "clone@npm:1.0.4"
   checksum: d06418b7335897209e77bdd430d04f882189582e67bd1f75a04565f3f07f5b3f119a9d670c943b6697d0afb100f03b866b3b8a1f91d4d02d72c4ecf2bb64b5dd
   languageName: node
   linkType: hard
 
-"cmd-shim@npm:5.0.0, cmd-shim@npm:^5.0.0":
+"cmd-shim@npm:5.0.0":
   version: 5.0.0
   resolution: "cmd-shim@npm:5.0.0"
   dependencies:
     mkdirp-infer-owner: ^2.0.0
   checksum: 83d2a46cdf4adbb38d3d3184364b2df0e4c001ac770f5ca94373825d7a48838b4cb8a59534ef48f02b0d556caa047728589ca65c640c17c0b417b3afb34acfbb
   languageName: node
   linkType: hard
 
+"cmd-shim@npm:^6.0.0":
+  version: 6.0.1
+  resolution: "cmd-shim@npm:6.0.1"
+  checksum: 359006b3a5bb4a0ff161a44ccc18fbba947db748ef0dd12273e476792e316a5edb0945d74bfa1e91cd88ce0511025fde87901eda092c479d83cfcd6734562683
+  languageName: node
+  linkType: hard
+
 "co@npm:^4.6.0":
   version: 4.6.0
   resolution: "co@npm:4.6.0"
   checksum: 5210d9223010eb95b29df06a91116f2cf7c8e0748a9013ed853b53f362ea0e822f1e5bb054fb3cefc645239a4cf966af1f6133a3b43f40d591f3b68ed6cf0510
   languageName: node
   linkType: hard
 
@@ -5339,19 +5617,19 @@
   version: 2.0.0
   resolution: "convert-source-map@npm:2.0.0"
   checksum: 63ae9933be5a2b8d4509daca5124e20c14d023c820258e484e32dc324d34c2754e71297c94a05784064ad27615037ef677e3f0c00469fb55f409d2bb21261035
   languageName: node
   linkType: hard
 
 "core-js-compat@npm:^3.25.1":
-  version: 3.28.0
-  resolution: "core-js-compat@npm:3.28.0"
+  version: 3.29.1
+  resolution: "core-js-compat@npm:3.29.1"
   dependencies:
     browserslist: ^4.21.5
-  checksum: 41d1d58c99ce7ee7abd8cf070f4c07a8f2655dbed1777d90a26246dddd7fac68315d53d2192584c8621a5328e6fe1a10da39b6bf2666e90fd5c2ff3b8f24e874
+  checksum: 7260f6bbaa98836cda09a3b61aa721149d3ae95040302fb3b27eb153ae9bbddc8dee5249e72004cdc9552532029de4d50a5b2b066c37414421d2929d6091b18f
   languageName: node
   linkType: hard
 
 "core-util-is@npm:~1.0.0":
   version: 1.0.3
   resolution: "core-util-is@npm:1.0.3"
   checksum: 9de8597363a8e9b9952491ebe18167e3b36e7707569eed0ebf14f8bba773611376466ae34575bca8cfe3c767890c859c74056084738f09d4e4a6f902b2ad7d99
@@ -5367,23 +5645,23 @@
     parse-json: ^5.0.0
     path-type: ^4.0.0
     yaml: ^1.10.0
   checksum: 6801feaa0249e9b9fdde5b3d70dc33b4f9c69095bec94d67e3fe08b66eac24dc7e2099f053597cfbc94b743de269aa5d2cfa7da3fde765433423b06bd122941a
   languageName: node
   linkType: hard
 
-"cosmiconfig@npm:^8.0.0":
-  version: 8.0.0
-  resolution: "cosmiconfig@npm:8.0.0"
+"cosmiconfig@npm:^8.1.0":
+  version: 8.1.3
+  resolution: "cosmiconfig@npm:8.1.3"
   dependencies:
     import-fresh: ^3.2.1
     js-yaml: ^4.1.0
     parse-json: ^5.0.0
     path-type: ^4.0.0
-  checksum: ff4cdf89ac1ae52e7520816622c21a9e04380d04b82d653f5139ec581aa4f7f29e096d46770bc76c4a63c225367e88a1dfa233ea791669a35101f5f9b972c7d1
+  checksum: b3d277bc3a8a9e649bf4c3fc9740f4c52bf07387481302aa79839f595045368903bf26ea24a8f7f7b8b180bf46037b027c5cb63b1391ab099f3f78814a147b2b
   languageName: node
   linkType: hard
 
 "crelt@npm:^1.0.5":
   version: 1.0.5
   resolution: "crelt@npm:1.0.5"
   checksum: 04a618c5878e12a14a9a328a49ff6e37bed76abb88b72e661c56b5f161d8a9aca133650da6bcbc5224ad1f7f43a69325627f209e92a21002986d52a8f844b367
@@ -5410,14 +5688,21 @@
     path-key: ^3.1.0
     shebang-command: ^2.0.0
     which: ^2.0.1
   checksum: 671cc7c7288c3a8406f3c69a3ae2fc85555c04169e9d611def9a675635472614f1c0ed0ef80955d5b6d4e724f6ced67f0ad1bb006c2ea643488fcfef994d7f52
   languageName: node
   linkType: hard
 
+"crypto-random-string@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "crypto-random-string@npm:2.0.0"
+  checksum: 0283879f55e7c16fdceacc181f87a0a65c53bc16ffe1d58b9d19a6277adcd71900d02bb2c4843dd55e78c51e30e89b0fec618a7f170ebcc95b33182c28f05fd6
+  languageName: node
+  linkType: hard
+
 "css-functions-list@npm:^3.1.0":
   version: 3.1.0
   resolution: "css-functions-list@npm:3.1.0"
   checksum: 8a7c9d4ae57cb2f01500263e65a21372048d359ca7aa6430a32a736fe2a421decfebe45e579124b9a158ec68aba2eadcd733e568495a7698240d9607d31f681b
   languageName: node
   linkType: hard
 
@@ -5539,21 +5824,14 @@
   peerDependenciesMeta:
     supports-color:
       optional: true
   checksum: 3dbad3f94ea64f34431a9cbf0bafb61853eda57bff2880036153438f50fb5a84f27683ba0d8e5426bf41a8c6ff03879488120cf5b3a761e77953169c0600a708
   languageName: node
   linkType: hard
 
-"debuglog@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "debuglog@npm:1.0.1"
-  checksum: 970679f2eb7a73867e04d45b52583e7ec6dee1f33c058e9147702e72a665a9647f9c3d6e7c2f66f6bf18510b23eb5ded1b617e48ac1db23603809c5ddbbb9763
-  languageName: node
-  linkType: hard
-
 "decamelize-keys@npm:^1.1.0":
   version: 1.1.1
   resolution: "decamelize-keys@npm:1.1.1"
   dependencies:
     decamelize: ^1.1.0
     map-obj: ^1.0.0
   checksum: fc645fe20b7bda2680bbf9481a3477257a7f9304b1691036092b97ab04c0ab53e3bf9fcc2d2ae382536568e402ec41fb11e1d4c3836a9abe2d813dd9ef4311e0
@@ -5585,17 +5863,17 @@
   version: 0.1.4
   resolution: "deep-is@npm:0.1.4"
   checksum: edb65dd0d7d1b9c40b2f50219aef30e116cedd6fc79290e740972c132c09106d2e80aa0bc8826673dd5a00222d4179c84b36a790eef63a4c4bca75a37ef90804
   languageName: node
   linkType: hard
 
 "deepmerge@npm:^4.2.2":
-  version: 4.3.0
-  resolution: "deepmerge@npm:4.3.0"
-  checksum: c7980eb5c5be040b371f1df0d566473875cfabed9f672ccc177b81ba8eee5686ce2478de2f1d0076391621cbe729e5eacda397179a59ef0f68901849647db126
+  version: 4.3.1
+  resolution: "deepmerge@npm:4.3.1"
+  checksum: 2024c6a980a1b7128084170c4cf56b0fd58a63f2da1660dcfe977415f27b17dbe5888668b59d0b063753f3220719d5e400b7f113609489c90160bb9a5518d052
   languageName: node
   linkType: hard
 
 "defaults@npm:^1.0.3":
   version: 1.0.4
   resolution: "defaults@npm:1.0.4"
   dependencies:
@@ -5627,32 +5905,48 @@
   dependencies:
     has-property-descriptors: ^1.0.0
     object-keys: ^1.1.1
   checksum: e60aee6a19b102df4e2b1f301816804e81ab48bb91f00d0d935f269bf4b3f79c88b39e4f89eaa132890d23267335fd1140dfcd8d5ccd61031a0a2c41a54e33a6
   languageName: node
   linkType: hard
 
+"del@npm:^6.0.0":
+  version: 6.1.1
+  resolution: "del@npm:6.1.1"
+  dependencies:
+    globby: ^11.0.1
+    graceful-fs: ^4.2.4
+    is-glob: ^4.0.1
+    is-path-cwd: ^2.2.0
+    is-path-inside: ^3.0.2
+    p-map: ^4.0.0
+    rimraf: ^3.0.2
+    slash: ^3.0.0
+  checksum: 563288b73b8b19a7261c47fd21a330eeab6e2acd7c6208c49790dfd369127120dd7836cdf0c1eca216b77c94782a81507eac6b4734252d3bef2795cb366996b6
+  languageName: node
+  linkType: hard
+
 "delayed-stream@npm:~1.0.0":
   version: 1.0.0
   resolution: "delayed-stream@npm:1.0.0"
   checksum: 46fe6e83e2cb1d85ba50bd52803c68be9bd953282fa7096f51fc29edd5d67ff84ff753c51966061e5ba7cb5e47ef6d36a91924eddb7f3f3483b1c560f77a0020
   languageName: node
   linkType: hard
 
 "delegates@npm:^1.0.0":
   version: 1.0.0
   resolution: "delegates@npm:1.0.0"
   checksum: a51744d9b53c164ba9c0492471a1a2ffa0b6727451bdc89e31627fdf4adda9d51277cfcbfb20f0a6f08ccb3c436f341df3e92631a3440226d93a8971724771fd
   languageName: node
   linkType: hard
 
-"depd@npm:^1.1.2":
-  version: 1.1.2
-  resolution: "depd@npm:1.1.2"
-  checksum: 6b406620d269619852885ce15965272b829df6f409724415e0002c8632ab6a8c0a08ec1f0bd2add05dc7bd7507606f7e2cc034fa24224ab829580040b835ecd9
+"depd@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "depd@npm:2.0.0"
+  checksum: abbe19c768c97ee2eed6282d8ce3031126662252c58d711f646921c9623f9052e3e1906443066beec1095832f534e57c523b7333f8e7e0d93051ab6baef5ab3a
   languageName: node
   linkType: hard
 
 "deprecation@npm:^2.0.0, deprecation@npm:^2.3.1":
   version: 2.3.1
   resolution: "deprecation@npm:2.3.1"
   checksum: f56a05e182c2c195071385455956b0c4106fe14e36245b00c689ceef8e8ab639235176a96977ba7c74afb173317fac2e0ec6ec7a1c6d1e6eaa401c586c714132
@@ -5669,24 +5963,14 @@
 "detect-newline@npm:^3.0.0":
   version: 3.1.0
   resolution: "detect-newline@npm:3.1.0"
   checksum: ae6cd429c41ad01b164c59ea36f264a2c479598e61cba7c99da24175a7ab80ddf066420f2bec9a1c57a6bead411b4655ff15ad7d281c000a89791f48cbe939e7
   languageName: node
   linkType: hard
 
-"dezalgo@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "dezalgo@npm:1.0.4"
-  dependencies:
-    asap: ^2.0.0
-    wrappy: 1
-  checksum: 895389c6aead740d2ab5da4d3466d20fa30f738010a4d3f4dcccc9fc645ca31c9d10b7e1804ae489b1eb02c7986f9f1f34ba132d409b043082a86d9a4e745624
-  languageName: node
-  linkType: hard
-
 "diff-sequences@npm:^29.4.3":
   version: 29.4.3
   resolution: "diff-sequences@npm:29.4.3"
   checksum: 28b265e04fdddcf7f9f814effe102cc95a9dec0564a579b5aed140edb24fc345c611ca52d76d725a3cab55d3888b915b5e8a4702e0f6058968a90fa5f41fcde7
   languageName: node
   linkType: hard
 
@@ -5805,28 +6089,28 @@
     lodash: ^4.17.4
     semver: ^5.4.1
   checksum: d77be45cb72d79a429c64d8f8f7603fea681d182fb795459a3d4afa608faad9a923378a7e80c6855f465263e1983140b6fc3682bd0213228b8cd7906ab4b934d
   languageName: node
   linkType: hard
 
 "ejs@npm:^3.1.7":
-  version: 3.1.8
-  resolution: "ejs@npm:3.1.8"
+  version: 3.1.9
+  resolution: "ejs@npm:3.1.9"
   dependencies:
     jake: ^10.8.5
   bin:
     ejs: bin/cli.js
-  checksum: 1d40d198ad52e315ccf37e577bdec06e24eefdc4e3c27aafa47751a03a0c7f0ec4310254c9277a5f14763c3cd4bbacce27497332b2d87c74232b9b1defef8efc
+  checksum: af6f10eb815885ff8a8cfacc42c6b6cf87daf97a4884f87a30e0c3271fedd85d76a3a297d9c33a70e735b97ee632887f85e32854b9cdd3a2d97edf931519a35f
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.284":
-  version: 1.4.302
-  resolution: "electron-to-chromium@npm:1.4.302"
-  checksum: aa764494f9a5b6916ba9f311c0204b2c73449addba18cc55d43e84e8c4465732af9cd6560a8efeb32f3c5a928299030e41352e5b3a081e9e56b086d5be618f45
+  version: 1.4.345
+  resolution: "electron-to-chromium@npm:1.4.345"
+  checksum: 4561a09c1259c04ecb0c6f0c9000b12c562a1a06dfd89858bf2388d3d6083d41a12a7ca5a425cae9b12fa2de2ccddf2dd0ba43fb26600ab66cec26d48a8c19b0
   languageName: node
   linkType: hard
 
 "emittery@npm:^0.13.1":
   version: 0.13.1
   resolution: "emittery@npm:0.13.1"
   checksum: 2b089ab6306f38feaabf4f6f02792f9ec85fc054fda79f44f6790e61bbf6bc4e1616afb9b232e0c5ec5289a8a452f79bfa6d905a6fd64e94b49981f0934001c6
@@ -5950,51 +6234,52 @@
   dependencies:
     is-arrayish: ^0.2.1
   checksum: c1c2b8b65f9c91b0f9d75f0debaa7ec5b35c266c2cac5de412c1a6de86d4cbae04ae44e510378cb14d032d0645a36925d0186f8bb7367bcc629db256b743a001
   languageName: node
   linkType: hard
 
 "es-abstract@npm:^1.19.0, es-abstract@npm:^1.20.4":
-  version: 1.21.1
-  resolution: "es-abstract@npm:1.21.1"
+  version: 1.21.2
+  resolution: "es-abstract@npm:1.21.2"
   dependencies:
+    array-buffer-byte-length: ^1.0.0
     available-typed-arrays: ^1.0.5
     call-bind: ^1.0.2
     es-set-tostringtag: ^2.0.1
     es-to-primitive: ^1.2.1
-    function-bind: ^1.1.1
     function.prototype.name: ^1.1.5
-    get-intrinsic: ^1.1.3
+    get-intrinsic: ^1.2.0
     get-symbol-description: ^1.0.0
     globalthis: ^1.0.3
     gopd: ^1.0.1
     has: ^1.0.3
     has-property-descriptors: ^1.0.0
     has-proto: ^1.0.1
     has-symbols: ^1.0.3
-    internal-slot: ^1.0.4
-    is-array-buffer: ^3.0.1
+    internal-slot: ^1.0.5
+    is-array-buffer: ^3.0.2
     is-callable: ^1.2.7
     is-negative-zero: ^2.0.2
     is-regex: ^1.1.4
     is-shared-array-buffer: ^1.0.2
     is-string: ^1.0.7
     is-typed-array: ^1.1.10
     is-weakref: ^1.0.2
-    object-inspect: ^1.12.2
+    object-inspect: ^1.12.3
     object-keys: ^1.1.1
     object.assign: ^4.1.4
     regexp.prototype.flags: ^1.4.3
     safe-regex-test: ^1.0.0
+    string.prototype.trim: ^1.2.7
     string.prototype.trimend: ^1.0.6
     string.prototype.trimstart: ^1.0.6
     typed-array-length: ^1.0.4
     unbox-primitive: ^1.0.2
     which-typed-array: ^1.1.9
-  checksum: 23ff60d42d17a55d150e7bcedbdb065d4077a8b98c436e0e2e1ef4dd532a6d78a56028673de0bd8ed464a43c46ba781c50d9af429b6a17e44dbd14c7d7fb7926
+  checksum: 037f55ee5e1cdf2e5edbab5524095a4f97144d95b94ea29e3611b77d852fd8c8a40e7ae7101fa6a759a9b9b1405f188c3c70928f2d3cd88d543a07fc0d5ad41a
   languageName: node
   linkType: hard
 
 "es-module-lexer@npm:^0.9.0":
   version: 0.9.3
   resolution: "es-module-lexer@npm:0.9.3"
   checksum: 84bbab23c396281db2c906c766af58b1ae2a1a2599844a504df10b9e8dc77ec800b3211fdaa133ff700f5703d791198807bba25d9667392d27a5e9feda344da8
@@ -6163,18 +6448,18 @@
   dependencies:
     esrecurse: ^4.3.0
     estraverse: ^5.2.0
   checksum: 9f6e974ab2db641ca8ab13508c405b7b859e72afe9f254e8131ff154d2f40c99ad4545ce326fd9fde3212ff29707102562a4834f1c48617b35d98c71a97fbf3e
   languageName: node
   linkType: hard
 
-"eslint-visitor-keys@npm:^3.3.0":
-  version: 3.3.0
-  resolution: "eslint-visitor-keys@npm:3.3.0"
-  checksum: d59e68a7c5a6d0146526b0eec16ce87fbf97fe46b8281e0d41384224375c4e52f5ffb9e16d48f4ea50785cde93f766b0c898e31ab89978d88b0e1720fbfb7808
+"eslint-visitor-keys@npm:^3.3.0, eslint-visitor-keys@npm:^3.4.0":
+  version: 3.4.0
+  resolution: "eslint-visitor-keys@npm:3.4.0"
+  checksum: 33159169462d3989321a1ec1e9aaaf6a24cc403d5d347e9886d1b5bfe18ffa1be73bdc6203143a28a606b142b1af49787f33cff0d6d0813eb5f2e8d2e1a6043c
   languageName: node
   linkType: hard
 
 "eslint@npm:~8.36.0":
   version: 8.36.0
   resolution: "eslint@npm:8.36.0"
   dependencies:
@@ -6220,45 +6505,36 @@
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
   checksum: e9a961fc3b3de5cff5a1cb2c92eeffaa7e155a715489e30b3e1e76f186bd1255e0481e09564f2094733c0b1dbd3453499fb72ae7c043c83156e11e6d965b2304
   languageName: node
   linkType: hard
 
-"espree@npm:^9.5.0":
-  version: 9.5.0
-  resolution: "espree@npm:9.5.0"
+"espree@npm:^9.5.0, espree@npm:^9.5.1":
+  version: 9.5.1
+  resolution: "espree@npm:9.5.1"
   dependencies:
     acorn: ^8.8.0
     acorn-jsx: ^5.3.2
-    eslint-visitor-keys: ^3.3.0
-  checksum: a7f110aefb6407e0d3237aa635ab3cea87106ae63748dd23c67031afccc640d04c4209fca2daf16e2233c82efb505faead0fb84097478fd9cc6e8f8dd80bf99d
+    eslint-visitor-keys: ^3.4.0
+  checksum: cdf6e43540433d917c4f2ee087c6e987b2063baa85a1d9cdaf51533d78275ebd5910c42154e7baf8e3e89804b386da0a2f7fad2264d8f04420e7506bf87b3b88
   languageName: node
   linkType: hard
 
 "esprima@npm:^4.0.0, esprima@npm:^4.0.1":
   version: 4.0.1
   resolution: "esprima@npm:4.0.1"
   bin:
     esparse: ./bin/esparse.js
     esvalidate: ./bin/esvalidate.js
   checksum: b45bc805a613dbea2835278c306b91aff6173c8d034223fa81498c77dcbce3b2931bf6006db816f62eacd9fd4ea975dfd85a5b7f3c6402cfd050d4ca3c13a628
   languageName: node
   linkType: hard
 
-"esquery@npm:^1.0.1":
-  version: 1.4.2
-  resolution: "esquery@npm:1.4.2"
-  dependencies:
-    estraverse: ^5.1.0
-  checksum: 2f4ad89c5aafaca61cc2c15e256190f0d6deb4791cae6552d3cb4b1eb8867958cdf27a56aaa3272ff17435e3eaa19ee0d4129fac336ca6373d7354d7b5da7966
-  languageName: node
-  linkType: hard
-
-"esquery@npm:^1.4.2":
+"esquery@npm:^1.0.1, esquery@npm:^1.4.2":
   version: 1.5.0
   resolution: "esquery@npm:1.5.0"
   dependencies:
     estraverse: ^5.1.0
   checksum: aefb0d2596c230118656cd4ec7532d447333a410a48834d80ea648b1e7b5c9bc9ed8b5e33a89cb04e487b60d622f44cf5713bf4abed7c97343edefdc84a35900
   languageName: node
   linkType: hard
@@ -6289,22 +6565,29 @@
 "esutils@npm:^2.0.2":
   version: 2.0.3
   resolution: "esutils@npm:2.0.3"
   checksum: 22b5b08f74737379a840b8ed2036a5fb35826c709ab000683b092d9054e5c2a82c27818f12604bfc2a9a76b90b6834ef081edbc1c7ae30d1627012e067c6ec87
   languageName: node
   linkType: hard
 
+"event-target-shim@npm:^5.0.0":
+  version: 5.0.1
+  resolution: "event-target-shim@npm:5.0.1"
+  checksum: 1ffe3bb22a6d51bdeb6bf6f7cf97d2ff4a74b017ad12284cc9e6a279e727dc30a5de6bb613e5596ff4dc3e517841339ad09a7eec44266eccb1aa201a30448166
+  languageName: node
+  linkType: hard
+
 "eventemitter3@npm:^4.0.4":
   version: 4.0.7
   resolution: "eventemitter3@npm:4.0.7"
   checksum: 1875311c42fcfe9c707b2712c32664a245629b42bb0a5a84439762dd0fd637fc54d078155ea83c2af9e0323c9ac13687e03cfba79b03af9f40c89b4960099374
   languageName: node
   linkType: hard
 
-"events@npm:^3.2.0":
+"events@npm:^3.2.0, events@npm:^3.3.0":
   version: 3.3.0
   resolution: "events@npm:3.3.0"
   checksum: f6f487ad2198aa41d878fa31452f1a3c00958f46e9019286ff4787c84aac329332ab45c9cdc8c445928fc6d7ded294b9e005a7fce9426488518017831b272780
   languageName: node
   linkType: hard
 
 "execa@npm:5.0.0":
@@ -6344,24 +6627,24 @@
 "exit@npm:^0.1.2":
   version: 0.1.2
   resolution: "exit@npm:0.1.2"
   checksum: abc407f07a875c3961e4781dfcb743b58d6c93de9ab263f4f8c9d23bb6da5f9b7764fc773f86b43dd88030444d5ab8abcb611cb680fba8ca075362b77114bba3
   languageName: node
   linkType: hard
 
-"expect@npm:^29.0.0, expect@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "expect@npm:29.4.3"
+"expect@npm:^29.0.0, expect@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "expect@npm:29.5.0"
   dependencies:
-    "@jest/expect-utils": ^29.4.3
+    "@jest/expect-utils": ^29.5.0
     jest-get-type: ^29.4.3
-    jest-matcher-utils: ^29.4.3
-    jest-message-util: ^29.4.3
-    jest-util: ^29.4.3
-  checksum: ff9dd8c50c0c6fd4b2b00f6dbd7ab0e2063fe1953be81a8c10ae1c005c7f5667ba452918e2efb055504b72b701a4f82575a081a0a7158efb16d87991b0366feb
+    jest-matcher-utils: ^29.5.0
+    jest-message-util: ^29.5.0
+    jest-util: ^29.5.0
+  checksum: 58f70b38693df6e5c6892db1bcd050f0e518d6f785175dc53917d4fa6a7359a048e5690e19ddcb96b65c4493881dd89a3dabdab1a84dfa55c10cdbdabf37b2d7
   languageName: node
   linkType: hard
 
 "external-editor@npm:^3.0.3":
   version: 3.1.0
   resolution: "external-editor@npm:3.1.0"
   dependencies:
@@ -6465,14 +6748,21 @@
   resolution: "file-entry-cache@npm:6.0.1"
   dependencies:
     flat-cache: ^3.0.4
   checksum: f49701feaa6314c8127c3c2f6173cfefff17612f5ed2daaafc6da13b5c91fd43e3b2a58fd0d63f9f94478a501b167615931e7200e31485e320f74a33885a9c74
   languageName: node
   linkType: hard
 
+"file-url@npm:3.0.0":
+  version: 3.0.0
+  resolution: "file-url@npm:3.0.0"
+  checksum: 4724f669ee22468f23a39e37b8349a14f94dd9abda8385920db9900a2b2ae5ad90a314d85ea0089b6f45e9d0850833a6d1e41ac15a81a5618685129c6d7c7629
+  languageName: node
+  linkType: hard
+
 "filelist@npm:^1.0.1":
   version: 1.0.4
   resolution: "filelist@npm:1.0.4"
   dependencies:
     minimatch: ^5.0.1
   checksum: a303573b0821e17f2d5e9783688ab6fbfce5d52aaac842790ae85e704a6f5e4e3538660a63183d6453834dedf1e0f19a9dadcebfa3e926c72397694ea11f5160
   languageName: node
@@ -6490,14 +6780,24 @@
 "find-root@npm:^1.0.0":
   version: 1.1.0
   resolution: "find-root@npm:1.1.0"
   checksum: b2a59fe4b6c932eef36c45a048ae8f93c85640212ebe8363164814990ee20f154197505965f3f4f102efc33bfb1cbc26fd17c4a2fc739ebc51b886b137cbefaf
   languageName: node
   linkType: hard
 
+"find-up@npm:5.0.0, find-up@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "find-up@npm:5.0.0"
+  dependencies:
+    locate-path: ^6.0.0
+    path-exists: ^4.0.0
+  checksum: 07955e357348f34660bde7920783204ff5a26ac2cafcaa28bace494027158a97b9f56faaf2d89a6106211a8174db650dd9f503f9c0d526b1202d5554a00b9095
+  languageName: node
+  linkType: hard
+
 "find-up@npm:^2.0.0":
   version: 2.1.0
   resolution: "find-up@npm:2.1.0"
   dependencies:
     locate-path: ^2.0.0
   checksum: 43284fe4da09f89011f08e3c32cd38401e786b19226ea440b75386c1b12a4cb738c94969808d53a84f564ede22f732c8409e3cfc3f7fb5b5c32378ad0bbf28bd
   languageName: node
@@ -6509,24 +6809,14 @@
   dependencies:
     locate-path: ^5.0.0
     path-exists: ^4.0.0
   checksum: 4c172680e8f8c1f78839486e14a43ef82e9decd0e74145f40707cc42e7420506d5ec92d9a11c22bd2c48fb0c384ea05dd30e10dd152fefeec6f2f75282a8b844
   languageName: node
   linkType: hard
 
-"find-up@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "find-up@npm:5.0.0"
-  dependencies:
-    locate-path: ^6.0.0
-    path-exists: ^4.0.0
-  checksum: 07955e357348f34660bde7920783204ff5a26ac2cafcaa28bace494027158a97b9f56faaf2d89a6106211a8174db650dd9f503f9c0d526b1202d5554a00b9095
-  languageName: node
-  linkType: hard
-
 "flat-cache@npm:^3.0.4":
   version: 3.0.4
   resolution: "flat-cache@npm:3.0.4"
   dependencies:
     flatted: ^3.1.0
     rimraf: ^3.0.2
   checksum: 4fdd10ecbcbf7d520f9040dd1340eb5dfe951e6f0ecf2252edeec03ee68d989ec8b9a20f4434270e71bcfd57800dc09b3344fca3966b2eb8f613072c7d9a2365
@@ -6613,33 +6903,42 @@
     jsonfile: ^6.0.1
     universalify: ^2.0.0
   checksum: dc94ab37096f813cc3ca12f0f1b5ad6744dfed9ed21e953d72530d103cea193c2f81584a39e9dee1bea36de5ee66805678c0dddc048e8af1427ac19c00fffc50
   languageName: node
   linkType: hard
 
 "fs-extra@npm:^11.1.0":
-  version: 11.1.0
-  resolution: "fs-extra@npm:11.1.0"
+  version: 11.1.1
+  resolution: "fs-extra@npm:11.1.1"
   dependencies:
     graceful-fs: ^4.2.0
     jsonfile: ^6.0.1
     universalify: ^2.0.0
-  checksum: 5ca476103fa1f5ff4a9b3c4f331548f8a3c1881edaae323a4415d3153b5dc11dc6a981c8d1dd93eec8367ceee27b53f8bd27eecbbf66ffcdd04927510c171e7f
+  checksum: fb883c68245b2d777fbc1f2082c9efb084eaa2bbf9fddaa366130d196c03608eebef7fb490541276429ee1ca99f317e2d73e96f5ca0999eefedf5a624ae1edfd
   languageName: node
   linkType: hard
 
 "fs-minipass@npm:^2.0.0, fs-minipass@npm:^2.1.0":
   version: 2.1.0
   resolution: "fs-minipass@npm:2.1.0"
   dependencies:
     minipass: ^3.0.0
   checksum: 1b8d128dae2ac6cc94230cc5ead341ba3e0efaef82dab46a33d171c044caaa6ca001364178d42069b2809c35a1c3c35079a32107c770e9ffab3901b59af8c8b1
   languageName: node
   linkType: hard
 
+"fs-minipass@npm:^3.0.0":
+  version: 3.0.1
+  resolution: "fs-minipass@npm:3.0.1"
+  dependencies:
+    minipass: ^4.0.0
+  checksum: ce1fd3ccef7d64caa9ee5f566db1abe250b6e0067defe53003288537b310956e6f42c433c3ee6001e044f656ce8ba5a0b2e5b5589c513c67b57470d11c3d9b07
+  languageName: node
+  linkType: hard
+
 "fs.realpath@npm:^1.0.0":
   version: 1.0.0
   resolution: "fs.realpath@npm:1.0.0"
   checksum: 99ddea01a7e75aa276c250a04eedeffe5662bce66c65c07164ad6264f9de18fb21be9433ead460e54cff20e31721c811f4fb5d70591799df5f85dce6d6746fd0
   languageName: node
   linkType: hard
 
@@ -6700,14 +6999,30 @@
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
     wide-align: ^1.1.5
   checksum: 788b6bfe52f1dd8e263cda800c26ac0ca2ff6de0b6eee2fe0d9e3abf15e149b651bd27bf5226be10e6e3edb5c4e5d5985a5a1a98137e7a892f75eff76467ad2d
   languageName: node
   linkType: hard
 
+"gauge@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "gauge@npm:5.0.0"
+  dependencies:
+    aproba: ^1.0.3 || ^2.0.0
+    color-support: ^1.1.3
+    console-control-strings: ^1.1.0
+    has-unicode: ^2.0.1
+    signal-exit: ^3.0.7
+    string-width: ^4.2.3
+    strip-ansi: ^6.0.1
+    wide-align: ^1.1.5
+  checksum: 663c3e9418a81274824301c5282d047f13e1612ccb458d96ea6cae5f63012c171af2829041501c459f7fa64845bbc5362d3574573747e9a114745d64ceb2480b
+  languageName: node
+  linkType: hard
+
 "gensync@npm:^1.0.0-beta.2":
   version: 1.0.0-beta.2
   resolution: "gensync@npm:1.0.0-beta.2"
   checksum: a7437e58c6be12aa6c90f7730eac7fa9833dc78872b4ad2963d2031b00a3367a93f98aec75f9aaac7220848e4026d67a8655e870b24f20a543d103c0d65952ec
   languageName: node
   linkType: hard
 
@@ -6908,14 +7223,26 @@
     inherits: 2
     minimatch: ^5.0.1
     once: ^1.3.0
   checksum: 92fbea3221a7d12075f26f0227abac435de868dd0736a17170663783296d0dd8d3d532a5672b4488a439bf5d7fb85cdd07c11185d6cd39184f0385cbdfb86a47
   languageName: node
   linkType: hard
 
+"glob@npm:^9.2.0, glob@npm:^9.3.0, glob@npm:^9.3.1":
+  version: 9.3.2
+  resolution: "glob@npm:9.3.2"
+  dependencies:
+    fs.realpath: ^1.0.0
+    minimatch: ^7.4.1
+    minipass: ^4.2.4
+    path-scurry: ^1.6.1
+  checksum: f3d188e9f70e24fa729a63ca197bcdb36d838677abec1fb9bbfe4b7620063bf90dc0f8d195203d632abfdfa049fad0edf22f93c60076de67cef20c23bcbfaee8
+  languageName: node
+  linkType: hard
+
 "glob@npm:~7.1.6":
   version: 7.1.7
   resolution: "glob@npm:7.1.7"
   dependencies:
     fs.realpath: ^1.0.0
     inflight: ^1.0.4
     inherits: 2
@@ -6967,15 +7294,15 @@
   resolution: "globalthis@npm:1.0.3"
   dependencies:
     define-properties: ^1.1.3
   checksum: fbd7d760dc464c886d0196166d92e5ffb4c84d0730846d6621a39fbbc068aeeb9c8d1421ad330e94b7bca4bb4ea092f5f21f3d36077812af5d098b4dc006c998
   languageName: node
   linkType: hard
 
-"globby@npm:11.1.0, globby@npm:^11.1.0":
+"globby@npm:11.1.0, globby@npm:^11.0.1, globby@npm:^11.1.0":
   version: 11.1.0
   resolution: "globby@npm:11.1.0"
   dependencies:
     array-union: ^2.1.0
     dir-glob: ^3.0.1
     fast-glob: ^3.2.9
     ignore: ^5.2.0
@@ -6997,21 +7324,28 @@
   resolution: "gopd@npm:1.0.1"
   dependencies:
     get-intrinsic: ^1.1.3
   checksum: a5ccfb8806e0917a94e0b3de2af2ea4979c1da920bc381667c260e00e7cafdbe844e2cb9c5bcfef4e5412e8bf73bab837285bc35c7ba73aaaf0134d4583393a6
   languageName: node
   linkType: hard
 
-"graceful-fs@npm:4.2.10, graceful-fs@npm:^4.1.11, graceful-fs@npm:^4.1.15, graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
+"graceful-fs@npm:4.2.10":
   version: 4.2.10
   resolution: "graceful-fs@npm:4.2.10"
   checksum: 3f109d70ae123951905d85032ebeae3c2a5a7a997430df00ea30df0e3a6c60cf6689b109654d6fdacd28810a053348c4d14642da1d075049e6be1ba5216218da
   languageName: node
   linkType: hard
 
+"graceful-fs@npm:^4.1.11, graceful-fs@npm:^4.1.15, graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
+  version: 4.2.11
+  resolution: "graceful-fs@npm:4.2.11"
+  checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
+  languageName: node
+  linkType: hard
+
 "grapheme-splitter@npm:^1.0.4":
   version: 1.0.4
   resolution: "grapheme-splitter@npm:1.0.4"
   checksum: 0c22ec54dee1b05cd480f78cf14f732cb5b108edc073572c4ec205df4cd63f30f8db8025afc5debc8835a8ddeacf648a1c7992fe3dcd6ad38f9a476d84906620
   languageName: node
   linkType: hard
 
@@ -7146,14 +7480,23 @@
   resolution: "hosted-git-info@npm:5.2.1"
   dependencies:
     lru-cache: ^7.5.1
   checksum: fa35df185224adfd69141f3b2f8cc31f50e705a5ebb415ccfbfd055c5b94bd08d3e658edf1edad9e2ac7d81831ac7cf261f5d219b3adc8d744fb8cdacaaf2ead
   languageName: node
   linkType: hard
 
+"hosted-git-info@npm:^6.0.0, hosted-git-info@npm:^6.1.1":
+  version: 6.1.1
+  resolution: "hosted-git-info@npm:6.1.1"
+  dependencies:
+    lru-cache: ^7.5.1
+  checksum: fcd3ca2eaa05f3201425ccbb8aa47f88cdda4a3a6d79453f8e269f7171356278bd1db08f059d8439eb5eaa91c6a8a20800fc49cca6e9e4e899b202a332d5ba6b
+  languageName: node
+  linkType: hard
+
 "html-encoding-sniffer@npm:^3.0.0":
   version: 3.0.0
   resolution: "html-encoding-sniffer@npm:3.0.0"
   dependencies:
     whatwg-encoding: ^2.0.0
   checksum: 8d806aa00487e279e5ccb573366a951a9f68f65c90298eac9c3a2b440a7ffe46615aff2995a2f61c6746c639234e6179a97e18ca5ccbbf93d3725ef2099a4502
   languageName: node
@@ -7181,15 +7524,15 @@
     domhandler: ^4.0.0
     domutils: ^2.5.2
     entities: ^2.0.0
   checksum: 81a7b3d9c3bb9acb568a02fc9b1b81ffbfa55eae7f1c41ae0bf840006d1dbf54cb3aa245b2553e2c94db674840a9f0fdad7027c9a9d01a062065314039058c4e
   languageName: node
   linkType: hard
 
-"http-cache-semantics@npm:^4.1.0":
+"http-cache-semantics@npm:^4.1.0, http-cache-semantics@npm:^4.1.1":
   version: 4.1.1
   resolution: "http-cache-semantics@npm:4.1.1"
   checksum: 83ac0bc60b17a3a36f9953e7be55e5c8f41acc61b22583060e8dedc9dd5e3607c823a88d0926f9150e571f90946835c7fe150732801010845c72cd8bbff1a236
   languageName: node
   linkType: hard
 
 "http-proxy-agent@npm:^5.0.0":
@@ -7261,15 +7604,15 @@
   resolution: "identity-obj-proxy@npm:3.0.0"
   dependencies:
     harmony-reflect: ^1.4.6
   checksum: 97559f8ea2aeaa1a880d279d8c49550dce01148321e00a2102cda5ddf9ce622fa1d7f3efc7bed63458af78889de888fdaebaf31c816312298bb3fdd0ef8aaf2c
   languageName: node
   linkType: hard
 
-"ieee754@npm:^1.1.13":
+"ieee754@npm:^1.1.13, ieee754@npm:^1.2.1":
   version: 1.2.1
   resolution: "ieee754@npm:1.2.1"
   checksum: 5144c0c9815e54ada181d80a0b810221a253562422e7c6c3a60b1901154184f49326ec239d618c416c1c5945a2e197107aee8d986a3dd836b53dffefd99b5e7e
   languageName: node
   linkType: hard
 
 "ignore-walk@npm:^5.0.1":
@@ -7277,14 +7620,23 @@
   resolution: "ignore-walk@npm:5.0.1"
   dependencies:
     minimatch: ^5.0.1
   checksum: 1a4ef35174653a1aa6faab3d9f8781269166536aee36a04946f6e2b319b2475c1903a75ed42f04219274128242f49d0a10e20c4354ee60d9548e97031451150b
   languageName: node
   linkType: hard
 
+"ignore-walk@npm:^6.0.0":
+  version: 6.0.2
+  resolution: "ignore-walk@npm:6.0.2"
+  dependencies:
+    minimatch: ^7.4.2
+  checksum: 99dda4d6977cf47b359ae17d62f4abfb9273a2507d14d38db7a29abcd8385ec45cc1d8cf00e73695f98ef4001e7439a4f5b619a3d4055a37bd953288be01b485
+  languageName: node
+  linkType: hard
+
 "ignore@npm:^5.0.4, ignore@npm:^5.2.0, ignore@npm:^5.2.4":
   version: 5.2.4
   resolution: "ignore@npm:5.2.4"
   checksum: 3d4c309c6006e2621659311783eaea7ebcd41fe4ca1d78c91c473157ad6666a57a2df790fe0d07a12300d9aac2888204d7be8d59f9aaf665b1c7fcdb432517ef
   languageName: node
   linkType: hard
 
@@ -7380,14 +7732,37 @@
     semver: ^7.3.5
     validate-npm-package-license: ^3.0.4
     validate-npm-package-name: ^4.0.0
   checksum: e027f60e4a1564809eee790d5a842341c784888fd7c7ace5f9a34ea76224c0adb6f3ab3bf205cf1c9c877a6e1a76c68b00847a984139f60813125d7b42a23a13
   languageName: node
   linkType: hard
 
+"inquirer@npm:8.2.4":
+  version: 8.2.4
+  resolution: "inquirer@npm:8.2.4"
+  dependencies:
+    ansi-escapes: ^4.2.1
+    chalk: ^4.1.1
+    cli-cursor: ^3.1.0
+    cli-width: ^3.0.0
+    external-editor: ^3.0.3
+    figures: ^3.0.0
+    lodash: ^4.17.21
+    mute-stream: 0.0.8
+    ora: ^5.4.1
+    run-async: ^2.4.0
+    rxjs: ^7.5.5
+    string-width: ^4.1.0
+    strip-ansi: ^6.0.0
+    through: ^2.3.6
+    wrap-ansi: ^7.0.0
+  checksum: dfcb6529d3af443dfea2241cb471508091b51f5121a088fdb8728b23ec9b349ef0a5e13a0ef2c8e19457b0bed22f7cbbcd561f7a4529d084c562a58c605e2655
+  languageName: node
+  linkType: hard
+
 "inquirer@npm:^8.2.4":
   version: 8.2.5
   resolution: "inquirer@npm:8.2.5"
   dependencies:
     ansi-escapes: ^4.2.1
     chalk: ^4.1.1
     cli-cursor: ^3.1.0
@@ -7403,15 +7778,15 @@
     strip-ansi: ^6.0.0
     through: ^2.3.6
     wrap-ansi: ^7.0.0
   checksum: f13ee4c444187786fb393609dedf6b30870115a57b603f2e6424f29a99abc13446fd45ee22461c33c9c40a92a60a8df62d0d6b25d74fc6676fa4cb211de55b55
   languageName: node
   linkType: hard
 
-"internal-slot@npm:^1.0.3, internal-slot@npm:^1.0.4":
+"internal-slot@npm:^1.0.3, internal-slot@npm:^1.0.5":
   version: 1.0.5
   resolution: "internal-slot@npm:1.0.5"
   dependencies:
     get-intrinsic: ^1.2.0
     has: ^1.0.3
     side-channel: ^1.0.4
   checksum: 97e84046bf9e7574d0956bd98d7162313ce7057883b6db6c5c7b5e5f05688864b0978ba07610c726d15d66544ffe4b1050107d93f8a39ebc59b15d8b429b497a
@@ -7428,22 +7803,22 @@
 "ip@npm:^2.0.0":
   version: 2.0.0
   resolution: "ip@npm:2.0.0"
   checksum: cfcfac6b873b701996d71ec82a7dd27ba92450afdb421e356f44044ed688df04567344c36cbacea7d01b1c39a4c732dc012570ebe9bebfb06f27314bca625349
   languageName: node
   linkType: hard
 
-"is-array-buffer@npm:^3.0.1":
-  version: 3.0.1
-  resolution: "is-array-buffer@npm:3.0.1"
+"is-array-buffer@npm:^3.0.1, is-array-buffer@npm:^3.0.2":
+  version: 3.0.2
+  resolution: "is-array-buffer@npm:3.0.2"
   dependencies:
     call-bind: ^1.0.2
-    get-intrinsic: ^1.1.3
+    get-intrinsic: ^1.2.0
     is-typed-array: ^1.1.10
-  checksum: f26ab87448e698285daf707e52a533920449f7abf63714140ffab9d5571aa5a71ac2fa2677e8b793ad0d5d3e40078d4d2c8a0ab39c957e3cfc6513bb6c9dfdc9
+  checksum: dcac9dda66ff17df9cabdc58214172bf41082f956eab30bb0d86bc0fab1e44b690fc8e1f855cf2481245caf4e8a5a006a982a71ddccec84032ed41f9d8da8c14
   languageName: node
   linkType: hard
 
 "is-arrayish@npm:^0.2.1":
   version: 0.2.1
   resolution: "is-arrayish@npm:0.2.1"
   checksum: eef4417e3c10e60e2c810b6084942b3ead455af16c4509959a27e490e7aee87cfb3f38e01bbde92220b528a0ee1a18d52b787e1458ee86174d8c7f0e58cd488f
@@ -7584,15 +7959,22 @@
 "is-obj@npm:^2.0.0":
   version: 2.0.0
   resolution: "is-obj@npm:2.0.0"
   checksum: c9916ac8f4621962a42f5e80e7ffdb1d79a3fab7456ceaeea394cd9e0858d04f985a9ace45be44433bf605673c8be8810540fe4cc7f4266fc7526ced95af5a08
   languageName: node
   linkType: hard
 
-"is-path-inside@npm:^3.0.3":
+"is-path-cwd@npm:^2.2.0":
+  version: 2.2.0
+  resolution: "is-path-cwd@npm:2.2.0"
+  checksum: 46a840921bb8cc0dc7b5b423a14220e7db338072a4495743a8230533ce78812dc152548c86f4b828411fe98c5451959f07cf841c6a19f611e46600bd699e8048
+  languageName: node
+  linkType: hard
+
+"is-path-inside@npm:^3.0.2, is-path-inside@npm:^3.0.3":
   version: 3.0.3
   resolution: "is-path-inside@npm:3.0.3"
   checksum: abd50f06186a052b349c15e55b182326f1936c89a78bf6c8f2b707412517c097ce04bc49a0ca221787bc44e1049f51f09a2ffb63d22899051988d3a618ba13e9
   languageName: node
   linkType: hard
 
 "is-plain-obj@npm:^1.0.0, is-plain-obj@npm:^1.1.0":
@@ -7822,212 +8204,213 @@
     minimatch: ^3.0.4
   bin:
     jake: ./bin/cli.js
   checksum: 56c913ecf5a8d74325d0af9bc17a233bad50977438d44864d925bb6c45c946e0fee8c4c1f5fe2225471ef40df5222e943047982717ebff0d624770564d3c46ba
   languageName: node
   linkType: hard
 
-"jest-changed-files@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-changed-files@npm:29.4.3"
+"jest-changed-files@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-changed-files@npm:29.5.0"
   dependencies:
     execa: ^5.0.0
     p-limit: ^3.1.0
-  checksum: 9a70bd8e92b37e18ad26d8bea97c516f41119fb7046b4255a13c76d557b0e54fa0629726de5a093fadfd6a0a08ce45da65a57086664d505b8db4b3133133e141
+  checksum: a67a7cb3c11f8f92bd1b7c79e84f724cbd11a9ad51f3cdadafe3ce7ee3c79ee50dbea128f920f5fddc807e9e4e83f5462143094391feedd959a77dd20ab96cf3
   languageName: node
   linkType: hard
 
-"jest-circus@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-circus@npm:29.4.3"
+"jest-circus@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-circus@npm:29.5.0"
   dependencies:
-    "@jest/environment": ^29.4.3
-    "@jest/expect": ^29.4.3
-    "@jest/test-result": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/environment": ^29.5.0
+    "@jest/expect": ^29.5.0
+    "@jest/test-result": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/node": "*"
     chalk: ^4.0.0
     co: ^4.6.0
     dedent: ^0.7.0
     is-generator-fn: ^2.0.0
-    jest-each: ^29.4.3
-    jest-matcher-utils: ^29.4.3
-    jest-message-util: ^29.4.3
-    jest-runtime: ^29.4.3
-    jest-snapshot: ^29.4.3
-    jest-util: ^29.4.3
+    jest-each: ^29.5.0
+    jest-matcher-utils: ^29.5.0
+    jest-message-util: ^29.5.0
+    jest-runtime: ^29.5.0
+    jest-snapshot: ^29.5.0
+    jest-util: ^29.5.0
     p-limit: ^3.1.0
-    pretty-format: ^29.4.3
+    pretty-format: ^29.5.0
+    pure-rand: ^6.0.0
     slash: ^3.0.0
     stack-utils: ^2.0.3
-  checksum: 2739bef9c888743b49ff3fe303131381618e5d2f250f613a91240d9c86e19e6874fc904cbd8bcb02ec9ec59a84e5dae4ffec929f0c6171e87ddbc05508a137f4
+  checksum: 44ff5d06acedae6de6c866e20e3b61f83e29ab94cf9f960826e7e667de49c12dd9ab9dffd7fa3b7d1f9688a8b5bfb1ebebadbea69d9ed0d3f66af4a0ff8c2b27
   languageName: node
   linkType: hard
 
-"jest-cli@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-cli@npm:29.4.3"
+"jest-cli@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-cli@npm:29.5.0"
   dependencies:
-    "@jest/core": ^29.4.3
-    "@jest/test-result": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/core": ^29.5.0
+    "@jest/test-result": ^29.5.0
+    "@jest/types": ^29.5.0
     chalk: ^4.0.0
     exit: ^0.1.2
     graceful-fs: ^4.2.9
     import-local: ^3.0.2
-    jest-config: ^29.4.3
-    jest-util: ^29.4.3
-    jest-validate: ^29.4.3
+    jest-config: ^29.5.0
+    jest-util: ^29.5.0
+    jest-validate: ^29.5.0
     prompts: ^2.0.1
     yargs: ^17.3.1
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
   bin:
     jest: bin/jest.js
-  checksum: f4c9f6d76cde2c60a4169acbebb3f862728be03bcf3fe0077d2e55da7f9f3c3e9483cfa6e936832d35eabf96ee5ebf0300c4b0bd43cffff099801793466bfdd8
+  checksum: 39897bbbc0f0d8a6b975ab12fd13887eaa28d92e3dee9e0173a5cb913ae8cc2ae46e090d38c6d723e84d9d6724429cd08685b4e505fa447d31ca615630c7dbba
   languageName: node
   linkType: hard
 
-"jest-config@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-config@npm:29.4.3"
+"jest-config@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-config@npm:29.5.0"
   dependencies:
     "@babel/core": ^7.11.6
-    "@jest/test-sequencer": ^29.4.3
-    "@jest/types": ^29.4.3
-    babel-jest: ^29.4.3
+    "@jest/test-sequencer": ^29.5.0
+    "@jest/types": ^29.5.0
+    babel-jest: ^29.5.0
     chalk: ^4.0.0
     ci-info: ^3.2.0
     deepmerge: ^4.2.2
     glob: ^7.1.3
     graceful-fs: ^4.2.9
-    jest-circus: ^29.4.3
-    jest-environment-node: ^29.4.3
+    jest-circus: ^29.5.0
+    jest-environment-node: ^29.5.0
     jest-get-type: ^29.4.3
     jest-regex-util: ^29.4.3
-    jest-resolve: ^29.4.3
-    jest-runner: ^29.4.3
-    jest-util: ^29.4.3
-    jest-validate: ^29.4.3
+    jest-resolve: ^29.5.0
+    jest-runner: ^29.5.0
+    jest-util: ^29.5.0
+    jest-validate: ^29.5.0
     micromatch: ^4.0.4
     parse-json: ^5.2.0
-    pretty-format: ^29.4.3
+    pretty-format: ^29.5.0
     slash: ^3.0.0
     strip-json-comments: ^3.1.1
   peerDependencies:
     "@types/node": "*"
     ts-node: ">=9.0.0"
   peerDependenciesMeta:
     "@types/node":
       optional: true
     ts-node:
       optional: true
-  checksum: 92f9a9c6850b18682cb01892774a33967472af23a5844438d8c68077d5f2a29b15b665e4e4db7de3d74002a6dca158cd5b2cb9f5debfd2cce5e1aee6c74e3873
+  checksum: c37c4dab964c54ab293d4e302d40b09687037ac9d00b88348ec42366970747feeaf265e12e3750cd3660b40c518d4031335eda11ac10b70b10e60797ebbd4b9c
   languageName: node
   linkType: hard
 
-"jest-diff@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-diff@npm:29.4.3"
+"jest-diff@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-diff@npm:29.5.0"
   dependencies:
     chalk: ^4.0.0
     diff-sequences: ^29.4.3
     jest-get-type: ^29.4.3
-    pretty-format: ^29.4.3
-  checksum: 877fd1edffef6b319688c27b152e5b28e2bc4bcda5ce0ca90d7e137f9fafda4280bae25403d4c0bfd9806c2c0b15d966aa2dfaf5f9928ec8f1ccea7fa1d08ed6
+    pretty-format: ^29.5.0
+  checksum: dfd0f4a299b5d127779c76b40106c37854c89c3e0785098c717d52822d6620d227f6234c3a9291df204d619e799e3654159213bf93220f79c8e92a55475a3d39
   languageName: node
   linkType: hard
 
 "jest-docblock@npm:^29.4.3":
   version: 29.4.3
   resolution: "jest-docblock@npm:29.4.3"
   dependencies:
     detect-newline: ^3.0.0
   checksum: e0e9df1485bb8926e5b33478cdf84b3387d9caf3658e7dc1eaa6dc34cb93dea0d2d74797f6e940f0233a88f3dadd60957f2288eb8f95506361f85b84bf8661df
   languageName: node
   linkType: hard
 
-"jest-each@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-each@npm:29.4.3"
+"jest-each@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-each@npm:29.5.0"
   dependencies:
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     chalk: ^4.0.0
     jest-get-type: ^29.4.3
-    jest-util: ^29.4.3
-    pretty-format: ^29.4.3
-  checksum: 1f72738338399efab0139eaea18bc198be0c6ed889770c8cbfa70bf9c724e8171fe1d3a29a94f9f39b8493ee6b2529bb350fb7c7c75e0d7eddfd28c253c79f9d
+    jest-util: ^29.5.0
+    pretty-format: ^29.5.0
+  checksum: b8b297534d25834c5d4e31e4c687359787b1e402519e42664eb704cc3a12a7a91a017565a75acb02e8cf9afd3f4eef3350bd785276bec0900184641b765ff7a5
   languageName: node
   linkType: hard
 
 "jest-environment-jsdom@npm:^29.3.0":
-  version: 29.4.3
-  resolution: "jest-environment-jsdom@npm:29.4.3"
+  version: 29.5.0
+  resolution: "jest-environment-jsdom@npm:29.5.0"
   dependencies:
-    "@jest/environment": ^29.4.3
-    "@jest/fake-timers": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/environment": ^29.5.0
+    "@jest/fake-timers": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/jsdom": ^20.0.0
     "@types/node": "*"
-    jest-mock: ^29.4.3
-    jest-util: ^29.4.3
+    jest-mock: ^29.5.0
+    jest-util: ^29.5.0
     jsdom: ^20.0.0
   peerDependencies:
     canvas: ^2.5.0
   peerDependenciesMeta:
     canvas:
       optional: true
-  checksum: 3fb29bb4b472e05a38fdb235aa936ad469dfa2f6c1cab97fe3d1a7c585351976d05c7bbbd715b9747f070a225dcf10a9166df1461e0fb838ea7a377a8e64bed4
+  checksum: 3df7fc85275711f20b483ac8cd8c04500704ed0f69791eb55c574b38f5a39470f03d775cf20c1025bc1884916ac0573aa2fa4db1bb74225bc7fdd95ba97ad0da
   languageName: node
   linkType: hard
 
-"jest-environment-node@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-environment-node@npm:29.4.3"
+"jest-environment-node@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-environment-node@npm:29.5.0"
   dependencies:
-    "@jest/environment": ^29.4.3
-    "@jest/fake-timers": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/environment": ^29.5.0
+    "@jest/fake-timers": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/node": "*"
-    jest-mock: ^29.4.3
-    jest-util: ^29.4.3
-  checksum: 3c7362edfdbd516e83af7367c95dde35761a482b174de9735c07633405486ec73e19624e9bea4333fca33c24e8d65eaa1aa6594e0cb6bfeeeb564ccc431ee61d
+    jest-mock: ^29.5.0
+    jest-util: ^29.5.0
+  checksum: 57981911cc20a4219b0da9e22b2e3c9f31b505e43f78e61c899e3227ded455ce1a3a9483842c69cfa4532f02cfb536ae0995bf245f9211608edacfc1e478d411
   languageName: node
   linkType: hard
 
 "jest-get-type@npm:^29.4.3":
   version: 29.4.3
   resolution: "jest-get-type@npm:29.4.3"
   checksum: 6ac7f2dde1c65e292e4355b6c63b3a4897d7e92cb4c8afcf6d397f2682f8080e094c8b0b68205a74d269882ec06bf696a9de6cd3e1b7333531e5ed7b112605ce
   languageName: node
   linkType: hard
 
-"jest-haste-map@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-haste-map@npm:29.4.3"
+"jest-haste-map@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-haste-map@npm:29.5.0"
   dependencies:
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     "@types/graceful-fs": ^4.1.3
     "@types/node": "*"
     anymatch: ^3.0.3
     fb-watchman: ^2.0.0
     fsevents: ^2.3.2
     graceful-fs: ^4.2.9
     jest-regex-util: ^29.4.3
-    jest-util: ^29.4.3
-    jest-worker: ^29.4.3
+    jest-util: ^29.5.0
+    jest-worker: ^29.5.0
     micromatch: ^4.0.4
     walker: ^1.0.8
   dependenciesMeta:
     fsevents:
       optional: true
-  checksum: c7a83ebe6008b3fe96a96235e8153092e54b14df68e0f4205faedec57450df26b658578495a71c6d82494c01fbb44bca98c1506a6b2b9c920696dcc5d2e2bc59
+  checksum: 3828ff7783f168e34be2c63887f82a01634261f605dcae062d83f979a61c37739e21b9607ecb962256aea3fbe5a530a1acee062d0026fcb47c607c12796cf3b7
   languageName: node
   linkType: hard
 
 "jest-junit@npm:^15.0.0":
   version: 15.0.0
   resolution: "jest-junit@npm:15.0.0"
   dependencies:
@@ -8035,61 +8418,61 @@
     strip-ansi: ^6.0.1
     uuid: ^8.3.2
     xml: ^1.0.1
   checksum: e8fe4d2f2ab843383ac41820a6fe495739d154ec435cd44ba590b44ec7fd62095676f3eef13f98392f81d4a3727ea58b4f4fad231fe367ac31243952b9ad716f
   languageName: node
   linkType: hard
 
-"jest-leak-detector@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-leak-detector@npm:29.4.3"
+"jest-leak-detector@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-leak-detector@npm:29.5.0"
   dependencies:
     jest-get-type: ^29.4.3
-    pretty-format: ^29.4.3
-  checksum: ec2b45e6f0abce81bd0dd0f6fd06b433c24d1ec865267af7640fae540ec868b93752598e407a9184d9c7419cbf32e8789007cc8c1be1a84f8f7321a0f8ad01f1
+    pretty-format: ^29.5.0
+  checksum: 0fb845da7ac9cdfc9b3b2e35f6f623a41c547d7dc0103ceb0349013459d00de5870b5689a625e7e37f9644934b40e8f1dcdd5422d14d57470600350364676313
   languageName: node
   linkType: hard
 
-"jest-matcher-utils@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-matcher-utils@npm:29.4.3"
+"jest-matcher-utils@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-matcher-utils@npm:29.5.0"
   dependencies:
     chalk: ^4.0.0
-    jest-diff: ^29.4.3
+    jest-diff: ^29.5.0
     jest-get-type: ^29.4.3
-    pretty-format: ^29.4.3
-  checksum: 9e13cbe42d2113bab2691110c7c3ba5cec3b94abad2727e1de90929d0f67da444e9b2066da3b476b5bf788df53a8ede0e0a950cfb06a04e4d6d566d115ee4f1d
+    pretty-format: ^29.5.0
+  checksum: 1d3e8c746e484a58ce194e3aad152eff21fd0896e8b8bf3d4ab1a4e2cbfed95fb143646f4ad9fdf6e42212b9e8fc033268b58e011b044a9929df45485deb5ac9
   languageName: node
   linkType: hard
 
-"jest-message-util@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-message-util@npm:29.4.3"
+"jest-message-util@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-message-util@npm:29.5.0"
   dependencies:
     "@babel/code-frame": ^7.12.13
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     "@types/stack-utils": ^2.0.0
     chalk: ^4.0.0
     graceful-fs: ^4.2.9
     micromatch: ^4.0.4
-    pretty-format: ^29.4.3
+    pretty-format: ^29.5.0
     slash: ^3.0.0
     stack-utils: ^2.0.3
-  checksum: 64f06b9550021e68da0059020bea8691283cf818918810bb67192d7b7fb9b691c7eadf55c2ca3cd04df5394918f2327245077095cdc0d6b04be3532d2c7d0ced
+  checksum: daddece6bbf846eb6a2ab9be9f2446e54085bef4e5cecd13d2a538fa9c01cb89d38e564c6b74fd8e12d37ed9eface8a362240ae9f21d68b214590631e7a0d8bf
   languageName: node
   linkType: hard
 
-"jest-mock@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-mock@npm:29.4.3"
+"jest-mock@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-mock@npm:29.5.0"
   dependencies:
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     "@types/node": "*"
-    jest-util: ^29.4.3
-  checksum: 8eb4a29b02d2cd03faac0290b6df6d23b4ffa43f72b21c7fff3c7dd04a2797355b1e85862b70b15341dd33ee3a693b17db5520a6f6e6b81ee75601987de6a1a2
+    jest-util: ^29.5.0
+  checksum: 2a9cf07509948fa8608898c445f04fe4dd6e2049ff431e5531eee028c808d3ba3c67f226ac87b0cf383feaa1055776900d197c895e89783016886ac17a4ff10c
   languageName: node
   linkType: hard
 
 "jest-pnp-resolver@npm:^1.2.2":
   version: 1.2.3
   resolution: "jest-pnp-resolver@npm:1.2.3"
   peerDependencies:
@@ -8104,222 +8487,221 @@
 "jest-regex-util@npm:^29.4.3":
   version: 29.4.3
   resolution: "jest-regex-util@npm:29.4.3"
   checksum: 96fc7fc28cd4dd73a63c13a526202c4bd8b351d4e5b68b1a2a2c88da3308c2a16e26feaa593083eb0bac38cca1aa9dd05025412e7de013ba963fb8e66af22b8a
   languageName: node
   linkType: hard
 
-"jest-resolve-dependencies@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-resolve-dependencies@npm:29.4.3"
+"jest-resolve-dependencies@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-resolve-dependencies@npm:29.5.0"
   dependencies:
     jest-regex-util: ^29.4.3
-    jest-snapshot: ^29.4.3
-  checksum: 3ad934cd2170c9658d8800f84a975dafc866ec85b7ce391c640c09c3744ced337787620d8667dc8d1fa5e0b1493f973caa1a1bb980e4e6a50b46a1720baf0bd1
+    jest-snapshot: ^29.5.0
+  checksum: 479d2e5365d58fe23f2b87001e2e0adcbffe0147700e85abdec8f14b9703b0a55758c1929a9989e3f5d5e954fb88870ea4bfa04783523b664562fcf5f10b0edf
   languageName: node
   linkType: hard
 
-"jest-resolve@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-resolve@npm:29.4.3"
+"jest-resolve@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-resolve@npm:29.5.0"
   dependencies:
     chalk: ^4.0.0
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.4.3
+    jest-haste-map: ^29.5.0
     jest-pnp-resolver: ^1.2.2
-    jest-util: ^29.4.3
-    jest-validate: ^29.4.3
+    jest-util: ^29.5.0
+    jest-validate: ^29.5.0
     resolve: ^1.20.0
     resolve.exports: ^2.0.0
     slash: ^3.0.0
-  checksum: 056a66beccf833f3c7e5a8fc9bfec218886e87b0b103decdbdf11893669539df489d1490cd6d5f0eea35731e8be0d2e955a6710498f970d2eae734da4df029dc
+  checksum: 9a125f3cf323ceef512089339d35f3ee37f79fe16a831fb6a26773ea6a229b9e490d108fec7af334142e91845b5996de8e7cdd85a4d8d617078737d804e29c8f
   languageName: node
   linkType: hard
 
-"jest-runner@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-runner@npm:29.4.3"
+"jest-runner@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-runner@npm:29.5.0"
   dependencies:
-    "@jest/console": ^29.4.3
-    "@jest/environment": ^29.4.3
-    "@jest/test-result": ^29.4.3
-    "@jest/transform": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/console": ^29.5.0
+    "@jest/environment": ^29.5.0
+    "@jest/test-result": ^29.5.0
+    "@jest/transform": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/node": "*"
     chalk: ^4.0.0
     emittery: ^0.13.1
     graceful-fs: ^4.2.9
     jest-docblock: ^29.4.3
-    jest-environment-node: ^29.4.3
-    jest-haste-map: ^29.4.3
-    jest-leak-detector: ^29.4.3
-    jest-message-util: ^29.4.3
-    jest-resolve: ^29.4.3
-    jest-runtime: ^29.4.3
-    jest-util: ^29.4.3
-    jest-watcher: ^29.4.3
-    jest-worker: ^29.4.3
+    jest-environment-node: ^29.5.0
+    jest-haste-map: ^29.5.0
+    jest-leak-detector: ^29.5.0
+    jest-message-util: ^29.5.0
+    jest-resolve: ^29.5.0
+    jest-runtime: ^29.5.0
+    jest-util: ^29.5.0
+    jest-watcher: ^29.5.0
+    jest-worker: ^29.5.0
     p-limit: ^3.1.0
     source-map-support: 0.5.13
-  checksum: c41108e5da01e0b8fdc2a06c5042eb49bb1d8db0e0d4651769fd1b9fe84ab45188617c11a3a8e1c83748b29bfe57dd77001ec57e86e3e3c30f3534e0314f8882
+  checksum: 437dea69c5dddca22032259787bac74790d5a171c9d804711415f31e5d1abfb64fa52f54a9015bb17a12b858fd0cf3f75ef6f3c9e94255a8596e179f707229c4
   languageName: node
   linkType: hard
 
-"jest-runtime@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-runtime@npm:29.4.3"
+"jest-runtime@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-runtime@npm:29.5.0"
   dependencies:
-    "@jest/environment": ^29.4.3
-    "@jest/fake-timers": ^29.4.3
-    "@jest/globals": ^29.4.3
+    "@jest/environment": ^29.5.0
+    "@jest/fake-timers": ^29.5.0
+    "@jest/globals": ^29.5.0
     "@jest/source-map": ^29.4.3
-    "@jest/test-result": ^29.4.3
-    "@jest/transform": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/test-result": ^29.5.0
+    "@jest/transform": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/node": "*"
     chalk: ^4.0.0
     cjs-module-lexer: ^1.0.0
     collect-v8-coverage: ^1.0.0
     glob: ^7.1.3
     graceful-fs: ^4.2.9
-    jest-haste-map: ^29.4.3
-    jest-message-util: ^29.4.3
-    jest-mock: ^29.4.3
+    jest-haste-map: ^29.5.0
+    jest-message-util: ^29.5.0
+    jest-mock: ^29.5.0
     jest-regex-util: ^29.4.3
-    jest-resolve: ^29.4.3
-    jest-snapshot: ^29.4.3
-    jest-util: ^29.4.3
+    jest-resolve: ^29.5.0
+    jest-snapshot: ^29.5.0
+    jest-util: ^29.5.0
     slash: ^3.0.0
     strip-bom: ^4.0.0
-  checksum: b99f8a910d1a38e7476058ba04ad44dfd3d93e837bb7c301d691e646a1085412fde87f06fbe271c9145f0e72d89400bfa7f6994bc30d456c7742269f37d0f570
+  checksum: 7af27bd9d54cf1c5735404cf8d76c6509d5610b1ec0106a21baa815c1aff15d774ce534ac2834bc440dccfe6348bae1885fd9a806f23a94ddafdc0f5bae4b09d
   languageName: node
   linkType: hard
 
-"jest-snapshot@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-snapshot@npm:29.4.3"
+"jest-snapshot@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-snapshot@npm:29.5.0"
   dependencies:
     "@babel/core": ^7.11.6
     "@babel/generator": ^7.7.2
     "@babel/plugin-syntax-jsx": ^7.7.2
     "@babel/plugin-syntax-typescript": ^7.7.2
     "@babel/traverse": ^7.7.2
     "@babel/types": ^7.3.3
-    "@jest/expect-utils": ^29.4.3
-    "@jest/transform": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/expect-utils": ^29.5.0
+    "@jest/transform": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/babel__traverse": ^7.0.6
     "@types/prettier": ^2.1.5
     babel-preset-current-node-syntax: ^1.0.0
     chalk: ^4.0.0
-    expect: ^29.4.3
+    expect: ^29.5.0
     graceful-fs: ^4.2.9
-    jest-diff: ^29.4.3
+    jest-diff: ^29.5.0
     jest-get-type: ^29.4.3
-    jest-haste-map: ^29.4.3
-    jest-matcher-utils: ^29.4.3
-    jest-message-util: ^29.4.3
-    jest-util: ^29.4.3
+    jest-matcher-utils: ^29.5.0
+    jest-message-util: ^29.5.0
+    jest-util: ^29.5.0
     natural-compare: ^1.4.0
-    pretty-format: ^29.4.3
+    pretty-format: ^29.5.0
     semver: ^7.3.5
-  checksum: 79ba52f2435e23ce72b1309be4b17fdbcb299d1c2ce97ebb61df9a62711e9463035f63b4c849181b2fe5aa17b3e09d30ee4668cc25fb3c6f59511c010b4d9494
+  checksum: fe5df54122ed10eed625de6416a45bc4958d5062b018f05b152bf9785ab7f355dcd55e40cf5da63895bf8278f8d7b2bb4059b2cfbfdee18f509d455d37d8aa2b
   languageName: node
   linkType: hard
 
-"jest-util@npm:^29.0.0, jest-util@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-util@npm:29.4.3"
+"jest-util@npm:^29.0.0, jest-util@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-util@npm:29.5.0"
   dependencies:
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     "@types/node": "*"
     chalk: ^4.0.0
     ci-info: ^3.2.0
     graceful-fs: ^4.2.9
     picomatch: ^2.2.3
-  checksum: 606b3e6077895baf8fb4ad4d08c134f37a6b81d5ba77ae654c942b1ae4b7294ab3b5a0eb93db34f129407b367970cf3b76bf5c80897b30f215f2bc8bf20a5f3f
+  checksum: fd9212950d34d2ecad8c990dda0d8ea59a8a554b0c188b53ea5d6c4a0829a64f2e1d49e6e85e812014933d17426d7136da4785f9cf76fff1799de51b88bc85d3
   languageName: node
   linkType: hard
 
-"jest-validate@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-validate@npm:29.4.3"
+"jest-validate@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-validate@npm:29.5.0"
   dependencies:
-    "@jest/types": ^29.4.3
+    "@jest/types": ^29.5.0
     camelcase: ^6.2.0
     chalk: ^4.0.0
     jest-get-type: ^29.4.3
     leven: ^3.1.0
-    pretty-format: ^29.4.3
-  checksum: 983e56430d86bed238448cae031535c1d908f760aa312cd4a4ec0e92f3bc1b6675415ddf57cdeceedb8ad9c698e5bcd10f0a856dfc93a8923bdecc7733f4ba80
+    pretty-format: ^29.5.0
+  checksum: 43ca5df7cb75572a254ac3e92fbbe7be6b6a1be898cc1e887a45d55ea003f7a112717d814a674d37f9f18f52d8de40873c8f084f17664ae562736c78dd44c6a1
   languageName: node
   linkType: hard
 
-"jest-watcher@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-watcher@npm:29.4.3"
+"jest-watcher@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-watcher@npm:29.5.0"
   dependencies:
-    "@jest/test-result": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/test-result": ^29.5.0
+    "@jest/types": ^29.5.0
     "@types/node": "*"
     ansi-escapes: ^4.2.1
     chalk: ^4.0.0
     emittery: ^0.13.1
-    jest-util: ^29.4.3
+    jest-util: ^29.5.0
     string-length: ^4.0.1
-  checksum: 44b64991b3414db853c3756f14690028f4edef7aebfb204a4291cc1901c2239fa27a8687c5c5abbecc74bf613e0bb9b1378bf766430c9febcc71e9c0cb5ad8fc
+  checksum: 62303ac7bdc7e61a8b4239a239d018f7527739da2b2be6a81a7be25b74ca769f1c43ee8558ce8e72bb857245c46d6e03af331227ffb00a57280abb2a928aa776
   languageName: node
   linkType: hard
 
 "jest-worker@npm:^27.4.5":
   version: 27.5.1
   resolution: "jest-worker@npm:27.5.1"
   dependencies:
     "@types/node": "*"
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
   checksum: 98cd68b696781caed61c983a3ee30bf880b5bd021c01d98f47b143d4362b85d0737f8523761e2713d45e18b4f9a2b98af1eaee77afade4111bb65c77d6f7c980
   languageName: node
   linkType: hard
 
-"jest-worker@npm:^29.4.3":
-  version: 29.4.3
-  resolution: "jest-worker@npm:29.4.3"
+"jest-worker@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "jest-worker@npm:29.5.0"
   dependencies:
     "@types/node": "*"
-    jest-util: ^29.4.3
+    jest-util: ^29.5.0
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
-  checksum: c99ae66f257564613e72c5797c3a68f21a22e1c1fb5f30d14695ff5b508a0d2405f22748f13a3df8d1015b5e16abb130170f81f047ff68f58b6b1d2ff6ebc51b
+  checksum: 1151a1ae3602b1ea7c42a8f1efe2b5a7bf927039deaa0827bf978880169899b705744e288f80a63603fb3fc2985e0071234986af7dc2c21c7a64333d8777c7c9
   languageName: node
   linkType: hard
 
 "jest@npm:^29.2.0":
-  version: 29.4.3
-  resolution: "jest@npm:29.4.3"
+  version: 29.5.0
+  resolution: "jest@npm:29.5.0"
   dependencies:
-    "@jest/core": ^29.4.3
-    "@jest/types": ^29.4.3
+    "@jest/core": ^29.5.0
+    "@jest/types": ^29.5.0
     import-local: ^3.0.2
-    jest-cli: ^29.4.3
+    jest-cli: ^29.5.0
   peerDependencies:
     node-notifier: ^8.0.1 || ^9.0.0 || ^10.0.0
   peerDependenciesMeta:
     node-notifier:
       optional: true
   bin:
     jest: bin/jest.js
-  checksum: 084d10d1ceaade3c40e6d3bbd71b9b71b8919ba6fbd6f1f6699bdc259a6ba2f7350c7ccbfa10c11f7e3e01662853650a6244210179542fe4ba87e77dc3f3109f
+  checksum: a8ff2eb0f421623412236e23cbe67c638127fffde466cba9606bc0c0553b4c1e5cb116d7e0ef990b5d1712851652c8ee461373b578df50857fe635b94ff455d5
   languageName: node
   linkType: hard
 
 "js-sdsl@npm:^4.1.4":
-  version: 4.3.0
-  resolution: "js-sdsl@npm:4.3.0"
-  checksum: ce908257cf6909e213af580af3a691a736f5ee8b16315454768f917a682a4ea0c11bde1b241bbfaecedc0eb67b72101b2c2df2ffaed32aed5d539fca816f054e
+  version: 4.4.0
+  resolution: "js-sdsl@npm:4.4.0"
+  checksum: 7bb08a2d746ab7ff742720339aa006c631afe05e77d11eda988c1c35fae8e03e492e4e347e883e786e3ce6170685d4780c125619111f0730c11fdb41b04059c7
   languageName: node
   linkType: hard
 
 "js-tokens@npm:^3.0.0 || ^4.0.0, js-tokens@npm:^4.0.0":
   version: 4.0.0
   resolution: "js-tokens@npm:4.0.0"
   checksum: 8a95213a5a77deb6cbe94d86340e8d9ace2b93bc367790b260101d2f36a2eaf4e4e22d9fa9cf459b38af3a32fb4190e638024cf82ec95ef708680e405ea7cc78
@@ -8416,14 +8798,21 @@
 "json-parse-even-better-errors@npm:^2.3.0, json-parse-even-better-errors@npm:^2.3.1":
   version: 2.3.1
   resolution: "json-parse-even-better-errors@npm:2.3.1"
   checksum: 798ed4cf3354a2d9ccd78e86d2169515a0097a5c133337807cdf7f1fc32e1391d207ccfc276518cc1d7d8d4db93288b8a50ba4293d212ad1336e52a8ec0a941f
   languageName: node
   linkType: hard
 
+"json-parse-even-better-errors@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "json-parse-even-better-errors@npm:3.0.0"
+  checksum: f1970b5220c7fa23d888565510752c3d5e863f93668a202fcaa719739fa41485dfc6a1db212f702ebd3c873851cc067aebc2917e3f79763cae2fdb95046f38f3
+  languageName: node
+  linkType: hard
+
 "json-schema-compare@npm:^0.2.2":
   version: 0.2.2
   resolution: "json-schema-compare@npm:0.2.2"
   dependencies:
     lodash: ^4.17.4
   checksum: dd6f2173857c8e3b77d6ebdfa05bd505bba5b08709ab46b532722f5d1c33b5fee1fc8f3c97d0c0d011db25f9f3b0baf7ab783bb5f55c32abd9f1201760e43c2c
   languageName: node
@@ -8531,18 +8920,18 @@
 "just-diff-apply@npm:^5.2.0":
   version: 5.5.0
   resolution: "just-diff-apply@npm:5.5.0"
   checksum: ed6bbd59781542ccb786bd843038e4591e8390aa788075beb69d358051f68fbeb122bda050b7f42515d51fb64b907d5c7bea694a0543b87b24ce406cfb5f5bfa
   languageName: node
   linkType: hard
 
-"just-diff@npm:^5.0.1":
-  version: 5.2.0
-  resolution: "just-diff@npm:5.2.0"
-  checksum: 5527fb6d28a446185250fba501ad857370c049bac7aa5a34c9ec82a45e1380af1a96137be7df2f87252d9f75ef67be41d4c0267d481ed0235b2ceb3ee1f5f75d
+"just-diff@npm:^6.0.0":
+  version: 6.0.2
+  resolution: "just-diff@npm:6.0.2"
+  checksum: 1a0c7524f640cb88ab013862733e710f840927834208fd3b85cbc5da2ced97acc75e7dcfe493268ac6a6514c51dd8624d2fd9d057050efba3c02b81a6dcb7ff9
   languageName: node
   linkType: hard
 
 "kind-of@npm:^6.0.2, kind-of@npm:^6.0.3":
   version: 6.0.3
   resolution: "kind-of@npm:6.0.3"
   checksum: 3ab01e7b1d440b22fe4c31f23d8d38b4d9b91d9f291df683476576493d5dfd2e03848a8b05813dd0c3f0e835bc63f433007ddeceb71f05cb25c45ae1b19c6d3b
@@ -8552,28 +8941,29 @@
 "kleur@npm:^3.0.3":
   version: 3.0.3
   resolution: "kleur@npm:3.0.3"
   checksum: df82cd1e172f957bae9c536286265a5cdbd5eeca487cb0a3b2a7b41ef959fc61f8e7c0e9aeea9c114ccf2c166b6a8dd45a46fd619c1c569d210ecd2765ad5169
   languageName: node
   linkType: hard
 
-"known-css-properties@npm:^0.26.0":
-  version: 0.26.0
-  resolution: "known-css-properties@npm:0.26.0"
-  checksum: e706f4af9d2683202df9f717e7d713f0f8c3330f155842c40d8f3b2a5837956c34aeb7ba08760977ccde1afce8b5377e29b40eb3e5c0b42bef28ddd108543cfb
+"known-css-properties@npm:^0.27.0":
+  version: 0.27.0
+  resolution: "known-css-properties@npm:0.27.0"
+  checksum: 8584fcf0526f984fe5a358af20200dec3b944373dd005dc23a3ce988895e1acd03e7d69c49533dda07d6d9b6d53990ed1119bd9d3e927f17545f8764c434a5cd
   languageName: node
   linkType: hard
 
 "lerna@npm:^6.5.1":
-  version: 6.5.1
-  resolution: "lerna@npm:6.5.1"
+  version: 6.6.1
+  resolution: "lerna@npm:6.6.1"
   dependencies:
-    "@lerna/child-process": 6.5.1
-    "@lerna/create": 6.5.1
-    "@npmcli/arborist": 5.3.0
+    "@lerna/child-process": 6.6.1
+    "@lerna/create": 6.6.1
+    "@lerna/legacy-package-management": 6.6.1
+    "@npmcli/arborist": 6.2.3
     "@npmcli/run-script": 4.1.7
     "@nrwl/devkit": ">=15.5.2 < 16"
     "@octokit/plugin-enterprise-rest": 6.0.1
     "@octokit/rest": 19.0.3
     byte-size: 7.0.0
     chalk: 4.1.0
     clone-deep: 4.0.1
@@ -8607,31 +8997,30 @@
     load-json-file: 6.2.0
     make-dir: 3.1.0
     minimatch: 3.0.5
     multimatch: 5.0.0
     node-fetch: 2.6.7
     npm-package-arg: 8.1.1
     npm-packlist: 5.1.1
-    npm-registry-fetch: 13.3.0
+    npm-registry-fetch: ^14.0.3
     npmlog: ^6.0.2
     nx: ">=15.5.2 < 16"
     p-map: 4.0.0
     p-map-series: 2.1.0
     p-pipe: 3.1.0
     p-queue: 6.6.2
     p-reduce: 2.1.0
     p-waterfall: 2.1.1
-    pacote: 13.6.1
-    path-exists: 4.0.0
+    pacote: 13.6.2
     pify: 5.0.0
     read-cmd-shim: 3.0.0
     read-package-json: 5.0.1
     resolve-from: 5.0.0
-    rimraf: ^3.0.2
-    semver: 7.3.4
+    rimraf: ^4.4.1
+    semver: ^7.3.8
     signal-exit: 3.0.7
     slash: 3.0.0
     ssri: 9.0.1
     strong-log-transformer: 2.1.0
     tar: 6.1.11
     temp-dir: 1.0.0
     typescript: ^3 || ^4
@@ -8641,15 +9030,15 @@
     validate-npm-package-name: 4.0.0
     write-file-atomic: 4.0.1
     write-pkg: 4.0.0
     yargs: 16.2.0
     yargs-parser: 20.2.4
   bin:
     lerna: dist/cli.js
-  checksum: f0f3ad0cd329ea34a0f9beb3b74adf3757af9b8b23b914efc987cf0aa5afa86da5284937da4879b62c0db76cbf3c6b575381dc32b71c760d2d6152c98d0b976b
+  checksum: 67c7c0975f6dcc2cab8d2b7bd2ddb7c769f88ca55cae7f88153e03b3009c3f3eebc58fe8953b635e04c0cf807f1fa7020c7d272e9f84b1bf1eb8fde9ff701cca
   languageName: node
   linkType: hard
 
 "level-codec@npm:^9.0.0":
   version: 9.0.2
   resolution: "level-codec@npm:9.0.2"
   dependencies:
@@ -8775,20 +9164,23 @@
   dependencies:
     prelude-ls: ~1.1.2
     type-check: ~0.3.2
   checksum: 0d084a524231a8246bb10fec48cdbb35282099f6954838604f3c7fc66f2e16fa66fd9cc2f3f20a541a113c4dafdf181e822c887c8a319c9195444e6c64ac395e
   languageName: node
   linkType: hard
 
-"lib0@npm:^0.2.31, lib0@npm:^0.2.42, lib0@npm:^0.2.49, lib0@npm:^0.2.52":
-  version: 0.2.62
-  resolution: "lib0@npm:0.2.62"
+"lib0@npm:^0.2.31, lib0@npm:^0.2.42, lib0@npm:^0.2.52, lib0@npm:^0.2.72":
+  version: 0.2.73
+  resolution: "lib0@npm:0.2.73"
   dependencies:
     isomorphic.js: ^0.2.4
-  checksum: f85f063b63426a53b703bf0b77f495283b55733ad7ac2dfa29cf693fc5d8264ba0054d38cac4500bb4f9afe148b352a5b15677b9319bf500f9708afa75333867
+  bin:
+    0gentesthtml: bin/gentesthtml.js
+    0serve: bin/0serve.js
+  checksum: a9a73513ef6e91a47602ae650483eed7a8f803c512dbea3e08ef1162bd63b463230c6cdcac4ca40d01925b24218398aa3fc3c16692227384eaa326968a220815
   languageName: node
   linkType: hard
 
 "libnpmaccess@npm:6.0.3":
   version: 6.0.3
   resolution: "libnpmaccess@npm:6.0.3"
   dependencies:
@@ -9001,18 +9393,18 @@
   resolution: "lru-cache@npm:6.0.0"
   dependencies:
     yallist: ^4.0.0
   checksum: f97f499f898f23e4585742138a22f22526254fdba6d75d41a1c2526b3b6cc5747ef59c5612ba7375f42aca4f8461950e925ba08c991ead0651b4918b7c978297
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^7.4.4, lru-cache@npm:^7.5.1, lru-cache@npm:^7.7.1":
-  version: 7.16.1
-  resolution: "lru-cache@npm:7.16.1"
-  checksum: 64618e3ed4fd1203afedd9bbf5247921b1419f8e3100f20e58e5f04e741f8287bd7d04fefaad332411bb53b3a73445714b235de750cf5d310cba1fa23bd82795
+"lru-cache@npm:^7.14.1, lru-cache@npm:^7.4.4, lru-cache@npm:^7.5.1, lru-cache@npm:^7.7.1":
+  version: 7.18.3
+  resolution: "lru-cache@npm:7.18.3"
+  checksum: e550d772384709deea3f141af34b6d4fa392e2e418c1498c078de0ee63670f1f46f5eee746e8ef7e69e1c895af0d4224e62ee33e66a543a14763b0f2e74c1356
   languageName: node
   linkType: hard
 
 "ltgt@npm:^2.1.2":
   version: 2.2.1
   resolution: "ltgt@npm:2.2.1"
   checksum: 7e3874296f7538bc8087b428ac4208008d7b76916354b34a08818ca7c83958c1df10ec427eeeaad895f6b81e41e24745b18d30f89abcc21d228b94f6961d50a2
@@ -9072,14 +9464,37 @@
     promise-retry: ^2.0.1
     socks-proxy-agent: ^7.0.0
     ssri: ^9.0.0
   checksum: 2332eb9a8ec96f1ffeeea56ccefabcb4193693597b132cd110734d50f2928842e22b84cfa1508e921b8385cdfd06dda9ad68645fed62b50fff629a580f5fb72c
   languageName: node
   linkType: hard
 
+"make-fetch-happen@npm:^11.0.0, make-fetch-happen@npm:^11.0.1":
+  version: 11.0.3
+  resolution: "make-fetch-happen@npm:11.0.3"
+  dependencies:
+    agentkeepalive: ^4.2.1
+    cacache: ^17.0.0
+    http-cache-semantics: ^4.1.1
+    http-proxy-agent: ^5.0.0
+    https-proxy-agent: ^5.0.0
+    is-lambda: ^1.0.1
+    lru-cache: ^7.7.1
+    minipass: ^4.0.0
+    minipass-fetch: ^3.0.0
+    minipass-flush: ^1.0.5
+    minipass-pipeline: ^1.2.4
+    negotiator: ^0.6.3
+    promise-retry: ^2.0.1
+    socks-proxy-agent: ^7.0.0
+    ssri: ^10.0.0
+  checksum: f718d6b6945d967fa02ae8c6b1146c6e36335b0f9654c5757fd57211a5bcc13bf1dfbaa0d2fdfe8bdd13f78b0e2aa79b4d4438f824dcf0d2ea74883baae1ae31
+  languageName: node
+  linkType: hard
+
 "makeerror@npm:1.0.12":
   version: 1.0.12
   resolution: "makeerror@npm:1.0.12"
   dependencies:
     tmpl: 1.0.5
   checksum: b38a025a12c8146d6eeea5a7f2bf27d51d8ad6064da8ca9405fcf7bf9b54acd43e3b30ddd7abb9b1bfa4ddb266019133313482570ddb207de568f71ecfcf6060
   languageName: node
@@ -9095,20 +9510,29 @@
 "map-obj@npm:^4.0.0":
   version: 4.3.0
   resolution: "map-obj@npm:4.3.0"
   checksum: fbc554934d1a27a1910e842bc87b177b1a556609dd803747c85ece420692380827c6ae94a95cce4407c054fa0964be3bf8226f7f2cb2e9eeee432c7c1985684e
   languageName: node
   linkType: hard
 
+"markdown-to-jsx@npm:^7.2.0":
+  version: 7.2.0
+  resolution: "markdown-to-jsx@npm:7.2.0"
+  peerDependencies:
+    react: ">= 0.14.0"
+  checksum: ea417e684d7eec9f1beebc9423aba377116ef77c3cd83a2d622df1b9030ffef99aa9b3f431192b94f3237943a33560e6dda9be8a4c1d25187518d09986dad22f
+  languageName: node
+  linkType: hard
+
 "marked@npm:^4.2.12":
-  version: 4.2.12
-  resolution: "marked@npm:4.2.12"
+  version: 4.3.0
+  resolution: "marked@npm:4.3.0"
   bin:
     marked: bin/marked.js
-  checksum: bd551cd61028ee639d4ca2ccdfcc5a6ba4227c1b143c4538f3cde27f569dcb57df8e6313560394645b418b84a7336c07ab1e438b89b6324c29d7d8cdd3102d63
+  checksum: 0db6817893952c3ec710eb9ceafb8468bf5ae38cb0f92b7b083baa13d70b19774674be04db5b817681fa7c5c6a088f61300815e4dd75a59696f4716ad69f6260
   languageName: node
   linkType: hard
 
 "mathml-tag-names@npm:^2.1.3":
   version: 2.1.3
   resolution: "mathml-tag-names@npm:2.1.3"
   checksum: 1201a25a137d6b9e328facd67912058b8b45b19a6c4cc62641c9476195da28a275ca6e0eca070af5378b905c2b11abc1114676ba703411db0b9ce007de921ad0
@@ -9219,21 +9643,21 @@
   version: 1.0.1
   resolution: "min-indent@npm:1.0.1"
   checksum: bfc6dd03c5eaf623a4963ebd94d087f6f4bbbfd8c41329a7f09706b0cb66969c4ddd336abeb587bc44bc6f08e13bf90f0b374f9d71f9f01e04adc2cd6f083ef1
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
-  version: 2.7.2
-  resolution: "mini-css-extract-plugin@npm:2.7.2"
+  version: 2.7.5
+  resolution: "mini-css-extract-plugin@npm:2.7.5"
   dependencies:
     schema-utils: ^4.0.0
   peerDependencies:
     webpack: ^5.0.0
-  checksum: cd65611d6dc452f230c6ebba8a47bc5f5146b813b13b0b402c6f4a69f6451242eeea781152bebd31cad8ca7c7e95dac91e7e464087f18fb65b2d1097b58cf4ae
+  checksum: afc37cdfb765e8826a1babbab3cd8a99ffc4eaeabb6c013a6b3c80801e44ebc37d930b98c6f66168bb8cd545fcb2e8fc2630d72b4501a1bb8add1547c2534a53
   languageName: node
   linkType: hard
 
 "mini-svg-data-uri@npm:^1.4.4":
   version: 1.4.4
   resolution: "mini-svg-data-uri@npm:1.4.4"
   bin:
@@ -9265,20 +9689,29 @@
   resolution: "minimatch@npm:5.1.6"
   dependencies:
     brace-expansion: ^2.0.1
   checksum: 7564208ef81d7065a370f788d337cd80a689e981042cb9a1d0e6580b6c6a8c9279eba80010516e258835a988363f99f54a6f711a315089b8b42694f5da9d0d77
   languageName: node
   linkType: hard
 
-"minimatch@npm:^7.1.3":
-  version: 7.4.2
-  resolution: "minimatch@npm:7.4.2"
+"minimatch@npm:^6.1.6":
+  version: 6.2.0
+  resolution: "minimatch@npm:6.2.0"
   dependencies:
     brace-expansion: ^2.0.1
-  checksum: 9e341b04e69d5ab03e4206dcb61c8a158e3b8709628bf5e1a4eaa9f3b72c0ba925e24ad959b1f6ce6835caa5a927131d5087fae6836b69e7d99d7d5e63ef0bd8
+  checksum: 0ffb77d05bd483fcc344ba3e64a501d569e658fa6c592d94e9716ffc7925de7a8c2ac294cafa822b160bd8b2cbf7e01012917e06ffb9a85cfa9604629b3f2c04
+  languageName: node
+  linkType: hard
+
+"minimatch@npm:^7.1.3, minimatch@npm:^7.4.1, minimatch@npm:^7.4.2":
+  version: 7.4.3
+  resolution: "minimatch@npm:7.4.3"
+  dependencies:
+    brace-expansion: ^2.0.1
+  checksum: daa954231b6859e3ba0e5fbd2486986d3cae283bb69acb7ed3833c84a293f8d7edb8514360ea62c01426ba791446b2a1e1cc0d718bed15c0212cef35c59a6b95
   languageName: node
   linkType: hard
 
 "minimist-options@npm:4.1.0":
   version: 4.1.0
   resolution: "minimist-options@npm:4.1.0"
   dependencies:
@@ -9316,14 +9749,29 @@
   dependenciesMeta:
     encoding:
       optional: true
   checksum: 3f216be79164e915fc91210cea1850e488793c740534985da017a4cbc7a5ff50506956d0f73bb0cb60e4fe91be08b6b61ef35101706d3ef5da2c8709b5f08f91
   languageName: node
   linkType: hard
 
+"minipass-fetch@npm:^3.0.0":
+  version: 3.0.1
+  resolution: "minipass-fetch@npm:3.0.1"
+  dependencies:
+    encoding: ^0.1.13
+    minipass: ^4.0.0
+    minipass-sized: ^1.0.3
+    minizlib: ^2.1.2
+  dependenciesMeta:
+    encoding:
+      optional: true
+  checksum: b5eecf462ab8409891e4b8a786260e411304b958e45e10820b0a5d31f7841ccbce5f85e49934a34fdb94501206c273bde1988b9c0ad1625bdfb9883d90285420
+  languageName: node
+  linkType: hard
+
 "minipass-flush@npm:^1.0.5":
   version: 1.0.5
   resolution: "minipass-flush@npm:1.0.5"
   dependencies:
     minipass: ^3.0.0
   checksum: 56269a0b22bad756a08a94b1ffc36b7c9c5de0735a4dd1ab2b06c066d795cfd1f0ac44a0fcae13eece5589b908ecddc867f04c745c7009be0b566421ea0944cf
   languageName: node
@@ -9362,18 +9810,18 @@
   resolution: "minipass@npm:3.3.6"
   dependencies:
     yallist: ^4.0.0
   checksum: a30d083c8054cee83cdcdc97f97e4641a3f58ae743970457b1489ce38ee1167b3aaf7d815cd39ec7a99b9c40397fd4f686e83750e73e652b21cb516f6d845e48
   languageName: node
   linkType: hard
 
-"minipass@npm:^4.0.0":
-  version: 4.0.3
-  resolution: "minipass@npm:4.0.3"
-  checksum: a09f405e2f380ae7f6ee0cbb53b45c1fcc1b6c70fc3896f4d20649d92a10e61892c57bd9960a64cedf6c90b50022cb6c195905b515039c335b423202f99e6f18
+"minipass@npm:^4.0.0, minipass@npm:^4.0.2, minipass@npm:^4.2.4":
+  version: 4.2.5
+  resolution: "minipass@npm:4.2.5"
+  checksum: 4f9c19af23a5d4a9e7156feefc9110634b178a8cff8f8271af16ec5ebf7e221725a97429952c856f5b17b30c2065ebd24c81722d90c93d2122611d75b952b48f
   languageName: node
   linkType: hard
 
 "minizlib@npm:^2.1.1, minizlib@npm:^2.1.2":
   version: 2.1.2
   resolution: "minizlib@npm:2.1.2"
   dependencies:
@@ -9441,19 +9889,19 @@
   version: 0.0.8
   resolution: "mute-stream@npm:0.0.8"
   checksum: ff48d251fc3f827e5b1206cda0ffdaec885e56057ee86a3155e1951bc940fd5f33531774b1cc8414d7668c10a8907f863f6561875ee6e8768931a62121a531a1
   languageName: node
   linkType: hard
 
 "nanoid@npm:^3.3.4":
-  version: 3.3.4
-  resolution: "nanoid@npm:3.3.4"
+  version: 3.3.6
+  resolution: "nanoid@npm:3.3.6"
   bin:
     nanoid: bin/nanoid.cjs
-  checksum: 2fddd6dee994b7676f008d3ffa4ab16035a754f4bb586c61df5a22cf8c8c94017aadd360368f47d653829e0569a92b129979152ff97af23a558331e47e37cd9c
+  checksum: 7d0eda657002738aa5206107bd0580aead6c95c460ef1bdd0b1a87a9c7ae6277ac2e9b945306aaa5b32c6dcb7feaf462d0f552e7f8b5718abfc6ead5c94a71b3
   languageName: node
   linkType: hard
 
 "napi-macros@npm:~2.0.0":
   version: 2.0.0
   resolution: "napi-macros@npm:2.0.0"
   checksum: 30384819386977c1f82034757014163fa60ab3c5a538094f778d38788bebb52534966279956f796a92ea771c7f8ae072b975df65de910d051ffbdc927f62320c
@@ -9584,33 +10032,33 @@
 "node-releases@npm:^2.0.8":
   version: 2.0.10
   resolution: "node-releases@npm:2.0.10"
   checksum: d784ecde25696a15d449c4433077f5cce620ed30a1656c4abf31282bfc691a70d9618bae6868d247a67914d1be5cc4fde22f65a05f4398cdfb92e0fc83cadfbc
   languageName: node
   linkType: hard
 
-"nopt@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "nopt@npm:5.0.0"
+"nopt@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "nopt@npm:6.0.0"
   dependencies:
-    abbrev: 1
+    abbrev: ^1.0.0
   bin:
     nopt: bin/nopt.js
-  checksum: d35fdec187269503843924e0114c0c6533fb54bbf1620d0f28b4b60ba01712d6687f62565c55cc20a504eff0fbe5c63e22340c3fad549ad40469ffb611b04f2f
+  checksum: 82149371f8be0c4b9ec2f863cc6509a7fd0fa729929c009f3a58e4eb0c9e4cae9920e8f1f8eb46e7d032fec8fb01bede7f0f41a67eb3553b7b8e14fa53de1dac
   languageName: node
   linkType: hard
 
-"nopt@npm:^6.0.0":
-  version: 6.0.0
-  resolution: "nopt@npm:6.0.0"
+"nopt@npm:^7.0.0":
+  version: 7.1.0
+  resolution: "nopt@npm:7.1.0"
   dependencies:
-    abbrev: ^1.0.0
+    abbrev: ^2.0.0
   bin:
     nopt: bin/nopt.js
-  checksum: 82149371f8be0c4b9ec2f863cc6509a7fd0fa729929c009f3a58e4eb0c9e4cae9920e8f1f8eb46e7d032fec8fb01bede7f0f41a67eb3553b7b8e14fa53de1dac
+  checksum: 77185170d491b2ffdda0c72ce12dcf222b670814b7fb5ba1b750c708a6e5421b5607345c1f6341602476c8ef0a26929f5b861efa284e106c60b4baa6e6edb262
   languageName: node
   linkType: hard
 
 "normalize-package-data@npm:^2.3.2, normalize-package-data@npm:^2.5.0":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
@@ -9642,14 +10090,26 @@
     is-core-module: ^2.8.1
     semver: ^7.3.5
     validate-npm-package-license: ^3.0.4
   checksum: 292e0aa740e73d62f84bbd9d55d4bfc078155f32d5d7572c32c9807f96d543af0f43ff7e5c80bfa6238667123fd68bd83cd412eae9b27b85b271fb041f624528
   languageName: node
   linkType: hard
 
+"normalize-package-data@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "normalize-package-data@npm:5.0.0"
+  dependencies:
+    hosted-git-info: ^6.0.0
+    is-core-module: ^2.8.1
+    semver: ^7.3.5
+    validate-npm-package-license: ^3.0.4
+  checksum: a459f05eaf7c2b643c61234177f08e28064fde97da15800e3d3ac0404e28450d43ac46fc95fbf6407a9bf20af4c58505ad73458a912dc1517f8c1687b1d68c27
+  languageName: node
+  linkType: hard
+
 "normalize-path@npm:^3.0.0":
   version: 3.0.0
   resolution: "normalize-path@npm:3.0.0"
   checksum: 88eeb4da891e10b1318c4b2476b6e2ecbeb5ff97d946815ffea7794c31a89017c70d7f34b3c2ebf23ef4e9fc9fb99f7dffe36da22011b5b5c6ffa34f4873ec20
   languageName: node
   linkType: hard
 
@@ -9667,48 +10127,85 @@
   resolution: "npm-bundled@npm:2.0.1"
   dependencies:
     npm-normalize-package-bin: ^2.0.0
   checksum: 7747293985c48c5268871efe691545b03731cb80029692000cbdb0b3344b9617be5187aa36281cabbe6b938e3651b4e87236d1c31f9e645eef391a1a779413e6
   languageName: node
   linkType: hard
 
+"npm-bundled@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "npm-bundled@npm:3.0.0"
+  dependencies:
+    npm-normalize-package-bin: ^3.0.0
+  checksum: 110859c2d6dcd7941dac0932a29171cbde123060486a4b6e897aaf5e025abeb3d9ffcdfe9e9271992e6396b2986c2c534f1029a45a7c196f1257fa244305dbf8
+  languageName: node
+  linkType: hard
+
 "npm-install-checks@npm:^5.0.0":
   version: 5.0.0
   resolution: "npm-install-checks@npm:5.0.0"
   dependencies:
     semver: ^7.1.1
   checksum: 0e7d1aae52b1fe9d3a0fd4a008850c7047931722dd49ee908afd13fd0297ac5ddb10964d9c59afcdaaa2ca04b51d75af2788f668c729ae71fec0e4cdac590ffc
   languageName: node
   linkType: hard
 
+"npm-install-checks@npm:^6.0.0":
+  version: 6.1.0
+  resolution: "npm-install-checks@npm:6.1.0"
+  dependencies:
+    semver: ^7.1.1
+  checksum: efbb4deac45bfe18ab8f619801f736f675ee9f80a60eeafc9fbf8f4657816b67d8e1b1a8dc50d47ee4226727f96e111974a752c4861e1aef1cc2e2ed70581e7c
+  languageName: node
+  linkType: hard
+
 "npm-normalize-package-bin@npm:^1.0.1":
   version: 1.0.1
   resolution: "npm-normalize-package-bin@npm:1.0.1"
   checksum: ae7f15155a1e3ace2653f12ddd1ee8eaa3c84452fdfbf2f1943e1de264e4b079c86645e2c55931a51a0a498cba31f70022a5219d5665fbcb221e99e58bc70122
   languageName: node
   linkType: hard
 
 "npm-normalize-package-bin@npm:^2.0.0":
   version: 2.0.0
   resolution: "npm-normalize-package-bin@npm:2.0.0"
   checksum: 7c5379f9b188b564c4332c97bdd9a5d6b7b15f02b5823b00989d6a0e6fb31eb0280f02b0a924f930e1fcaf00e60fae333aec8923d2a4c7747613c7d629d8aa25
   languageName: node
   linkType: hard
 
+"npm-normalize-package-bin@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "npm-normalize-package-bin@npm:3.0.0"
+  checksum: 6a34886c150b0f5302aad52a9446e5c939aa14eeb462323e75681517b36c6b9eaef83e1f5bc2d7e5154b3b752cbce81bed05e290db3f1f7edf857cbb895e35c0
+  languageName: node
+  linkType: hard
+
 "npm-package-arg@npm:8.1.1":
   version: 8.1.1
   resolution: "npm-package-arg@npm:8.1.1"
   dependencies:
     hosted-git-info: ^3.0.6
     semver: ^7.0.0
     validate-npm-package-name: ^3.0.0
   checksum: 406c59f92d8fac5acbd1df62f4af8075e925af51131b6bc66245641ea71ddb0e60b3e2c56fafebd4e8ffc3ba0453e700a221a36a44740dc9f7488cec97ae4c55
   languageName: node
   linkType: hard
 
+"npm-package-arg@npm:^10.0.0, npm-package-arg@npm:^10.1.0":
+  version: 10.1.0
+  resolution: "npm-package-arg@npm:10.1.0"
+  dependencies:
+    hosted-git-info: ^6.0.0
+    proc-log: ^3.0.0
+    semver: ^7.3.5
+    validate-npm-package-name: ^5.0.0
+  checksum: 8fe4b6a742502345e4836ed42fdf26c544c9f75563c476c67044a481ada6e81f71b55462489c7e1899d516e4347150e58028036a90fa11d47e320bcc9365fd30
+  languageName: node
+  linkType: hard
+
 "npm-package-arg@npm:^9.0.0, npm-package-arg@npm:^9.0.1":
   version: 9.1.2
   resolution: "npm-package-arg@npm:9.1.2"
   dependencies:
     hosted-git-info: ^5.0.0
     proc-log: ^2.0.1
     semver: ^7.3.5
@@ -9741,38 +10238,59 @@
     npm-normalize-package-bin: ^2.0.0
   bin:
     npm-packlist: bin/index.js
   checksum: 94cc9c66740e8f80243301de85eb0a2cec5bbd570c3f26b6ad7af1a3eca155f7e810580dc7ea4448f12a8fd82f6db307e7132a5fe69e157eb45b325acadeb22a
   languageName: node
   linkType: hard
 
+"npm-packlist@npm:^7.0.0":
+  version: 7.0.4
+  resolution: "npm-packlist@npm:7.0.4"
+  dependencies:
+    ignore-walk: ^6.0.0
+  checksum: 5ffa1f8f0b32141a60a66713fa3ed03b8ee4800b1ed6b59194d03c3c85da88f3fc21e1de29b665f322678bae85198732b16aa76c0a7cb0e283f9e0db50752233
+  languageName: node
+  linkType: hard
+
 "npm-pick-manifest@npm:^7.0.0":
   version: 7.0.2
   resolution: "npm-pick-manifest@npm:7.0.2"
   dependencies:
     npm-install-checks: ^5.0.0
     npm-normalize-package-bin: ^2.0.0
     npm-package-arg: ^9.0.0
     semver: ^7.3.5
   checksum: a93ec449c12219a2be8556837db9ac5332914f304a69469bb6f1f47717adc6e262aa318f79166f763512688abd9c4e4b6a2d83b2dd19753a7abe5f0360f2c8bc
   languageName: node
   linkType: hard
 
-"npm-registry-fetch@npm:13.3.0":
-  version: 13.3.0
-  resolution: "npm-registry-fetch@npm:13.3.0"
+"npm-pick-manifest@npm:^8.0.0, npm-pick-manifest@npm:^8.0.1":
+  version: 8.0.1
+  resolution: "npm-pick-manifest@npm:8.0.1"
   dependencies:
-    make-fetch-happen: ^10.0.6
-    minipass: ^3.1.6
-    minipass-fetch: ^2.0.3
+    npm-install-checks: ^6.0.0
+    npm-normalize-package-bin: ^3.0.0
+    npm-package-arg: ^10.0.0
+    semver: ^7.3.5
+  checksum: b8e16f2fbcc40ba7d1405c9b566bcee32488c6709f883207f709b0715ed34e2f3f3bc5bf5cb9563d6aa23cb878102bf0011ba22cce9235caa9a0349784b48ecd
+  languageName: node
+  linkType: hard
+
+"npm-registry-fetch@npm:14.0.3, npm-registry-fetch@npm:^14.0.0, npm-registry-fetch@npm:^14.0.3":
+  version: 14.0.3
+  resolution: "npm-registry-fetch@npm:14.0.3"
+  dependencies:
+    make-fetch-happen: ^11.0.0
+    minipass: ^4.0.0
+    minipass-fetch: ^3.0.0
     minipass-json-stream: ^1.0.1
     minizlib: ^2.1.2
-    npm-package-arg: ^9.0.1
-    proc-log: ^2.0.0
-  checksum: f153e471b7204eef260d4b774087291981a0d2909db7568540d77759409300d10f8e2a464af0da15ab1c4da4d6285c5d746ba09707dd55a4bd66f5f0ceafcf64
+    npm-package-arg: ^10.0.0
+    proc-log: ^3.0.0
+  checksum: 451224e7272c8418000f6a0e27fb01d7eb5231bcd98dbd42acac3f275f0b5317590c152860cc84afa706427121b59f9422939e00af5690442b70e64cfa39de0a
   languageName: node
   linkType: hard
 
 "npm-registry-fetch@npm:^13.0.0, npm-registry-fetch@npm:^13.0.1":
   version: 13.3.1
   resolution: "npm-registry-fetch@npm:13.3.1"
   dependencies:
@@ -9813,48 +10331,60 @@
   resolution: "npm-run-path@npm:4.0.1"
   dependencies:
     path-key: ^3.0.0
   checksum: 5374c0cea4b0bbfdfae62da7bbdf1e1558d338335f4cacf2515c282ff358ff27b2ecb91ffa5330a8b14390ac66a1e146e10700440c1ab868208430f56b5f4d23
   languageName: node
   linkType: hard
 
-"npmlog@npm:^6.0.0, npmlog@npm:^6.0.2":
+"npmlog@npm:6.0.2, npmlog@npm:^6.0.0, npmlog@npm:^6.0.2":
   version: 6.0.2
   resolution: "npmlog@npm:6.0.2"
   dependencies:
     are-we-there-yet: ^3.0.0
     console-control-strings: ^1.1.0
     gauge: ^4.0.3
     set-blocking: ^2.0.0
   checksum: ae238cd264a1c3f22091cdd9e2b106f684297d3c184f1146984ecbe18aaa86343953f26b9520dedd1b1372bc0316905b736c1932d778dbeb1fcf5a1001390e2a
   languageName: node
   linkType: hard
 
+"npmlog@npm:^7.0.1":
+  version: 7.0.1
+  resolution: "npmlog@npm:7.0.1"
+  dependencies:
+    are-we-there-yet: ^4.0.0
+    console-control-strings: ^1.1.0
+    gauge: ^5.0.0
+    set-blocking: ^2.0.0
+  checksum: caabeb1f557c1094ad7ed3275b968b83ccbaefc133f17366ebb9fe8eb44e1aace28c31419d6244bfc0422aede1202875d555fe6661978bf04386f6cf617f43a4
+  languageName: node
+  linkType: hard
+
 "nwsapi@npm:^2.2.2":
   version: 2.2.2
   resolution: "nwsapi@npm:2.2.2"
   checksum: 43769106292bc95f776756ca2f3513dab7b4d506a97c67baec32406447841a35f65f29c1f95ab5d42785210fd41668beed33ca16fa058780be43b101ad73e205
   languageName: node
   linkType: hard
 
-"nx@npm:15.7.2, nx@npm:>=15.5.2 < 16":
-  version: 15.7.2
-  resolution: "nx@npm:15.7.2"
-  dependencies:
-    "@nrwl/cli": 15.7.2
-    "@nrwl/nx-darwin-arm64": 15.7.2
-    "@nrwl/nx-darwin-x64": 15.7.2
-    "@nrwl/nx-linux-arm-gnueabihf": 15.7.2
-    "@nrwl/nx-linux-arm64-gnu": 15.7.2
-    "@nrwl/nx-linux-arm64-musl": 15.7.2
-    "@nrwl/nx-linux-x64-gnu": 15.7.2
-    "@nrwl/nx-linux-x64-musl": 15.7.2
-    "@nrwl/nx-win32-arm64-msvc": 15.7.2
-    "@nrwl/nx-win32-x64-msvc": 15.7.2
-    "@nrwl/tao": 15.7.2
+"nx@npm:15.8.9, nx@npm:>=15.5.2 < 16":
+  version: 15.8.9
+  resolution: "nx@npm:15.8.9"
+  dependencies:
+    "@nrwl/cli": 15.8.9
+    "@nrwl/nx-darwin-arm64": 15.8.9
+    "@nrwl/nx-darwin-x64": 15.8.9
+    "@nrwl/nx-linux-arm-gnueabihf": 15.8.9
+    "@nrwl/nx-linux-arm64-gnu": 15.8.9
+    "@nrwl/nx-linux-arm64-musl": 15.8.9
+    "@nrwl/nx-linux-x64-gnu": 15.8.9
+    "@nrwl/nx-linux-x64-musl": 15.8.9
+    "@nrwl/nx-win32-arm64-msvc": 15.8.9
+    "@nrwl/nx-win32-x64-msvc": 15.8.9
+    "@nrwl/tao": 15.8.9
     "@parcel/watcher": 2.0.4
     "@yarnpkg/lockfile": ^1.1.0
     "@yarnpkg/parsers": ^3.0.0-rc.18
     "@zkochan/js-yaml": 0.0.6
     axios: ^1.0.0
     chalk: ^4.1.0
     cli-cursor: 3.1.0
@@ -9909,26 +10439,26 @@
   peerDependenciesMeta:
     "@swc-node/register":
       optional: true
     "@swc/core":
       optional: true
   bin:
     nx: bin/nx.js
-  checksum: c5765575146bb94f54c1da3d6dec600e6414c0cc64c198821a3de10a72583933f1a752a61452b74f02492e3518f4ead3c287416173b1bb3bbc15ce82bd8d2bb4
+  checksum: bbd8417a2d1edea9d710a5841ee7d21d8744f92bf3d45659da48642fd0a4ba8322ed422b6214528ca777377f853ec0599683c18a8107e59c9fc2e65b1ded7d1e
   languageName: node
   linkType: hard
 
 "object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
   languageName: node
   linkType: hard
 
-"object-inspect@npm:^1.12.2, object-inspect@npm:^1.9.0":
+"object-inspect@npm:^1.12.3, object-inspect@npm:^1.9.0":
   version: 1.12.3
   resolution: "object-inspect@npm:1.12.3"
   checksum: dabfd824d97a5f407e6d5d24810d888859f6be394d8b733a77442b277e0808860555176719c5905e765e3743a7cada6b8b0a3b85e5331c530fd418cc8ae991db
   languageName: node
   linkType: hard
 
 "object-keys@npm:^1.1.1":
@@ -10008,21 +10538,21 @@
   dependencies:
     mimic-fn: ^2.1.0
   checksum: 2478859ef817fc5d4e9c2f9e5728512ddd1dbc9fb7829ad263765bb6d3b91ce699d6e2332eef6b7dff183c2f490bd3349f1666427eaba4469fba0ac38dfd0d34
   languageName: node
   linkType: hard
 
 "open@npm:^8.4.0":
-  version: 8.4.1
-  resolution: "open@npm:8.4.1"
+  version: 8.4.2
+  resolution: "open@npm:8.4.2"
   dependencies:
     define-lazy-prop: ^2.0.0
     is-docker: ^2.1.1
     is-wsl: ^2.2.0
-  checksum: dbe8e1d98889df60b5179eab8b94b9591744d1f0033bce1a9a10738ba140bd9d625d6bcde7ff9f043e379aafb918975c2daa03b87cef13eb046ac18ed807f06d
+  checksum: 6388bfff21b40cb9bd8f913f9130d107f2ed4724ea81a8fd29798ee322b361ca31fa2cdfb491a5c31e43a3996cfe9566741238c7a741ada8d7af1cb78d85cf26
   languageName: node
   linkType: hard
 
 "optionator@npm:^0.8.1":
   version: 0.8.3
   resolution: "optionator@npm:0.8.3"
   dependencies:
@@ -10203,17 +10733,17 @@
   resolution: "p-waterfall@npm:2.1.1"
   dependencies:
     p-reduce: ^2.0.0
   checksum: 8588bb8b004ee37e559c7e940a480c1742c42725d477b0776ff30b894920a3e48bddf8f60aa0ae82773e500a8fc99d75e947c450e0c2ce187aff72cc1b248f6d
   languageName: node
   linkType: hard
 
-"pacote@npm:13.6.1":
-  version: 13.6.1
-  resolution: "pacote@npm:13.6.1"
+"pacote@npm:13.6.2, pacote@npm:^13.6.1":
+  version: 13.6.2
+  resolution: "pacote@npm:13.6.2"
   dependencies:
     "@npmcli/git": ^3.0.0
     "@npmcli/installed-package-contents": ^1.0.7
     "@npmcli/promise-spawn": ^3.0.0
     "@npmcli/run-script": ^4.1.0
     cacache: ^16.0.0
     chownr: ^2.0.0
@@ -10230,66 +10760,63 @@
     read-package-json: ^5.0.0
     read-package-json-fast: ^2.0.3
     rimraf: ^3.0.2
     ssri: ^9.0.0
     tar: ^6.1.11
   bin:
     pacote: lib/bin.js
-  checksum: 26cebb59aea93d03ad051d82c4f2300beb333ded0f16ba92cfe976b5600157bd1ee034afe1c86406bbe5eacd51d413797939b08aa58adcf73f7680aead9e667f
+  checksum: a7b7f97094ab570a23e1c174537e9953a4d53176cc4b18bac77d7728bd89e2b9fa331d0f78fa463add03df79668a918bbdaa2750819504ee39242063abf53c6e
   languageName: node
   linkType: hard
 
-"pacote@npm:^13.0.3, pacote@npm:^13.6.1":
-  version: 13.6.2
-  resolution: "pacote@npm:13.6.2"
-  dependencies:
-    "@npmcli/git": ^3.0.0
-    "@npmcli/installed-package-contents": ^1.0.7
-    "@npmcli/promise-spawn": ^3.0.0
-    "@npmcli/run-script": ^4.1.0
-    cacache: ^16.0.0
-    chownr: ^2.0.0
-    fs-minipass: ^2.1.0
-    infer-owner: ^1.0.4
-    minipass: ^3.1.6
-    mkdirp: ^1.0.4
-    npm-package-arg: ^9.0.0
-    npm-packlist: ^5.1.0
-    npm-pick-manifest: ^7.0.0
-    npm-registry-fetch: ^13.0.1
-    proc-log: ^2.0.0
+"pacote@npm:^15.0.0, pacote@npm:^15.0.8":
+  version: 15.1.1
+  resolution: "pacote@npm:15.1.1"
+  dependencies:
+    "@npmcli/git": ^4.0.0
+    "@npmcli/installed-package-contents": ^2.0.1
+    "@npmcli/promise-spawn": ^6.0.1
+    "@npmcli/run-script": ^6.0.0
+    cacache: ^17.0.0
+    fs-minipass: ^3.0.0
+    minipass: ^4.0.0
+    npm-package-arg: ^10.0.0
+    npm-packlist: ^7.0.0
+    npm-pick-manifest: ^8.0.0
+    npm-registry-fetch: ^14.0.0
+    proc-log: ^3.0.0
     promise-retry: ^2.0.1
-    read-package-json: ^5.0.0
-    read-package-json-fast: ^2.0.3
-    rimraf: ^3.0.2
-    ssri: ^9.0.0
+    read-package-json: ^6.0.0
+    read-package-json-fast: ^3.0.0
+    sigstore: ^1.0.0
+    ssri: ^10.0.0
     tar: ^6.1.11
   bin:
     pacote: lib/bin.js
-  checksum: a7b7f97094ab570a23e1c174537e9953a4d53176cc4b18bac77d7728bd89e2b9fa331d0f78fa463add03df79668a918bbdaa2750819504ee39242063abf53c6e
+  checksum: 109388e873615cdad342f5dbd3639389c00aaac2c84b824dcb1a9460b4cf1c66264387b1d0200b1769abda7feca94165804d1308ca5e59904ae24d489d3bfb13
   languageName: node
   linkType: hard
 
 "parent-module@npm:^1.0.0":
   version: 1.0.1
   resolution: "parent-module@npm:1.0.1"
   dependencies:
     callsites: ^3.0.0
   checksum: 6ba8b255145cae9470cf5551eb74be2d22281587af787a2626683a6c20fbb464978784661478dd2a3f1dad74d1e802d403e1b03c1a31fab310259eec8ac560ff
   languageName: node
   linkType: hard
 
-"parse-conflict-json@npm:^2.0.1":
-  version: 2.0.2
-  resolution: "parse-conflict-json@npm:2.0.2"
+"parse-conflict-json@npm:^3.0.0":
+  version: 3.0.1
+  resolution: "parse-conflict-json@npm:3.0.1"
   dependencies:
-    json-parse-even-better-errors: ^2.3.1
-    just-diff: ^5.0.1
+    json-parse-even-better-errors: ^3.0.0
+    just-diff: ^6.0.0
     just-diff-apply: ^5.2.0
-  checksum: 076f65c958696586daefb153f59d575dfb59648be43116a21b74d5ff69ec63dd56f585a27cc2da56d8e64ca5abf0373d6619b8330c035131f8d1e990c8406378
+  checksum: d8d2656bc02d4df36846366baec36b419da2fe944e31298719a4d28d28f772aa7cad2a69d01f6f329918e7c298ac481d1e6a9138d62d5662d5620a74f794af8f
   languageName: node
   linkType: hard
 
 "parse-json@npm:^4.0.0":
   version: 4.0.0
   resolution: "parse-json@npm:4.0.0"
   dependencies:
@@ -10348,28 +10875,28 @@
 "path-browserify@npm:^1.0.0":
   version: 1.0.1
   resolution: "path-browserify@npm:1.0.1"
   checksum: c6d7fa376423fe35b95b2d67990060c3ee304fc815ff0a2dc1c6c3cfaff2bd0d572ee67e18f19d0ea3bbe32e8add2a05021132ac40509416459fffee35200699
   languageName: node
   linkType: hard
 
-"path-exists@npm:4.0.0, path-exists@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "path-exists@npm:4.0.0"
-  checksum: 505807199dfb7c50737b057dd8d351b82c033029ab94cb10a657609e00c1bc53b951cfdbccab8de04c5584d5eff31128ce6afd3db79281874a5ef2adbba55ed1
-  languageName: node
-  linkType: hard
-
 "path-exists@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-exists@npm:3.0.0"
   checksum: 96e92643aa34b4b28d0de1cd2eba52a1c5313a90c6542d03f62750d82480e20bfa62bc865d5cfc6165f5fcd5aeb0851043c40a39be5989646f223300021bae0a
   languageName: node
   linkType: hard
 
+"path-exists@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "path-exists@npm:4.0.0"
+  checksum: 505807199dfb7c50737b057dd8d351b82c033029ab94cb10a657609e00c1bc53b951cfdbccab8de04c5584d5eff31128ce6afd3db79281874a5ef2adbba55ed1
+  languageName: node
+  linkType: hard
+
 "path-is-absolute@npm:^1.0.0":
   version: 1.0.1
   resolution: "path-is-absolute@npm:1.0.1"
   checksum: 060840f92cf8effa293bcc1bea81281bd7d363731d214cbe5c227df207c34cd727430f70c6037b5159c8a870b9157cba65e775446b0ab06fd5ecc7e54615a3b8
   languageName: node
   linkType: hard
 
@@ -10390,14 +10917,24 @@
 "path-parse@npm:^1.0.7":
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
+"path-scurry@npm:^1.6.1":
+  version: 1.6.3
+  resolution: "path-scurry@npm:1.6.3"
+  dependencies:
+    lru-cache: ^7.14.1
+    minipass: ^4.0.2
+  checksum: 814ebd7f8df717e2381dc707ba3a3ddf84d0a4f9d653036c7554cb1fea632d4d78eb17dd5f4c85111b78ba8b8c0a5b59c756645c9d343bdacacda4ba8d1626c2
+  languageName: node
+  linkType: hard
+
 "path-type@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-type@npm:3.0.0"
   dependencies:
     pify: ^3.0.0
   checksum: 735b35e256bad181f38fa021033b1c33cfbe62ead42bb2222b56c210e42938eecb272ae1949f3b6db4ac39597a61b44edd8384623ec4d79bfdc9a9c0f12537a6
   languageName: node
@@ -10540,15 +11077,15 @@
   resolution: "postcss-safe-parser@npm:6.0.0"
   peerDependencies:
     postcss: ^8.3.3
   checksum: 06c733eaad83a3954367e7ee02ddfe3796e7a44d4299ccf9239f40964a4daac153c7d77613f32964b5a86c0c6c2f6167738f31d578b73b17cb69d0c4446f0ebe
   languageName: node
   linkType: hard
 
-"postcss-selector-parser@npm:^6.0.11, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
+"postcss-selector-parser@npm:^6.0.10, postcss-selector-parser@npm:^6.0.11, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
   version: 6.0.11
   resolution: "postcss-selector-parser@npm:6.0.11"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
   checksum: 0b01aa9c2d2c8dbeb51e9b204796b678284be9823abc8d6d40a8b16d4149514e922c264a8ed4deb4d6dbced564b9be390f5942c058582d8656351516d6c49cde
   languageName: node
@@ -10592,40 +11129,58 @@
   dependencies:
     fast-diff: ^1.1.2
   checksum: 00ce8011cf6430158d27f9c92cfea0a7699405633f7f1d4a45f07e21bf78e99895911cbcdc3853db3a824201a7c745bd49bfea8abd5fb9883e765a90f74f8392
   languageName: node
   linkType: hard
 
 "prettier@npm:^2.8.4":
-  version: 2.8.4
-  resolution: "prettier@npm:2.8.4"
+  version: 2.8.7
+  resolution: "prettier@npm:2.8.7"
   bin:
     prettier: bin-prettier.js
-  checksum: c173064bf3df57b6d93d19aa98753b9b9dd7657212e33b41ada8e2e9f9884066bb9ca0b4005b89b3ab137efffdf8fbe0b462785aba20364798ff4303aadda57e
+  checksum: fdc8f2616f099f5f0d685907f4449a70595a0fc1d081a88919604375989e0d5e9168d6121d8cc6861f21990b31665828e00472544d785d5940ea08a17660c3a6
   languageName: node
   linkType: hard
 
-"pretty-format@npm:^29.0.0, pretty-format@npm:^29.4.3":
+"pretty-format@npm:29.4.3":
   version: 29.4.3
   resolution: "pretty-format@npm:29.4.3"
   dependencies:
     "@jest/schemas": ^29.4.3
     ansi-styles: ^5.0.0
     react-is: ^18.0.0
   checksum: 3258b9a010bd79b3cf73783ad1e4592b6326fc981b6e31b742f316f14e7fbac09b48a9dbf274d092d9bde404db9fe16f518370e121837dc078a597392e6e5cc5
   languageName: node
   linkType: hard
 
+"pretty-format@npm:^29.0.0, pretty-format@npm:^29.5.0":
+  version: 29.5.0
+  resolution: "pretty-format@npm:29.5.0"
+  dependencies:
+    "@jest/schemas": ^29.4.3
+    ansi-styles: ^5.0.0
+    react-is: ^18.0.0
+  checksum: 4065356b558e6db25b4d41a01efb386935a6c06a0c9c104ef5ce59f2f476b8210edb8b3949b386e60ada0a6dc5ebcb2e6ccddc8c64dfd1a9943c3c3a9e7eaf89
+  languageName: node
+  linkType: hard
+
 "proc-log@npm:^2.0.0, proc-log@npm:^2.0.1":
   version: 2.0.1
   resolution: "proc-log@npm:2.0.1"
   checksum: f6f23564ff759097db37443e6e2765af84979a703d2c52c1b9df506ee9f87caa101ba49d8fdc115c1a313ec78e37e8134704e9069e6a870f3499d98bb24c436f
   languageName: node
   linkType: hard
 
+"proc-log@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "proc-log@npm:3.0.0"
+  checksum: 02b64e1b3919e63df06f836b98d3af002b5cd92655cab18b5746e37374bfb73e03b84fe305454614b34c25b485cc687a9eebdccf0242cda8fda2475dd2c97e02
+  languageName: node
+  linkType: hard
+
 "process-nextick-args@npm:~2.0.0":
   version: 2.0.1
   resolution: "process-nextick-args@npm:2.0.1"
   checksum: 1d38588e520dab7cea67cbbe2efdd86a10cc7a074c09657635e34f035277b59fbb57d09d8638346bf7090f8e8ebc070c96fa5fd183b777fff4f5edff5e9466cf
   languageName: node
   linkType: hard
 
@@ -10735,14 +11290,21 @@
 "punycode@npm:^2.1.0, punycode@npm:^2.1.1":
   version: 2.3.0
   resolution: "punycode@npm:2.3.0"
   checksum: 39f760e09a2a3bbfe8f5287cf733ecdad69d6af2fe6f97ca95f24b8921858b91e9ea3c9eeec6e08cede96181b3bb33f95c6ffd8c77e63986508aa2e8159fa200
   languageName: node
   linkType: hard
 
+"pure-rand@npm:^6.0.0":
+  version: 6.0.1
+  resolution: "pure-rand@npm:6.0.1"
+  checksum: 4bb565399993b815658a72e359f574ce4f04827a42a905105d61163ae86f456d91595a0e4241e7bce04328fae0638ae70ac0428d93ecb55971c465bd084f8648
+  languageName: node
+  linkType: hard
+
 "q@npm:^1.5.1":
   version: 1.5.1
   resolution: "q@npm:1.5.1"
   checksum: 147baa93c805bc1200ed698bdf9c72e9e42c05f96d007e33a558b5fdfd63e5ea130e99313f28efc1783e90e6bdb4e48b67a36fcc026b7b09202437ae88a1fb12
   languageName: node
   linkType: hard
 
@@ -10814,31 +11376,41 @@
 "read-cmd-shim@npm:3.0.0":
   version: 3.0.0
   resolution: "read-cmd-shim@npm:3.0.0"
   checksum: b518c6026f3320e30b692044f6ff5c4dc80f9c71261296da8994101b569b26b12b8e5df397bba2d4691dd3a3a2f770a1eca7be18a69ec202fac6dcfadc5016fd
   languageName: node
   linkType: hard
 
-"read-cmd-shim@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "read-cmd-shim@npm:3.0.1"
-  checksum: 79fe66aa78eddcca8dc196765ae3168b3a56e2b69ba54071525eb00a9eeee8cc83b3d5f784432c3d8ce868787fdc059b1a1e0b605246b5108c9003fc927ea263
+"read-cmd-shim@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "read-cmd-shim@npm:4.0.0"
+  checksum: 2fb5a8a38984088476f559b17c6a73324a5db4e77e210ae0aab6270480fd85c355fc990d1c79102e25e555a8201606ed12844d6e3cd9f35d6a1518791184e05b
   languageName: node
   linkType: hard
 
-"read-package-json-fast@npm:^2.0.2, read-package-json-fast@npm:^2.0.3":
+"read-package-json-fast@npm:^2.0.3":
   version: 2.0.3
   resolution: "read-package-json-fast@npm:2.0.3"
   dependencies:
     json-parse-even-better-errors: ^2.3.0
     npm-normalize-package-bin: ^1.0.1
   checksum: fca37b3b2160b9dda7c5588b767f6a2b8ce68d03a044000e568208e20bea0cf6dd2de17b90740ce8da8b42ea79c0b3859649dadf29510bbe77224ea65326a903
   languageName: node
   linkType: hard
 
+"read-package-json-fast@npm:^3.0.0, read-package-json-fast@npm:^3.0.2":
+  version: 3.0.2
+  resolution: "read-package-json-fast@npm:3.0.2"
+  dependencies:
+    json-parse-even-better-errors: ^3.0.0
+    npm-normalize-package-bin: ^3.0.0
+  checksum: 8d406869f045f1d76e2a99865a8fd1c1af9c1dc06200b94d2b07eef87ed734b22703a8d72e1cd36ea36cc48e22020bdd187f88243c7dd0563f72114d38c17072
+  languageName: node
+  linkType: hard
+
 "read-package-json@npm:5.0.1":
   version: 5.0.1
   resolution: "read-package-json@npm:5.0.1"
   dependencies:
     glob: ^8.0.1
     json-parse-even-better-errors: ^2.3.1
     normalize-package-data: ^4.0.0
@@ -10855,14 +11427,26 @@
     json-parse-even-better-errors: ^2.3.1
     normalize-package-data: ^4.0.0
     npm-normalize-package-bin: ^2.0.0
   checksum: 0882ac9cec1bc92fb5515e9727611fb2909351e1e5c840dce3503cbb25b4cd48eb44b61071986e0fc51043208161f07d364a7336206c8609770186818753b51a
   languageName: node
   linkType: hard
 
+"read-package-json@npm:^6.0.0":
+  version: 6.0.1
+  resolution: "read-package-json@npm:6.0.1"
+  dependencies:
+    glob: ^9.3.0
+    json-parse-even-better-errors: ^3.0.0
+    normalize-package-data: ^5.0.0
+    npm-normalize-package-bin: ^3.0.0
+  checksum: 2fb5c2248da02d5a7180c0538c5b9ebdf04920f4bbf5c19d336d656277d99f1559ba90f2afcdfd6f580c3182a46fe5fb1d3d8c01bc63ffdeae927c91a11a82c9
+  languageName: node
+  linkType: hard
+
 "read-pkg-up@npm:^3.0.0":
   version: 3.0.0
   resolution: "read-pkg-up@npm:3.0.0"
   dependencies:
     find-up: ^2.0.0
     read-pkg: ^3.0.0
   checksum: 16175573f2914ab9788897bcbe2a62b5728d0075e62285b3680cebe97059e2911e0134a062cf6e51ebe3e3775312bc788ac2039ed6af38ec68d2c10c6f2b30fb
@@ -10909,48 +11493,48 @@
   dependencies:
     mute-stream: ~0.0.4
   checksum: 2777c254e5732cac96f5d0a1c0f6b836c89ae23d8febd405b206f6f24d5de1873420f1a0795e0e3721066650d19adf802c7882c4027143ee0acf942a4f34f97b
   languageName: node
   linkType: hard
 
 "readable-stream@npm:3, readable-stream@npm:^3.0.0, readable-stream@npm:^3.0.2, readable-stream@npm:^3.1.1, readable-stream@npm:^3.4.0, readable-stream@npm:^3.6.0":
-  version: 3.6.0
-  resolution: "readable-stream@npm:3.6.0"
+  version: 3.6.2
+  resolution: "readable-stream@npm:3.6.2"
   dependencies:
     inherits: ^2.0.3
     string_decoder: ^1.1.1
     util-deprecate: ^1.0.1
-  checksum: d4ea81502d3799439bb955a3a5d1d808592cf3133350ed352aeaa499647858b27b1c4013984900238b0873ec8d0d8defce72469fb7a83e61d53f5ad61cb80dc8
+  checksum: bdcbe6c22e846b6af075e32cf8f4751c2576238c5043169a1c221c92ee2878458a816a4ea33f4c67623c0b6827c8a400409bfb3cf0bf3381392d0b1dfb52ac8d
+  languageName: node
+  linkType: hard
+
+"readable-stream@npm:^4.1.0":
+  version: 4.3.0
+  resolution: "readable-stream@npm:4.3.0"
+  dependencies:
+    abort-controller: ^3.0.0
+    buffer: ^6.0.3
+    events: ^3.3.0
+    process: ^0.11.10
+  checksum: 5f8d5fc1eb0c6eb47771ad4537881126d6280666e1f10ba1e2262a670a0352c36f59e6a04d17c9a6f7c888218984836dc67f55e95a77de8bfdf06fb75f00f670
   languageName: node
   linkType: hard
 
 "readable-stream@npm:~2.3.6":
-  version: 2.3.7
-  resolution: "readable-stream@npm:2.3.7"
+  version: 2.3.8
+  resolution: "readable-stream@npm:2.3.8"
   dependencies:
     core-util-is: ~1.0.0
     inherits: ~2.0.3
     isarray: ~1.0.0
     process-nextick-args: ~2.0.0
     safe-buffer: ~5.1.1
     string_decoder: ~1.1.1
     util-deprecate: ~1.0.1
-  checksum: e4920cf7549a60f8aaf694d483a0e61b2a878b969d224f89b3bc788b8d920075132c4b55a7494ee944c7b6a9a0eada28a7f6220d80b0312ece70bbf08eeca755
-  languageName: node
-  linkType: hard
-
-"readdir-scoped-modules@npm:^1.1.0":
-  version: 1.1.0
-  resolution: "readdir-scoped-modules@npm:1.1.0"
-  dependencies:
-    debuglog: ^1.0.1
-    dezalgo: ^1.0.0
-    graceful-fs: ^4.1.2
-    once: ^1.3.0
-  checksum: 6d9f334e40dfd0f5e4a8aab5e67eb460c95c85083c690431f87ab2c9135191170e70c2db6d71afcafb78e073d23eb95dcb3fc33ef91308f6ebfe3197be35e608
+  checksum: 65645467038704f0c8aaf026a72fbb588a9e2ef7a75cd57a01702ee9db1c4a1e4b03aaad36861a6a0926546a74d174149c8c207527963e0c2d3eee2f37678a42
   languageName: node
   linkType: hard
 
 "rechoir@npm:^0.8.0":
   version: 0.8.0
   resolution: "rechoir@npm:0.8.0"
   dependencies:
@@ -11008,25 +11592,25 @@
     call-bind: ^1.0.2
     define-properties: ^1.1.3
     functions-have-names: ^1.2.2
   checksum: 51228bae732592adb3ededd5e15426be25f289e9c4ef15212f4da73f4ec3919b6140806374b8894036a86020d054a8d2657d3fee6bb9b4d35d8939c20030b7a6
   languageName: node
   linkType: hard
 
-"regexpu-core@npm:^5.2.1":
-  version: 5.3.1
-  resolution: "regexpu-core@npm:5.3.1"
+"regexpu-core@npm:^5.3.1":
+  version: 5.3.2
+  resolution: "regexpu-core@npm:5.3.2"
   dependencies:
     "@babel/regjsgen": ^0.8.0
     regenerate: ^1.4.2
     regenerate-unicode-properties: ^10.1.0
     regjsparser: ^0.9.1
     unicode-match-property-ecmascript: ^2.0.0
     unicode-match-property-value-ecmascript: ^2.1.0
-  checksum: 446fbbb79059afcd64d11ea573276e2df97ee7ad45aa452834d3b2aef7edf7bfe206c310f57f9345d8c95bfedbf9c16a9529f9219a05ae6a6b0d6f0dbe523b33
+  checksum: 95bb97088419f5396e07769b7de96f995f58137ad75fac5811fb5fe53737766dfff35d66a0ee66babb1eb55386ef981feaef392f9df6d671f3c124812ba24da2
   languageName: node
   linkType: hard
 
 "regjsparser@npm:^0.9.1":
   version: 0.9.1
   resolution: "regjsparser@npm:0.9.1"
   dependencies:
@@ -11078,17 +11662,17 @@
   version: 4.0.0
   resolution: "resolve-from@npm:4.0.0"
   checksum: f4ba0b8494846a5066328ad33ef8ac173801a51739eb4d63408c847da9a2e1c1de1e6cbbf72699211f3d13f8fc1325648b169bd15eb7da35688e30a5fb0e4a7f
   languageName: node
   linkType: hard
 
 "resolve.exports@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "resolve.exports@npm:2.0.0"
-  checksum: d8bee3b0cc0a0ae6c8323710983505bc6a3a2574f718e96f01e048a0f0af035941434b386cc9efc7eededc5e1199726185c306ec6f6a1aa55d5fbad926fd0634
+  version: 2.0.2
+  resolution: "resolve.exports@npm:2.0.2"
+  checksum: 1c7778ca1b86a94f8ab4055d196c7d87d1874b96df4d7c3e67bbf793140f0717fd506dcafd62785b079cd6086b9264424ad634fb904409764c3509c3df1653f2
   languageName: node
   linkType: hard
 
 "resolve@npm:^1.10.0, resolve@npm:^1.14.2, resolve@npm:^1.20.0":
   version: 1.22.1
   resolution: "resolve@npm:1.22.1"
   dependencies:
@@ -11171,20 +11755,22 @@
     glob: ^7.1.3
   bin:
     rimraf: bin.js
   checksum: 87f4164e396f0171b0a3386cc1877a817f572148ee13a7e113b238e48e8a9f2f31d009a92ec38a591ff1567d9662c6b67fd8818a2dbbaed74bc26a87a2a4a9a0
   languageName: node
   linkType: hard
 
-"rimraf@npm:^4.1.2":
-  version: 4.1.2
-  resolution: "rimraf@npm:4.1.2"
+"rimraf@npm:^4.1.2, rimraf@npm:^4.4.1":
+  version: 4.4.1
+  resolution: "rimraf@npm:4.4.1"
+  dependencies:
+    glob: ^9.2.0
   bin:
     rimraf: dist/cjs/src/bin.js
-  checksum: 480b8147fd9bcbef3ac118f88a7b1169c3872977a3411a0c84df838bfc30e175a394c0db6f9619fc8b8a886a18c6d779d5e74f380a0075ecc710afaf81b3f50c
+  checksum: b786adc02651e2e24bbedb04bbdea80652fc9612632931ff2d9f898c5e4708fe30956186597373c568bd5230a4dc2fadfc816ccacba8a1daded3a006a6b74f1a
   languageName: node
   linkType: hard
 
 "run-async@npm:^2.4.0":
   version: 2.4.1
   resolution: "run-async@npm:2.4.1"
   checksum: a2c88aa15df176f091a2878eb840e68d0bdee319d8d97bbb89112223259cebecb94bc0defd735662b83c2f7a30bed8cddb7d1674eb48ae7322dc602b22d03797
@@ -11323,15 +11909,15 @@
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
   checksum: 96451bfd7cba9b60ee87571959dc47e87c95b2fe58a9312a926340fee9907fc7bc062c352efdaf5bb24b2dff59c145e14faf7eb9d718a84b4751312531b39f43
   languageName: node
   linkType: hard
 
-"semver@npm:7.x, semver@npm:^7.0.0, semver@npm:^7.1.1, semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.7, semver@npm:^7.3.8":
+"semver@npm:7.3.8, semver@npm:7.x, semver@npm:^7.0.0, semver@npm:^7.1.1, semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.7, semver@npm:^7.3.8":
   version: 7.3.8
   resolution: "semver@npm:7.3.8"
   dependencies:
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
   checksum: ba9c7cbbf2b7884696523450a61fee1a09930d888b7a8d7579025ad93d459b2d1949ee5bbfeb188b2be5f4ac163544c5e98491ad6152df34154feebc2cc337c1
@@ -11343,15 +11929,15 @@
   resolution: "semver@npm:6.3.0"
   bin:
     semver: ./bin/semver.js
   checksum: 1b26ecf6db9e8292dd90df4e781d91875c0dcc1b1909e70f5d12959a23c7eebb8f01ea581c00783bbee72ceeaad9505797c381756326073850dc36ed284b21b9
   languageName: node
   linkType: hard
 
-"serialize-javascript@npm:^6.0.0, serialize-javascript@npm:^6.0.1":
+"serialize-javascript@npm:^6.0.1":
   version: 6.0.1
   resolution: "serialize-javascript@npm:6.0.1"
   dependencies:
     randombytes: ^2.1.0
   checksum: 3c4f4cb61d0893b988415bdb67243637333f3f574e9e9cc9a006a2ced0b390b0b3b44aef8d51c951272a9002ec50885eefdc0298891bc27eb2fe7510ea87dc4f
   languageName: node
   linkType: hard
@@ -11437,14 +12023,27 @@
 "signal-exit@npm:3.0.7, signal-exit@npm:^3.0.2, signal-exit@npm:^3.0.3, signal-exit@npm:^3.0.7":
   version: 3.0.7
   resolution: "signal-exit@npm:3.0.7"
   checksum: a2f098f247adc367dffc27845853e9959b9e88b01cb301658cfe4194352d8d2bb32e18467c786a7fe15f1d44b233ea35633d076d5e737870b7139949d1ab6318
   languageName: node
   linkType: hard
 
+"sigstore@npm:^1.0.0":
+  version: 1.2.0
+  resolution: "sigstore@npm:1.2.0"
+  dependencies:
+    "@sigstore/protobuf-specs": ^0.1.0
+    make-fetch-happen: ^11.0.1
+    tuf-js: ^1.0.0
+  bin:
+    sigstore: bin/sigstore.js
+  checksum: 8b06341a1bee97f363a8cab62102b27c88714c5ad9743fada5effb46cc3a5935c27c8149669384f0be7040c8f0c4e69bb7d533f138bdcf3aba91b803a69eac77
+  languageName: node
+  linkType: hard
+
 "simulate-event@npm:~1.4.0":
   version: 1.4.0
   resolution: "simulate-event@npm:1.4.0"
   dependencies:
     xtend: ^4.0.1
   checksum: d2cbb62f7a0c22aa1964e4df7a01b717c3c437df40dde70112fc06046cb8c7a03ca582571754653abc7c8c06df43d28c57b4f0bdf7a587094e4d6282357eb506
   languageName: node
@@ -11565,20 +12164,20 @@
   version: 0.6.1
   resolution: "source-map@npm:0.6.1"
   checksum: 59ce8640cf3f3124f64ac289012c2b8bd377c238e316fb323ea22fbfe83da07d81e000071d7242cad7a23cd91c7de98e4df8830ec3f133cb6133a5f6e9f67bc2
   languageName: node
   linkType: hard
 
 "spdx-correct@npm:^3.0.0":
-  version: 3.1.1
-  resolution: "spdx-correct@npm:3.1.1"
+  version: 3.2.0
+  resolution: "spdx-correct@npm:3.2.0"
   dependencies:
     spdx-expression-parse: ^3.0.0
     spdx-license-ids: ^3.0.0
-  checksum: 77ce438344a34f9930feffa61be0eddcda5b55fc592906ef75621d4b52c07400a97084d8701557b13f7d2aae0cb64f808431f469e566ef3fe0a3a131dcb775a6
+  checksum: e9ae98d22f69c88e7aff5b8778dc01c361ef635580e82d29e5c60a6533cc8f4d820803e67d7432581af0cc4fb49973125076ee3b90df191d153e223c004193b2
   languageName: node
   linkType: hard
 
 "spdx-exceptions@npm:^2.1.0":
   version: 2.3.0
   resolution: "spdx-exceptions@npm:2.3.0"
   checksum: cb69a26fa3b46305637123cd37c85f75610e8c477b6476fa7354eb67c08128d159f1d36715f19be6f9daf4b680337deb8c65acdcae7f2608ba51931540687ac0
@@ -11592,17 +12191,17 @@
     spdx-exceptions: ^2.1.0
     spdx-license-ids: ^3.0.0
   checksum: a1c6e104a2cbada7a593eaa9f430bd5e148ef5290d4c0409899855ce8b1c39652bcc88a725259491a82601159d6dc790bedefc9016c7472f7de8de7361f8ccde
   languageName: node
   linkType: hard
 
 "spdx-license-ids@npm:^3.0.0":
-  version: 3.0.12
-  resolution: "spdx-license-ids@npm:3.0.12"
-  checksum: 92a4dddce62ce1db6fe54a7a839cf85e06abc308fc83b776a55b44e4f1906f02e7ebd506120847039e976bbbad359ea8bdfafb7925eae5cd7e73255f02e0b7d6
+  version: 3.0.13
+  resolution: "spdx-license-ids@npm:3.0.13"
+  checksum: 3469d85c65f3245a279fa11afc250c3dca96e9e847f2f79d57f466940c5bb8495da08a542646086d499b7f24a74b8d0b42f3fc0f95d50ff99af1f599f6360ad7
   languageName: node
   linkType: hard
 
 "split2@npm:^3.0.0":
   version: 3.2.2
   resolution: "split2@npm:3.2.2"
   dependencies:
@@ -11632,14 +12231,23 @@
   resolution: "ssri@npm:9.0.1"
   dependencies:
     minipass: ^3.1.1
   checksum: fb58f5e46b6923ae67b87ad5ef1c5ab6d427a17db0bead84570c2df3cd50b4ceb880ebdba2d60726588272890bae842a744e1ecce5bd2a2a582fccd5068309eb
   languageName: node
   linkType: hard
 
+"ssri@npm:^10.0.0, ssri@npm:^10.0.1":
+  version: 10.0.1
+  resolution: "ssri@npm:10.0.1"
+  dependencies:
+    minipass: ^4.0.0
+  checksum: f35b147e5e16a3e1c8e3f71a4aaf5b1f7a9eb5559acbba21213c8171827921cecf56d3570118da7ade124776d25ed17d5e4c80eccbb2a083b17ce36dd24c3e5e
+  languageName: node
+  linkType: hard
+
 "stack-utils@npm:^2.0.3":
   version: 2.0.6
   resolution: "stack-utils@npm:2.0.6"
   dependencies:
     escape-string-regexp: ^2.0.0
   checksum: 052bf4d25bbf5f78e06c1d5e67de2e088b06871fa04107ca8d3f0e9d9263326e2942c8bedee3545795fc77d787d443a538345eef74db2f8e35db3558c6f91ff7
   languageName: node
@@ -11689,14 +12297,25 @@
     call-bind: ^1.0.2
     define-properties: ^1.1.4
     es-abstract: ^1.20.4
   checksum: 76e07238fe31dc12177428f0436b7ed6985f6a7ba97470fd53e4f0a6d9860bfee127d81957f3073cc879b434233df143825d140581e1340278053ad993c92f6c
   languageName: node
   linkType: hard
 
+"string.prototype.trim@npm:^1.2.7":
+  version: 1.2.7
+  resolution: "string.prototype.trim@npm:1.2.7"
+  dependencies:
+    call-bind: ^1.0.2
+    define-properties: ^1.1.4
+    es-abstract: ^1.20.4
+  checksum: 05b7b2d6af63648e70e44c4a8d10d8cc457536df78b55b9d6230918bde75c5987f6b8604438c4c8652eb55e4fc9725d2912789eb4ec457d6995f3495af190c09
+  languageName: node
+  linkType: hard
+
 "string.prototype.trimend@npm:^1.0.6":
   version: 1.0.6
   resolution: "string.prototype.trimend@npm:1.0.6"
   dependencies:
     call-bind: ^1.0.2
     define-properties: ^1.1.4
     es-abstract: ^1.20.4
@@ -11789,19 +12408,19 @@
   bin:
     sl-log-transformer: bin/sl-log-transformer.js
   checksum: abf9a4ac143118f26c3a0771b204b02f5cf4fa80384ae158f25e02bfbff761038accc44a7f65869ccd5a5995a7f2c16b1466b83149644ba6cecd3072a8927297
   languageName: node
   linkType: hard
 
 "style-loader@npm:~3.3.1":
-  version: 3.3.1
-  resolution: "style-loader@npm:3.3.1"
+  version: 3.3.2
+  resolution: "style-loader@npm:3.3.2"
   peerDependencies:
     webpack: ^5.0.0
-  checksum: 470feef680f59e2fce4d6601b5c55b88c01ad8d1dd693c528ffd591ff5fd7c01a4eff3bdbe62f26f847d6bd2430c9ab594be23307cfe7a3446ab236683f0d066
+  checksum: 5ee5ce2dc885369eccb55d429376e83d02570d473ac5edeb69fd65ee894847f1e51429cf078351f617bd04516ece8a1dd967f9f40464bd8fa76d903c6b2a6f08
   languageName: node
   linkType: hard
 
 "style-mod@npm:^4.0.0":
   version: 4.0.2
   resolution: "style-mod@npm:4.0.2"
   checksum: 4bac8877e039c61481fc729981378791979c3ebb2f827a54240e95ccca5bca92a6d660566cacb87a8d7cc1ffb26bcd5eafa10c697e131adb5ca9541f3a9cbff6
@@ -11844,39 +12463,39 @@
     prettier: ">=2.0.0"
     stylelint: ">=14.0.0"
   checksum: 094f53ef5dbe3806524db7f580b9312ceca444651803fc08c8baa48cd9a270985c709fa4f083681a685310dc347b8e55aa93d462554ba7d4ae6258a3bdf6a278
   languageName: node
   linkType: hard
 
 "stylelint@npm:^15.2.0":
-  version: 15.2.0
-  resolution: "stylelint@npm:15.2.0"
+  version: 15.3.0
+  resolution: "stylelint@npm:15.3.0"
   dependencies:
     "@csstools/css-parser-algorithms": ^2.0.1
-    "@csstools/css-tokenizer": ^2.0.1
+    "@csstools/css-tokenizer": ^2.1.0
     "@csstools/media-query-list-parser": ^2.0.1
     "@csstools/selector-specificity": ^2.1.1
     balanced-match: ^2.0.0
     colord: ^2.9.3
-    cosmiconfig: ^8.0.0
+    cosmiconfig: ^8.1.0
     css-functions-list: ^3.1.0
     css-tree: ^2.3.1
     debug: ^4.3.4
     fast-glob: ^3.2.12
     fastest-levenshtein: ^1.0.16
     file-entry-cache: ^6.0.1
     global-modules: ^2.0.0
     globby: ^11.1.0
     globjoin: ^0.1.4
     html-tags: ^3.2.0
     ignore: ^5.2.4
     import-lazy: ^4.0.0
     imurmurhash: ^0.1.4
     is-plain-object: ^5.0.0
-    known-css-properties: ^0.26.0
+    known-css-properties: ^0.27.0
     mathml-tag-names: ^2.1.3
     meow: ^9.0.0
     micromatch: ^4.0.5
     normalize-path: ^3.0.0
     picocolors: ^1.0.0
     postcss: ^8.4.21
     postcss-media-query-parser: ^0.2.3
@@ -11884,22 +12503,22 @@
     postcss-safe-parser: ^6.0.0
     postcss-selector-parser: ^6.0.11
     postcss-value-parser: ^4.2.0
     resolve-from: ^5.0.0
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
     style-search: ^0.1.0
-    supports-hyperlinks: ^2.3.0
+    supports-hyperlinks: ^3.0.0
     svg-tags: ^1.0.0
     table: ^6.8.1
     v8-compile-cache: ^2.3.0
     write-file-atomic: ^5.0.0
   bin:
     stylelint: bin/stylelint.js
-  checksum: 2a52d1b36345659e92280317554d82fc621203341d3a6baf1b19f3c28d06a07b8c5f7a25b9be2383f73a4e6a395d69dfbbe4daeca19bd119b88673dd8b6518ac
+  checksum: d6ef20cfc498dba274fc2b17ea9d342e0ca1a24bc07755066842f0a28e1dc6f36c2b67f4cf87a3a232ae98cf42864e884cdcd11428fe4caf0f5f1677cac8d85a
   languageName: node
   linkType: hard
 
 "supports-color@npm:^5.3.0":
   version: 5.5.0
   resolution: "supports-color@npm:5.5.0"
   dependencies:
@@ -11922,21 +12541,21 @@
   resolution: "supports-color@npm:8.1.1"
   dependencies:
     has-flag: ^4.0.0
   checksum: c052193a7e43c6cdc741eb7f378df605636e01ad434badf7324f17fb60c69a880d8d8fcdcb562cf94c2350e57b937d7425ab5b8326c67c2adc48f7c87c1db406
   languageName: node
   linkType: hard
 
-"supports-hyperlinks@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "supports-hyperlinks@npm:2.3.0"
+"supports-hyperlinks@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "supports-hyperlinks@npm:3.0.0"
   dependencies:
     has-flag: ^4.0.0
     supports-color: ^7.0.0
-  checksum: 9ee0de3c8ce919d453511b2b1588a8205bd429d98af94a01df87411391010fe22ca463f268c84b2ce2abad019dfff8452aa02806eeb5c905a8d7ad5c4f4c52b8
+  checksum: 41021305de5255b10d821bf93c7a781f783e1693d0faec293d7fc7ccf17011b90bde84b0295fa92ba75c6c390351fe84fdd18848cad4bf656e464a958243c3e7
   languageName: node
   linkType: hard
 
 "supports-preserve-symlinks-flag@npm:^1.0.0":
   version: 1.0.0
   resolution: "supports-preserve-symlinks-flag@npm:1.0.0"
   checksum: 53b1e247e68e05db7b3808b99b892bd36fb096e6fba213a06da7fab22045e97597db425c724f2bbd6c99a3c295e1e73f3e4de78592289f38431049e1277ca0ae
@@ -12021,37 +12640,35 @@
 "temp-dir@npm:1.0.0":
   version: 1.0.0
   resolution: "temp-dir@npm:1.0.0"
   checksum: cb2b58ddfb12efa83e939091386ad73b425c9a8487ea0095fe4653192a40d49184a771a1beba99045fbd011e389fd563122d79f54f82be86a55620667e08a6b2
   languageName: node
   linkType: hard
 
-"terser-webpack-plugin@npm:^5.1.3":
-  version: 5.3.6
-  resolution: "terser-webpack-plugin@npm:5.3.6"
+"temp-dir@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "temp-dir@npm:2.0.0"
+  checksum: cc4f0404bf8d6ae1a166e0e64f3f409b423f4d1274d8c02814a59a5529f07db6cd070a749664141b992b2c1af337fa9bb451a460a43bb9bcddc49f235d3115aa
+  languageName: node
+  linkType: hard
+
+"tempy@npm:1.0.0":
+  version: 1.0.0
+  resolution: "tempy@npm:1.0.0"
   dependencies:
-    "@jridgewell/trace-mapping": ^0.3.14
-    jest-worker: ^27.4.5
-    schema-utils: ^3.1.1
-    serialize-javascript: ^6.0.0
-    terser: ^5.14.1
-  peerDependencies:
-    webpack: ^5.1.0
-  peerDependenciesMeta:
-    "@swc/core":
-      optional: true
-    esbuild:
-      optional: true
-    uglify-js:
-      optional: true
-  checksum: 8f3448d7fdb0434ce6a0c09d95c462bfd2f4a5a430233d854163337f734a7f5c07c74513d16081e06d4ca33d366d5b1a36f5444219bc41a7403afd6162107bad
+    del: ^6.0.0
+    is-stream: ^2.0.0
+    temp-dir: ^2.0.0
+    type-fest: ^0.16.0
+    unique-string: ^2.0.0
+  checksum: 11541b9d4c5b6b6e4912ded3058cfb5a1294dcc0519b73fc1fc74f950f9a68cd380f78cbefe38514ac9233f749efc6486ac14592dcb29ad35a9b3807328cba1b
   languageName: node
   linkType: hard
 
-"terser-webpack-plugin@npm:^5.3.7":
+"terser-webpack-plugin@npm:^5.1.3, terser-webpack-plugin@npm:^5.3.7":
   version: 5.3.7
   resolution: "terser-webpack-plugin@npm:5.3.7"
   dependencies:
     "@jridgewell/trace-mapping": ^0.3.17
     jest-worker: ^27.4.5
     schema-utils: ^3.1.1
     serialize-javascript: ^6.0.1
@@ -12065,39 +12682,25 @@
       optional: true
     uglify-js:
       optional: true
   checksum: 095e699fdeeb553cdf2c6f75f983949271b396d9c201d7ae9fc633c45c1c1ad14c7257ef9d51ccc62213dd3e97f875870ba31550f6d4f1b6674f2615562da7f7
   languageName: node
   linkType: hard
 
-"terser@npm:^5.14.1":
-  version: 5.16.4
-  resolution: "terser@npm:5.16.4"
-  dependencies:
-    "@jridgewell/source-map": ^0.3.2
-    acorn: ^8.5.0
-    commander: ^2.20.0
-    source-map-support: ~0.5.20
-  bin:
-    terser: bin/terser
-  checksum: 92c7b38b7322340993d6a3578d74818c3556f362b3014f18a9b3d079ac7fa5da57954fda9a0d40d53013bc3ba82f50758296881abc40761e1bafdbde9a2ab967
-  languageName: node
-  linkType: hard
-
 "terser@npm:^5.16.5":
-  version: 5.16.6
-  resolution: "terser@npm:5.16.6"
+  version: 5.16.8
+  resolution: "terser@npm:5.16.8"
   dependencies:
     "@jridgewell/source-map": ^0.3.2
     acorn: ^8.5.0
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: f763a7bcc7b98cb2bfc41434f7b92bfe8a701a12c92ea6049377736c8e6de328240d654a20dfe15ce170fd783491b9873fad9f4cd8fee4f6c6fb8ca407859dee
+  checksum: f4a3ef4848a71f74f637c009395cf5a28660b56237fb8f13532cecfb24d6263e2dfbc1a511a11a94568988898f79cdcbecb9a4d8e104db35a0bea9639b70a325
   languageName: node
   linkType: hard
 
 "test-exclude@npm:^6.0.0":
   version: 6.0.0
   resolution: "test-exclude@npm:6.0.0"
   dependencies:
@@ -12222,18 +12825,18 @@
 "tr46@npm:~0.0.3":
   version: 0.0.3
   resolution: "tr46@npm:0.0.3"
   checksum: 726321c5eaf41b5002e17ffbd1fb7245999a073e8979085dacd47c4b4e8068ff5777142fc6726d6ca1fd2ff16921b48788b87225cbc57c72636f6efa8efbffe3
   languageName: node
   linkType: hard
 
-"treeverse@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "treeverse@npm:2.0.0"
-  checksum: 3c6b2b890975a4d42c86b9a0f1eb932b4450db3fa874be5c301c4f5e306fd76330c6a490cf334b0937b3a44b049787ba5d98c88bc7b140f34fdb3ab1f83e5269
+"treeverse@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "treeverse@npm:3.0.0"
+  checksum: 73168d9887fa57b0719218f176c5a3cfbaaf310922879acb4adf76665bc17dcdb6ed3e4163f0c27eee17e346886186a1515ea6f87e96cdc10df1dce13bf622a0
   languageName: node
   linkType: hard
 
 "trim-newlines@npm:^3.0.0":
   version: 3.0.1
   resolution: "trim-newlines@npm:3.0.1"
   checksum: b530f3fadf78e570cf3c761fb74fef655beff6b0f84b29209bac6c9622db75ad1417f4a7b5d54c96605dcd72734ad44526fef9f396807b90839449eb543c6206
@@ -12270,21 +12873,21 @@
   bin:
     ts-jest: cli.js
   checksum: f60f129c2287f4c963d9ee2677132496c5c5a5d39c27ad234199a1140c26318a7d5bda34890ab0e30636ec42a8de28f84487c09e9dcec639c9c67812b3a38373
   languageName: node
   linkType: hard
 
 "tsconfig-paths@npm:^4.1.2":
-  version: 4.1.2
-  resolution: "tsconfig-paths@npm:4.1.2"
+  version: 4.2.0
+  resolution: "tsconfig-paths@npm:4.2.0"
   dependencies:
     json5: ^2.2.2
     minimist: ^1.2.6
     strip-bom: ^3.0.0
-  checksum: 3d9151ecea139594e25618717de15769ab9f38f8e6d510ac16e592b23e7f7105ea13cec5694c3de7e132c98277b775e18edd1651964164ee6d75737c408494cc
+  checksum: 28c5f7bbbcabc9dabd4117e8fdc61483f6872a1c6b02a4b1c4d68c5b79d06896c3cc9547610c4c3ba64658531caa2de13ead1ea1bf321c7b53e969c4752b98c7
   languageName: node
   linkType: hard
 
 "tslib@npm:^1.8.1":
   version: 1.14.1
   resolution: "tslib@npm:1.14.1"
   checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
@@ -12305,14 +12908,24 @@
     tslib: ^1.8.1
   peerDependencies:
     typescript: ">=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta"
   checksum: 1843f4c1b2e0f975e08c4c21caa4af4f7f65a12ac1b81b3b8489366826259323feb3fc7a243123453d2d1a02314205a7634e048d4a8009921da19f99755cdc48
   languageName: node
   linkType: hard
 
+"tuf-js@npm:^1.0.0":
+  version: 1.1.2
+  resolution: "tuf-js@npm:1.1.2"
+  dependencies:
+    "@tufjs/models": 1.0.1
+    make-fetch-happen: ^11.0.1
+  checksum: 05fd85c12de74fddd7ddc7d6dd3e4d36f09cd4834d1b9fbcb4c067f0cdf7e9a9cb9323f515f014f5e17441376d417ef634ffd2aa0850aead63db5f9e41ccce09
+  languageName: node
+  linkType: hard
+
 "type-check@npm:^0.4.0, type-check@npm:~0.4.0":
   version: 0.4.0
   resolution: "type-check@npm:0.4.0"
   dependencies:
     prelude-ls: ^1.2.1
   checksum: ec688ebfc9c45d0c30412e41ca9c0cdbd704580eb3a9ccf07b9b576094d7b86a012baebc95681999dd38f4f444afd28504cb3a89f2ef16b31d4ab61a0739025a
   languageName: node
@@ -12330,14 +12943,21 @@
 "type-detect@npm:4.0.8":
   version: 4.0.8
   resolution: "type-detect@npm:4.0.8"
   checksum: 62b5628bff67c0eb0b66afa371bd73e230399a8d2ad30d852716efcc4656a7516904570cd8631a49a3ce57c10225adf5d0cbdcb47f6b0255fe6557c453925a15
   languageName: node
   linkType: hard
 
+"type-fest@npm:^0.16.0":
+  version: 0.16.0
+  resolution: "type-fest@npm:0.16.0"
+  checksum: 1a4102c06dc109db00418c753062e206cab65befd469d000ece4452ee649bf2a9cf57686d96fb42326bc9d918d9a194d4452897b486dcc41989e5c99e4e87094
+  languageName: node
+  linkType: hard
+
 "type-fest@npm:^0.18.0":
   version: 0.18.1
   resolution: "type-fest@npm:0.18.1"
   checksum: e96dcee18abe50ec82dab6cbc4751b3a82046da54c52e3b2d035b3c519732c0b3dd7a2fa9df24efd1a38d953d8d4813c50985f215f1957ee5e4f26b0fe0da395
   languageName: node
   linkType: hard
 
@@ -12517,23 +13137,50 @@
   resolution: "unique-filename@npm:2.0.1"
   dependencies:
     unique-slug: ^3.0.0
   checksum: 807acf3381aff319086b64dc7125a9a37c09c44af7620bd4f7f3247fcd5565660ac12d8b80534dcbfd067e6fe88a67e621386dd796a8af828d1337a8420a255f
   languageName: node
   linkType: hard
 
+"unique-filename@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "unique-filename@npm:3.0.0"
+  dependencies:
+    unique-slug: ^4.0.0
+  checksum: 8e2f59b356cb2e54aab14ff98a51ac6c45781d15ceaab6d4f1c2228b780193dc70fae4463ce9e1df4479cb9d3304d7c2043a3fb905bdeca71cc7e8ce27e063df
+  languageName: node
+  linkType: hard
+
 "unique-slug@npm:^3.0.0":
   version: 3.0.0
   resolution: "unique-slug@npm:3.0.0"
   dependencies:
     imurmurhash: ^0.1.4
   checksum: 49f8d915ba7f0101801b922062ee46b7953256c93ceca74303bd8e6413ae10aa7e8216556b54dc5382895e8221d04f1efaf75f945c2e4a515b4139f77aa6640c
   languageName: node
   linkType: hard
 
+"unique-slug@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "unique-slug@npm:4.0.0"
+  dependencies:
+    imurmurhash: ^0.1.4
+  checksum: 0884b58365af59f89739e6f71e3feacb5b1b41f2df2d842d0757933620e6de08eff347d27e9d499b43c40476cbaf7988638d3acb2ffbcb9d35fd035591adfd15
+  languageName: node
+  linkType: hard
+
+"unique-string@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "unique-string@npm:2.0.0"
+  dependencies:
+    crypto-random-string: ^2.0.0
+  checksum: ef68f639136bcfe040cf7e3cd7a8dff076a665288122855148a6f7134092e6ed33bf83a7f3a9185e46c98dddc445a0da6ac25612afa1a7c38b8b654d6c02498e
+  languageName: node
+  linkType: hard
+
 "universal-user-agent@npm:^6.0.0":
   version: 6.0.0
   resolution: "universal-user-agent@npm:6.0.0"
   checksum: 5092bbc80dd0d583cef0b62c17df0043193b74f425112ea6c1f69bc5eda21eeec7a08d8c4f793a277eb2202ffe9b44bec852fa3faff971234cd209874d1b79ef
   languageName: node
   linkType: hard
 
@@ -12547,15 +13194,15 @@
 "universalify@npm:^2.0.0":
   version: 2.0.0
   resolution: "universalify@npm:2.0.0"
   checksum: 2406a4edf4a8830aa6813278bab1f953a8e40f2f63a37873ffa9a3bc8f9745d06cc8e88f3572cb899b7e509013f7f6fcc3e37e8a6d914167a5381d8440518c44
   languageName: node
   linkType: hard
 
-"upath@npm:^2.0.1":
+"upath@npm:2.0.1, upath@npm:^2.0.1":
   version: 2.0.1
   resolution: "upath@npm:2.0.1"
   checksum: 2db04f24a03ef72204c7b969d6991abec9e2cb06fb4c13a1fd1c59bc33b46526b16c3325e55930a11ff86a77a8cbbcda8f6399bf914087028c5beae21ecdb33c
   languageName: node
   linkType: hard
 
 "update-browserslist-db@npm:^1.0.10":
@@ -12649,14 +13296,23 @@
   resolution: "validate-npm-package-name@npm:3.0.0"
   dependencies:
     builtins: ^1.0.3
   checksum: ce4c68207abfb22c05eedb09ff97adbcedc80304a235a0844f5344f1fd5086aa80e4dbec5684d6094e26e35065277b765c1caef68bcea66b9056761eddb22967
   languageName: node
   linkType: hard
 
+"validate-npm-package-name@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "validate-npm-package-name@npm:5.0.0"
+  dependencies:
+    builtins: ^5.0.0
+  checksum: 5342a994986199b3c28e53a8452a14b2bb5085727691ea7aa0d284a6606b127c371e0925ae99b3f1ef7cc7d2c9de75f52eb61a3d1cc45e39bca1e3a9444cbb4e
+  languageName: node
+  linkType: hard
+
 "validate.io-array@npm:^1.0.3":
   version: 1.0.6
   resolution: "validate.io-array@npm:1.0.6"
   checksum: 54eca83ebc702e3e46499f9d9e77287a95ae25c4e727cd2fafee29c7333b3a36cca0c5d8f090b9406262786de80750fba85e7e7ef41e20bf8cc67d5570de449b
   languageName: node
   linkType: hard
 
@@ -12835,16 +13491,16 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.76.2
-  resolution: "webpack@npm:5.76.2"
+  version: 5.77.0
+  resolution: "webpack@npm:5.77.0"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^0.0.51
     "@webassemblyjs/ast": 1.11.1
     "@webassemblyjs/wasm-edit": 1.11.1
     "@webassemblyjs/wasm-parser": 1.11.1
     acorn: ^8.7.1
@@ -12867,15 +13523,15 @@
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 86db98299a175c371031449c26077e87b33acd8f45de7f7945ed4b9b37c8ca11bc5169af9c44743efccd4d55e08042a3aa3a3bc42aff831309a0821ffbcd395e
+  checksum: 21341bb72cbbf61dfb3af91eabe9290a6c05139f268eff3c419e5339deb6c79f2f36de55d9abf017d3ccbad290a535c02325001b2816acc393f3c022e67ac17c
   languageName: node
   linkType: hard
 
 "whatwg-encoding@npm:^2.0.0":
   version: 2.0.0
   resolution: "whatwg-encoding@npm:2.0.0"
   dependencies:
@@ -12974,14 +13630,25 @@
     isexe: ^2.0.0
   bin:
     node-which: ./bin/node-which
   checksum: 1a5c563d3c1b52d5f893c8b61afe11abc3bab4afac492e8da5bde69d550de701cf9806235f20a47b5c8fa8a1d6a9135841de2596535e998027a54589000e66d1
   languageName: node
   linkType: hard
 
+"which@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "which@npm:3.0.0"
+  dependencies:
+    isexe: ^2.0.0
+  bin:
+    node-which: bin/which.js
+  checksum: fdcf3cadab414e60b86c6836e7ac9de9273561a8926f57cbc28641b602a771527239ee4d47f2689ed255666f035ba0a0d72390986cc0c4e45344491adc7d0eeb
+  languageName: node
+  linkType: hard
+
 "wide-align@npm:^1.1.5":
   version: 1.1.5
   resolution: "wide-align@npm:1.1.5"
   dependencies:
     string-width: ^1.0.2 || 2 || 3 || 4
   checksum: d5fc37cd561f9daee3c80e03b92ed3e84d80dde3365a8767263d03dacfc8fa06b065ffe1df00d8c2a09f731482fcacae745abfbb478d4af36d0a891fad4834d3
   languageName: node
@@ -13055,15 +13722,15 @@
     graceful-fs: ^4.1.11
     imurmurhash: ^0.1.4
     signal-exit: ^3.0.2
   checksum: 2db81f92ae974fd87ab4a5e7932feacaca626679a7c98fcc73ad8fcea5a1950eab32fa831f79e9391ac99b562ca091ad49be37a79045bd65f595efbb8f4596ae
   languageName: node
   linkType: hard
 
-"write-file-atomic@npm:^4.0.0, write-file-atomic@npm:^4.0.2":
+"write-file-atomic@npm:^4.0.2":
   version: 4.0.2
   resolution: "write-file-atomic@npm:4.0.2"
   dependencies:
     imurmurhash: ^0.1.4
     signal-exit: ^3.0.7
   checksum: 5da60bd4eeeb935eec97ead3df6e28e5917a6bd317478e4a85a5285e8480b8ed96032bbcc6ecd07b236142a24f3ca871c924ec4a6575e623ec1b11bf8c1c253c
   languageName: node
@@ -13110,25 +13777,25 @@
   dependencies:
     async-limiter: ~1.0.0
   checksum: aec3154ec51477c094ac2cb5946a156e17561a581fa27005cbf22c53ac57f8d4e5f791dd4bbba6a488602cb28778c8ab7df06251d590507c3c550fd8ebeee949
   languageName: node
   linkType: hard
 
 "ws@npm:^8.11.0":
-  version: 8.12.1
-  resolution: "ws@npm:8.12.1"
+  version: 8.13.0
+  resolution: "ws@npm:8.13.0"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ">=5.0.2"
   peerDependenciesMeta:
     bufferutil:
       optional: true
     utf-8-validate:
       optional: true
-  checksum: 97301c1c4d838fc81bd413f370f75c12aabe44527b31323b761eab3043a9ecb7e32ffd668548382c9a6a5ad3a1c3a9249608e8338e6b939f2f9540f1e21970b5
+  checksum: 53e991bbf928faf5dc6efac9b8eb9ab6497c69feeb94f963d648b7a3530a720b19ec2e0ec037344257e05a4f35bd9ad04d9de6f289615ffb133282031b18c61c
   languageName: node
   linkType: hard
 
 "xml-name-validator@npm:^4.0.0":
   version: 4.0.0
   resolution: "xml-name-validator@npm:4.0.0"
   checksum: af100b79c29804f05fa35aa3683e29a321db9b9685d5e5febda3fa1e40f13f85abc40f45a6b2bf7bee33f68a1dc5e8eaef4cec100a304a9db565e6061d4cb5ad
@@ -13174,16 +13841,16 @@
   dependencies:
     lib0: ^0.2.42
   checksum: d19404a4ebafcf3761c28b881abe8c32ab6e457db0e5ffc7dbb749cbc2c3bb98e003a43f3e8eba7f245b2698c76f2c4cdd1c2db869f8ec0c6ef94736d9a88652
   languageName: node
   linkType: hard
 
 "y-websocket@npm:^1.3.15":
-  version: 1.4.5
-  resolution: "y-websocket@npm:1.4.5"
+  version: 1.5.0
+  resolution: "y-websocket@npm:1.5.0"
   dependencies:
     lib0: ^0.2.52
     lodash.debounce: ^4.0.8
     ws: ^6.2.1
     y-leveldb: ^0.1.0
     y-protocols: ^1.0.5
   peerDependencies:
@@ -13192,15 +13859,15 @@
     ws:
       optional: true
     y-leveldb:
       optional: true
   bin:
     y-websocket: bin/server.js
     y-websocket-server: bin/server.js
-  checksum: 19dbd9a568940dbbb9e47e39db93f3fae1ae596b9788bf169a35e7c48d2059f1a06c85b1150b358b2aac0a0fb1f5475777eb2701df9c6202cbc9ad43450d42ce
+  checksum: 0e532f7d488e9430b011814eab67f37c002b0b102ccc169c65250ad9fddd901b2f979ac0f26453e7ac625fe2f2fe84d208b90b47e9e3572ac449b01572884fb8
   languageName: node
   linkType: hard
 
 "y18n@npm:^5.0.5":
   version: 5.0.8
   resolution: "y18n@npm:5.0.8"
   checksum: 54f0fb95621ee60898a38c572c515659e51cc9d9f787fb109cef6fde4befbe1c4602dc999d30110feee37456ad0f1660fa2edcfde6a9a740f86a290999550d30
@@ -13261,34 +13928,34 @@
     y18n: ^5.0.5
     yargs-parser: ^20.2.2
   checksum: b14afbb51e3251a204d81937c86a7e9d4bdbf9a2bcee38226c900d00f522969ab675703bee2a6f99f8e20103f608382936034e64d921b74df82b63c07c5e8f59
   languageName: node
   linkType: hard
 
 "yargs@npm:^17.3.1, yargs@npm:^17.6.2":
-  version: 17.7.0
-  resolution: "yargs@npm:17.7.0"
+  version: 17.7.1
+  resolution: "yargs@npm:17.7.1"
   dependencies:
     cliui: ^8.0.1
     escalade: ^3.1.1
     get-caller-file: ^2.0.5
     require-directory: ^2.1.1
     string-width: ^4.2.3
     y18n: ^5.0.5
     yargs-parser: ^21.1.1
-  checksum: e7d5f5b60e63b04ded7c27c3d4b194565565cac3ea19fffcdbb183bed973a83106822a04dda28ebba4811ce92949a9d9858d3935186ff8f343548bf98aab2120
+  checksum: 3d8a43c336a4942bc68080768664aca85c7bd406f018bad362fd255c41c8f4e650277f42fd65d543fce99e084124ddafee7bbfc1a5c6a8fda4cec78609dcf8d4
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.40":
-  version: 13.5.46
-  resolution: "yjs@npm:13.5.46"
+  version: 13.5.51
+  resolution: "yjs@npm:13.5.51"
   dependencies:
-    lib0: ^0.2.49
-  checksum: 04fe71356e6f0e82fc5343b2acfc0fb9c09132f1113cb6cfd93b1663043c0a883f804230faae1af3e4ddfd9493235e4ea7eb333b9179bf755a480a7e354e9a7e
+    lib0: ^0.2.72
+  checksum: 4dea7a4c71163fd64f24cc153c25af641cefed7c7aadbc7e0973e2f35398635a58b5da4a45f8e10e0fc4331cde517869ac626e6b449d66766fc61d12e81b06f7
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `jupyter_collaboration-1.0.0a7/docs/Makefile` & `jupyter_collaboration-1.0.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/docs/make.bat` & `jupyter_collaboration-1.0.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/docs/source/conf.py` & `jupyter_collaboration-1.0.0a8/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,19 +81,13 @@
     # Copy changelog.md file
     dest = HERE / "changelog.md"
     shutil.copy(str(HERE.parent.parent / "CHANGELOG.md"), str(dest))
 
     # Build JavaScript Docs
     js = HERE.parent.parent
     js_docs = HERE / "ts" / "api"
-    collaboration = js_docs / "collaboration"
-    docprovider = js_docs / "docprovider"
-    extension = js_docs / "collaboration-extension"
+    if js_docs.exists():
+        shutil.rmtree(js_docs)
 
-    if collaboration.exists() and docprovider.exists() and extension.exists():
-        # avoid rebuilding docs because it takes forever
-        # `make clean` to force a rebuild
-        print(f"already have {js_docs!s}")
-    else:
-        print("Building JavaScript API docs")
-        check_call(["jlpm", "install"], cwd=str(js))
-        check_call(["jlpm", "run", "docs"], cwd=str(js))
+    print("Building JavaScript API docs")
+    check_call(["jlpm", "install"], cwd=str(js))
+    check_call(["jlpm", "run", "docs"], cwd=str(js))
```

### Comparing `jupyter_collaboration-1.0.0a7/docs/source/configuration.md` & `jupyter_collaboration-1.0.0a8/docs/source/configuration.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/docs/source/index.md` & `jupyter_collaboration-1.0.0a8/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/docs/source/_static/jupyter_logo.svg` & `jupyter_collaboration-1.0.0a8/docs/source/_static/jupyter_logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/docs/source/_static/logo-icon.png` & `jupyter_collaboration-1.0.0a8/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/docs/source/developer/contributing.rst` & `jupyter_collaboration-1.0.0a8/docs/source/developer/contributing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-General Jupyter contributor guidelines
-======================================
+Developer documentation
+=======================
 
 If you're reading this section, you're probably interested in contributing to
 Jupyter.  Welcome and thanks for your interest in contributing!
 
 Please take a look at the Contributor documentation, familiarize yourself with
 using the Jupyter Server, and introduce yourself on the mailing list and
 share what area of the project you are interested in working on.
```

### Comparing `jupyter_collaboration-1.0.0a7/docs/source/images/rtc_shared_cursors.png` & `jupyter_collaboration-1.0.0a8/docs/source/images/rtc_shared_cursors.png`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/app.py` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 from jupyter_server.extension.application import ExtensionApp
 from traitlets import Float, Int, Type
 from ypy_websocket.ystore import BaseYStore
 
-from .handlers import DocSessionHandler, SQLiteYStore, YDocWebSocketHandler
+from .handlers import DocSessionHandler, YDocWebSocketHandler
+from .stores import SQLiteYStore
 
 
 class YDocExtension(ExtensionApp):
     name = "jupyter_collaboration"
 
     file_poll_interval = Int(
         1,
@@ -57,7 +58,10 @@
     def initialize_handlers(self):
         self.handlers.extend(
             [
                 (r"/api/collaboration/room/(.*)", YDocWebSocketHandler),
                 (r"/api/collaboration/session/(.*)", DocSessionHandler),
             ]
         )
+
+    async def stop_extension(self):
+        YDocWebSocketHandler.clean_up()
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/handlers.py` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,109 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import asyncio
 import json
 import uuid
-from logging import Logger
+from logging import getLogger
 from pathlib import Path
-from typing import Any, Dict, Optional, Set, Tuple
+from typing import Any, Dict, Optional, Set
 
 from jupyter_server.auth import authorized
 from jupyter_server.base.handlers import APIHandler, JupyterHandler
-from jupyter_server.utils import ensure_async
+from jupyter_server.serverapp import ServerWebApplication
 from jupyter_ydoc import ydocs as YDOCS
 from tornado import web
+from tornado.httputil import HTTPServerRequest
 from tornado.websocket import WebSocketHandler
-from traitlets import Int, Unicode
-from traitlets.config import LoggingConfigurable
 from ypy_websocket.websocket_server import WebsocketServer, YRoom
-from ypy_websocket.ystore import BaseYStore
-from ypy_websocket.ystore import SQLiteYStore as _SQLiteYStore
-from ypy_websocket.ystore import TempFileYStore as _TempFileYStore
-from ypy_websocket.ystore import YDocNotFound
 from ypy_websocket.yutils import YMessageType
 
+from .loaders import FileLoader
+from .rooms import DocumentRoom, TransientRoom
+from .utils import decode_file_path
+
 YFILE = YDOCS["file"]
 
 SERVER_SESSION = str(uuid.uuid4())
 
 
-class TempFileYStore(_TempFileYStore):
-    prefix_dir = "jupyter_ystore_"
-
-
-class SQLiteYStoreMetaclass(type(LoggingConfigurable), type(_SQLiteYStore)):  # type: ignore
+class RoomNotFound(Exception):
     pass
 
 
-class SQLiteYStore(LoggingConfigurable, _SQLiteYStore, metaclass=SQLiteYStoreMetaclass):
-    db_path = Unicode(
-        ".jupyter_ystore.db",
-        config=True,
-        help="""The path to the YStore database. Defaults to '.jupyter_ystore.db' in the current
-        directory.""",
-    )
-
-    document_ttl = Int(
-        None,
-        allow_none=True,
-        config=True,
-        help="""The document time-to-live in seconds. Defaults to None (document history is never
-        cleared).""",
-    )
-
-
-class DocumentRoom(YRoom):
-    """A Y room for a possibly stored document (e.g. a notebook)."""
-
-    def __init__(self, type: str, ystore: BaseYStore, log: Optional[Logger]):
-        super().__init__(ready=False, ystore=ystore, log=log)
-        self.type = type
-        self.cleaner: Optional["asyncio.Task[Any]"] = None
-        self.watcher: Optional["asyncio.Task[Any]"] = None
-        self.document = YDOCS.get(type, YFILE)(self.ydoc)
-
-
-class TransientRoom(YRoom):
-    """A Y room for sharing state (e.g. awareness)."""
-
-    def __init__(self, log: Optional[Logger]):
-        super().__init__(log=log)
-
-
 class JupyterWebsocketServer(WebsocketServer):
     rooms: Dict[str, YRoom]
     ypatch_nb: int
     connected_user: Dict[int, str]
     background_tasks: Set[asyncio.Task[Any]]
 
     def __init__(self, *args, **kwargs):
         self.ystore_class = kwargs.pop("ystore_class")
         self.log = kwargs["log"]
         super().__init__(*args, **kwargs)
         self.ypatch_nb = 0
         self.connected_users = {}
         self.background_tasks = set()
-        self.monitor_task = asyncio.create_task(self.monitor())
+        self.monitor_task = asyncio.create_task(self._monitor())
+
+    def room_exists(self, path: str) -> bool:
+        """
+        Returns true is the room exist or false otherwise.
+
+            Parameters:
+                path (str): Room ID.
+
+            Returns:
+                exists (bool): Whether the room exists or not.
+        """
+        return path in self.rooms
+
+    def add_room(self, path: str, room: YRoom) -> None:
+        """
+        Adds a new room.
+
+            Parameters:
+                path (str): Room ID.
+                room (YRoom): A room.
+        """
+        self.rooms[path] = room
+
+    def get_room(self, path: str) -> YRoom:
+        """
+        Returns the room for the specified room ID or raises a RoomNotFound
+        error if the room doesn't exist.
+
+            Parameters:
+                path (str): Room ID.
+
+            Returns:
+                room (YRoom): The room.
+        """
+        if path not in self.rooms:
+            # Document rooms need a file
+            raise RoomNotFound
 
-    async def monitor(self):
+        return self.rooms[path]
+
+    async def _monitor(self):
+        """
+        An infinite loop with a 60 seconds delay for counting the number
+        of patches processed in a minute and how many clients are connected.
+
+        #### Note:
+            This method runs in a coroutine for debugging purposes.
+        """
         while True:
             await asyncio.sleep(60)
             clients_nb = sum(len(room.clients) for room in self.rooms.values())
             self.log.info("Processed %s Y patches in one minute", self.ypatch_nb)
             self.log.info("Connected Y users: %s", clients_nb)
             self.ypatch_nb = 0
 
-    def get_room(self, path: str) -> YRoom:
-        if path not in self.rooms:
-            if path.count(":") >= 2:
-                # it is a stored document (e.g. a notebook)
-                file_format, file_type, file_path = path.split(":", 2)
-                p = Path(file_path)
-                updates_file_path = str(p.parent / f".{file_type}:{p.name}.y")
-                ystore = self.ystore_class(path=updates_file_path, log=self.log)
-                self.rooms[path] = DocumentRoom(file_type, ystore, self.log)
-            else:
-                # it is a transient document (e.g. awareness)
-                self.rooms[path] = TransientRoom(self.log)
-        return self.rooms[path]
-
 
 class YDocWebSocketHandler(WebSocketHandler, JupyterHandler):
     """`YDocWebSocketHandler` uses the singleton pattern for ``WebsocketServer``,
     which is a subclass of ypy-websocket's ``WebsocketServer``.
 
     In ``WebsocketServer``, we expect to use a WebSocket object as follows:
 
@@ -125,171 +117,172 @@
        Messages received in Tornado's `on_message(message)` are put in an async
        ``_message_queue``, from which we get them asynchronously.
     - The ``send(message)`` method is async and calls Tornado's ``write_message(message)``.
     - Although it's currently not used in ypy-websocket, ``recv()`` is an async method for
        receiving a message.
     """
 
-    saving_document: Optional["asyncio.Task[Any]"]
+    files: Dict[str, FileLoader] = {}
     websocket_server: Optional[JupyterWebsocketServer] = None
     _message_queue: "asyncio.Queue[Any]"
 
-    # Override max_message size to 1GB
+    def __init__(
+        self, app: ServerWebApplication, request: HTTPServerRequest, **kwargs: Dict[str, Any]
+    ):
+        super().__init__(app, request, **kwargs)
+
+        # CONFIG
+        file_id_manager = self.settings["file_id_manager"]
+        ystore_class = self.settings["collaborative_ystore_class"]
+        self._cleanup_delay = self.settings["collaborative_document_cleanup_delay"]
+        # self.settings["collaborative_file_poll_interval"]
+        # self.settings["collaborative_document_save_delay"]
+
+        # Instantiate the JupyterWebsocketServer as a Class property
+        # if it doesn't exist yet
+        if self.websocket_server is None:
+            for k, v in self.config.get(ystore_class.__name__, {}).items():
+                setattr(ystore_class, k, v)
+
+            YDocWebSocketHandler.websocket_server = JupyterWebsocketServer(
+                rooms_ready=False,
+                auto_clean_rooms=False,
+                ystore_class=ystore_class,
+                log=self.log,
+            )
+
+        assert self.websocket_server is not None
+        self._message_queue = asyncio.Queue()
+
+        # Get room
+        self._room_id: str = request.path.split("/")[-1]
+
+        if self.websocket_server.room_exists(self._room_id):
+            self.room: YRoom = self.websocket_server.get_room(self._room_id)
+
+        else:
+            if self._room_id.count(":") >= 2:
+                # DocumentRoom
+                file_format, file_type, file_id = decode_file_path(self._room_id)
+                path = file_id_manager.get_path(file_id)
+
+                # Instantiate the FileLoader if it doesn't exist yet
+                file = YDocWebSocketHandler.files.get(file_id)
+                if file is None:
+                    self.log.info("Creating FileLoader for: %s", path)
+                    file = FileLoader(
+                        file_id,
+                        file_format,
+                        file_type,
+                        file_id_manager,
+                        self.contents_manager,
+                        self.log,
+                        self.settings["collaborative_file_poll_interval"],
+                    )
+                    self.files[file_id] = file
+
+                path = Path(path)
+                updates_file_path = str(path.parent / f".{file_type}:{path.name}.y")
+                ystore = ystore_class(path=updates_file_path, log=self.log)
+                self.room = DocumentRoom(
+                    self._room_id,
+                    file_format,
+                    file_type,
+                    file,
+                    ystore,
+                    self.log,
+                    self.settings["collaborative_document_save_delay"],
+                )
+
+            else:
+                # TransientRoom
+                # it is a transient document (e.g. awareness)
+                self.room = TransientRoom(self._room_id, self.log)
+
+            self.websocket_server.add_room(self._room_id, self.room)
+
+    @property
+    def path(self):
+        """
+        Returns the room id. It needs to be called 'path' for compatibility with
+        the WebsocketServer (websocket.path).
+        """
+        return self._room_id
+
     @property
     def max_message_size(self):
+        """
+        Override max_message size to 1GB
+        """
         return 1024 * 1024 * 1024
 
     def __aiter__(self):
         # needed to be compatible with WebsocketServer (async for message in websocket)
         return self
 
     async def __anext__(self):
         # needed to be compatible with WebsocketServer (async for message in websocket)
         message = await self._message_queue.get()
         if not message:
             raise StopAsyncIteration()
         return message
 
-    def get_file_info(self) -> Tuple[str, str, str]:
-        assert self.websocket_server is not None
-        assert isinstance(self.room, DocumentRoom)
-        room_name = self.websocket_server.get_room_name(self.room)
-        file_format: str
-        file_type: str
-        file_path: Optional[str]
-        file_id: str
-        file_format, file_type, file_id = room_name.split(":", 2)
-        file_path = self.settings["file_id_manager"].get_path(file_id)
-        if file_path is None:
-            raise RuntimeError(f"File {self.room.document.path} cannot be found anymore")
-        assert file_path is not None
-        if file_path != self.room.document.path:
-            self.log.debug(
-                "File with ID %s was moved from %s to %s",
-                file_id,
-                self.room.document.path,
-                file_path,
-            )
-            self.room.document.path = file_path
-        return file_format, file_type, file_path
-
-    def set_file_info(self, value: str) -> None:
-        assert self.websocket_server is not None
-        self.websocket_server.rename_room(value, from_room=self.room)
-        self.path = value  # needed to be compatible with WebsocketServer (websocket.path)
-
     async def get(self, *args, **kwargs):
+        """
+        Overrides default behavior to check whether the client is authenticated or not.
+        """
         if self.get_current_user() is None:
             self.log.warning("Couldn't authenticate WebSocket connection")
             raise web.HTTPError(403)
         return await super().get(*args, **kwargs)
 
-    async def open(self, path):
-        ystore_class = self.settings["collaborative_ystore_class"]
-        if self.websocket_server is None:
-            for k, v in self.config.get(ystore_class.__name__, {}).items():
-                setattr(ystore_class, k, v)
-            YDocWebSocketHandler.websocket_server = JupyterWebsocketServer(
-                rooms_ready=False,
-                auto_clean_rooms=False,
-                ystore_class=ystore_class,
-                log=self.log,
-            )
-        self._message_queue = asyncio.Queue()
-        self.lock = asyncio.Lock()
+    async def open(self, room_id):
+        """
+        On connection open.
+        """
         assert self.websocket_server is not None
-        self.room = self.websocket_server.get_room(path)
-        self.set_file_info(path)
-        self.saving_document = None
+
         task = asyncio.create_task(self.websocket_server.serve(self))
         self.websocket_server.background_tasks.add(task)
         task.add_done_callback(self.websocket_server.background_tasks.discard)
 
-        # Close the connection if the document session expired
-        session_id = self.get_query_argument("sessionId", "")
-        if isinstance(self.room, DocumentRoom) and SERVER_SESSION != session_id:
-            self.close(1003, f"Document session {session_id} expired")
-
-        # cancel the deletion of the room if it was scheduled
-        if isinstance(self.room, DocumentRoom) and self.room.cleaner is not None:
-            self.room.cleaner.cancel()
-
-        if isinstance(self.room, DocumentRoom) and not self.room.ready:
-            file_format, file_type, file_path = self.get_file_info()
-            self.log.debug("Opening Y document from disk: %s", file_path)
-            model = await ensure_async(
-                self.contents_manager.get(file_path, type=file_type, format=file_format)
-            )
-            self.last_modified = model["last_modified"]
-            # check again if ready, because loading the file can be async
-            if not self.room.ready:
-                # try to apply Y updates from the YStore for this document
-                read_from_source = True
-                if self.room.ystore is not None:
-                    try:
-                        await self.room.ystore.apply_updates(self.room.ydoc)
-                        read_from_source = False
-                    except YDocNotFound:
-                        # YDoc not found in the YStore, create the document from the source file (no change history)
-                        pass
-                if not read_from_source:
-                    # if YStore updates and source file are out-of-sync, resync updates with source
-                    if self.room.document.source != model["content"]:
-                        read_from_source = True
-
-                if read_from_source:
-                    self.room.document.source = model["content"]
-                    if self.room.ystore:
-                        await self.room.ystore.encode_state_as_update(self.room.ydoc)
-                self.room.document.dirty = False
-                self.room.ready = True
-                self.room.watcher = asyncio.create_task(self.watch_file())
-                # save the document when changed
-                self.room.document.observe(self.on_document_change)
-
-    async def watch_file(self):
-        assert isinstance(self.room, DocumentRoom)
-        poll_interval = self.settings["collaborative_file_poll_interval"]
-        if not poll_interval:
-            self.room.watcher = None
-            return
-        while True:
-            await asyncio.sleep(poll_interval)
-            await self.maybe_load_document()
+        if isinstance(self.room, DocumentRoom):
+            # Close the connection if the document session expired
+            session_id = self.get_query_argument("sessionId", "")
+            if SERVER_SESSION != session_id:
+                self.close(1003, f"Document session {session_id} expired")
+
+            # cancel the deletion of the room if it was scheduled
+            if self.room.cleaner is not None:
+                self.room.cleaner.cancel()
 
-    async def maybe_load_document(self):
-        assert isinstance(self.room, DocumentRoom)
-        file_format, file_type, file_path = self.get_file_info()
-        async with self.lock:
-            model = await ensure_async(
-                self.contents_manager.get(
-                    file_path, content=False, type=file_type, format=file_format
-                )
-            )
-        # do nothing if the file was saved by us
-        if self.last_modified < model["last_modified"]:
-            self.log.debug("Reverting file that had out-of-band changes: %s", file_path)
-            model = await ensure_async(
-                self.contents_manager.get(file_path, type=file_type, format=file_format)
-            )
-            self.room.document.source = model["content"]
-            self.last_modified = model["last_modified"]
+            # Initialize the room
+            await self.room.initialize()
 
     async def send(self, message):
+        """
+        Send a message to the client.
+        """
         # needed to be compatible with WebsocketServer (websocket.send)
         try:
             self.write_message(message, binary=True)
         except Exception as e:
             self.log.debug("Failed to write message", exc_info=e)
 
     async def recv(self):
+        """
+        Receive a message from the client.
+        """
         message = await self._message_queue.get()
         return message
 
     def on_message(self, message):
+        """
+        On message receive.
+        """
         assert self.websocket_server is not None
         message_type = message[0]
         if message_type == YMessageType.AWARENESS:
             # awareness
             skip = False
             changes = self.room.awareness.get_changes(message[1:])
             added_users = changes["added"]
@@ -308,96 +301,109 @@
             # filter out message depending on changes
             if skip:
                 self.log.debug(
                     "Filtered out Y message of type: %s",
                     YMessageType(message_type).name,
                 )
                 return skip
+
         self._message_queue.put_nowait(message)
         self.websocket_server.ypatch_nb += 1
 
     def on_close(self) -> None:
+        """
+        On connection close.
+        """
         # stop serving this client
         self._message_queue.put_nowait(b"")
         if isinstance(self.room, DocumentRoom) and self.room.clients == [self]:
             # no client in this room after we disconnect
             # keep the document for a while in case someone reconnects
-            self.room.cleaner = asyncio.create_task(self.clean_room())
+            self.log.info("Cleaning room: %s", self._room_id)
+            self.room.cleaner = asyncio.create_task(self._clean_room())
 
-    async def clean_room(self) -> None:
+    async def _clean_room(self) -> None:
+        """
+        Async task for cleaning up the resources.
+
+        When all the clients of a room leave, we setup a task to clean up the resources
+        after a certain amount of time. We need to wait a few seconds to clean up the room
+        because sometimes websockets unintentionally disconnect.
+
+        During the clean up, we need to delete the room to free resources since the room
+        contains a copy of the document. In addition, we remove the file if there is no rooms
+        subscribed to it.
+        """
         assert isinstance(self.room, DocumentRoom)
-        seconds = self.settings["collaborative_document_cleanup_delay"]
-        if seconds is None:
+
+        if self._cleanup_delay is None:
             return
-        await asyncio.sleep(seconds)
-        if self.room.watcher is not None:
-            self.room.watcher.cancel()
-        self.room.document.unobserve()
+
+        await asyncio.sleep(self._cleanup_delay)
+
+        # Remove the room from the websocket server
         assert self.websocket_server is not None
-        file_format, file_type, file_path = self.get_file_info()
-        self.log.debug("Deleting Y document from memory: %s", file_path)
+        self.log.info("Deleting Y document from memory: %s", self.room.room_id)
         self.websocket_server.delete_room(room=self.room)
 
-    def on_document_change(self, target, event):
-        if target == "state" and "dirty" in event.keys:
-            dirty = event.keys["dirty"]["newValue"]
-            if not dirty:
-                # we cleared the dirty flag, nothing to save
-                return
-        if self.saving_document is not None and not self.saving_document.done():
-            # the document is being saved, cancel that
-            self.saving_document.cancel()
-            self.saving_document = None
-        self.saving_document = asyncio.create_task(self.maybe_save_document())
-
-    async def maybe_save_document(self):
-        assert isinstance(self.room, DocumentRoom)
-        seconds = self.settings["collaborative_document_save_delay"]
-        if seconds is None:
-            return
-        # save after X seconds of inactivity
-        await asyncio.sleep(seconds)
-        # if the room cannot be found, don't save
-        try:
-            file_format, file_type, file_path = self.get_file_info()
-        except Exception:
-            return
-        self.log.debug("Opening Y document from disk: %s", file_path)
-        async with self.lock:
-            model = await ensure_async(
-                self.contents_manager.get(file_path, type=file_type, format=file_format)
-            )
-        if self.last_modified < model["last_modified"]:
-            # file changed on disk, let's revert
-            self.log.debug("Reverting file that had out-of-band changes: %s", file_path)
-            self.room.document.source = model["content"]
-            self.last_modified = model["last_modified"]
-            return
-        if model["content"] != self.room.document.source:
-            # don't save if not needed
-            # this also prevents the dirty flag from bouncing between windows of
-            # the same document opened as different types (e.g. notebook/text editor)
-            model["format"] = file_format
-            model["content"] = self.room.document.source
-            self.log.debug("Saving Y document to disk: %s", file_path)
-            async with self.lock:
-                model = await ensure_async(self.contents_manager.save(model, file_path))
-                self.last_modified = model["last_modified"]
-        self.room.document.dirty = False
+        # Clean room
+        del self.room
+        self.log.info("Room %s deleted", self._room_id)
+
+        # Clean the file loader if there are not rooms using it
+        _, _, file_id = decode_file_path(self._room_id)
+        file = self.files[file_id]
+        if file.number_of_subscriptions == 0:
+            self.log.info("Deleting file %s", file.path)
+            file.clean()
+            del self.files[file_id]
 
     def check_origin(self, origin):
+        """
+        Check origin
+        """
         return True
 
+    @classmethod
+    def clean_up(cls):
+        """
+        Class method to stop every coroutine.
+
+        Useful to clean up tasks on server shut down.
+        """
+        log = getLogger(__name__)
+        log.info("Cleaning up resources before server shut down.")
+        if cls.websocket_server is not None:
+            # Cancel tasks and clean up
+            # TODO: should we wait for any save task?
+            rooms = list(cls.websocket_server.rooms.values())
+            log.info("Deleting rooms.")
+            for room in rooms:
+                cls.websocket_server.delete_room(room=room)
+
+        for file in cls.files.values():
+            file.clean()
+
+        log.info("Deleting files.")
+        cls.files.clear()
+
 
 class DocSessionHandler(APIHandler):
+    """
+    Jupyter Server's handler to retrieve the document's session.
+    """
+
     auth_resource = "contents"
 
     @web.authenticated
     @authorized
     async def put(self, path):
+        """
+        Creates a new session for a given document or returns an existing one.
+        """
         body = json.loads(self.request.body)
         format = body["format"]
         content_type = body["type"]
         file_id_manager = self.settings["file_id_manager"]
 
         idx = file_id_manager.get_id(path)
         if idx is not None:
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/package.json` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756201723113488%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.0-alpha.8', '@jupyter/docprovider': "*

 * *                   "'^1.0.0-alpha.8'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c7ae49e75d2022d8409a.js'}}",*

 * * "'version'": "'1.0.0-alpha.8'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.7",
-        "@jupyter/docprovider": "^1.0.0-alpha.7",
+        "@jupyter/collaboration": "^1.0.0-alpha.8",
+        "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyterlab/application": "^4.0.0-beta.0",
         "@jupyterlab/apputils": "^4.0.0-beta.0",
         "@jupyterlab/codemirror": "^4.0.0-beta.0",
         "@jupyterlab/coreutils": "^6.0.0-beta.0",
         "@jupyterlab/filebrowser": "^4.0.0-beta.0",
         "@jupyterlab/services": "^7.0.0-beta.0",
         "@jupyterlab/settingregistry": "^4.0.0-beta.0",
@@ -41,15 +41,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter_collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ed732341b4b6f42ac23d.js",
+            "load": "static/remoteEntry.c7ae49e75d2022d8409a.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/filebrowser-extension:defaultFileBrowser"
         ],
         "extension": true,
         "outputDir": "../../jupyter_collaboration/labextension",
@@ -125,9 +125,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.7"
+    "version": "1.0.0-alpha.8"
 }
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/schemas/@jupyter/collaboration-extension/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759358288770053%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.0-alpha.8', '@jupyter/docprovider': "*

 * *                   "'^1.0.0-alpha.8'}",*

 * * "'version'": "'1.0.0-alpha.8'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.7",
-        "@jupyter/docprovider": "^1.0.0-alpha.7",
+        "@jupyter/collaboration": "^1.0.0-alpha.8",
+        "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyterlab/application": "^4.0.0-beta.0",
         "@jupyterlab/apputils": "^4.0.0-beta.0",
         "@jupyterlab/codemirror": "^4.0.0-beta.0",
         "@jupyterlab/coreutils": "^6.0.0-beta.0",
         "@jupyterlab/filebrowser": "^4.0.0-beta.0",
         "@jupyterlab/services": "^7.0.0-beta.0",
         "@jupyterlab/settingregistry": "^4.0.0-beta.0",
@@ -120,9 +120,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.7"
+    "version": "1.0.0-alpha.8"
 }
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/413.ed870732b79e27f9bc6d.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/413.cf154c48ecaa08648e56.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -13,20 +13,23 @@
                 c = n(3205),
                 a = n(6834),
                 o = n(7225),
                 i = n(5852);
             const r = new Map,
                 d = "undefined" == typeof BroadcastChannel ? class {
                     constructor(e) {
-                        this.room = e, this.onmessage = null, i.z((s => s.key === e && null !== this.onmessage && this.onmessage({
+                        this.room = e, this.onmessage = null, this._onChange = s => s.key === e && null !== this.onmessage && this.onmessage({
                             data: o.Gh(s.newValue || "")
-                        })))
+                        }), i.z2(this._onChange)
                     }
                     postMessage(e) {
-                        i.X.setItem(this.room, o.s3(o.eh(e)))
+                        i.XN.setItem(this.room, o.s3(o.eh(e)))
+                    }
+                    close() {
+                        i.F(this._onChange)
                     }
                 } : BroadcastChannel,
                 h = e => c.Yu(r, e, (() => {
                     const s = a.Ue(),
                         n = new d(e);
                     return n.onmessage = e => s.forEach((s => s(e.data, "broadcastchannel"))), {
                         bc: n,
@@ -55,16 +58,16 @@
                         console.error("Caught error while handling a Yjs update", e)
                     }
                 },
                 _ = y;
             var g = n(6493),
                 p = n(2019),
                 v = n(1332),
-                k = n(9600),
-                E = n(4406);
+                E = n(9600),
+                k = n(4406);
             const C = 0,
                 I = 3,
                 M = 1,
                 U = 2,
                 H = [];
             H[C] = (e, s, n, t, c) => {
                 w.uE(e, C);
@@ -101,57 +104,58 @@
                 x = (e, s, n) => {
                     const t = f.l1(s),
                         c = w.Mf(),
                         a = f.yg(t),
                         o = e.messageHandlers[a];
                     return o ? o(c, t, e, n, a) : console.error("Unable to compute message"), c
                 },
-                B = e => {
+                P = e => {
                     if (e.shouldConnect && null === e.ws) {
                         const s = new e._WS(e.url);
                         s.binaryType = "arraybuffer", e.ws = s, e.wsconnecting = !0, e.wsconnected = !1, e.synced = !1, s.onmessage = n => {
                             e.wsLastMessageReceived = u.ZG();
                             const t = x(e, new Uint8Array(n.data), !0);
                             w.kE(t) > 1 && s.send(w._f(t))
                         }, s.onerror = s => {
                             e.emit("connection-error", [s, e])
                         }, s.onclose = s => {
                             e.emit("connection-close", [s, e]), e.ws = null, e.wsconnecting = !1, e.wsconnected ? (e.wsconnected = !1, e.synced = !1, g.Ag(e.awareness, Array.from(e.awareness.getStates().keys()).filter((s => s !== e.doc.clientID)), e), e.emit("status", [{
                                 status: "disconnected"
-                            }])) : e.wsUnsuccessfulReconnects++, setTimeout(B, v.VV(100 * v.sQ(2, e.wsUnsuccessfulReconnects), e.maxBackoffTime), e)
+                            }])) : e.wsUnsuccessfulReconnects++, setTimeout(P, v.VV(100 * v.sQ(2, e.wsUnsuccessfulReconnects), e.maxBackoffTime), e)
                         }, s.onopen = () => {
                             e.wsLastMessageReceived = u.ZG(), e.wsconnecting = !1, e.wsconnected = !0, e.wsUnsuccessfulReconnects = 0, e.emit("status", [{
                                 status: "connected"
                             }]);
                             const n = w.Mf();
                             if (w.uE(n, C), b(n, e.doc), s.send(w._f(n)), null !== e.awareness.getLocalState()) {
                                 const n = w.Mf();
                                 w.uE(n, M), w.mP(n, g.xq(e.awareness, [e.doc.clientID])), s.send(w._f(n))
                             }
                         }, e.emit("status", [{
                             status: "connecting"
                         }])
                     }
                 },
-                P = (e, s) => {
-                    e.wsconnected && e.ws.send(s), e.bcconnected && l(e.bcChannel, s, e)
+                B = (e, s) => {
+                    const n = e.ws;
+                    e.wsconnected && n && n.readyState === n.OPEN && n.send(s), e.bcconnected && l(e.bcChannel, s, e)
                 };
             class A extends p.y {
                 constructor(e, s, n, {
                     connect: t = !0,
                     awareness: c = new g.GL(n),
                     params: a = {},
                     WebSocketPolyfill: o = WebSocket,
                     resyncInterval: i = -1,
                     maxBackoffTime: r = 2500,
                     disableBc: d = !1
                 } = {}) {
                     for (super();
                         "/" === e[e.length - 1];) e = e.slice(0, e.length - 1);
-                    const h = (e => k.UI(e, ((e, s) => `${encodeURIComponent(s)}=${encodeURIComponent(e)}`)).join("&"))(a);
+                    const h = (e => E.UI(e, ((e, s) => `${encodeURIComponent(s)}=${encodeURIComponent(e)}`)).join("&"))(a);
                     this.maxBackoffTime = r, this.bcChannel = e + "/" + s, this.url = e + "/" + s + (0 === h.length ? "" : "?" + h), this.roomname = s, this.doc = n, this._WS = o, this.awareness = c, this.wsconnected = !1, this.wsconnecting = !1, this.bcconnected = !1, this.disableBc = d, this.wsUnsuccessfulReconnects = 0, this.messageHandlers = H.slice(), this._synced = !1, this.ws = null, this.wsLastMessageReceived = 0, this.shouldConnect = t, this._resyncInterval = 0, i > 0 && (this._resyncInterval = setInterval((() => {
                         if (this.ws && this.ws.readyState === WebSocket.OPEN) {
                             const e = w.Mf();
                             w.uE(e, C), b(e, n), this.ws.send(w._f(e))
                         }
                     }), i)), this._bcSubscriber = (e, s) => {
                         if (s !== this) {
@@ -159,38 +163,38 @@
                             w.kE(s) > 1 && l(this.bcChannel, w._f(s), this)
                         }
                     }, this._updateHandler = (e, s) => {
                         if (s !== this) {
                             const s = w.Mf();
                             w.uE(s, C), ((e, s) => {
                                 w.uE(e, 2), w.mP(e, s)
-                            })(s, e), P(this, w._f(s))
+                            })(s, e), B(this, w._f(s))
                         }
                     }, this.doc.on("update", this._updateHandler), this._awarenessUpdateHandler = ({
                         added: e,
                         updated: s,
                         removed: n
                     }, t) => {
                         const a = e.concat(s).concat(n),
                             o = w.Mf();
-                        w.uE(o, M), w.mP(o, g.xq(c, a)), P(this, w._f(o))
+                        w.uE(o, M), w.mP(o, g.xq(c, a)), B(this, w._f(o))
                     }, this._unloadHandler = () => {
                         g.Ag(this.awareness, [n.clientID], "window unload")
-                    }, "undefined" != typeof window ? window.addEventListener("unload", this._unloadHandler) : void 0 !== E && E.on("exit", this._unloadHandler), c.on("update", this._awarenessUpdateHandler), this._checkInterval = setInterval((() => {
+                    }, "undefined" != typeof window ? window.addEventListener("unload", this._unloadHandler) : void 0 !== k && k.on("exit", this._unloadHandler), c.on("update", this._awarenessUpdateHandler), this._checkInterval = setInterval((() => {
                         this.wsconnected && 3e4 < u.ZG() - this.wsLastMessageReceived && this.ws.close()
                     }), 3e3), t && this.connect()
                 }
                 get synced() {
                     return this._synced
                 }
                 set synced(e) {
                     this._synced !== e && (this._synced = e, this.emit("synced", [e]), this.emit("sync", [e]))
                 }
                 destroy() {
-                    0 !== this._resyncInterval && clearInterval(this._resyncInterval), clearInterval(this._checkInterval), this.disconnect(), "undefined" != typeof window ? window.removeEventListener("unload", this._unloadHandler) : void 0 !== E && E.off("exit", this._unloadHandler), this.awareness.off("update", this._awarenessUpdateHandler), this.doc.off("update", this._updateHandler), super.destroy()
+                    0 !== this._resyncInterval && clearInterval(this._resyncInterval), clearInterval(this._checkInterval), this.disconnect(), "undefined" != typeof window ? window.removeEventListener("unload", this._unloadHandler) : void 0 !== k && k.off("exit", this._unloadHandler), this.awareness.off("update", this._awarenessUpdateHandler), this.doc.off("update", this._updateHandler), super.destroy()
                 }
                 connectBc() {
                     if (this.disableBc) return;
                     var e, s;
                     this.bcconnected || (e = this.bcChannel, s = this._bcSubscriber, h(e).subs.add(s), this.bcconnected = !0);
                     const n = w.Mf();
                     w.uE(n, C), b(n, this.doc), l(this.bcChannel, w._f(n), this);
@@ -199,22 +203,22 @@
                     const c = w.Mf();
                     w.uE(c, I), l(this.bcChannel, w._f(c), this);
                     const a = w.Mf();
                     w.uE(a, M), w.mP(a, g.xq(this.awareness, [this.doc.clientID])), l(this.bcChannel, w._f(a), this)
                 }
                 disconnectBc() {
                     const e = w.Mf();
-                    w.uE(e, M), w.mP(e, g.xq(this.awareness, [this.doc.clientID], new Map)), P(this, w._f(e)), this.bcconnected && (((e, s) => {
+                    w.uE(e, M), w.mP(e, g.xq(this.awareness, [this.doc.clientID], new Map)), B(this, w._f(e)), this.bcconnected && (((e, s) => {
                         const n = h(e);
                         n.subs.delete(s) && 0 === n.subs.size && (n.bc.close(), r.delete(e))
                     })(this.bcChannel, this._bcSubscriber), this.bcconnected = !1)
                 }
                 disconnect() {
                     this.shouldConnect = !1, this.disconnectBc(), null !== this.ws && this.ws.close()
                 }
                 connect() {
-                    this.shouldConnect = !0, this.wsconnected || null !== this.ws || (B(this), this.connectBc())
+                    this.shouldConnect = !0, this.wsconnected || null !== this.ws || (P(this), this.connectBc())
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/493.186e89468d33ae2f1acb.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/493.0975334cbddac1bcf819.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,427 +1,429 @@
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
     [493], {
-        5650: (t, e, r) => {
+        5650: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 $2: () => o,
                 RP: () => a,
                 jS: () => c,
-                rc: () => n,
+                rc: () => r,
                 x1: () => s
             });
-            const n = 64,
+            const r = 64,
                 s = 128,
                 o = 63,
                 c = 127,
                 a = 2147483647
         },
-        7225: (t, e, r) => {
+        7225: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 eh: () => m,
                 Te: () => y,
-                Gh: () => w,
+                Gh: () => v,
                 s3: () => b
             });
-            var n = r(5931),
-                s = r(3205);
-            var o = r(5852),
-                c = r(1872),
-                a = r(4406);
+            var r = n(5931),
+                s = n(3205);
+            var o = n(5852),
+                c = n(1985),
+                a = n(4406);
             const i = void 0 !== a && a.release && /node|io\.js/.test(a.release.name),
-                l = "undefined" != typeof window && !i;
+                l = "undefined" != typeof window && "undefined" != typeof document && !i;
             let u;
             "undefined" != typeof navigator && /Mac/.test(navigator.platform);
             const h = [],
                 f = t => (() => {
                     if (void 0 === u)
                         if (i) {
                             u = s.Ue();
                             const t = a.argv;
                             let e = null;
-                            for (let r = 0; r < t.length; r++) {
-                                const n = t[r];
-                                "-" === n[0] ? (null !== e && u.set(e, ""), e = n) : null !== e ? (u.set(e, n), e = null) : h.push(n)
+                            for (let n = 0; n < t.length; n++) {
+                                const r = t[n];
+                                "-" === r[0] ? (null !== e && u.set(e, ""), e = r) : null !== e ? (u.set(e, r), e = null) : h.push(r)
                             }
                             null !== e && u.set(e, "")
                         } else "object" == typeof location ? (u = s.Ue(), (location.search || "?").slice(1).split("&").forEach((t => {
                             if (0 !== t.length) {
-                                const [e, r] = t.split("=");
-                                u.set(`--${n.NF(e,"-")}`, r), u.set(`-${n.NF(e,"-")}`, r)
+                                const [e, n] = t.split("=");
+                                u.set(`--${r.NF(e,"-")}`, n), u.set(`-${r.NF(e,"-")}`, n)
                             }
                         }))) : u = s.Ue();
                     return u
                 })().has(t),
                 d = t => {
-                    return void 0 === (e = i ? a.env[t.toUpperCase()] : o.X.getItem(t)) ? null : e;
+                    return void 0 === (e = i ? a.env[t.toUpperCase()] : o.XN.getItem(t)) ? null : e;
                     var e
                 };
             f("--" + "production") || d("production");
             const p = i && c.gB(a.env.FORCE_COLOR, ["true", "1", "2"]),
                 g = (!f("no-colors") && (!i || a.stdout.isTTY || p) && (!i || f("color") || p || null !== d("COLORTERM") || (d("TERM") || "").includes("color")), t => new Uint8Array(t)),
-                y = (t, e, r) => new Uint8Array(t, e, r),
+                y = (t, e, n) => new Uint8Array(t, e, n),
                 m = t => new Uint8Array(t),
                 b = l ? t => {
                     let e = "";
-                    for (let r = 0; r < t.byteLength; r++) e += n.IK(t[r]);
+                    for (let n = 0; n < t.byteLength; n++) e += r.IK(t[n]);
                     return btoa(e)
                 } : t => Buffer.from(t.buffer, t.byteOffset, t.byteLength).toString("base64"),
-                w = l ? t => {
+                v = l ? t => {
                     const e = atob(t),
-                        r = g(e.length);
-                    for (let t = 0; t < e.length; t++) r[t] = e.charCodeAt(t);
-                    return r
+                        n = g(e.length);
+                    for (let t = 0; t < e.length; t++) n[t] = e.charCodeAt(t);
+                    return n
                 } : t => {
                     const e = Buffer.from(t, "base64");
                     return new Uint8Array(e.buffer, e.byteOffset, e.byteLength)
                 }
         },
-        2256: (t, e, r) => {
+        2256: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 l1: () => h,
                 kf: () => g,
                 yg: () => p,
                 HN: () => f
             });
-            var n = r(7225),
-                s = r(5650);
-            r(1332);
+            var r = n(7225),
+                s = n(5650);
+            n(1332);
             const o = Number.MAX_SAFE_INTEGER;
             Number.MIN_SAFE_INTEGER, s.RP, Number.isInteger, Number.isNaN, Number.parseInt;
-            var c = r(5931);
+            var c = n(5931);
             const a = t => new Error(t),
                 i = a("Unexpected end of array"),
                 l = a("Integer out of Range");
             class u {
                 constructor(t) {
                     this.arr = t, this.pos = 0
                 }
             }
             const h = t => new u(t),
                 f = t => ((t, e) => {
-                    const r = n.Te(t.arr.buffer, t.pos + t.arr.byteOffset, e);
-                    return t.pos += e, r
+                    const n = r.Te(t.arr.buffer, t.pos + t.arr.byteOffset, e);
+                    return t.pos += e, n
                 })(t, p(t)),
                 d = t => t.arr[t.pos++],
                 p = t => {
                     let e = 0,
-                        r = 1;
-                    const n = t.arr.length;
-                    for (; t.pos < n;) {
-                        const n = t.arr[t.pos++];
-                        if (e += (n & s.jS) * r, r *= 128, n < s.x1) return e;
+                        n = 1;
+                    const r = t.arr.length;
+                    for (; t.pos < r;) {
+                        const r = t.arr[t.pos++];
+                        if (e += (r & s.jS) * n, n *= 128, r < s.x1) return e;
                         if (e > o) throw l
                     }
                     throw i
                 },
                 g = c.CO ? t => c.CO.decode(f(t)) : t => {
                     let e = p(t);
                     if (0 === e) return ""; {
-                        let r = String.fromCodePoint(d(t));
+                        let n = String.fromCodePoint(d(t));
                         if (--e < 100)
-                            for (; e--;) r += String.fromCodePoint(d(t));
+                            for (; e--;) n += String.fromCodePoint(d(t));
                         else
                             for (; e > 0;) {
-                                const n = e < 1e4 ? e : 1e4,
-                                    s = t.arr.subarray(t.pos, t.pos + n);
-                                t.pos += n, r += String.fromCodePoint.apply(null, s), e -= n
+                                const r = e < 1e4 ? e : 1e4,
+                                    s = t.arr.subarray(t.pos, t.pos + r);
+                                t.pos += r, n += String.fromCodePoint.apply(null, s), e -= r
                             }
-                        return decodeURIComponent(escape(r))
+                        return decodeURIComponent(escape(n))
                     }
                 }
         },
-        9476: (t, e, r) => {
+        9476: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 Mf: () => i,
                 _f: () => u,
                 kE: () => l,
                 mP: () => y,
                 uE: () => f,
                 uw: () => g
             });
-            var n = r(7225),
-                s = r(1332),
-                o = r(5650),
-                c = r(5931);
+            var r = n(7225),
+                s = n(1332),
+                o = n(5650),
+                c = n(5931);
             class a {
                 constructor() {
                     this.cpos = 0, this.cbuf = new Uint8Array(100), this.bufs = []
                 }
             }
             const i = () => new a,
                 l = t => {
                     let e = t.cpos;
-                    for (let r = 0; r < t.bufs.length; r++) e += t.bufs[r].length;
+                    for (let n = 0; n < t.bufs.length; n++) e += t.bufs[n].length;
                     return e
                 },
                 u = t => {
                     const e = new Uint8Array(l(t));
-                    let r = 0;
-                    for (let n = 0; n < t.bufs.length; n++) {
-                        const s = t.bufs[n];
-                        e.set(s, r), r += s.length
+                    let n = 0;
+                    for (let r = 0; r < t.bufs.length; r++) {
+                        const s = t.bufs[r];
+                        e.set(s, n), n += s.length
                     }
-                    return e.set(n.Te(t.cbuf.buffer, 0, t.cpos), r), e
+                    return e.set(r.Te(t.cbuf.buffer, 0, t.cpos), n), e
                 },
                 h = (t, e) => {
-                    const r = t.cbuf.length;
-                    t.cpos === r && (t.bufs.push(t.cbuf), t.cbuf = new Uint8Array(2 * r), t.cpos = 0), t.cbuf[t.cpos++] = e
+                    const n = t.cbuf.length;
+                    t.cpos === n && (t.bufs.push(t.cbuf), t.cbuf = new Uint8Array(2 * n), t.cpos = 0), t.cbuf[t.cpos++] = e
                 },
                 f = (t, e) => {
                     for (; e > o.jS;) h(t, o.x1 | o.jS & e), e = s.GW(e / 128);
                     h(t, o.jS & e)
                 },
                 d = new Uint8Array(3e4),
                 p = d.length / 3,
                 g = c.YZ && c.YZ.encodeInto ? (t, e) => {
                     if (e.length < p) {
-                        const r = c.YZ.encodeInto(e, d).written || 0;
-                        f(t, r);
-                        for (let e = 0; e < r; e++) h(t, d[e])
+                        const n = c.YZ.encodeInto(e, d).written || 0;
+                        f(t, n);
+                        for (let e = 0; e < n; e++) h(t, d[e])
                     } else y(t, c.lz(e))
                 } : (t, e) => {
-                    const r = unescape(encodeURIComponent(e)),
-                        n = r.length;
-                    f(t, n);
-                    for (let e = 0; e < n; e++) h(t, r.codePointAt(e))
+                    const n = unescape(encodeURIComponent(e)),
+                        r = n.length;
+                    f(t, r);
+                    for (let e = 0; e < r; e++) h(t, n.codePointAt(e))
                 },
                 y = (t, e) => {
                     f(t, e.byteLength), ((t, e) => {
-                        const r = t.cbuf.length,
-                            n = t.cpos,
-                            o = s.VV(r - n, e.length),
+                        const n = t.cbuf.length,
+                            r = t.cpos,
+                            o = s.VV(n - r, e.length),
                             c = e.length - o;
-                        t.cbuf.set(e.subarray(0, o), n), t.cpos += o, c > 0 && (t.bufs.push(t.cbuf), t.cbuf = new Uint8Array(s.Fp(2 * r, c)), t.cbuf.set(e.subarray(o)), t.cpos = c)
+                        t.cbuf.set(e.subarray(0, o), r), t.cpos += o, c > 0 && (t.bufs.push(t.cbuf), t.cbuf = new Uint8Array(s.Fp(2 * n, c)), t.cbuf.set(e.subarray(o)), t.cpos = c)
                     })(t, e)
                 };
             new DataView(new ArrayBuffer(4))
         },
-        1872: (t, e, r) => {
+        1985: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 Hi: () => s,
                 gB: () => o
             });
-            var n = r(9600);
+            var r = n(9600);
             const s = (t, e) => {
                     if (null == t || null == e) return ((t, e) => t === e)(t, e);
                     if (t.constructor !== e.constructor) return !1;
                     if (t === e) return !0;
                     switch (t.constructor) {
                         case ArrayBuffer:
                             t = new Uint8Array(t), e = new Uint8Array(e);
                         case Uint8Array:
                             if (t.byteLength !== e.byteLength) return !1;
-                            for (let r = 0; r < t.length; r++)
-                                if (t[r] !== e[r]) return !1;
+                            for (let n = 0; n < t.length; n++)
+                                if (t[n] !== e[n]) return !1;
                             break;
                         case Set:
                             if (t.size !== e.size) return !1;
-                            for (const r of t)
-                                if (!e.has(r)) return !1;
+                            for (const n of t)
+                                if (!e.has(n)) return !1;
                             break;
                         case Map:
                             if (t.size !== e.size) return !1;
-                            for (const r of t.keys())
-                                if (!e.has(r) || !s(t.get(r), e.get(r))) return !1;
+                            for (const n of t.keys())
+                                if (!e.has(n) || !s(t.get(n), e.get(n))) return !1;
                             break;
                         case Object:
-                            if (n.kE(t) !== n.kE(e)) return !1;
-                            for (const r in t)
-                                if (!n.l$(t, r) || !s(t[r], e[r])) return !1;
+                            if (r.kE(t) !== r.kE(e)) return !1;
+                            for (const n in t)
+                                if (!r.l$(t, n) || !s(t[n], e[n])) return !1;
                             break;
                         case Array:
                             if (t.length !== e.length) return !1;
-                            for (let r = 0; r < t.length; r++)
-                                if (!s(t[r], e[r])) return !1;
+                            for (let n = 0; n < t.length; n++)
+                                if (!s(t[n], e[n])) return !1;
                             break;
                         default:
                             return !1
                     }
                     return !0
                 },
                 o = (t, e) => e.includes(t)
         },
-        3205: (t, e, r) => {
+        3205: (t, e, n) => {
             "use strict";
-            r.d(e, {
-                Ue: () => n,
+            n.d(e, {
+                Ue: () => r,
                 Yu: () => s
             });
-            const n = () => new Map,
-                s = (t, e, r) => {
-                    let n = t.get(e);
-                    return void 0 === n && t.set(e, n = r()), n
+            const r = () => new Map,
+                s = (t, e, n) => {
+                    let r = t.get(e);
+                    return void 0 === r && t.set(e, r = n()), r
                 }
         },
-        1332: (t, e, r) => {
+        1332: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 Fp: () => o,
-                GW: () => n,
+                GW: () => r,
                 VV: () => s,
                 sQ: () => c
             });
-            const n = Math.floor,
+            const r = Math.floor,
                 s = (Math.ceil, Math.abs, Math.imul, Math.round, Math.log10, Math.log2, Math.log, Math.sqrt, (t, e) => t < e ? t : e),
                 o = (t, e) => t > e ? t : e,
                 c = (Number.isNaN, Math.pow);
             Math.sign
         },
-        9600: (t, e, r) => {
+        9600: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 UI: () => s,
                 kE: () => o,
                 l$: () => c
             }), Object.assign;
-            const n = Object.keys,
+            const r = Object.keys,
                 s = (t, e) => {
-                    const r = [];
-                    for (const n in t) r.push(e(t[n], n));
-                    return r
+                    const n = [];
+                    for (const r in t) n.push(e(t[r], r));
+                    return n
                 },
-                o = t => n(t).length,
+                o = t => r(t).length,
                 c = (t, e) => Object.prototype.hasOwnProperty.call(t, e)
         },
-        2019: (t, e, r) => {
+        2019: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 y: () => c
             });
-            var n = r(3205),
-                s = r(6834);
+            var r = n(3205),
+                s = n(6834);
             const o = Array.from;
             Array.isArray;
             class c {
                 constructor() {
-                    this._observers = n.Ue()
+                    this._observers = r.Ue()
                 }
                 on(t, e) {
-                    n.Yu(this._observers, t, s.Ue).add(e)
+                    r.Yu(this._observers, t, s.Ue).add(e)
                 }
                 once(t, e) {
-                    const r = (...n) => {
-                        this.off(t, r), e(...n)
+                    const n = (...r) => {
+                        this.off(t, n), e(...r)
                     };
-                    this.on(t, r)
+                    this.on(t, n)
                 }
                 off(t, e) {
-                    const r = this._observers.get(t);
-                    void 0 !== r && (r.delete(e), 0 === r.size && this._observers.delete(t))
+                    const n = this._observers.get(t);
+                    void 0 !== n && (n.delete(e), 0 === n.size && this._observers.delete(t))
                 }
                 emit(t, e) {
-                    return o((this._observers.get(t) || n.Ue()).values()).forEach((t => t(...e)))
+                    return o((this._observers.get(t) || r.Ue()).values()).forEach((t => t(...e)))
                 }
                 destroy() {
-                    this._observers = n.Ue()
+                    this._observers = r.Ue()
                 }
             }
         },
-        6834: (t, e, r) => {
+        6834: (t, e, n) => {
             "use strict";
-            r.d(e, {
-                Ue: () => n
+            n.d(e, {
+                Ue: () => r
             });
-            const n = () => new Set
+            const r = () => new Set
         },
-        5852: (t, e, r) => {
+        5852: (t, e, n) => {
             "use strict";
-            r.d(e, {
-                X: () => o,
-                z: () => c
+            n.d(e, {
+                F: () => a,
+                XN: () => o,
+                z2: () => c
             });
-            let n = new class {
+            let r = new class {
                     constructor() {
                         this.map = new Map
                     }
                     setItem(t, e) {
                         this.map.set(t, e)
                     }
                     getItem(t) {
                         return this.map.get(t)
                     }
                 },
                 s = !0;
             try {
-                "undefined" != typeof localStorage && (n = localStorage, s = !1)
+                "undefined" != typeof localStorage && (r = localStorage, s = !1)
             } catch (t) {}
-            const o = n,
-                c = t => s || addEventListener("storage", t)
+            const o = r,
+                c = t => s || addEventListener("storage", t),
+                a = t => s || removeEventListener("storage", t)
         },
-        5931: (t, e, r) => {
+        5931: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 CO: () => l,
-                IK: () => n,
+                IK: () => r,
                 NF: () => c,
                 YZ: () => a,
                 lz: () => i
             });
-            const n = String.fromCharCode,
+            const r = String.fromCharCode,
                 s = (String.fromCodePoint, /^\s*/g),
                 o = /([A-Z])/g,
                 c = (t, e) => (t => t.replace(s, ""))(t.replace(o, (t => `${e}${(t=>t.toLowerCase())(t)}`))),
                 a = "undefined" != typeof TextEncoder ? new TextEncoder : null,
                 i = a ? t => a.encode(t) : t => {
                     const e = unescape(encodeURIComponent(t)),
-                        r = e.length,
-                        n = new Uint8Array(r);
-                    for (let t = 0; t < r; t++) n[t] = e.codePointAt(t);
-                    return n
+                        n = e.length,
+                        r = new Uint8Array(n);
+                    for (let t = 0; t < n; t++) r[t] = e.codePointAt(t);
+                    return r
                 };
             let l = "undefined" == typeof TextDecoder ? null : new TextDecoder("utf-8", {
                 fatal: !0,
                 ignoreBOM: !0
             });
             l && 1 === l.decode(new Uint8Array).length && (l = null)
         },
-        870: (t, e, r) => {
+        870: (t, e, n) => {
             "use strict";
-            r.d(e, {
-                ZG: () => n
+            n.d(e, {
+                ZG: () => r
             });
-            const n = Date.now
+            const r = Date.now
         },
         4406: t => {
-            var e, r, n = t.exports = {};
+            var e, n, r = t.exports = {};
 
             function s() {
                 throw new Error("setTimeout has not been defined")
             }
 
             function o() {
                 throw new Error("clearTimeout has not been defined")
             }
 
             function c(t) {
                 if (e === setTimeout) return setTimeout(t, 0);
                 if ((e === s || !e) && setTimeout) return e = setTimeout, setTimeout(t, 0);
                 try {
                     return e(t, 0)
-                } catch (r) {
+                } catch (n) {
                     try {
                         return e.call(null, t, 0)
-                    } catch (r) {
+                    } catch (n) {
                         return e.call(this, t, 0)
                     }
                 }
             }! function() {
                 try {
                     e = "function" == typeof setTimeout ? setTimeout : s
                 } catch (t) {
                     e = s
                 }
                 try {
-                    r = "function" == typeof clearTimeout ? clearTimeout : o
+                    n = "function" == typeof clearTimeout ? clearTimeout : o
                 } catch (t) {
-                    r = o
+                    n = o
                 }
             }();
             var a, i = [],
                 l = !1,
                 u = -1;
 
             function h() {
@@ -434,94 +436,94 @@
                     l = !0;
                     for (var e = i.length; e;) {
                         for (a = i, i = []; ++u < e;) a && a[u].run();
                         u = -1, e = i.length
                     }
                     a = null, l = !1,
                         function(t) {
-                            if (r === clearTimeout) return clearTimeout(t);
-                            if ((r === o || !r) && clearTimeout) return r = clearTimeout, clearTimeout(t);
+                            if (n === clearTimeout) return clearTimeout(t);
+                            if ((n === o || !n) && clearTimeout) return n = clearTimeout, clearTimeout(t);
                             try {
-                                return r(t)
+                                return n(t)
                             } catch (e) {
                                 try {
-                                    return r.call(null, t)
+                                    return n.call(null, t)
                                 } catch (e) {
-                                    return r.call(this, t)
+                                    return n.call(this, t)
                                 }
                             }
                         }(t)
                 }
             }
 
             function d(t, e) {
                 this.fun = t, this.array = e
             }
 
             function p() {}
-            n.nextTick = function(t) {
+            r.nextTick = function(t) {
                 var e = new Array(arguments.length - 1);
                 if (arguments.length > 1)
-                    for (var r = 1; r < arguments.length; r++) e[r - 1] = arguments[r];
+                    for (var n = 1; n < arguments.length; n++) e[n - 1] = arguments[n];
                 i.push(new d(t, e)), 1 !== i.length || l || c(f)
             }, d.prototype.run = function() {
                 this.fun.apply(null, this.array)
-            }, n.title = "browser", n.browser = !0, n.env = {}, n.argv = [], n.version = "", n.versions = {}, n.on = p, n.addListener = p, n.once = p, n.off = p, n.removeListener = p, n.removeAllListeners = p, n.emit = p, n.prependListener = p, n.prependOnceListener = p, n.listeners = function(t) {
+            }, r.title = "browser", r.browser = !0, r.env = {}, r.argv = [], r.version = "", r.versions = {}, r.on = p, r.addListener = p, r.once = p, r.off = p, r.removeListener = p, r.removeAllListeners = p, r.emit = p, r.prependListener = p, r.prependOnceListener = p, r.listeners = function(t) {
                 return []
-            }, n.binding = function(t) {
+            }, r.binding = function(t) {
                 throw new Error("process.binding is not supported")
-            }, n.cwd = function() {
+            }, r.cwd = function() {
                 return "/"
-            }, n.chdir = function(t) {
+            }, r.chdir = function(t) {
                 throw new Error("process.chdir is not supported")
-            }, n.umask = function() {
+            }, r.umask = function() {
                 return 0
             }
         },
-        6493: (t, e, r) => {
+        6493: (t, e, n) => {
             "use strict";
-            r.d(e, {
+            n.d(e, {
                 Ag: () => u,
                 GL: () => l,
                 oy: () => f,
                 xq: () => h
             });
-            var n = r(9476),
-                s = r(2256),
-                o = r(870),
-                c = r(1332),
-                a = r(2019),
-                i = r(1872);
-            r(981);
+            var r = n(9476),
+                s = n(2256),
+                o = n(870),
+                c = n(1332),
+                a = n(2019),
+                i = n(1985);
+            n(981);
             class l extends a.y {
                 constructor(t) {
                     super(), this.doc = t, this.clientID = t.clientID, this.states = new Map, this.meta = new Map, this._checkInterval = setInterval((() => {
                         const t = o.ZG();
                         null !== this.getLocalState() && 15e3 <= t - this.meta.get(this.clientID).lastUpdated && this.setLocalState(this.getLocalState());
                         const e = [];
-                        this.meta.forEach(((r, n) => {
-                            n !== this.clientID && 3e4 <= t - r.lastUpdated && this.states.has(n) && e.push(n)
+                        this.meta.forEach(((n, r) => {
+                            r !== this.clientID && 3e4 <= t - n.lastUpdated && this.states.has(r) && e.push(r)
                         })), e.length > 0 && u(this, e, "timeout")
                     }), c.GW(3e3)), t.on("destroy", (() => {
                         this.destroy()
                     })), this.setLocalState({})
                 }
                 destroy() {
                     this.emit("destroy", [this]), this.setLocalState(null), super.destroy(), clearInterval(this._checkInterval)
                 }
                 getLocalState() {
                     return this.states.get(this.clientID) || null
                 }
                 setLocalState(t) {
                     const e = this.clientID,
-                        r = this.meta.get(e),
-                        n = void 0 === r ? 0 : r.clock + 1,
+                        n = this.meta.get(e),
+                        r = void 0 === n ? 0 : n.clock + 1,
                         s = this.states.get(e);
                     null === t ? this.states.delete(e) : this.states.set(e, t), this.meta.set(e, {
-                        clock: n,
+                        clock: r,
                         lastUpdated: o.ZG()
                     });
                     const c = [],
                         a = [],
                         l = [],
                         u = [];
                     null === t ? u.push(e) : null == s ? null != t && c.push(e) : (a.push(e), i.Hi(s, t) || l.push(e)), (c.length > 0 || l.length > 0 || u.length > 0) && this.emit("change", [{
@@ -531,86 +533,86 @@
                     }, "local"]), this.emit("update", [{
                         added: c,
                         updated: a,
                         removed: u
                     }, "local"])
                 }
                 setLocalStateField(t, e) {
-                    const r = this.getLocalState();
-                    null !== r && this.setLocalState({
-                        ...r,
+                    const n = this.getLocalState();
+                    null !== n && this.setLocalState({
+                        ...n,
                         [t]: e
                     })
                 }
                 getStates() {
                     return this.states
                 }
             }
-            const u = (t, e, r) => {
-                    const n = [];
-                    for (let r = 0; r < e.length; r++) {
-                        const s = e[r];
+            const u = (t, e, n) => {
+                    const r = [];
+                    for (let n = 0; n < e.length; n++) {
+                        const s = e[n];
                         if (t.states.has(s)) {
                             if (t.states.delete(s), s === t.clientID) {
                                 const e = t.meta.get(s);
                                 t.meta.set(s, {
                                     clock: e.clock + 1,
                                     lastUpdated: o.ZG()
                                 })
                             }
-                            n.push(s)
+                            r.push(s)
                         }
                     }
-                    n.length > 0 && (t.emit("change", [{
+                    r.length > 0 && (t.emit("change", [{
                         added: [],
                         updated: [],
-                        removed: n
-                    }, r]), t.emit("update", [{
+                        removed: r
+                    }, n]), t.emit("update", [{
                         added: [],
                         updated: [],
-                        removed: n
-                    }, r]))
+                        removed: r
+                    }, n]))
                 },
-                h = (t, e, r = t.states) => {
+                h = (t, e, n = t.states) => {
                     const s = e.length,
-                        o = n.Mf();
-                    n.uE(o, s);
+                        o = r.Mf();
+                    r.uE(o, s);
                     for (let c = 0; c < s; c++) {
                         const s = e[c],
-                            a = r.get(s) || null,
+                            a = n.get(s) || null,
                             i = t.meta.get(s).clock;
-                        n.uE(o, s), n.uE(o, i), n.uw(o, JSON.stringify(a))
+                        r.uE(o, s), r.uE(o, i), r.uw(o, JSON.stringify(a))
                     }
-                    return n._f(o)
+                    return r._f(o)
                 },
-                f = (t, e, r) => {
-                    const n = s.l1(e),
+                f = (t, e, n) => {
+                    const r = s.l1(e),
                         c = o.ZG(),
                         a = [],
                         l = [],
                         u = [],
                         h = [],
-                        f = s.yg(n);
+                        f = s.yg(r);
                     for (let e = 0; e < f; e++) {
-                        const e = s.yg(n);
-                        let r = s.yg(n);
-                        const o = JSON.parse(s.kf(n)),
+                        const e = s.yg(r);
+                        let n = s.yg(r);
+                        const o = JSON.parse(s.kf(r)),
                             f = t.meta.get(e),
                             d = t.states.get(e),
                             p = void 0 === f ? 0 : f.clock;
-                        (p < r || p === r && null === o && t.states.has(e)) && (null === o ? e === t.clientID && null != t.getLocalState() ? r++ : t.states.delete(e) : t.states.set(e, o), t.meta.set(e, {
-                            clock: r,
+                        (p < n || p === n && null === o && t.states.has(e)) && (null === o ? e === t.clientID && null != t.getLocalState() ? n++ : t.states.delete(e) : t.states.set(e, o), t.meta.set(e, {
+                            clock: n,
                             lastUpdated: c
                         }), void 0 === f && null !== o ? a.push(e) : void 0 !== f && null === o ? h.push(e) : null !== o && (i.Hi(o, d) || u.push(e), l.push(e)))
                     }(a.length > 0 || u.length > 0 || h.length > 0) && t.emit("change", [{
                         added: a,
                         updated: u,
                         removed: h
-                    }, r]), (a.length > 0 || l.length > 0 || h.length > 0) && t.emit("update", [{
+                    }, n]), (a.length > 0 || l.length > 0 || h.length > 0) && t.emit("update", [{
                         added: a,
                         updated: l,
                         removed: h
-                    }, r])
+                    }, n])
                 }
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/497.53bcecf29101af297e6d.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/497.ab1a0ee570b8e4f31289.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,208 +1,212 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
     [497], {
-        9497: (e, r, t) => {
-            t.r(r), t.d(r, {
+        9497: (e, t, r) => {
+            r.r(t), r.d(t, {
                 default: () => S
             });
-            var o, a = t(8872),
-                n = t(9582),
-                s = t(2998),
-                i = t(225),
-                l = t(3e3),
-                c = t(9831);
+            var o, n = r(2281),
+                a = r(1371),
+                i = r(726),
+                s = r(5581),
+                l = r(3e3),
+                c = r(5996);
             ! function(e) {
                 e.openPath = "filebrowser:open-path"
             }(o || (o = {}));
             const d = {
                     id: "@jupyter/collaboration-extension:drive",
+                    description: "The default collaborative drive provider",
                     provides: c.ICollaborativeDrive,
-                    requires: [s.ITranslator],
+                    requires: [i.ITranslator],
                     optional: [],
-                    activate: (e, r) => {
-                        const t = r.load("jupyter_collaboration"),
-                            o = new c.YDrive(e.serviceManager.user, t);
+                    activate: (e, t) => {
+                        const r = t.load("jupyter_collaboration"),
+                            o = new c.YDrive(e.serviceManager.user, r);
                         return e.serviceManager.contents.addDrive(o), o
                     }
                 },
                 u = {
                     id: "@jupyter/collaboration-extension:yfile",
+                    description: "Plugin to register the shared model factory for the content type 'file'",
                     autoStart: !0,
                     requires: [c.ICollaborativeDrive],
                     optional: [],
-                    activate: (e, r) => {
-                        r.sharedModelFactory.registerDocumentFactory("file", (() => new l.YFile))
+                    activate: (e, t) => {
+                        t.sharedModelFactory.registerDocumentFactory("file", (() => new l.YFile))
                     }
                 },
                 p = {
                     id: "@jupyter/collaboration-extension:ynotebook",
+                    description: "Plugin to register the shared model factory for the content type 'notebook'",
                     autoStart: !0,
                     requires: [c.ICollaborativeDrive],
-                    optional: [i.ISettingRegistry],
-                    activate: (e, r, t) => {
+                    optional: [s.ISettingRegistry],
+                    activate: (e, t, r) => {
                         let o = !0;
-                        t && t.load("@jupyterlab/notebook-extension:tracker").then((e => {
-                            const r = e => {
-                                var r;
-                                const t = null == e ? void 0 : e.get("experimentalEnableDocumentWideUndoRedo").composite;
-                                o = null === (r = !t) || void 0 === r || r
+                        r && r.load("@jupyterlab/notebook-extension:tracker").then((e => {
+                            const t = e => {
+                                var t;
+                                const r = null == e ? void 0 : e.get("experimentalEnableDocumentWideUndoRedo").composite;
+                                o = null === (t = !r) || void 0 === t || t
                             };
-                            r(e), e.changed.connect((e => r(e)))
-                        })), r.sharedModelFactory.registerDocumentFactory("notebook", (() => new l.YNotebook({
+                            t(e), e.changed.connect((e => t(e)))
+                        })), t.sharedModelFactory.registerDocumentFactory("notebook", (() => new l.YNotebook({
                             disableDocumentWideUndoRedo: o
                         })))
                     }
                 },
                 v = {
                     id: "@jupyter/collaboration-extension:defaultFileBrowser",
-                    provides: n.IDefaultFileBrowser,
-                    requires: [c.ICollaborativeDrive, n.IFileBrowserFactory],
-                    optional: [a.IRouter, a.JupyterFrontEnd.ITreeResolver, a.ILabShell, i.ISettingRegistry],
-                    activate: async (e, r, t, o, a, n) => {
+                    description: "The default file browser factory provider",
+                    provides: a.IDefaultFileBrowser,
+                    requires: [c.ICollaborativeDrive, a.IFileBrowserFactory],
+                    optional: [n.IRouter, n.JupyterFrontEnd.ITreeResolver, n.ILabShell, s.ISettingRegistry],
+                    activate: async (e, t, r, o, n, a) => {
                         const {
-                            commands: s
+                            commands: i
                         } = e;
-                        e.serviceManager.contents.addDrive(r);
-                        const i = t.createFileBrowser("filebrowser", {
+                        e.serviceManager.contents.addDrive(t);
+                        const s = r.createFileBrowser("filebrowser", {
                             auto: !1,
                             restore: !1,
-                            driveName: r.name
+                            driveName: t.name
                         });
-                        return w.restoreBrowser(i, s, o, a, n), i
+                        return b.restoreBrowser(s, i, o, n, a), s
                     }
                 };
-            var w;
+            var b;
             ! function(e) {
-                e.restoreBrowser = async function(e, r, t, a, n) {
-                    const s = "jp-mod-restoring";
-                    if (e.addClass(s), !t) return await e.model.restore(e.id), await e.model.refresh(), void e.removeClass(s);
-                    const i = async () => {
-                        t.routed.disconnect(i);
-                        const l = await (null == a ? void 0 : a.paths);
-                        (null == l ? void 0 : l.file) || (null == l ? void 0 : l.browser) ? (await e.model.restore(e.id, !1), l.file && await r.execute(o.openPath, {
+                e.restoreBrowser = async function(e, t, r, n, a) {
+                    const i = "jp-mod-restoring";
+                    if (e.addClass(i), !r) return await e.model.restore(e.id), await e.model.refresh(), void e.removeClass(i);
+                    const s = async () => {
+                        r.routed.disconnect(s);
+                        const l = await (null == n ? void 0 : n.paths);
+                        (null == l ? void 0 : l.file) || (null == l ? void 0 : l.browser) ? (await e.model.restore(e.id, !1), l.file && await t.execute(o.openPath, {
                             path: l.file,
                             dontShowBrowser: !0
-                        }), l.browser && await r.execute(o.openPath, {
+                        }), l.browser && await t.execute(o.openPath, {
                             path: l.browser,
                             dontShowBrowser: !0
-                        })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(s), (null == n ? void 0 : n.isEmpty("main")) && r.execute("launcher:create")
+                        })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(i), (null == a ? void 0 : a.isEmpty("main")) && t.execute("launcher:create")
                     };
-                    t.routed.connect(i)
+                    r.routed.connect(s)
                 }
-            }(w || (w = {}));
-            var b = t(7678),
-                m = t(7765),
-                y = t(5654),
-                h = t(669),
-                f = t(1144),
-                g = t(8281),
-                x = t(3530),
-                I = t(8632),
-                M = t(981),
-                C = t(6493),
-                j = t(7099);
+            }(b || (b = {}));
+            var w = r(60),
+                y = r(7478),
+                m = r(9041),
+                h = r(9190),
+                f = r(8778),
+                g = r(4989),
+                x = r(8256),
+                I = r(1682),
+                M = r(981),
+                C = r(6493),
+                j = r(7099);
             const S = [d, u, p, v, {
                 id: "@jupyter/collaboration-extension:userMenu",
                 description: "Provide connected user menu.",
                 requires: [],
-                provides: y.IUserMenu,
+                provides: m.IUserMenu,
                 activate: e => {
                     const {
-                        commands: r
+                        commands: t
                     } = e, {
-                        user: t
+                        user: r
                     } = e.serviceManager;
-                    return new y.UserMenu({
-                        commands: r,
-                        user: t
+                    return new m.UserMenu({
+                        commands: t,
+                        user: r
                     })
                 }
             }, {
                 id: "@jupyter/collaboration-extension:userMenuBar",
                 description: "Add user menu to the interface.",
                 autoStart: !0,
-                requires: [y.IUserMenu],
-                activate: async (e, r) => {
+                requires: [m.IUserMenu],
+                activate: async (e, t) => {
                     const {
-                        shell: t
+                        shell: r
                     } = e, {
                         user: o
-                    } = e.serviceManager, a = new f.MenuBar({
+                    } = e.serviceManager, n = new f.MenuBar({
                         forceItemsPosition: {
                             forceX: !1,
                             forceY: !1
                         },
-                        renderer: new y.RendererUserMenu(o)
+                        renderer: new m.RendererUserMenu(o)
                     });
-                    a.id = "jp-UserMenu", o.userChanged.connect((() => a.update())), a.addMenu(r), t.add(a, "top", {
+                    n.id = "jp-UserMenu", o.userChanged.connect((() => n.update())), n.addMenu(t), r.add(n, "top", {
                         rank: 1e3
                     })
                 }
             }, {
                 id: "@jupyter/collaboration-extension:rtcGlobalAwareness",
                 description: "Add global awareness to share working document of users.",
                 requires: [I.IStateDB],
-                provides: y.IGlobalAwareness,
-                activate: (e, r) => {
+                provides: m.IGlobalAwareness,
+                activate: (e, t) => {
                     const {
-                        user: t
-                    } = e.serviceManager, o = new M.Doc, a = new C.GL(o), n = x.ServerConnection.makeSettings(), s = g.URLExt.join(n.wsUrl, "api/collaboration/room");
-                    new j.WebsocketProvider(s, "JupyterLab:globalAwareness", o, {
-                        awareness: a
+                        user: r
+                    } = e.serviceManager, o = new M.Doc, n = new C.GL(o), a = x.ServerConnection.makeSettings(), i = g.URLExt.join(a.wsUrl, "api/collaboration/room");
+                    new j.WebsocketProvider(i, "JupyterLab:globalAwareness", o, {
+                        awareness: n
                     });
-                    const i = () => {
-                        a.setLocalStateField("user", t.identity)
+                    const s = () => {
+                        n.setLocalStateField("user", r.identity)
                     };
-                    return t.isReady && i(), t.ready.then(i).catch((e => console.error(e))), t.userChanged.connect(i), r.changed.connect((async () => {
-                        var e, t;
-                        const o = (null === (t = null === (e = (await r.toJSON())["layout-restorer:data"]) || void 0 === e ? void 0 : e.main) || void 0 === t ? void 0 : t.current) || "";
-                        o.startsWith("editor") || o.startsWith("notebook") ? a.setLocalStateField("current", o) : a.setLocalStateField("current", null)
-                    })), a
+                    return r.isReady && s(), r.ready.then(s).catch((e => console.error(e))), r.userChanged.connect(s), t.changed.connect((async () => {
+                        var e, r;
+                        const o = (null === (r = null === (e = (await t.toJSON())["layout-restorer:data"]) || void 0 === e ? void 0 : e.main) || void 0 === r ? void 0 : r.current) || "";
+                        o.startsWith("editor") || o.startsWith("notebook") ? n.setLocalStateField("current", o) : n.setLocalStateField("current", null)
+                    })), n
                 }
             }, {
                 id: "@jupyter/collaboration-extension:rtcPanel",
                 description: "Add side panel to display all currently connected users.",
                 autoStart: !0,
-                requires: [y.IGlobalAwareness],
-                optional: [s.ITranslator],
-                activate: (e, r, t) => {
+                requires: [m.IGlobalAwareness],
+                optional: [i.ITranslator],
+                activate: (e, t, r) => {
                     const {
                         user: o
-                    } = e.serviceManager, a = (null != t ? t : s.nullTranslator).load("jupyter_collaboration"), n = new h.SidePanel({
+                    } = e.serviceManager, n = (null != r ? r : i.nullTranslator).load("jupyter_collaboration"), a = new h.SidePanel({
                         alignment: "justify"
                     });
-                    n.id = b.DOMUtils.createDomID(), n.title.icon = h.usersIcon, n.title.caption = a.__("Collaboration"), n.addClass("jp-RTCPanel"), e.shell.add(n, "left", {
+                    a.id = w.DOMUtils.createDomID(), a.title.icon = h.usersIcon, a.title.caption = n.__("Collaboration"), a.addClass("jp-RTCPanel"), e.shell.add(a, "left", {
                         rank: 300
                     });
-                    const i = new y.UserInfoPanel(o);
-                    i.title.label = a.__("User info"), i.title.caption = a.__("User information"), n.addWidget(i);
-                    const l = new y.CollaboratorsPanel(o, r, (r => {
+                    const s = new m.UserInfoPanel(o);
+                    s.title.label = n.__("User info"), s.title.caption = n.__("User information"), a.addWidget(s);
+                    const l = new m.CollaboratorsPanel(o, t, (t => {
                         e.commands.execute("docmanager:open", {
-                            path: r
+                            path: t
                         })
                     }));
-                    l.title.label = a.__("Online Collaborators"), n.addWidget(l)
+                    l.title.label = n.__("Online Collaborators"), a.addWidget(l)
                 }
             }, {
                 id: "@jupyter/collaboration-extension:userEditorCursors",
                 description: "Add CodeMirror extension to display remote user cursors and selections.",
                 autoStart: !0,
-                requires: [m.IEditorExtensionRegistry],
-                activate: (e, r) => {
-                    r.addExtension({
+                requires: [y.IEditorExtensionRegistry],
+                activate: (e, t) => {
+                    t.addExtension({
                         name: "remote-user-cursors",
                         factory(e) {
                             const {
-                                awareness: r,
-                                ysource: t
+                                awareness: t,
+                                ysource: r
                             } = e.model.sharedModel;
-                            return m.EditorExtensionRegistry.createImmutableExtension((0, y.remoteUserCursors)({
-                                awareness: r,
-                                ytext: t
+                            return y.EditorExtensionRegistry.createImmutableExtension((0, m.remoteUserCursors)({
+                                awareness: t,
+                                ytext: r
                             }))
                         }
                     })
                 }
             }]
         }
     }
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/8.e96092f47976d91f296d.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/8.6b2a09634af3599cbddb.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -3,24 +3,24 @@
     [8, 933], {
         2008: (e, t, s) => {
             s.r(t), s.d(t, {
                 ICollaborativeDrive: () => p,
                 WebSocketProvider: () => h,
                 YDrive: () => d
             });
-            var o = s(8281),
-                r = s(3530),
-                n = s(7678),
+            var o = s(60),
+                r = s(4989),
+                n = s(8256),
                 i = s(7930),
                 a = s(4901),
                 c = s(7099);
             class h {
                 constructor(e) {
                     this._onConnectionClosed = e => {
-                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, n.showErrorMessage)(this._trans.__("Session expired"), this._trans.__("The document session expired. You need to reload this browser tab."), [n.Dialog.okButton({
+                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, o.showErrorMessage)(this._trans.__("Session expired"), this._trans.__("The document session expired. You need to reload this browser tab."), [o.Dialog.okButton({
                             label: this._trans.__("Reload")
                         })]).then((e => {
                             e.button.accept && window.location.reload()
                         })).catch((e => window.location.reload())), this._sharedModel.dispose())
                     }, this._ready = new i.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
                     const t = e.user;
                     t.ready.then((() => {
@@ -36,18 +36,18 @@
                 dispose() {
                     var e, t;
                     this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.destroy(), a.Signal.clearData(this))
                 }
                 _connect() {
                     (async function(e, t, s) {
                         const {
-                            makeSettings: n,
+                            makeSettings: o,
                             makeRequest: i,
                             ResponseError: a
-                        } = r.ServerConnection, c = n(), h = o.URLExt.join(c.baseUrl, "api/collaboration/session", encodeURIComponent(s)), d = {
+                        } = n.ServerConnection, c = o(), h = r.URLExt.join(c.baseUrl, "api/collaboration/session", encodeURIComponent(s)), d = {
                             method: "PUT",
                             body: JSON.stringify({
                                 format: e,
                                 type: t
                             })
                         }, l = await i(h, d, c);
                         if (200 !== l.status && 201 !== l.status) throw new a(l);
@@ -62,34 +62,43 @@
                         }), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                     })).then((e => this._ready.resolve())).catch((e => console.warn(e)))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class d extends r.Drive {
+            class d extends n.Drive {
                 constructor(e, t) {
                     super({
                         name: "RTC"
                     }), this._onCreate = (e, t) => {
                         if ("string" == typeof e.format) try {
                             const s = new h({
-                                    url: o.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
+                                    url: r.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
                                     path: e.path,
                                     format: e.format,
                                     contentType: e.contentType,
                                     model: t,
                                     user: this._user,
                                     translator: this._trans
                                 }),
-                                r = `${e.format}:${e.contentType}:${e.path}`;
-                            this._providers.set(r, s), t.disposed.connect((() => {
-                                const e = this._providers.get(r);
-                                e && (e.dispose(), this._providers.delete(r))
-                            }))
+                                n = `${e.format}:${e.contentType}:${e.path}`;
+                            this._providers.set(n, s), t.disposed.connect((() => {
+                                const e = this._providers.get(n);
+                                e && (e.dispose(), this._providers.delete(n))
+                            }));
+                            for (const t of this._providers.keys()) {
+                                if (t === n) continue;
+                                const s = t.split(":")[2];
+                                e.path === s && (0, o.showDialog)({
+                                    title: this._trans.__("Warning"),
+                                    body: this._trans.__("Opening a document with multiple views simultaneously is not supported.Please, close one view otherwise, you might lose some of your changes."),
+                                    buttons: [o.Dialog.okButton()]
+                                })
+                            }
                         } catch (t) {
                             console.error(`Failed to open websocket connection for ${e.path}.\n:${t}`)
                         }
                     }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new l(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
@@ -120,14 +129,15 @@
                 }
             }
             class l {
                 constructor(e) {
                     this._onCreate = e, this.collaborative = !0, this._documentFactories = new Map
                 }
                 registerDocumentFactory(e, t) {
+                    if (this._documentFactories.has(e)) throw new Error(`The content type ${e} already exists`);
                     this._documentFactories.set(e, t)
                 }
                 createNew(e) {
                     if ("string" == typeof e.format) {
                         if (e.collaborative && this._documentFactories.has(e.contentType)) {
                             const t = this._documentFactories.get(e.contentType)(e);
                             return this._onCreate(e, t), t
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/839.b379ccb87adf98b344b9.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/839.2efa17f8ec8b5c6c87a6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,66 +3,66 @@
     [839], {
         6450: (n, e, o) => {
             o.d(e, {
                 Z: () => s
             });
             var r = o(9601),
                 t = o.n(r),
-                a = o(2609),
-                i = o.n(a),
+                i = o(2609),
+                a = o.n(i),
                 l = o(6435),
                 c = o(8974),
-                p = i()(t());
+                p = a()(t());
             p.i(l.Z), p.i(c.Z), p.push([n.id, "/* -----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|---------------------------------------------------------------------------- */\n", ""]);
             const s = p
         },
         6435: (n, e, o) => {
             o.d(e, {
                 Z: () => l
             });
             var r = o(9601),
                 t = o.n(r),
-                a = o(2609),
-                i = o.n(a)()(t());
-            i.push([n.id, "/* -----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|---------------------------------------------------------------------------- */\n\n.jp-MenuBar-label {\n  margin-left: 25px;\n}\n\n.jp-MenuBar-anonymousIcon span {\n  width: 24px;\n  text-align: center;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-MenuBar-anonymousIcon,\n.jp-MenuBar-imageIcon {\n  position: absolute;\n  top: 1px;\n  left: 8px;\n  width: 24px;\n  height: 24px;\n  display: flex;\n  align-items: center;\n  vertical-align: middle;\n  border-radius: 100%;\n}\n\n.jp-MenuBar-imageIcon img {\n  width: 24px;\n  border-radius: 100%;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-UserMenu-caretDownIcon {\n  height: 22px;\n  position: relative;\n  top: 15%;\n}\n", ""]);
-            const l = i
+                i = o(2609),
+                a = o.n(i)()(t());
+            a.push([n.id, "/* -----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|---------------------------------------------------------------------------- */\n\n.jp-MenuBar-label {\n  margin-left: 25px;\n}\n\n.jp-MenuBar-anonymousIcon span {\n  width: 24px;\n  text-align: center;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-MenuBar-anonymousIcon,\n.jp-MenuBar-imageIcon {\n  position: absolute;\n  top: 1px;\n  left: 8px;\n  width: 24px;\n  height: 24px;\n  display: flex;\n  align-items: center;\n  vertical-align: middle;\n  border-radius: 100%;\n}\n\n.jp-MenuBar-imageIcon img {\n  width: 24px;\n  border-radius: 100%;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-UserMenu-caretDownIcon {\n  height: 22px;\n  position: relative;\n  top: 15%;\n}\n", ""]);
+            const l = a
         },
         8974: (n, e, o) => {
             o.d(e, {
                 Z: () => l
             });
             var r = o(9601),
                 t = o.n(r),
-                a = o(2609),
-                i = o.n(a)()(t());
-            i.push([n.id, "/*\n * Copyright (c) Jupyter Development Team.\n * Distributed under the terms of the Modified BSD License.\n */\n\n/************************************************************\n                      Main Panel\n*************************************************************/\n\n.jp-RTCPanel {\n  min-width: var(--jp-sidebar-min-width) !important;\n  color: var(--jp-ui-font-color1);\n  background: var(--jp-layout-color1);\n  font-size: var(--jp-ui-font-size1);\n}\n\n/************************************************************\n                      User Info Panel\n*************************************************************/\n.jp-UserInfoPanel {\n  display: flex;\n  flex-direction: column;\n  max-height: 140px;\n  padding-top: 3px;\n}\n\n.jp-UserInfo-Container {\n  margin: 20px;\n  display: flex;\n  flex-direction: column;\n  align-items: center;\n}\n\n.jp-UserInfo-Icon {\n  margin: auto;\n  width: 50px;\n  height: 50px;\n  border-radius: 50px;\n  display: inline-flex;\n  align-items: center;\n}\n\n.jp-UserInfo-Icon span {\n  margin: auto;\n  text-align: center;\n  font-size: 25px;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-UserInfo-Info {\n  margin: 20px;\n  display: inline-flex;\n  flex-direction: column;\n}\n\n.jp-UserInfo-Info label {\n  font-weight: bold;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-UserInfo-Info input {\n  text-decoration: none;\n  border-top: none;\n  border-left: none;\n  border-right: none;\n  border-color: var(--jp-ui-font-color1);\n  border-width: 0.5px;\n  background-color: transparent;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n/************************************************************\n                Collaborators Info Panel\n*************************************************************/\n\n.jp-CollaboratorsPanel {\n  overflow-y: auto;\n}\n\n.jp-CollaboratorsList {\n  flex-direction: column;\n  display: flex;\n  z-index: 1000;\n}\n\n.jp-Collaborator {\n  padding: 10px;\n  display: flex;\n  align-items: center;\n  font-size: var(--jp-ui-font-size0);\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-ClickableCollaborator:hover {\n  cursor: pointer;\n  background-color: var(--jp-layout-color2);\n  fill: var(--jp-ui-font-color0);\n  color: var(--jp-ui-font-color0);\n}\n\n.jp-Collaborator > span {\n  padding-left: 7px;\n}\n\n.jp-CollaboratorIcon {\n  border-radius: 100%;\n  padding: 2px;\n  width: 24px;\n  height: 24px;\n  display: flex;\n}\n\n.jp-CollaboratorIcon > span {\n  text-align: center;\n  margin: auto;\n  font-size: 12px;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-CollaboratorCurrent {\n  position: absolute;\n  right: 0;\n}\n", ""]);
-            const l = i
+                i = o(2609),
+                a = o.n(i)()(t());
+            a.push([n.id, "/*\n * Copyright (c) Jupyter Development Team.\n * Distributed under the terms of the Modified BSD License.\n */\n\n/************************************************************\n                      Main Panel\n*************************************************************/\n\n.jp-RTCPanel {\n  min-width: var(--jp-sidebar-min-width) !important;\n  color: var(--jp-ui-font-color1);\n  background: var(--jp-layout-color1);\n  font-size: var(--jp-ui-font-size1);\n}\n\n/************************************************************\n                      User Info Panel\n*************************************************************/\n.jp-UserInfoPanel {\n  display: flex;\n  flex-direction: column;\n  max-height: 140px;\n  padding-top: 3px;\n}\n\n.jp-UserInfo-Container {\n  margin: 20px;\n  display: flex;\n  flex-direction: column;\n  align-items: center;\n}\n\n.jp-UserInfo-Icon {\n  margin: auto;\n  width: 50px;\n  height: 50px;\n  border-radius: 50px;\n  display: inline-flex;\n  align-items: center;\n}\n\n.jp-UserInfo-Icon span {\n  margin: auto;\n  text-align: center;\n  font-size: 25px;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-UserInfo-Info {\n  margin: 20px;\n  display: inline-flex;\n  flex-direction: column;\n}\n\n.jp-UserInfo-Info label {\n  font-weight: bold;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-UserInfo-Info input {\n  text-decoration: none;\n  border-top: none;\n  border-left: none;\n  border-right: none;\n  border-color: var(--jp-ui-font-color1);\n  border-width: 0.5px;\n  background-color: transparent;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n/************************************************************\n                Collaborators Info Panel\n*************************************************************/\n\n.jp-CollaboratorsPanel {\n  overflow-y: auto;\n}\n\n.jp-CollaboratorsList {\n  flex-direction: column;\n  display: flex;\n  z-index: 1000;\n}\n\n.jp-Collaborator {\n  padding: 10px;\n  display: flex;\n  align-items: center;\n  font-size: var(--jp-ui-font-size0);\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-ClickableCollaborator:hover {\n  cursor: pointer;\n  background-color: var(--jp-layout-color2);\n  fill: var(--jp-ui-font-color0);\n  color: var(--jp-ui-font-color0);\n}\n\n.jp-Collaborator > span {\n  padding-left: 7px;\n}\n\n.jp-CollaboratorIcon {\n  border-radius: 100%;\n  padding: 2px;\n  width: 24px;\n  height: 24px;\n  display: flex;\n}\n\n.jp-CollaboratorIcon > span {\n  text-align: center;\n  margin: auto;\n  font-size: 12px;\n  fill: var(--jp-ui-font-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.jp-CollaboratorCurrent {\n  position: absolute;\n  right: 0;\n}\n", ""]);
+            const l = a
         },
         2609: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
                         var o = "",
                             r = void 0 !== e[5];
                         return e[4] && (o += "@supports (".concat(e[4], ") {")), e[2] && (o += "@media ".concat(e[2], " {")), r && (o += "@layer".concat(e[5].length > 0 ? " ".concat(e[5]) : "", " {")), o += n(e), r && (o += "}"), e[2] && (o += "}"), e[4] && (o += "}"), o
                     })).join("")
-                }, e.i = function(n, o, r, t, a) {
+                }, e.i = function(n, o, r, t, i) {
                     "string" == typeof n && (n = [
                         [null, n, void 0]
                     ]);
-                    var i = {};
+                    var a = {};
                     if (r)
                         for (var l = 0; l < this.length; l++) {
                             var c = this[l][0];
-                            null != c && (i[c] = !0)
+                            null != c && (a[c] = !0)
                         }
                     for (var p = 0; p < n.length; p++) {
                         var s = [].concat(n[p]);
-                        r && i[s[0]] || (void 0 !== a && (void 0 === s[5] || (s[1] = "@layer".concat(s[5].length > 0 ? " ".concat(s[5]) : "", " {").concat(s[1], "}")), s[5] = a), o && (s[2] ? (s[1] = "@media ".concat(s[2], " {").concat(s[1], "}"), s[2] = o) : s[2] = o), t && (s[4] ? (s[1] = "@supports (".concat(s[4], ") {").concat(s[1], "}"), s[4] = t) : s[4] = "".concat(t)), e.push(s))
+                        r && a[s[0]] || (void 0 !== i && (void 0 === s[5] || (s[1] = "@layer".concat(s[5].length > 0 ? " ".concat(s[5]) : "", " {").concat(s[1], "}")), s[5] = i), o && (s[2] ? (s[1] = "@media ".concat(s[2], " {").concat(s[1], "}"), s[2] = o) : s[2] = o), t && (s[4] ? (s[1] = "@supports (".concat(s[4], ") {").concat(s[1], "}"), s[4] = t) : s[4] = "".concat(t)), e.push(s))
                     }
                 }, e
             }
         },
         9601: n => {
             n.exports = function(n) {
                 return n[1]
@@ -76,20 +76,20 @@
                     if (e[r].identifier === n) {
                         o = r;
                         break
                     } return o
             }
 
             function r(n, r) {
-                for (var a = {}, i = [], l = 0; l < n.length; l++) {
+                for (var i = {}, a = [], l = 0; l < n.length; l++) {
                     var c = n[l],
                         p = r.base ? c[0] + r.base : c[0],
-                        s = a[p] || 0,
+                        s = i[p] || 0,
                         u = "".concat(p, " ").concat(s);
-                    a[p] = s + 1;
+                    i[p] = s + 1;
                     var f = o(u),
                         d = {
                             css: c[1],
                             media: c[2],
                             sourceMap: c[3],
                             supports: c[4],
                             layer: c[5]
@@ -99,42 +99,42 @@
                         var v = t(d, r);
                         r.byIndex = l, e.splice(l, 0, {
                             identifier: u,
                             updater: v,
                             references: 1
                         })
                     }
-                    i.push(u)
+                    a.push(u)
                 }
-                return i
+                return a
             }
 
             function t(n, e) {
                 var o = e.domAPI(e);
                 return o.update(n),
                     function(e) {
                         if (e) {
                             if (e.css === n.css && e.media === n.media && e.sourceMap === n.sourceMap && e.supports === n.supports && e.layer === n.layer) return;
                             o.update(n = e)
                         } else o.remove()
                     }
             }
             n.exports = function(n, t) {
-                var a = r(n = n || [], t = t || {});
+                var i = r(n = n || [], t = t || {});
                 return function(n) {
                     n = n || [];
-                    for (var i = 0; i < a.length; i++) {
-                        var l = o(a[i]);
+                    for (var a = 0; a < i.length; a++) {
+                        var l = o(i[a]);
                         e[l].references--
                     }
-                    for (var c = r(n, t), p = 0; p < a.length; p++) {
-                        var s = o(a[p]);
+                    for (var c = r(n, t), p = 0; p < i.length; p++) {
+                        var s = o(i[p]);
                         0 === e[s].references && (e[s].updater(), e.splice(s, 1))
                     }
-                    a = c
+                    i = c
                 }
             }
         },
         6793: n => {
             var e = {};
             n.exports = function(n, o) {
                 var r = function(n) {
@@ -163,24 +163,28 @@
             n.exports = function(n) {
                 var e = o.nc;
                 e && n.setAttribute("nonce", e)
             }
         },
         4036: n => {
             n.exports = function(n) {
+                if ("undefined" == typeof document) return {
+                    update: function() {},
+                    remove: function() {}
+                };
                 var e = n.insertStyleElement(n);
                 return {
                     update: function(o) {
                         ! function(n, e, o) {
                             var r = "";
                             o.supports && (r += "@supports (".concat(o.supports, ") {")), o.media && (r += "@media ".concat(o.media, " {"));
                             var t = void 0 !== o.layer;
                             t && (r += "@layer".concat(o.layer.length > 0 ? " ".concat(o.layer) : "", " {")), r += o.css, t && (r += "}"), o.media && (r += "}"), o.supports && (r += "}");
-                            var a = o.sourceMap;
-                            a && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleTagTransform(r, n, e.options)
+                            var i = o.sourceMap;
+                            i && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), e.styleTagTransform(r, n, e.options)
                         }(e, n, o)
                     },
                     remove: function() {
                         ! function(n) {
                             if (null === n.parentNode) return !1;
                             n.parentNode.removeChild(n)
                         }(e)
@@ -197,23 +201,23 @@
                 }
             }
         },
         8839: (n, e, o) => {
             o.r(e);
             var r = o(6062),
                 t = o.n(r),
-                a = o(4036),
-                i = o.n(a),
+                i = o(4036),
+                a = o.n(i),
                 l = o(6793),
                 c = o.n(l),
                 p = o(7892),
                 s = o.n(p),
                 u = o(1173),
                 f = o.n(u),
                 d = o(2464),
                 v = o.n(d),
                 h = o(6450),
                 m = {};
-            m.styleTagTransform = v(), m.setAttributes = s(), m.insert = c().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = f(), t()(h.Z, m), h.Z && h.Z.locals && h.Z.locals
+            m.styleTagTransform = v(), m.setAttributes = s(), m.insert = c().bind(null, "head"), m.domAPI = a(), m.insertStyleElement = f(), t()(h.Z, m), h.Z && h.Z.locals && h.Z.locals
         }
     }
 ]);
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/9.1a44b656eb74a0222c38.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/9.f46ff2dd7fa86c1246e8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -194,16 +194,16 @@
                         parent: document.body
                     })]
                 });
 
             function v(e) {
                 return [c.of(e), y]
             }
-            var b = r(669),
-                _ = r(1144),
+            var b = r(9190),
+                _ = r(8778),
                 g = r(4059);
             class w extends _.MenuBar.Renderer {
                 constructor(e) {
                     super(), this._user = e
                 }
                 renderItem(e) {
                     const t = this.createItemClass(e),
@@ -239,15 +239,15 @@
                 }
             }
             class I extends _.Menu {
                 constructor(e) {
                     super(e)
                 }
             }
-            var x = r(7678),
+            var x = r(60),
                 j = r(6029);
             const k = e => {
                 const {
                     user: t
                 } = e;
                 return j.createElement("div", {
                     className: "jp-UserInfo-Container"
@@ -278,15 +278,15 @@
                 }
                 render() {
                     return j.createElement(k, {
                         user: this._user
                     })
                 }
             }
-            var R = r(8281);
+            var R = r(4989);
             const E = "jp-Collaborator";
             class A extends _.Panel {
                 constructor(e, t, r) {
                     super({}), this._onAwarenessChanged = () => {
                         const e = this._awareness.getStates(),
                             t = [];
                         e.forEach(((e, r) => {
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/933.6dbefb158f22077b6dbf.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/933.f161fc3dcf0d2c141b27.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -3,24 +3,24 @@
     [933, 8], {
         2008: (e, t, s) => {
             s.r(t), s.d(t, {
                 ICollaborativeDrive: () => p,
                 WebSocketProvider: () => h,
                 YDrive: () => d
             });
-            var o = s(8281),
-                r = s(3530),
-                n = s(7678),
+            var o = s(60),
+                r = s(4989),
+                n = s(8256),
                 i = s(7930),
                 a = s(4901),
                 c = s(7099);
             class h {
                 constructor(e) {
                     this._onConnectionClosed = e => {
-                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, n.showErrorMessage)(this._trans.__("Session expired"), this._trans.__("The document session expired. You need to reload this browser tab."), [n.Dialog.okButton({
+                        1003 === e.code && (console.error("Document provider closed:", e.reason), (0, o.showErrorMessage)(this._trans.__("Session expired"), this._trans.__("The document session expired. You need to reload this browser tab."), [o.Dialog.okButton({
                             label: this._trans.__("Reload")
                         })]).then((e => {
                             e.button.accept && window.location.reload()
                         })).catch((e => window.location.reload())), this._sharedModel.dispose())
                     }, this._ready = new i.PromiseDelegate, this._isDisposed = !1, this._path = e.path, this._contentType = e.contentType, this._format = e.format, this._serverUrl = e.url, this._sharedModel = e.model, this._awareness = e.model.awareness, this._yWebsocketProvider = null, this._trans = e.translator;
                     const t = e.user;
                     t.ready.then((() => {
@@ -36,18 +36,18 @@
                 dispose() {
                     var e, t;
                     this.isDisposed || (this._isDisposed = !0, null === (e = this._yWebsocketProvider) || void 0 === e || e.off("connection-close", this._onConnectionClosed), null === (t = this._yWebsocketProvider) || void 0 === t || t.destroy(), a.Signal.clearData(this))
                 }
                 _connect() {
                     (async function(e, t, s) {
                         const {
-                            makeSettings: n,
+                            makeSettings: o,
                             makeRequest: i,
                             ResponseError: a
-                        } = r.ServerConnection, c = n(), h = o.URLExt.join(c.baseUrl, "api/collaboration/session", encodeURIComponent(s)), d = {
+                        } = n.ServerConnection, c = o(), h = r.URLExt.join(c.baseUrl, "api/collaboration/session", encodeURIComponent(s)), d = {
                             method: "PUT",
                             body: JSON.stringify({
                                 format: e,
                                 type: t
                             })
                         }, l = await i(h, d, c);
                         if (200 !== l.status && 201 !== l.status) throw new a(l);
@@ -62,34 +62,43 @@
                         }), this._yWebsocketProvider.on("connection-close", this._onConnectionClosed)
                     })).then((e => this._ready.resolve())).catch((e => console.warn(e)))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            class d extends r.Drive {
+            class d extends n.Drive {
                 constructor(e, t) {
                     super({
                         name: "RTC"
                     }), this._onCreate = (e, t) => {
                         if ("string" == typeof e.format) try {
                             const s = new h({
-                                    url: o.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
+                                    url: r.URLExt.join(this.serverSettings.wsUrl, "api/collaboration/room"),
                                     path: e.path,
                                     format: e.format,
                                     contentType: e.contentType,
                                     model: t,
                                     user: this._user,
                                     translator: this._trans
                                 }),
-                                r = `${e.format}:${e.contentType}:${e.path}`;
-                            this._providers.set(r, s), t.disposed.connect((() => {
-                                const e = this._providers.get(r);
-                                e && (e.dispose(), this._providers.delete(r))
-                            }))
+                                n = `${e.format}:${e.contentType}:${e.path}`;
+                            this._providers.set(n, s), t.disposed.connect((() => {
+                                const e = this._providers.get(n);
+                                e && (e.dispose(), this._providers.delete(n))
+                            }));
+                            for (const t of this._providers.keys()) {
+                                if (t === n) continue;
+                                const s = t.split(":")[2];
+                                e.path === s && (0, o.showDialog)({
+                                    title: this._trans.__("Warning"),
+                                    body: this._trans.__("Opening a document with multiple views simultaneously is not supported.Please, close one view otherwise, you might lose some of your changes."),
+                                    buttons: [o.Dialog.okButton()]
+                                })
+                            }
                         } catch (t) {
                             console.error(`Failed to open websocket connection for ${e.path}.\n:${t}`)
                         }
                     }, this._user = e, this._trans = t, this._providers = new Map, this.sharedModelFactory = new l(this._onCreate)
                 }
                 dispose() {
                     this.isDisposed || (this._providers.forEach((e => e.dispose())), this._providers.clear(), super.dispose())
@@ -120,14 +129,15 @@
                 }
             }
             class l {
                 constructor(e) {
                     this._onCreate = e, this.collaborative = !0, this._documentFactories = new Map
                 }
                 registerDocumentFactory(e, t) {
+                    if (this._documentFactories.has(e)) throw new Error(`The content type ${e} already exists`);
                     this._documentFactories.set(e, t)
                 }
                 createNew(e) {
                     if ("string" == typeof e.format) {
                         if (e.collaborative && this._documentFactories.has(e.contentType)) {
                             const t = this._documentFactories.get(e.contentType)(e);
                             return this._onCreate(e, t), t
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/remoteEntry.ed732341b4b6f42ac23d.js` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/remoteEntry.c7ae49e75d2022d8409a.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, o, n, i, l, u, d, f, s, c, p, b, h, v, y, m, g = {
             9704: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(493), t.e(546), t.e(981), t.e(602), t.e(674), t.e(497)]).then((() => () => t(9497))),
-                        "./extension": () => Promise.all([t.e(493), t.e(546), t.e(981), t.e(602), t.e(674), t.e(497)]).then((() => () => t(9497))),
+                        "./index": () => Promise.all([t.e(493), t.e(726), t.e(981), t.e(260), t.e(801), t.e(497)]).then((() => () => t(9497))),
+                        "./extension": () => Promise.all([t.e(493), t.e(726), t.e(981), t.e(260), t.e(801), t.e(497)]).then((() => () => t(9497))),
                         "./style": () => t.e(839).then((() => () => t(8839)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -43,41 +43,41 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        8: "e96092f47976d91f296d",
-        9: "1a44b656eb74a0222c38",
-        413: "ed870732b79e27f9bc6d",
-        493: "186e89468d33ae2f1acb",
-        497: "53bcecf29101af297e6d",
-        546: "25710ed78a2a5bfa2212",
-        602: "96b458ac44c408dafaf8",
-        674: "b54d7b84c621d6dcb3c6",
-        839: "b379ccb87adf98b344b9",
-        901: "98b88a83ce3037dbf9e8",
-        930: "1c248b32764d56a2842d",
-        933: "6dbefb158f22077b6dbf",
-        981: "f6fb4e4359dd250dff8d"
+        8: "6b2a09634af3599cbddb",
+        9: "f46ff2dd7fa86c1246e8",
+        260: "55fece40a4703413e008",
+        413: "cf154c48ecaa08648e56",
+        493: "0975334cbddac1bcf819",
+        497: "ab1a0ee570b8e4f31289",
+        726: "dcde0771b563d36178d7",
+        801: "1ce5dfec9291e64bf68b",
+        839: "2efa17f8ec8b5c6c87a6",
+        901: "f3045e1e297ffd031efd",
+        930: "0236d410b0d873232513",
+        933: "f161fc3dcf0d2c141b27",
+        981: "9470c3f446e34a475ff7"
     } [e] + ".js?v=" + {
-        8: "e96092f47976d91f296d",
-        9: "1a44b656eb74a0222c38",
-        413: "ed870732b79e27f9bc6d",
-        493: "186e89468d33ae2f1acb",
-        497: "53bcecf29101af297e6d",
-        546: "25710ed78a2a5bfa2212",
-        602: "96b458ac44c408dafaf8",
-        674: "b54d7b84c621d6dcb3c6",
-        839: "b379ccb87adf98b344b9",
-        901: "98b88a83ce3037dbf9e8",
-        930: "1c248b32764d56a2842d",
-        933: "6dbefb158f22077b6dbf",
-        981: "f6fb4e4359dd250dff8d"
+        8: "6b2a09634af3599cbddb",
+        9: "f46ff2dd7fa86c1246e8",
+        260: "55fece40a4703413e008",
+        413: "cf154c48ecaa08648e56",
+        493: "0975334cbddac1bcf819",
+        497: "ab1a0ee570b8e4f31289",
+        726: "dcde0771b563d36178d7",
+        801: "1ce5dfec9291e64bf68b",
+        839: "2efa17f8ec8b5c6c87a6",
+        901: "f3045e1e297ffd031efd",
+        930: "0236d410b0d873232513",
+        933: "f161fc3dcf0d2c141b27",
+        981: "9470c3f446e34a475ff7"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -129,15 +129,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter/collaboration-extension", "1.0.0-alpha.7", (() => Promise.all([w.e(493), w.e(546), w.e(981), w.e(602), w.e(674), w.e(497)]).then((() => () => w(9497))))), l("@jupyter/collaboration", "1.0.0-alpha.7", (() => Promise.all([w.e(930), w.e(546), w.e(981), w.e(9), w.e(602)]).then((() => () => w(6009))))), l("@jupyter/docprovider", "1.0.0-alpha.7", (() => Promise.all([w.e(930), w.e(546), w.e(674), w.e(901), w.e(8)]).then((() => () => w(2008))))), l("y-websocket", "1.4.5", (() => Promise.all([w.e(493), w.e(413), w.e(981)]).then((() => () => w(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter/collaboration-extension", "1.0.0-alpha.8", (() => Promise.all([w.e(493), w.e(726), w.e(981), w.e(260), w.e(801), w.e(497)]).then((() => () => w(9497))))), l("@jupyter/collaboration", "1.0.0-alpha.8", (() => Promise.all([w.e(930), w.e(726), w.e(981), w.e(9), w.e(260)]).then((() => () => w(6009))))), l("@jupyter/docprovider", "1.0.0-alpha.8", (() => Promise.all([w.e(930), w.e(726), w.e(801), w.e(901), w.e(8)]).then((() => () => w(2008))))), l("y-websocket", "1.5.0", (() => Promise.all([w.e(493), w.e(413), w.e(981)]).then((() => () => w(413)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -234,42 +234,42 @@
     }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, a, o) {
         var n = w.I(r);
         return n && n.then ? n.then(e.bind(e, r, w.S[r], t, a, o)) : e(r, w.S[r], t, a, o)
     })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), b = c(((e, r, t, a, o) => r && w.o(r, t) ? d(r, 0, t, a) : o())), h = c(((e, r, t, a, o) => {
         var n = r && w.o(r, t) && f(r, t, a);
         return n ? s(n) : o()
     })), v = {}, y = {
-        7678: () => p("default", "@jupyterlab/apputils", [1, 4, 0, 0, , "beta", 0]),
-        8281: () => p("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 0]),
+        60: () => p("default", "@jupyterlab/apputils", [1, 4, 0, 0, , "beta", 1]),
+        4989: () => p("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 1]),
         981: () => p("default", "yjs", [1, 13, 5, 40]),
-        669: () => p("default", "@jupyterlab/ui-components", [1, 4, 0, 0, , "beta", 0]),
-        1144: () => p("default", "@lumino/widgets", [1, 2, 0, 0]),
-        3530: () => p("default", "@jupyterlab/services", [1, 7, 0, 0, , "beta", 0]),
+        8778: () => p("default", "@lumino/widgets", [1, 2, 0, 1]),
+        9190: () => p("default", "@jupyterlab/ui-components", [1, 4, 0, 0, , "beta", 1]),
         7099: () => h("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([w.e(493), w.e(413), w.e(981)]).then((() => () => w(413))))),
-        225: () => p("default", "@jupyterlab/settingregistry", [1, 4, 0, 0, , "beta", 0]),
-        2998: () => p("default", "@jupyterlab/translation", [1, 4, 0, 0, , "beta", 0]),
+        8256: () => p("default", "@jupyterlab/services", [1, 7, 0, 0, , "beta", 1]),
+        726: () => p("default", "@jupyterlab/translation", [1, 4, 0, 0, , "beta", 1]),
+        1371: () => p("default", "@jupyterlab/filebrowser", [1, 4, 0, 0, , "beta", 1]),
+        1682: () => p("default", "@jupyterlab/statedb", [1, 4, 0, 0, , "beta", 1]),
+        2281: () => p("default", "@jupyterlab/application", [1, 4, 0, 0, , "beta", 1]),
         3e3: () => p("default", "@jupyter/ydoc", [2, 0, 3, 4]),
-        5654: () => b("default", "@jupyter/collaboration", [1, 1, 0, 0, , "alpha", 7], (() => Promise.all([w.e(930), w.e(9)]).then((() => () => w(6009))))),
-        7765: () => p("default", "@jupyterlab/codemirror", [1, 4, 0, 0, , "beta", 0]),
-        8632: () => p("default", "@jupyterlab/statedb", [1, 4, 0, 0, , "beta", 0]),
-        8872: () => p("default", "@jupyterlab/application", [1, 4, 0, 0, , "beta", 0]),
-        9582: () => p("default", "@jupyterlab/filebrowser", [1, 4, 0, 0, , "beta", 0]),
-        9831: () => b("default", "@jupyter/docprovider", [1, 1, 0, 0, , "alpha", 7], (() => Promise.all([w.e(930), w.e(901), w.e(933)]).then((() => () => w(2008))))),
+        5581: () => p("default", "@jupyterlab/settingregistry", [1, 4, 0, 0, , "beta", 1]),
+        5996: () => b("default", "@jupyter/docprovider", [1, 1, 0, 0, , "alpha", 8], (() => Promise.all([w.e(930), w.e(901), w.e(933)]).then((() => () => w(2008))))),
+        7478: () => p("default", "@jupyterlab/codemirror", [1, 4, 0, 0, , "beta", 1]),
+        9041: () => b("default", "@jupyter/collaboration", [1, 1, 0, 0, , "alpha", 8], (() => Promise.all([w.e(930), w.e(9)]).then((() => () => w(6009))))),
         7930: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
         4059: () => p("default", "@lumino/virtualdom", [1, 2, 0, 0]),
         6029: () => p("default", "react", [1, 18, 2, 0]),
         8204: () => p("default", "@codemirror/state", [1, 6, 2, 0]),
         9502: () => p("default", "@codemirror/view", [1, 6, 7, 0]),
         4901: () => p("default", "@lumino/signaling", [1, 2, 0, 0])
     }, m = {
         9: [4059, 6029, 8204, 9502],
-        497: [225, 2998, 3e3, 5654, 7765, 8632, 8872, 9582, 9831],
-        546: [7678, 8281],
-        602: [669, 1144],
-        674: [3530, 7099],
+        260: [8778, 9190],
+        497: [726, 1371, 1682, 2281, 3e3, 5581, 5996, 7478, 9041],
+        726: [60, 4989],
+        801: [7099, 8256],
         901: [4901],
         930: [7930],
         981: [981]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
@@ -293,15 +293,15 @@
         var e = {
             510: 0
         };
         w.f.j = (r, t) => {
             var a = w.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(9(01|30|81)|546|602|674)$/.test(r)) e[r] = 0;
+                else if (/^(9(01|30|81)|260|726|801)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
                 var n = w.p + w.u(r),
                     i = new Error;
                 w.l(n, (t => {
                     if (w.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
```

### Comparing `jupyter_collaboration-1.0.0a7/jupyter_collaboration/labextension/static/third-party-licenses.json` & `jupyter_collaboration-1.0.0a8/jupyter_collaboration/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9609375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.0.0-alpha.8'}, 1: {'versionInfo': '1.0.0-alpha.8'}, 3: "*

 * *               "{'versionInfo': '0.2.73'}, 5: {'versionInfo': '3.3.2'}, 7: {'versionInfo': "*

 * *               "'1.5.0'}}"}*

```diff
@@ -1,52 +1,52 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/collaboration",
-            "versionInfo": "1.0.0-alpha.7"
+            "versionInfo": "1.0.0-alpha.8"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "1.0.0-alpha.7"
+            "versionInfo": "1.0.0-alpha.8"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.7.3"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019 Kevin Jahns <kevin.jahns@protonmail.com>.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "lib0",
-            "versionInfo": "0.2.62"
+            "versionInfo": "0.2.73"
         },
         {
             "extractedText": "(The MIT License)\n\nCopyright (c) 2013 Roman Shtylman <shtylman@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "process",
             "versionInfo": "0.11.10"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "3.3.1"
+            "versionInfo": "3.3.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019 Kevin Jahns <kevin.jahns@protonmail.com>.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "y-protocols",
             "versionInfo": "1.0.5"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019 Kevin Jahns <kevin.jahns@protonmail.com>.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "y-websocket",
-            "versionInfo": "1.4.5"
+            "versionInfo": "1.5.0"
         }
     ]
 }
```

### Comparing `jupyter_collaboration-1.0.0a7/scripts/bump_version.py` & `jupyter_collaboration-1.0.0a8/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/package.json` & `jupyter_collaboration-1.0.0a8/packages/collaboration/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'1.0.0-alpha.8'"}*

```diff
@@ -62,9 +62,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.7"
+    "version": "1.0.0-alpha.8"
 }
```

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/src/collaboratorspanel.tsx` & `jupyter_collaboration-1.0.0a8/packages/collaboration/src/collaboratorspanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/src/components.tsx` & `jupyter_collaboration-1.0.0a8/packages/collaboration/src/components.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/src/cursors.ts` & `jupyter_collaboration-1.0.0a8/packages/collaboration/src/cursors.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/src/menu.ts` & `jupyter_collaboration-1.0.0a8/packages/collaboration/src/menu.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/src/tokens.ts` & `jupyter_collaboration-1.0.0a8/packages/collaboration/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/src/userinfopanel.tsx` & `jupyter_collaboration-1.0.0a8/packages/collaboration/src/userinfopanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/src/utils.ts` & `jupyter_collaboration-1.0.0a8/packages/collaboration/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/style/menu.css` & `jupyter_collaboration-1.0.0a8/packages/collaboration/style/menu.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration/style/sidepanel.css` & `jupyter_collaboration-1.0.0a8/packages/collaboration/style/sidepanel.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration-extension/package.json` & `jupyter_collaboration-1.0.0a8/packages/collaboration-extension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759358288770053%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^1.0.0-alpha.8', '@jupyter/docprovider': "*

 * *                   "'^1.0.0-alpha.8'}",*

 * * "'version'": "'1.0.0-alpha.8'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^1.0.0-alpha.7",
-        "@jupyter/docprovider": "^1.0.0-alpha.7",
+        "@jupyter/collaboration": "^1.0.0-alpha.8",
+        "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyterlab/application": "^4.0.0-beta.0",
         "@jupyterlab/apputils": "^4.0.0-beta.0",
         "@jupyterlab/codemirror": "^4.0.0-beta.0",
         "@jupyterlab/coreutils": "^6.0.0-beta.0",
         "@jupyterlab/filebrowser": "^4.0.0-beta.0",
         "@jupyterlab/services": "^7.0.0-beta.0",
         "@jupyterlab/settingregistry": "^4.0.0-beta.0",
@@ -120,9 +120,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.7"
+    "version": "1.0.0-alpha.8"
 }
```

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration-extension/src/collaboration.ts` & `jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/collaboration.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration-extension/src/filebrowser.ts` & `jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/filebrowser.ts`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,19 @@
  * The command IDs used by the file browser plugin.
  */
 namespace CommandIDs {
   export const openPath = 'filebrowser:open-path';
 }
 
 /**
- * The default file browser factory provider.
+ * The default collaborative drive provider.
  */
 export const drive: JupyterFrontEndPlugin<ICollaborativeDrive> = {
   id: '@jupyter/collaboration-extension:drive',
+  description: 'The default collaborative drive provider',
   provides: ICollaborativeDrive,
   requires: [ITranslator],
   optional: [],
   activate: (
     app: JupyterFrontEnd,
     translator: ITranslator
   ): ICollaborativeDrive => {
@@ -45,34 +46,38 @@
     const drive = new YDrive(app.serviceManager.user, trans);
     app.serviceManager.contents.addDrive(drive);
     return drive;
   }
 };
 
 /**
- * The default file browser factory provider.
+ * Plugin to register the shared model factory for the content type 'file'.
  */
 export const yfile: JupyterFrontEndPlugin<void> = {
   id: '@jupyter/collaboration-extension:yfile',
+  description:
+    "Plugin to register the shared model factory for the content type 'file'",
   autoStart: true,
   requires: [ICollaborativeDrive],
   optional: [],
   activate: (app: JupyterFrontEnd, drive: ICollaborativeDrive): void => {
     const yFileFactory: SharedDocumentFactory = () => {
       return new YFile();
     };
     drive.sharedModelFactory.registerDocumentFactory('file', yFileFactory);
   }
 };
 
 /**
- * The default file browser factory provider.
+ * Plugin to register the shared model factory for the content type 'notebook'.
  */
 export const ynotebook: JupyterFrontEndPlugin<void> = {
   id: '@jupyter/collaboration-extension:ynotebook',
+  description:
+    "Plugin to register the shared model factory for the content type 'notebook'",
   autoStart: true,
   requires: [ICollaborativeDrive],
   optional: [ISettingRegistry],
   activate: (
     app: JupyterFrontEnd,
     drive: ICollaborativeDrive,
     settingRegistry: ISettingRegistry | null
@@ -112,14 +117,15 @@
 };
 
 /**
  * The default file browser factory provider.
  */
 export const defaultFileBrowser: JupyterFrontEndPlugin<IDefaultFileBrowser> = {
   id: '@jupyter/collaboration-extension:defaultFileBrowser',
+  description: 'The default file browser factory provider',
   provides: IDefaultFileBrowser,
   requires: [ICollaborativeDrive, IFileBrowserFactory],
   optional: [
     IRouter,
     JupyterFrontEnd.ITreeResolver,
     ILabShell,
     ISettingRegistry
```

### Comparing `jupyter_collaboration-1.0.0a7/packages/collaboration-extension/src/index.ts` & `jupyter_collaboration-1.0.0a8/packages/collaboration-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/docprovider/jest.config.js` & `jupyter_collaboration-1.0.0a8/packages/docprovider/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/docprovider/package.json` & `jupyter_collaboration-1.0.0a8/packages/docprovider/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.970679012345679%*

 * *Differences: {"'dependencies'": "{'@jupyter/ydoc': '^1.0.0'}", "'version'": "'1.0.0-alpha.8'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter_collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/ydoc": "^0.3.4",
+        "@jupyter/ydoc": "^1.0.0",
         "@jupyterlab/coreutils": "^6.0.0-beta.0",
         "@jupyterlab/services": "^7.0.0-beta.0",
         "@lumino/coreutils": "^2.0.0",
         "@lumino/disposable": "^2.0.0",
         "@lumino/signaling": "^2.0.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
@@ -60,9 +60,9 @@
     ],
     "typedoc": {
         "displayName": "@jupyter/docprovider",
         "entryPoint": "./src/index.ts",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-alpha.7"
+    "version": "1.0.0-alpha.8"
 }
```

### Comparing `jupyter_collaboration-1.0.0a7/packages/docprovider/src/requests.ts` & `jupyter_collaboration-1.0.0a8/packages/docprovider/src/requests.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/docprovider/src/tokens.ts` & `jupyter_collaboration-1.0.0a8/packages/docprovider/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/packages/docprovider/src/ydrive.ts` & `jupyter_collaboration-1.0.0a8/packages/docprovider/src/ydrive.ts`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
-import { DocumentChange, ISharedDocument, YDocument } from '@jupyter/ydoc';
+import { showDialog, Dialog } from '@jupyterlab/apputils';
 import { URLExt } from '@jupyterlab/coreutils';
 import { TranslationBundle } from '@jupyterlab/translation';
 import { Contents, Drive, User } from '@jupyterlab/services';
+
+import { DocumentChange, ISharedDocument, YDocument } from '@jupyter/ydoc';
+
 import { WebSocketProvider } from './yprovider';
 import {
   ICollaborativeDrive,
   ISharedModelFactory,
   SharedDocumentFactory
 } from './tokens';
 
@@ -134,14 +137,31 @@
       sharedModel.disposed.connect(() => {
         const provider = this._providers.get(key);
         if (provider) {
           provider.dispose();
           this._providers.delete(key);
         }
       });
+
+      for (const provider of this._providers.keys()) {
+        if (provider === key) {
+          continue;
+        }
+        const path = provider.split(':')[2];
+
+        if (options.path === path) {
+          showDialog({
+            title: this._trans.__('Warning'),
+            body: this._trans.__(
+              'Opening a document with multiple views simultaneously is not supported.Please, close one view otherwise, you might lose some of your changes.'
+            ),
+            buttons: [Dialog.okButton()]
+          });
+        }
+      }
     } catch (error) {
       // Falling back to the contents API if opening the websocket failed
       //  This may happen if the shared document is not a YDocument.
       console.error(
         `Failed to open websocket connection for ${options.path}.\n:${error}`
       );
     }
@@ -183,14 +203,17 @@
    * @param type Document type
    * @param factory Document factory
    */
   registerDocumentFactory(
     type: Contents.ContentType,
     factory: SharedDocumentFactory
   ) {
+    if (this._documentFactories.has(type)) {
+      throw new Error(`The content type ${type} already exists`);
+    }
     this._documentFactories.set(type, factory);
   }
 
   /**
    * Create a new `ISharedDocument` instance.
    *
    * It should return `undefined` if the factory is not able to create a `ISharedDocument`.
```

### Comparing `jupyter_collaboration-1.0.0a7/packages/docprovider/src/yprovider.ts` & `jupyter_collaboration-1.0.0a8/packages/docprovider/src/yprovider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/.gitignore` & `jupyter_collaboration-1.0.0a8/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/LICENSE` & `jupyter_collaboration-1.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/README.md` & `jupyter_collaboration-1.0.0a8/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration-1.0.0a7/pyproject.toml` & `jupyter_collaboration-1.0.0a8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
 ]
 dependencies = [
     "jupyter_server>=2.0.0,<3.0.0",
-    "jupyter_ydoc>=0.3.2,<0.4.0",
+    "jupyter_ydoc>=1.0.1,<2.0.0",
     "ypy-websocket>=0.8.3,<0.9.0",
     "jupyter_server_fileid>=0.6.0,<1"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 dev = [
@@ -137,27 +137,27 @@
 ]
 
 [tool.mypy]
 exclude=[
     "^binder/jupyter_config\\.py$",
 ]
 check_untyped_defs = true
-disallow_any_generics = true
+disallow_any_generics = false
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 no_implicit_reexport = true
 pretty = true
 show_error_context = true
 show_error_codes = true
 strict_equality = true
 strict_optional = true
 warn_unused_configs = true
 warn_redundant_casts = true
-warn_return_any = true
+warn_return_any = false
 warn_unused_ignores = true
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
     "traitlets.*",
     "jupyter_server.*",
```

### Comparing `jupyter_collaboration-1.0.0a7/PKG-INFO` & `jupyter_collaboration-1.0.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_collaboration
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: JupyterLab Extension enabling Real-Time Collaboration
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter_collaboration
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter_collaboration/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter_collaboration.git
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
@@ -79,15 +79,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: jupyter-server-fileid<1,>=0.6.0
 Requires-Dist: jupyter-server<3.0.0,>=2.0.0
-Requires-Dist: jupyter-ydoc<0.4.0,>=0.3.2
+Requires-Dist: jupyter-ydoc<2.0.0,>=1.0.1
 Requires-Dist: ypy-websocket<0.9.0,>=0.8.3
 Provides-Extra: dev
 Requires-Dist: click; extra == 'dev'
 Requires-Dist: jupyter-releaser; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: jupyterlab>=4.0.0a32; extra == 'docs'
```

