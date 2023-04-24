# Comparing `tmp/rbcl-0.4.6-cp39-abi3-win32.whl.zip` & `tmp/rbcl-1.0.0-cp37-abi3-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 10550 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1320 b- defN 23-Feb-03 21:55 rbcl/__init__.py
--rw-rw-rw-  2.0 fat     1119 b- defN 23-Feb-03 21:55 rbcl/_sodium.tmpl
--rw-rw-rw-  2.0 fat    28190 b- defN 23-Feb-03 21:55 rbcl/rbcl.py
--rw-rw-rw-  2.0 fat      624 b- defN 23-Feb-03 21:55 rbcl/sodium_ffi.py
--rw-rw-rw-  2.0 fat     1093 b- defN 23-Feb-03 21:57 rbcl-0.4.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9540 b- defN 23-Feb-03 21:57 rbcl-0.4.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       96 b- defN 23-Feb-03 21:57 rbcl-0.4.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Feb-03 21:57 rbcl-0.4.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      662 b- defN 23-Feb-03 21:57 rbcl-0.4.6.dist-info/RECORD
-9 files, 42657 bytes uncompressed, 9430 bytes compressed:  77.9%
+Zip file size: 291472 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1246 b- defN 23-Apr-24 06:24 rbcl-1.0.0.data/purelib/rbcl/__init__.py
+-rw-r--r--  2.0 unx  1301610 b- defN 23-Apr-24 06:30 rbcl-1.0.0.data/purelib/rbcl/_sodium.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-Apr-24 06:24 rbcl-1.0.0.data/purelib/rbcl/_sodium.tmpl
+-rw-r--r--  2.0 unx     9780 b- defN 23-Apr-24 06:24 rbcl-1.0.0.data/purelib/rbcl/_sodium_build.py
+-rw-r--r--  2.0 unx    32815 b- defN 23-Apr-24 06:24 rbcl-1.0.0.data/purelib/rbcl/rbcl.py
+-rwxr-xr-x  2.0 unx     1072 b- defN 23-Apr-24 06:31 rbcl-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9729 b- defN 23-Apr-24 06:31 rbcl-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-24 06:31 rbcl-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-24 06:30 rbcl-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      861 b- defN 23-Apr-24 06:31 rbcl-1.0.0.dist-info/RECORD
+10 files, 1358324 bytes uncompressed, 290000 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
-Filename: rbcl/__init__.py
+Filename: rbcl-1.0.0.data/purelib/rbcl/__init__.py
 Comment: 
 
-Filename: rbcl/_sodium.tmpl
+Filename: rbcl-1.0.0.data/purelib/rbcl/_sodium.py
 Comment: 
 
-Filename: rbcl/rbcl.py
+Filename: rbcl-1.0.0.data/purelib/rbcl/_sodium.tmpl
 Comment: 
 
-Filename: rbcl/sodium_ffi.py
+Filename: rbcl-1.0.0.data/purelib/rbcl/_sodium_build.py
 Comment: 
 
-Filename: rbcl-0.4.6.dist-info/LICENSE
+Filename: rbcl-1.0.0.data/purelib/rbcl/rbcl.py
 Comment: 
 
