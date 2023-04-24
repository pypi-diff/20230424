# Comparing `tmp/repairwheel-0.2.2.tar.gz` & `tmp/repairwheel-0.2.3.tar.gz`

## Comparing `repairwheel-0.2.2.tar` & `repairwheel-0.2.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.2/CHANGELOG.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 repairwheel-0.2.2/codecov.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/__main__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/compat.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/fileutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/py.typed
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/repair.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel.pyi
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/vendor.txt
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/LICENSE
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/LICENSE.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/__main__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/condatools.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/elfutils.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/error.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/genericpkgctx.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/hashfile.py
--rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/lddtree.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/libc.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main_addtag.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main_lddtree.py
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main_repair.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main_show.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/musllinux.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/patcher.py
--rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/repair.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/tmpdirs.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/tools.py
--rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/wheel_abi.py
--rw-r--r--   0        0        0     9516 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/wheeltools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/__init__.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/__init__.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/__init__.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/external_references.py
--rw-r--r--   0        0        0    53261 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/LICENSE
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/_version.py
--rw-r--r--   0        0        0    33312 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/delocating.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/fuse.py
--rw-r--r--   0        0        0    27193 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/libsana.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/pkginfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/py.typed
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/tmpdirs.py
--rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/tools.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/wheeltools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/__init__.py
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_path.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/linux/__init__.py
--rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/linux/elffile.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/linux/monkeypatch.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/linux/patcher.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/linux/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/macos/__init__.py
--rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/macos/machosign.py
--rw-r--r--   0        0        0    11400 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/macos/machotools.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/macos/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/windows/__init__.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 repairwheel-0.2.2/src/repairwheel/windows/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/test_common.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/test_windows.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/gen_check/__init__.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/gen_check/test_check.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/gen_check/test_generate.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-native/README.md
--rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-native/build.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-native/testwheel.c
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-native/testdep/testdep.c
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-native/testdep/testdep.h
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-python/build.sh
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-python/pyproject.toml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-python/testwheel/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/build-python/testwheel/testwheel.py
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl
--rw-r--r--   0        0        0    16944 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib
--rw-r--r--   0        0        0    64683 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl
--rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tools/vendoring/patches/auditwheel.patch
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tools/vendoring/patches/delocate.chmod.patch
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 repairwheel-0.2.2/tools/vendoring/patches/delocate.patch
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 repairwheel-0.2.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.2/LICENSE
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 repairwheel-0.2.2/README.md
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 repairwheel-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 repairwheel-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.3/CHANGELOG.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 repairwheel-0.2.3/codecov.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/__main__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/compat.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/fileutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/py.typed
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/repair.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel.pyi
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/vendor.txt
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/__main__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/condatools.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/elfutils.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/error.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/genericpkgctx.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/hashfile.py
+-rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/lddtree.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/libc.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_addtag.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_lddtree.py
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_repair.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_show.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/musllinux.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/patcher.py
+-rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/repair.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tmpdirs.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tools.py
+-rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheel_abi.py
+-rw-r--r--   0        0        0     9516 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheeltools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/__init__.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/__init__.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/__init__.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/external_references.py
+-rw-r--r--   0        0        0    53261 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/LICENSE
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/_version.py
+-rw-r--r--   0        0        0    33312 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/delocating.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/fuse.py
+-rw-r--r--   0        0        0    27193 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/libsana.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/pkginfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/py.typed
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tmpdirs.py
+-rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tools.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/wheeltools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/__init__.py
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_path.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/__init__.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/elffile.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/monkeypatch.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/patcher.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/__init__.py
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/machosign.py
+-rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/machotools.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/windows/__init__.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/windows/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/test_common.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/test_windows.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/gen_check/__init__.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/gen_check/test_check.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/gen_check/test_generate.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/README.md
+-rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/build.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/testwheel.c
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/testdep/testdep.c
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/testdep/testdep.h
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/build.sh
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/pyproject.toml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/testwheel/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/testwheel/testwheel.py
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl
+-rw-r--r--   0        0        0    16944 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib
+-rw-r--r--   0        0        0    64683 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl
+-rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tools/vendoring/patches/auditwheel.patch
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tools/vendoring/patches/delocate.chmod.patch
+-rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tools/vendoring/patches/delocate.patch
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 repairwheel-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 repairwheel-0.2.3/README.md
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 repairwheel-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 repairwheel-0.2.3/PKG-INFO
```

### Comparing `repairwheel-0.2.2/src/repairwheel/compat.py` & `repairwheel-0.2.3/src/repairwheel/compat.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/fileutil.py` & `repairwheel-0.2.3/src/repairwheel/fileutil.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/repair.py` & `repairwheel-0.2.3/src/repairwheel/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/wheel.py` & `repairwheel-0.2.3/src/repairwheel/wheel.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/LICENSE` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/LICENSE.txt` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/condatools.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/condatools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/elfutils.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/elfutils.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/genericpkgctx.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/genericpkgctx.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/lddtree.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/lddtree.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main_addtag.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_addtag.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main_repair.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/main_show.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_show.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/musllinux.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/musllinux.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/patcher.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/patcher.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/repair.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/tmpdirs.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/tools.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/wheel_abi.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheel_abi.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/wheeltools.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheeltools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/__init__.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/external_references.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/external_references.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/LICENSE` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/delocating.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/delocating.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/fuse.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/fuse.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/libsana.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/libsana.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/pkginfo.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/pkginfo.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/tmpdirs.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/tools.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/wheeltools.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/wheeltools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_path.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_path.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py` & `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/linux/elffile.py` & `repairwheel-0.2.3/src/repairwheel/linux/elffile.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/linux/monkeypatch.py` & `repairwheel-0.2.3/src/repairwheel/linux/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/linux/patcher.py` & `repairwheel-0.2.3/src/repairwheel/linux/patcher.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/linux/repair.py` & `repairwheel-0.2.3/src/repairwheel/linux/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/macos/machosign.py` & `repairwheel-0.2.3/src/repairwheel/macos/machosign.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/macos/machotools.py` & `repairwheel-0.2.3/src/repairwheel/macos/machotools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import struct
 from typing import Callable
 from typing import FrozenSet
 from typing import Optional
 from typing import Tuple
 from typing import TypeVar
 from macholib.MachO import MachO
 from macholib.MachO import MachOHeader
@@ -17,14 +18,18 @@
 from macholib.mach_o import get_cpu_subtype
 
 from . import machosign
 
 LOG = logging.getLogger(__name__)
 T = TypeVar("T")
 
+# Errors that we ignore when attempting to read files. Delocate will attempt
+# to read all files (e.g., py.typed) even if they aren't dylibs.
+IGNORED_READ_ERRORS = (ValueError, struct.error)
+
 # Maps from macholib's CPU_TYPE_NAMES entry and get_cpu_subtype output to
 # what lipo would print
 LIPO_ARCH_NAMES = {
     "MC680x0": {
         "CPU_SUBTYPE_MC680x0_ALL": "m68k",
         "CPU_SUBTYPE_MC68030_ONLY": "m68030",
         "CPU_SUBTYPE_MC68040": "m68040",
@@ -157,15 +162,15 @@
             results.append(lc_str_value(cmd.name, entry).decode("utf-8"))
 
         return tuple(results)
 
     try:
         macho = MachO(filename)
         return _all_arches_same_value(macho, _val)
-    except ValueError:
+    except IGNORED_READ_ERRORS:
         return ()
 
 
 def get_install_id(filename: str) -> Optional[str]:
     """Return install id from library named in `filename`
 
     Returns None if no install id, or if this is not an object file.
@@ -192,15 +197,15 @@
             entry = header.commands[header.id_cmd]
             _, cmd, _ = entry
             return lc_str_value(cmd.name, entry).decode("utf-8")
 
     try:
         macho = MachO(filename)
         return _all_arches_same_value(macho, _val)
-    except ValueError:
+    except IGNORED_READ_ERRORS:
         return None
 
 
 def set_install_name(filename: str, oldname: str, newname: str, ad_hoc_sign: bool = True) -> None:
     """Set install name `oldname` to `newname` in library filename
 
     Parameters
@@ -304,15 +309,15 @@
             results.append(lc_str_value(cmd.path, entry).decode("utf-8"))
 
         return tuple(results)
 
     try:
         macho = MachO(filename)
         return _all_arches_same_value(macho, _val)
-    except ValueError:
+    except IGNORED_READ_ERRORS:
         return ()
 
 
 def get_archs(filename: str) -> FrozenSet[str]:
     """Return architecture types from library `libname`
 
     Parameters
```

