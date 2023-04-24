# Comparing `tmp/limepkg-scrive-2.0.2.tar.gz` & `tmp/limepkg-scrive-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limepkg-scrive-2.0.2.tar", last modified: Thu May  5 05:15:48 2022, max compression
+gzip compressed data, was "limepkg-scrive-2.0.3.tar", last modified: Mon Apr 24 12:25:43 2023, max compression
```

## Comparing `limepkg-scrive-2.0.2.tar` & `limepkg-scrive-2.0.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     2807 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/__init__.py
--rw-r--r--   0        0        0     2630 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/config/__init__.py
--rw-r--r--   0        0        0      407 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/config/schema.py
--rw-r--r--   0        0        0     2021 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/conftest.py
--rw-r--r--   0        0        0       70 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/.dockerignore
--rw-r--r--   0        0        0      279 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/.editorconfig
--rw-r--r--   0        0        0        0 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/.eslintignore
--rw-r--r--   0        0        0      269 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/.gitignore
--rw-r--r--   0        0        0       86 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/.npmignore
--rw-r--r--   0        0        0      201 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/.prettierrc
--rw-r--r--   0        0        0      220 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/Dockerfile
--rw-r--r--   0        0        0     3875 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/README.md
--rw-r--r--   0        0        0      566 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/assets/icons/question_mark.svg
--rw-r--r--   0        0        0     1577 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/assets/icons/scrive.svg
--rw-r--r--   0        0        0      566 2022-05-05 05:15:35.594963 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/assets/icons/question_mark.svg
--rw-r--r--   0        0        0     1577 2022-05-05 05:15:35.594963 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/assets/icons/scrive.svg
--rw-r--r--   0        0        0    44733 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/core-12852af1.js
--rw-r--r--   0        0        0    21942 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/css-shim-6aaf713d-bfe06088.js
--rw-r--r--   0        0        0    19796 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/dom-76cc7c7d-769a0dda.js
--rw-r--r--   0        0        0       15 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/index.cjs.js
--rw-r--r--   0        0        0      455 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/limepkg-scrive-lwc-components.cjs.js
--rw-r--r--   0        0        0      622 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/loader.cjs.js
--rw-r--r--   0        0        0      419 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/lwc-limepkg-scrive-loader.cjs.entry.js
--rw-r--r--   0        0        0    13723 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/lwc-limepkg-scrive.cjs.entry.js
--rw-r--r--   0        0        0    14422 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/shadow-css-4889ae62-03827a39.js
--rw-r--r--   0        0        0      298 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/collection/collection-manifest.json
--rw-r--r--   0        0        0       63 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive/lwc-limepkg-scrive.css
--rw-r--r--   0        0        0     6161 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive/lwc-limepkg-scrive.js
--rw-r--r--   0        0        0     2067 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.js
--rw-r--r--   0        0        0      183 2022-05-05 05:15:35.594963 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/collection/lime-web-component-platform.browser.js
--rw-r--r--   0        0        0    43799 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/core-2d5e9821.js
--rw-r--r--   0        0        0    21927 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/css-shim-6aaf713d-9b13816a.js
--rw-r--r--   0        0        0    19781 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/dom-76cc7c7d-0a082895.js
--rw-r--r--   0        0        0        1 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/index.mjs
--rw-r--r--   0        0        0      454 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/limepkg-scrive-lwc-components.mjs
--rw-r--r--   0        0        0      533 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/loader.mjs
--rw-r--r--   0        0        0      355 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/lwc-limepkg-scrive-loader.entry.js
--rw-r--r--   0        0        0    13624 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/lwc-limepkg-scrive.entry.js
--rw-r--r--   0        0        0    80225 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/core-js.js
--rw-r--r--   0        0        0    21928 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/css-shim.js
--rw-r--r--   0        0        0    20246 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/dom.js
--rw-r--r--   0        0        0      635 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/es5-html-element.js
--rw-r--r--   0        0        0     1041 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/index.js
--rw-r--r--   0        0        0     6855 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/promise.js
--rw-r--r--   0        0        0     4383 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/system.js
--rw-r--r--   0        0        0    14399 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/shadow-css-4889ae62-23996f3f.js
--rw-r--r--   0        0        0    49313 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/core-2d5e9821.js
--rw-r--r--   0        0        0    21939 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/css-shim-6aaf713d-9b13816a.js
--rw-r--r--   0        0        0    27836 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/dom-76cc7c7d-0a082895.js
--rw-r--r--   0        0        0        0 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/index.mjs
--rw-r--r--   0        0        0      494 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/limepkg-scrive-lwc-components.mjs
--rw-r--r--   0        0        0      580 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/loader.mjs
--rw-r--r--   0        0        0      458 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/lwc-limepkg-scrive-loader.entry.js
--rw-r--r--   0        0        0    15058 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/lwc-limepkg-scrive.entry.js
--rw-r--r--   0        0        0    15479 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/shadow-css-4889ae62-23996f3f.js
--rw-r--r--   0        0        0       47 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/index.js
--rw-r--r--   0        0        0       36 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/index.mjs
--rw-r--r--   0        0        0        0 2022-05-05 05:15:43.355000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/index.esm.js
--rw-r--r--   0        0        0      322 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/limepkg-scrive-lwc-components.esm.js
--rw-r--r--   0        0        0   136027 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/limepkg-scrive-lwc-components.js
--rw-r--r--   0        0        0    14911 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-1614c895.system.js
--rw-r--r--   0        0        0      306 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-27qqixta.system.entry.js
--rw-r--r--   0        0        0    18569 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-3b66a627.js
--rw-r--r--   0        0        0     9203 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-447ccb56.system.js
--rw-r--r--   0        0        0       76 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-50ea2036.system.js
--rw-r--r--   0        0        0     6156 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-5sossif3.system.entry.js
--rw-r--r--   0        0        0     8288 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-73bc5e11.js
--rw-r--r--   0        0        0    19088 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-7f10eb01.system.js
--rw-r--r--   0        0        0     8368 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-8af21e1f.js
--rw-r--r--   0        0        0      454 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-ae62b563.system.js
--rw-r--r--   0        0        0     4539 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-affe7c09.js
--rw-r--r--   0        0        0     5930 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-ed968002.system.js
--rw-r--r--   0        0        0     4824 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-eqwj2sbz.entry.js
--rw-r--r--   0        0        0      159 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-polpjbtb.entry.js
--rw-r--r--   0        0        0     1084 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components.js
--rw-r--r--   0        0        0      124 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/cdn.js
--rw-r--r--   0        0        0      124 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/index.cjs.js
--rw-r--r--   0        0        0      688 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/index.d.ts
--rw-r--r--   0        0        0       79 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/index.es2017.mjs
--rw-r--r--   0        0        0      719 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/index.mjs
--rw-r--r--   0        0        0      153 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/node-main.js
--rw-r--r--   0        0        0      299 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/package.json
--rw-r--r--   0        0        0      187 2022-05-05 05:15:35.594963 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/lwc.config.json
--rw-r--r--   0        0        0      654 2022-05-05 05:15:42.566996 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/components/lwc-limepkg-scrive/lwc-limepkg-scrive.d.ts
--rw-r--r--   0        0        0      329 2022-05-05 05:15:42.562996 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.d.ts
--rw-r--r--   0        0        0     2529 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/components.d.ts
--rw-r--r--   0        0        0      199 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/interface.d.ts
--rw-r--r--   0        0        0    41093 2022-05-05 05:15:43.359000 limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/stencil.core.d.ts
--rw-r--r--   0        0        0      239 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/eslint.js
--rw-r--r--   0        0        0      187 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/lwc.config.json
--rw-r--r--   0        0        0   222824 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/package-lock.json
--rw-r--r--   0        0        0     2934 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/package.json
--rw-r--r--   0        0        0      798 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.e2e.tsx
--rw-r--r--   0        0        0       67 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.scss
--rw-r--r--   0        0        0      163 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.spec.tsx
--rw-r--r--   0        0        0     4535 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.tsx
--rw-r--r--   0        0        0      927 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.tsx
--rw-r--r--   0        0        0      199 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/interface.d.ts
--rw-r--r--   0        0        0      183 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/lime-web-component-platform.browser.js
--rw-r--r--   0        0        0      597 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/stencil.config.dist.ts
--rw-r--r--   0        0        0      531 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/stencil.config.ts
--rw-r--r--   0        0        0      510 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/tsconfig.dev.json
--rw-r--r--   0        0        0      511 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/tsconfig.json
--rw-r--r--   0        0        0     1245 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/tslint.config.js
--rw-r--r--   0        0        0     4656 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/tslint.js
--rw-r--r--   0        0        0      411 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/frontend/tslint.specs.js
--rw-r--r--   0        0        0      175 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/__init__.py
--rw-r--r--   0        0        0      975 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/da.po
--rw-r--r--   0        0        0      975 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/de.po
--rw-r--r--   0        0        0      728 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/en.po
--rw-r--r--   0        0        0      976 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/fi.po
--rw-r--r--   0        0        0      974 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/nl.po
--rw-r--r--   0        0        0      978 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/no.po
--rw-r--r--   0        0        0      976 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/translations/sv.po
--rw-r--r--   0        0        0     1674 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/web_components/__init__.py
--rw-r--r--   0        0        0      165 2022-05-05 05:15:00.890848 limepkg-scrive-2.0.2/limepkg_scrive/web_components/web_components_test.py
--rw-r--r--   0        0        0     1039 2022-05-05 05:15:00.894848 limepkg-scrive-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2085 2022-05-05 05:15:49.871562 limepkg-scrive-2.0.2/setup.py
--rw-r--r--   0        0        0      223 2022-05-05 05:15:49.872090 limepkg-scrive-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2807 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/__init__.py
+-rw-r--r--   0        0        0     2630 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/config/__init__.py
+-rw-r--r--   0        0        0      407 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/config/schema.py
+-rw-r--r--   0        0        0     2021 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/conftest.py
+-rw-r--r--   0        0        0       70 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/.dockerignore
+-rw-r--r--   0        0        0      279 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/.editorconfig
+-rw-r--r--   0        0        0        0 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/.eslintignore
+-rw-r--r--   0        0        0      269 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/.gitignore
+-rw-r--r--   0        0        0       86 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/.npmignore
+-rw-r--r--   0        0        0      201 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/.prettierrc
+-rw-r--r--   0        0        0      220 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/Dockerfile
+-rw-r--r--   0        0        0     3875 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/README.md
+-rw-r--r--   0        0        0      566 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/assets/icons/question_mark.svg
+-rw-r--r--   0        0        0     1577 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/assets/icons/scrive.svg
+-rw-r--r--   0        0        0      566 2023-04-24 12:25:33.133337 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/assets/icons/question_mark.svg
+-rw-r--r--   0        0        0     1577 2023-04-24 12:25:33.133337 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/assets/icons/scrive.svg
+-rw-r--r--   0        0        0    44733 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/core-12852af1.js
+-rw-r--r--   0        0        0    21942 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/css-shim-6aaf713d-bfe06088.js
+-rw-r--r--   0        0        0    19796 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/dom-76cc7c7d-769a0dda.js
+-rw-r--r--   0        0        0       15 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/index.cjs.js
+-rw-r--r--   0        0        0      455 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/limepkg-scrive-lwc-components.cjs.js
+-rw-r--r--   0        0        0      622 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/loader.cjs.js
+-rw-r--r--   0        0        0      419 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/lwc-limepkg-scrive-loader.cjs.entry.js
+-rw-r--r--   0        0        0    13723 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/lwc-limepkg-scrive.cjs.entry.js
+-rw-r--r--   0        0        0    14422 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/shadow-css-4889ae62-03827a39.js
+-rw-r--r--   0        0        0      298 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/collection/collection-manifest.json
+-rw-r--r--   0        0        0       63 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive/lwc-limepkg-scrive.css
+-rw-r--r--   0        0        0     6161 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive/lwc-limepkg-scrive.js
+-rw-r--r--   0        0        0     2067 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.js
+-rw-r--r--   0        0        0      183 2023-04-24 12:25:33.133337 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/collection/lime-web-component-platform.browser.js
+-rw-r--r--   0        0        0    43799 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/core-2d5e9821.js
+-rw-r--r--   0        0        0    21927 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/css-shim-6aaf713d-9b13816a.js
+-rw-r--r--   0        0        0    19781 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/dom-76cc7c7d-0a082895.js
+-rw-r--r--   0        0        0        1 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/index.mjs
+-rw-r--r--   0        0        0      454 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/limepkg-scrive-lwc-components.mjs
+-rw-r--r--   0        0        0      533 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/loader.mjs
+-rw-r--r--   0        0        0      355 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/lwc-limepkg-scrive-loader.entry.js
+-rw-r--r--   0        0        0    13624 2023-04-24 12:25:39.525530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/lwc-limepkg-scrive.entry.js
+-rw-r--r--   0        0        0    80225 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/core-js.js
+-rw-r--r--   0        0        0    21928 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/css-shim.js
+-rw-r--r--   0        0        0    20246 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/dom.js
+-rw-r--r--   0        0        0      635 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/es5-html-element.js
+-rw-r--r--   0        0        0     1041 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/index.js
+-rw-r--r--   0        0        0     6855 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/promise.js
+-rw-r--r--   0        0        0     4383 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/system.js
+-rw-r--r--   0        0        0    14399 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/shadow-css-4889ae62-23996f3f.js
+-rw-r--r--   0        0        0    49313 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/core-2d5e9821.js
+-rw-r--r--   0        0        0    21939 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/css-shim-6aaf713d-9b13816a.js
+-rw-r--r--   0        0        0    27836 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/dom-76cc7c7d-0a082895.js
+-rw-r--r--   0        0        0        0 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/index.mjs
+-rw-r--r--   0        0        0      494 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/limepkg-scrive-lwc-components.mjs
+-rw-r--r--   0        0        0      580 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/loader.mjs
+-rw-r--r--   0        0        0      458 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/lwc-limepkg-scrive-loader.entry.js
+-rw-r--r--   0        0        0    15058 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/lwc-limepkg-scrive.entry.js
+-rw-r--r--   0        0        0    15479 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/shadow-css-4889ae62-23996f3f.js
+-rw-r--r--   0        0        0       47 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/index.js
+-rw-r--r--   0        0        0       36 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/index.mjs
+-rw-r--r--   0        0        0        0 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/index.esm.js
+-rw-r--r--   0        0        0      322 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/limepkg-scrive-lwc-components.esm.js
+-rw-r--r--   0        0        0   136027 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/limepkg-scrive-lwc-components.js
+-rw-r--r--   0        0        0    14911 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-1614c895.system.js
+-rw-r--r--   0        0        0      306 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-27qqixta.system.entry.js
+-rw-r--r--   0        0        0    18569 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-3b66a627.js
+-rw-r--r--   0        0        0     9203 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-447ccb56.system.js
+-rw-r--r--   0        0        0       76 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-50ea2036.system.js
+-rw-r--r--   0        0        0     6156 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-5sossif3.system.entry.js
+-rw-r--r--   0        0        0     8288 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-73bc5e11.js
+-rw-r--r--   0        0        0    19088 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-7f10eb01.system.js
+-rw-r--r--   0        0        0     8368 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-8af21e1f.js
+-rw-r--r--   0        0        0      454 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-ae62b563.system.js
+-rw-r--r--   0        0        0     4539 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-affe7c09.js
+-rw-r--r--   0        0        0     5930 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-ed968002.system.js
+-rw-r--r--   0        0        0     4824 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-eqwj2sbz.entry.js
+-rw-r--r--   0        0        0      159 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-polpjbtb.entry.js
+-rw-r--r--   0        0        0     1084 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components.js
+-rw-r--r--   0        0        0      124 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/cdn.js
+-rw-r--r--   0        0        0      124 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/index.cjs.js
+-rw-r--r--   0        0        0      688 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/index.d.ts
+-rw-r--r--   0        0        0       79 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/index.es2017.mjs
+-rw-r--r--   0        0        0      719 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/index.mjs
+-rw-r--r--   0        0        0      153 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/node-main.js
+-rw-r--r--   0        0        0      299 2023-04-24 12:25:39.521530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/package.json
+-rw-r--r--   0        0        0      187 2023-04-24 12:25:33.133337 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/lwc.config.json
+-rw-r--r--   0        0        0      654 2023-04-24 12:25:38.865511 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/components/lwc-limepkg-scrive/lwc-limepkg-scrive.d.ts
+-rw-r--r--   0        0        0      329 2023-04-24 12:25:38.865511 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.d.ts
+-rw-r--r--   0        0        0     2529 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/components.d.ts
+-rw-r--r--   0        0        0      199 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/interface.d.ts
+-rw-r--r--   0        0        0    41093 2023-04-24 12:25:39.529530 limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/stencil.core.d.ts
+-rw-r--r--   0        0        0      239 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/eslint.js
+-rw-r--r--   0        0        0      187 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/lwc.config.json
+-rw-r--r--   0        0        0   222824 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/package-lock.json
+-rw-r--r--   0        0        0     2934 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/package.json
+-rw-r--r--   0        0        0      798 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.e2e.tsx
+-rw-r--r--   0        0        0       67 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.scss
+-rw-r--r--   0        0        0      163 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.spec.tsx
+-rw-r--r--   0        0        0     4535 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.tsx
+-rw-r--r--   0        0        0      927 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.tsx
+-rw-r--r--   0        0        0      199 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/interface.d.ts
+-rw-r--r--   0        0        0      183 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/lime-web-component-platform.browser.js
+-rw-r--r--   0        0        0      597 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/stencil.config.dist.ts
+-rw-r--r--   0        0        0      531 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/stencil.config.ts
+-rw-r--r--   0        0        0      510 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/tsconfig.dev.json
+-rw-r--r--   0        0        0      511 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/tsconfig.json
+-rw-r--r--   0        0        0     1245 2023-04-24 12:25:07.848574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/tslint.config.js
+-rw-r--r--   0        0        0     4656 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/tslint.js
+-rw-r--r--   0        0        0      411 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/frontend/tslint.specs.js
+-rw-r--r--   0        0        0      175 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/__init__.py
+-rw-r--r--   0        0        0      975 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/da.po
+-rw-r--r--   0        0        0      975 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/de.po
+-rw-r--r--   0        0        0      728 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/en.po
+-rw-r--r--   0        0        0      976 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/fi.po
+-rw-r--r--   0        0        0      974 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/nl.po
+-rw-r--r--   0        0        0      978 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/no.po
+-rw-r--r--   0        0        0      976 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/translations/sv.po
+-rw-r--r--   0        0        0     1674 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/web_components/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/limepkg_scrive/web_components/web_components_test.py
+-rw-r--r--   0        0        0     1039 2023-04-24 12:25:07.852574 limepkg-scrive-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2085 2023-04-24 12:25:45.063769 limepkg-scrive-2.0.3/setup.py
+-rw-r--r--   0        0        0      273 2023-04-24 12:25:45.064138 limepkg-scrive-2.0.3/PKG-INFO
```

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/__init__.py` & `limepkg-scrive-2.0.3/limepkg_scrive/__init__.py`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/config/__init__.py` & `limepkg-scrive-2.0.3/limepkg_scrive/config/__init__.py`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/conftest.py` & `limepkg-scrive-2.0.3/limepkg_scrive/conftest.py`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/README.md` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/README.md`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/assets/icons/question_mark.svg` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/assets/icons/question_mark.svg`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/assets/icons/scrive.svg` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/assets/icons/scrive.svg`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/assets/icons/question_mark.svg` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/assets/icons/question_mark.svg`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/assets/icons/scrive.svg` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/assets/icons/scrive.svg`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/core-12852af1.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/core-12852af1.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/css-shim-6aaf713d-bfe06088.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/css-shim-6aaf713d-bfe06088.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/dom-76cc7c7d-769a0dda.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/dom-76cc7c7d-769a0dda.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/loader.cjs.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/loader.cjs.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/lwc-limepkg-scrive.cjs.entry.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/lwc-limepkg-scrive.cjs.entry.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/cjs/shadow-css-4889ae62-03827a39.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/cjs/shadow-css-4889ae62-03827a39.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive/lwc-limepkg-scrive.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive/lwc-limepkg-scrive.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/collection/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/core-2d5e9821.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/core-2d5e9821.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/css-shim-6aaf713d-9b13816a.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/css-shim-6aaf713d-9b13816a.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/dom-76cc7c7d-0a082895.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/dom-76cc7c7d-0a082895.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/loader.mjs` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/loader.mjs`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/lwc-limepkg-scrive.entry.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/lwc-limepkg-scrive.entry.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/core-js.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/core-js.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/css-shim.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/css-shim.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/dom.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/dom.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/es5-html-element.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/es5-html-element.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/index.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/index.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/promise.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/promise.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/polyfills/system.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/polyfills/system.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm/shadow-css-4889ae62-23996f3f.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm/shadow-css-4889ae62-23996f3f.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/core-2d5e9821.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/core-2d5e9821.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/css-shim-6aaf713d-9b13816a.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/css-shim-6aaf713d-9b13816a.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/dom-76cc7c7d-0a082895.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/dom-76cc7c7d-0a082895.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/loader.mjs` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/loader.mjs`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/lwc-limepkg-scrive.entry.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/lwc-limepkg-scrive.entry.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/esm-es5/shadow-css-4889ae62-23996f3f.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/esm-es5/shadow-css-4889ae62-23996f3f.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/limepkg-scrive-lwc-components.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/limepkg-scrive-lwc-components.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-1614c895.system.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-1614c895.system.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-3b66a627.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-3b66a627.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-447ccb56.system.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-447ccb56.system.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-5sossif3.system.entry.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-5sossif3.system.entry.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-73bc5e11.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-73bc5e11.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-7f10eb01.system.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-7f10eb01.system.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-8af21e1f.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-8af21e1f.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-affe7c09.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-affe7c09.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-ed968002.system.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-ed968002.system.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-eqwj2sbz.entry.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components/p-eqwj2sbz.entry.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/limepkg-scrive-lwc-components.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/index.d.ts` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/index.d.ts`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/loader/index.mjs` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/loader/index.mjs`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/components/lwc-limepkg-scrive/lwc-limepkg-scrive.d.ts` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/components/lwc-limepkg-scrive/lwc-limepkg-scrive.d.ts`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/components.d.ts` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/components.d.ts`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/dist/types/stencil.core.d.ts` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/dist/types/stencil.core.d.ts`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/package-lock.json` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/package.json` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/package.json`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.e2e.tsx` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.e2e.tsx`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.tsx` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive/lwc-limepkg-scrive.tsx`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.tsx` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/src/components/lwc-limepkg-scrive-loader/lwc-limepkg-scrive-loader.tsx`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/stencil.config.dist.ts` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/stencil.config.dist.ts`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/stencil.config.ts` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/stencil.config.ts`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/tslint.config.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/tslint.config.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/frontend/tslint.js` & `limepkg-scrive-2.0.3/limepkg_scrive/frontend/tslint.js`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/translations/da.po` & `limepkg-scrive-2.0.3/limepkg_scrive/translations/da.po`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/translations/de.po` & `limepkg-scrive-2.0.3/limepkg_scrive/translations/de.po`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/translations/en.po` & `limepkg-scrive-2.0.3/limepkg_scrive/translations/en.po`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/translations/fi.po` & `limepkg-scrive-2.0.3/limepkg_scrive/translations/fi.po`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/translations/nl.po` & `limepkg-scrive-2.0.3/limepkg_scrive/translations/nl.po`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/translations/no.po` & `limepkg-scrive-2.0.3/limepkg_scrive/translations/no.po`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/translations/sv.po` & `limepkg-scrive-2.0.3/limepkg_scrive/translations/sv.po`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/limepkg_scrive/web_components/__init__.py` & `limepkg-scrive-2.0.3/limepkg_scrive/web_components/__init__.py`

 * *Files identical despite different names*