-Filename: rbcl-0.4.6.dist-info/METADATA
+Filename: rbcl-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: rbcl-0.4.6.dist-info/WHEEL
+Filename: rbcl-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: rbcl-0.4.6.dist-info/top_level.txt
+Filename: rbcl-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: rbcl-0.4.6.dist-info/RECORD
+Filename: rbcl-1.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: rbcl-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rbcl/__init__.py` & `rbcl-1.0.0.data/purelib/rbcl/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-"""Allow users to use functions directly."""
-try:
-    # Import _sodium.py file which is emitted by build step
-    from rbcl._sodium import _sodium
-except ImportError:
-    pass
-
-from rbcl.rbcl import \
-    crypto_scalarmult_ristretto255, \
-    crypto_scalarmult_ristretto255_allow_scalar_zero, \
-    crypto_scalarmult_ristretto255_BYTES, \
-    crypto_scalarmult_ristretto255_SCALARBYTES, \
-    crypto_scalarmult_ristretto255_base, \
-    crypto_scalarmult_ristretto255_base_allow_scalar_zero, \
-    crypto_core_ristretto255_BYTES, \
-    crypto_core_ristretto255_HASHBYTES, \
-    crypto_core_ristretto255_NONREDUCEDSCALARBYTES, \
-    crypto_core_ristretto255_SCALARBYTES, \
-    crypto_core_ristretto255_add, \
-    crypto_core_ristretto255_from_hash, \
-    crypto_core_ristretto255_is_valid_point, \
-    crypto_core_ristretto255_random, \
-    crypto_core_ristretto255_scalar_add, \
-    crypto_core_ristretto255_scalar_complement, \
-    crypto_core_ristretto255_scalar_invert, \
-    crypto_core_ristretto255_scalar_mul, \
-    crypto_core_ristretto255_scalar_negate, \
-    crypto_core_ristretto255_scalar_random, \
-    crypto_core_ristretto255_scalar_reduce, \
-    crypto_core_ristretto255_scalar_sub, \
-    crypto_core_ristretto255_sub, \
-    randombytes, \
-    randombytes_buf_deterministic
+"""Gives users direct access to functions."""
+from rbcl.rbcl import _sodium # pylint: disable=import-self
+
+from rbcl.rbcl import \
+    randombytes_SEEDBYTES, \
+    crypto_core_ristretto255_BYTES, \
+    crypto_core_ristretto255_HASHBYTES, \
+    crypto_core_ristretto255_NONREDUCEDSCALARBYTES, \
+    crypto_core_ristretto255_SCALARBYTES, \
+    crypto_scalarmult_ristretto255_BYTES, \
+    crypto_scalarmult_ristretto255_SCALARBYTES, \
+    randombytes, \
+    randombytes_buf_deterministic, \
+    crypto_core_ristretto255_is_valid_point, \
+    crypto_core_ristretto255_random, \
+    crypto_core_ristretto255_from_hash, \
+    crypto_core_ristretto255_add, \
+    crypto_core_ristretto255_sub, \
+    crypto_core_ristretto255_scalar_random, \
+    crypto_core_ristretto255_scalar_reduce, \
+    crypto_core_ristretto255_scalar_negate, \
+    crypto_core_ristretto255_scalar_complement, \
+    crypto_core_ristretto255_scalar_invert, \
+    crypto_core_ristretto255_scalar_add, \
+    crypto_core_ristretto255_scalar_sub, \
+    crypto_core_ristretto255_scalar_mul, \
+    crypto_scalarmult_ristretto255_base, \
+    crypto_scalarmult_ristretto255_base_allow_scalar_zero, \
+    crypto_scalarmult_ristretto255, \
+    crypto_scalarmult_ristretto255_allow_scalar_zero
```

## Comparing `rbcl-0.4.6.dist-info/LICENSE` & `rbcl-1.0.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Nth Party, Ltd.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Nth Party, Ltd.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `rbcl-0.4.6.dist-info/METADATA` & `rbcl-1.0.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,175 +1,206 @@
-Metadata-Version: 2.1
-Name: rbcl
-Version: 0.4.6
-Summary: Python library that bundles libsodium and provides wrappers for its Ristretto group functions.
-Home-page: https://github.com/nthparty/rbcl
-Author: Nth Party, Ltd.
-Author-email: team@nthparty.com
-License: MIT
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: cffi (~=1.15)
-Requires-Dist: barriers (~=1.0)
-Requires-Dist: pystache (~=0.6)
-Provides-Extra: build
-Requires-Dist: setuptools (~=62.0) ; extra == 'build'
-Requires-Dist: wheel (~=0.37) ; extra == 'build'
-Requires-Dist: cffi (~=1.15) ; extra == 'build'
-Requires-Dist: pystache (~=0.6) ; extra == 'build'
-Provides-Extra: coveralls
-Requires-Dist: coveralls (~=3.3.1) ; extra == 'coveralls'
-Provides-Extra: docs
-Requires-Dist: sphinx (~=4.2.0) ; extra == 'docs'
-Requires-Dist: sphinx-rtd-theme (~=1.0.0) ; extra == 'docs'
-Provides-Extra: lint
-Requires-Dist: pylint (~=2.14.0) ; extra == 'lint'
-Provides-Extra: publish
-Requires-Dist: twine (~=4.0) ; extra == 'publish'
-Provides-Extra: test
-Requires-Dist: pytest (~=7.0) ; extra == 'test'
-Requires-Dist: pytest-cov (~=3.0) ; extra == 'test'
-
-====
-rbcl
-====
-
-Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__ and provides wrappers for its Ristretto group functions.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/rbcl.svg
-   :target: https://badge.fury.io/py/rbcl
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/rbcl/badge/?version=latest
-   :target: https://rbcl.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/rbcl/workflows/lint-test-cover-docs-build-upload/badge.svg
-   :target: https://github.com/nthparty/rbcl/actions
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/rbcl/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/rbcl?branch=main
-   :alt: Coveralls test coverage summary.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__::
-
-    python -m pip install rbcl
-
-The library can be imported in the usual ways::
-
-    import rbcl
-    from rbcl import *
-
-Examples
-^^^^^^^^
-
-A few usage examples are presented below::
-
-    >>> from rbcl import *
-    >>> x = crypto_core_ristretto255_random()
-    >>> assert crypto_core_ristretto255_is_valid_point(x)
-    >>> y = crypto_core_ristretto255_from_hash(b'\xF0'*64)
-    >>> assert crypto_core_ristretto255_is_valid_point(y)
-    >>> z1 = crypto_core_ristretto255_add(x, y)
-    >>> z2 = crypto_core_ristretto255_add(y, x)
-    >>> assert z1 == z2  # Assert that point addition commutes.
-    >>> s1 = crypto_core_ristretto255_scalar_random()
-    >>> s2 = crypto_core_ristretto255_scalar_random()
-    >>> w1 = crypto_scalarmult_ristretto255(s1, crypto_scalarmult_ristretto255(s2, x))
-    >>> w2 = crypto_scalarmult_ristretto255(s2, crypto_scalarmult_ristretto255(s1, x))
-    >>> assert w1 == w2  # Assert that point multiplication (by a scalar) is repeated addition.
-
-This library exports Python wrappers for `constructors <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#encoded-element-validation>`__, `point arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-multiplication>`__, and `scalar arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-arithmetic-over-l>`__.
-
-Development, Build, and Manual Installation Instructions
---------------------------------------------------------
-All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.py``. The ``extras_require`` parameter is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Building from Source
-^^^^^^^^^^^^^^^^^^^^
-The library can be built manually from source **within Linux and macOS** using the sequence of commands below::
-
-    python -m pip install .[build]
-    python setup.py bdist_wheel
-
-Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python setup.py bdist_wheel`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location::
-
-    wget -O src/rbcl/libsodium.tar.gz https://github.com/jedisct1/libsodium/releases/download/1.0.18-RELEASE/libsodium-1.0.18.tar.gz
-
-The process for building manually from source within a Windows environment is not currently documented, but an example of one sequence of steps can be found in the Windows job entry within the GitHub Actions workflow defined in the file ``.github/workflows/lint-test-cover-docs-build-upload.yml``.
-
-Preparation for Local Development
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it)::
-
-    cp build/lib*/rbcl/_sodium*.* src/rbcl
-
-Manual Installation
-^^^^^^^^^^^^^^^^^^^
-Once the package is `built <#building-from-source>`_, it can be installed manually using the command below::
-
-    python -m pip install -f dist . --upgrade
-
-Documentation
-^^^^^^^^^^^^^
-Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../setup.py ../src/rbcl/sodium_ffi.py && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-Before unit tests can be executed, it is first necessary to prepare for local development by compiling and moving into its designated location the libsodium shared library file (as described in `the relevant subsection above <#preparation-for-local-development>`__).
-
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
-
-    python src/rbcl/rbcl.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/rbcl
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/rbcl>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``setup.py``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python setup.py sdist
-
-Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain::
-
-    cd dist && for i in `ls *.zip`; do unzip $i; done && rm *.zip && cd ..
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+Metadata-Version: 2.1
+Name: rbcl
+Version: 1.0.0
+Summary: Python library that bundles libsodium and provides wrappers for its Ristretto group functions.
+Author: Nth Party
+Author-email: team@nthparty.com
+License: MIT
+Requires-Python: >=3.7
+License-File: LICENSE
+Requires-Dist: barriers (~=1.1)
+Provides-Extra: build
+Requires-Dist: setuptools (~=67.6) ; extra == 'build'
+Requires-Dist: wheel (~=0.37) ; extra == 'build'
+Requires-Dist: pystache (~=0.6) ; extra == 'build'
+Requires-Dist: build (~=0.10) ; extra == 'build'
+Provides-Extra: coveralls
+Requires-Dist: coveralls (~=3.3.1) ; extra == 'coveralls'
+Provides-Extra: docs
+Requires-Dist: sphinx (~=4.2.0) ; extra == 'docs'
+Requires-Dist: sphinx-rtd-theme (~=1.0.0) ; extra == 'docs'
+Provides-Extra: lint
+Requires-Dist: pylint (~=2.17.0) ; extra == 'lint'
+Provides-Extra: publish
+Requires-Dist: twine (~=4.0) ; extra == 'publish'
+Provides-Extra: test
+Requires-Dist: pytest (~=7.2) ; extra == 'test'
+Requires-Dist: pytest-cov (~=4.0) ; extra == 'test'
+
+====
+rbcl
+====
+
+Python library that bundles `libsodium <https://github.com/jedisct1/libsodium>`__ and provides wrappers for its Ristretto group functions.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/rbcl.svg
+   :target: https://badge.fury.io/py/rbcl
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/rbcl/badge/?version=latest
+   :target: https://rbcl.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/rbcl/workflows/lint-test-cover-docs-build-upload/badge.svg
+   :target: https://github.com/nthparty/rbcl/actions
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/rbcl/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/rbcl?branch=main
+   :alt: Coveralls test coverage summary.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/rbcl>`__:
+
+.. code-block:: bash
+
+    python -m pip install rbcl
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import rbcl
+    from rbcl import *
+
+Examples
+^^^^^^^^
+
+A few usage examples are presented below:
+
+.. code-block:: python
+
+    >>> from rbcl import *
+    >>> x = crypto_core_ristretto255_random()
+    >>> assert crypto_core_ristretto255_is_valid_point(x)
+    >>> y = crypto_core_ristretto255_from_hash(b'\xF0' * 64)
+    >>> assert crypto_core_ristretto255_is_valid_point(y)
+    >>> z1 = crypto_core_ristretto255_add(x, y)
+    >>> z2 = crypto_core_ristretto255_add(y, x)
+    >>> assert z1 == z2 # Point addition commutes.
+    >>> s1 = crypto_core_ristretto255_scalar_random()
+    >>> s2 = crypto_core_ristretto255_scalar_random()
+    >>> w1 = crypto_scalarmult_ristretto255(s1, crypto_scalarmult_ristretto255(s2, x))
+    >>> w2 = crypto_scalarmult_ristretto255(s2, crypto_scalarmult_ristretto255(s1, x))
+    >>> assert w1 == w2 # Multiplication of a point by a scalar is repeated addition.
+
+This library exports Python wrappers for `constructors <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#encoded-element-validation>`__, `point arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-multiplication>`__, and `scalar arithmetic functions <https://libsodium.gitbook.io/doc/advanced/point-arithmetic/ristretto#scalar-arithmetic-over-l>`__.
+
+Development, Build, and Manual Installation Instructions
+--------------------------------------------------------
+All development and installation dependencies are managed using `setuptools <https://pypi.org/project/setuptools>`__ and are fully specified in ``setup.cfg``. The ``extras_require`` option is used to `specify optional requirements <https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__ (assuming that the library has already been built successfully):
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Building from Source
+^^^^^^^^^^^^^^^^^^^^
+The library can be built manually from source **within Linux and macOS** using the sequence of commands below:
+
+.. code-block:: bash
+
+    python -m pip install .[build]
+    python -m build --sdist --wheel .
+
+Developing the library further in a local environment and/or building the library from source requires `libsodium <https://doc.libsodium.org>`__. The step ``python -m build --sdist --wheel .`` in the above attempts to automatically locate a copy of the libsodium source archive ``src/rbcl/libsodium.tar.gz``. If the archive corresponding to the operating system is not found, the build process attempts to download it. To support building offline, it is necessary to first download the appropriate libsodium archive to its designated location:
+
+.. code-block:: bash
+
+    wget -O src/rbcl/libsodium.tar.gz https://github.com/jedisct1/libsodium/releases/download/1.0.18-RELEASE/libsodium-1.0.18.tar.gz
+
+The process for building manually from source within a Windows environment is not currently documented, but an example of one sequence of steps can be found in the Windows job entry within the GitHub Actions workflow defined in the file ``.github/workflows/lint-test-cover-docs-build-upload.yml``.
+
+Preparation for Local Development
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Before `documentation can be generated <#documentation>`_ or `tests can be executed <#testing-and-conventions>`_, it is necessary to `run the build process <#building-from-source>`_ and then to use the command below to move the compiled libsodium shared/dynamic library file into its designated location (so that the module file ``src/rbcl/rbcl.py`` is able to import it):
+
+.. code-block:: bash
+
+    cp build/lib*/rbcl/_sodium.py src/rbcl
+
+Manual Installation
+^^^^^^^^^^^^^^^^^^^
+Once the package is `built <#building-from-source>`_, it can be installed manually using the command below:
+
+.. code-block:: bash
+
+    python -m pip install -f dist . --upgrade
+
+Documentation
+^^^^^^^^^^^^^
+Once the libsodium shared library file is compiled and moved into its designated location (as described in `the relevant subsection above <#preparation-for-local-development>`_), the documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. ../src/rbcl/_sodium_build.py && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+Before unit tests can be executed, it is first necessary to prepare for local development by compiling and moving into its designated location the libsodium shared library file (as described in `the relevant subsection above <#preparation-for-local-development>`__).
+
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see ``pyproject.toml`` for configuration details):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
+
+    python src/rbcl/rbcl.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/rbcl src/rbcl/_sodium.tmpl src/rbcl/_sodium_build.py --disable=duplicate-code
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/rbcl>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/rbcl>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``setup.cfg``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist .
+
+Next, navigate to the appropriate GitHub Actions run of the workflow defined in ``lint-test-cover-docs-build-upload.yml``. Click on the workflow and scroll down to the **Artifacts** panel. Download the archive files to the ``dist`` directory. Unzip all the archive files so that only the ``*.whl`` files remain:
+
+.. code-block:: bash
+
+    cd dist && for i in `ls *.zip`; do unzip $i; done && rm *.zip && cd ..
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