### Comparing `repairwheel-0.2.2/src/repairwheel/macos/repair.py` & `repairwheel-0.2.3/src/repairwheel/macos/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/src/repairwheel/windows/repair.py` & `repairwheel-0.2.3/src/repairwheel/windows/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/conftest.py` & `repairwheel-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/test_common.py` & `repairwheel-0.2.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/test_windows.py` & `repairwheel-0.2.3/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/util.py` & `repairwheel-0.2.3/tests/util.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/gen_check/test_check.py` & `repairwheel-0.2.3/tests/gen_check/test_check.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/build-native/build.py` & `repairwheel-0.2.3/tests/testwheel/build-native/build.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/build-native/testwheel.c` & `repairwheel-0.2.3/tests/testwheel/build-native/testwheel.c`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll` & `repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl` & `repairwheel-0.2.3/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tools/vendoring/patches/auditwheel.patch` & `repairwheel-0.2.3/tools/vendoring/patches/auditwheel.patch`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tools/vendoring/patches/delocate.chmod.patch` & `repairwheel-0.2.3/tools/vendoring/patches/delocate.chmod.patch`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/tools/vendoring/patches/delocate.patch` & `repairwheel-0.2.3/tools/vendoring/patches/delocate.patch`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/LICENSE` & `repairwheel-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/README.md` & `repairwheel-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.2/pyproject.toml` & `repairwheel-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repairwheel"
-version = "0.2.2"
+version = "0.2.3"
 description = "Repair any wheel, anywhere"
 readme = "README.md"
 requires-python = ">= 3.7"
 license.file = "LICENSE"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
```

### Comparing `repairwheel-0.2.2/PKG-INFO` & `repairwheel-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repairwheel
-Version: 0.2.2
+Version: 0.2.3
 Summary: Repair any wheel, anywhere
 Project-URL: homepage, https://github.com/jvolkman/repairwheel
 License: Copyright © 2023 Jeremy Volkman
         
         Permission is hereby granted, free of charge, to any person obtaining a
         copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
```