### Comparing `limepkg-scrive-2.0.2/pyproject.toml` & `limepkg-scrive-2.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 [tool.metadata]
 display_name  = ''
 package_name  = 'limepkg-scrive'
 lib_name      = 'limepkg_scrive'
 
 [tool.poetry]
 name        = 'limepkg-scrive'
-version     = '2.0.2'
+version     = '2.0.3'
 description = 'Scrive eSigning'
 authors     = ['Scrive AB']
 
 [[tool.poetry.source]]
 name = 'lime'
 url  = 'https://pypi.lime.tech/simple'
 
 [tool.poetry.plugins.'lime_plugins']
 'limepkg-scrive' = 'limepkg_scrive'
 
 [tool.poetry.dependencies]
 lime-crm = '^2.76.0'
-python = '~3.7.3'
+python = '^3.7.3'
 
 [tool.poetry.dev-dependencies]
 click = '>=5.1'
 autopep8 = '>=1'
 flake8 = '>=2.1.0'
 ipdb = '>=0.8.1'
 pyreadline = '>=2.1'
```

### Comparing `limepkg-scrive-2.0.2/setup.py` & `limepkg-scrive-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,24 +36,24 @@
 ['lime-crm>=2.76.0,<3.0.0']
 
 entry_points = \
 {'lime_plugins': ['limepkg-scrive = limepkg_scrive']}
 
 setup_kwargs = {
     'name': 'limepkg-scrive',
-    'version': '2.0.2',
+    'version': '2.0.3',
     'description': 'Scrive eSigning',
     'long_description': None,
     'author': 'Scrive AB',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.3,<3.8.0',
+    'python_requires': '>=3.7.3,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

