# Comparing `tmp/whoisdomain-1.20230417.6.tar.gz` & `tmp/whoisdomain-1.20230424.7.tar.gz`

## Comparing `whoisdomain-1.20230417.6.tar` & `whoisdomain-1.20230424.7.tar`

### file list

```diff
@@ -1,198 +1,206 @@
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Historical.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/MANIFEST.in
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/license
--rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pypi-test.sh
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pypi.sh
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pyproject.toml-template
--rwxr-xr-x   0        0        0     2288 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/test.py
--rwxr-xr-x   0        0        0    15950 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/test2.py
--rwxr-xr-x   0        0        0     1340 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/test_adjust.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   190007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    55638 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    62946 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1146965 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   126768 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   115786 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   147473 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    95073 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   136157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    23854 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    88645 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    92150 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    47582 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    37124 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    80882 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   151599 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    29543 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52507 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   175017 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   150518 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    46067 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   254545 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   446688 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    54794 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    92867 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   390721 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   135868 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25468 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    62332 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    32673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73584 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    68120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    95559 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    15557 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   369261 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.data.json
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.meta.json
--rw-r--r--   0        0        0    14086 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.data.json
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json
--rw-r--r--   0        0        0    12157 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.data.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.meta.json
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.meta.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/DONE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/TODO
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/analize_patterns.py
--rwxr-xr-x   0        0        0     2623 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/compare_known_tld.py
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/convert_to_dict.sh
--rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/makeTestdataAll.sh
--rwxr-xr-x   0        0        0     8753 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/test.py
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/test.sh
--rwxr-xr-x   0        0        0    11070 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/test3.py
--rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/testExtend.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/bin/find_input_no_output.sh
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/failed-parsing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/invalid-tld.txt
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/new-test.txt
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/ok-domains.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/private-reg.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/Old/tests/unknown-dateformat.txt
--rwxr-xr-x   0        0        0     1796 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/make_testdata.sh
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.com/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.com/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.com/output
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.net/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.net/nameservers
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.net/output
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.org/input
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.org/nameservers
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/example.org/output
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/google.com/input
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/google.com/nameservers
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/google.com/output
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/hello.xyz/input
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/hello.xyz/nameservers
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/hello.xyz/output
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.jp/input
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.jp/nameservers
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.jp/output
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.uk/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.uk/nameservers
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.co.uk/output
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com/input
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com/nameservers
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com/output
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.sg/input
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.sg/nameservers
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.sg/output
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.tr/input
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.tr/nameservers
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.com.tr/output
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.jp/input
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.jp/nameservers
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.jp/output
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.kr/input
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.kr/nameservers
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/meta.kr/output
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/xs4all.nl/input
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/xs4all.nl/nameservers
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/testdata/xs4all.nl/output
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_1_query.py
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/exceptions.py
--rw-r--r--   0        0        0   104888 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.gitignore
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/.hgignore
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/README.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/pyproject.toml
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 whoisdomain-1.20230417.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Historical.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/MANIFEST.in
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/license
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pypi-test.sh
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pypi.sh
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pyproject.toml-template
+-rwxr-xr-x   0        0        0     2472 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test.py
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test.sh
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test2.py
+-rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/test_adjust.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.github/workflows/lint.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   190007 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    55638 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    62946 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1146965 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   126768 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   115786 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0   147473 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0    95073 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0   136157 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    23854 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/getopt.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/getopt.meta.json
+-rw-r--r--   0        0        0    88645 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    92150 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    47582 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    37124 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    80882 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   151599 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    29543 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    52507 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   175017 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   150518 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test.meta.json
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test2.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test2.meta.json
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test_adjust.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/test_adjust.meta.json
+-rw-r--r--   0        0        0    46067 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   254545 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   446688 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    54794 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    92867 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   390721 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   135868 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25468 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    62332 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    32673 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    73584 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    68120 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    95559 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12461 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    15557 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   369261 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json
+-rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_1_query.data.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_1_query.meta.json
+-rw-r--r--   0        0        0    13575 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_2_parse.data.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json
+-rw-r--r--   0        0        0    12064 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json
+-rw-r--r--   0        0        0    17214 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/__init__.data.json
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/__init__.meta.json
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/exceptions.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/exceptions.meta.json
+-rw-r--r--   0        0        0    19586 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/main.data.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/main.meta.json
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json
+-rw-r--r--   0        0        0    14355 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/whoisdomain.data.json
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/whoisdomain.meta.json
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/DONE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/TODO
+-rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/analize_patterns.py
+-rwxr-xr-x   0        0        0     2623 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/compare_known_tld.py
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/convert_to_dict.sh
+-rwxr-xr-x   0        0        0     6984 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/makeTestdataAll.sh
+-rwxr-xr-x   0        0        0     8753 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/test.py
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/test.sh
+-rwxr-xr-x   0        0        0    11070 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/test3.py
+-rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/testExtend.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/bin/find_input_no_output.sh
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/failed-parsing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/invalid-tld.txt
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/new-test.txt
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/ok-domains.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/private-reg.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/Old/tests/unknown-dateformat.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/docs/index.html
+-rwxr-xr-x   0        0        0     1733 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/make_testdata.sh
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.com/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.com/nameservers
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.com/output
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.net/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.net/nameservers
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.net/output
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.org/input
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.org/nameservers
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/example.org/output
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/hello.xyz/input
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/hello.xyz/nameservers
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/hello.xyz/output
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.jp/input
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.jp/nameservers
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.jp/output
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.uk/input
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.uk/nameservers
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.co.uk/output
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com/input
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com/nameservers
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com/output
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com.tr/input
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com.tr/nameservers
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.com.tr/output
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.jp/input
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.jp/nameservers
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.jp/output
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.kr/input
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.kr/nameservers
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/meta.kr/output
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/xs4all.nl/input
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/xs4all.nl/nameservers
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/testdata/xs4all.nl/output
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0     9929 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    16746 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/main.py
+-rw-r--r--   0        0        0   104916 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.gitignore
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/.hgignore
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/README.md
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/pyproject.toml
+-rw-r--r--   0        0        0     8388 2020-02-02 00:00:00.000000 whoisdomain-1.20230424.7/PKG-INFO
```

### Comparing `whoisdomain-1.20230417.6/Historical.txt` & `whoisdomain-1.20230424.7/Historical.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/pypi-test.sh` & `whoisdomain-1.20230424.7/pypi-test.sh`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     if [ -z "${TODAY_SEQ}" ]
     then
         TODAY_SEQ="1"
     else
         TODAY_SEQ=$(( TODAY_SEQ + 1))
     fi
 
+    mkdir -p ./work/
     # keep track of the latest version string
     echo "${VERSION}.${DATE}.${TODAY_SEQ}" >./work/version
 }
 
 makeTomlFile()
 {
     cat pyproject.toml-template |
@@ -48,14 +49,15 @@
 {
     twine upload -r testpypi dist/*"${VERSION}.${DATE}.${TODAY_SEQ}"*
 }
 
 main()
 {
     ./reformat-code.sh
+    mypy --implicit-optional *.py
     mypy --implicit-optional whoisdomain
 
     setupVersionNumberToday
     makeTomlFile
     buildDist
     uploadTwineTest
 }
```

### Comparing `whoisdomain-1.20230417.6/pyproject.toml-template` & `whoisdomain-1.20230424.7/pyproject.toml-template`

 * *Files 4% similar despite different names*

```diff
@@ -43,11 +43,15 @@
     "tld",
     "domain",
     "expiration",
     "cctld",
     "registrar",
 ]
 
+[project.scripts]
+whoisdomain = 'whoisdomain.main:main'
+
 [project.urls]
 "Bug Tracker" = "https://github.com/mboot-github/WhoisDomain/issues"
 "Home Page" = "https://github.com/mboot-github/WhoisDomain/"
 "Repository" = "https://github.com/mboot-github/WhoisDomain/"
+
```

### Comparing `whoisdomain-1.20230417.6/test.py` & `whoisdomain-1.20230424.7/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # from: https://github.com/maarten-boot/python-whois-extended
 
 import sys
 
+from typing import (
+    Optional,
+    # Dict,
+    List,
+    # Any,
+)
+
+
 import whoisdomain as whois
 
-DOMAINS = """
+DOMAINS: str = """
 google.com
 www.fsdfsdfsdfsd.google.com
 google.org
 google.net
 google.pl
 google.co
 google.co.uk
@@ -76,24 +84,28 @@
 nic.ge,whois.nic.ge
 nic.рус
 whois.twnic.net.tw
 nic.онлайн
 """
 
 
-def query(domain, host=None):
+def query(
+    domain: str,
+    host: Optional[str] = None,
+) -> None:
+
     print("")
     print("-" * 80)
     print("Domain: {0}, host: {1}".format(domain, host))
 
     timout = 30  # seconds
     try:
         w = whois.query(
             domain,
-            host,
+            server=host,
             ignore_returncode=True,
             verbose=False,
             internationalized=True,
             include_raw_whois_text=False,
             timeout=timout,
         )
         if w:
@@ -103,26 +115,31 @@
         else:
             print("None")
             print("\n", whois.get_last_raw_whois_data())
     except Exception as e:
         print(e)
 
 
-def parse(data):
-    if "," in data:
-        data = data.split(",")
-        if len(data) == 1:
-            query(data[0])
-        elif len(data) == 2:
-            query(data[0], data[1])
-    else:
+def parse(data: str) -> None:
+    if "," not in data:
         query(data)
+        return
+
+    dList: List[str] = data.split(",")
+
+    if len(dList) == 1:
+        query(dList[0])
+        return
+
+    if len(dList) == 2:
+        query(dList[0], dList[1])
+        return
 
 
-def main():
+def main() -> None:
     if len(sys.argv) > 1:
         domains = sys.argv[1:]
     else:
         domains = DOMAINS.split("\n")
 
     for data in domains:
         if data:
```

### Comparing `whoisdomain-1.20230417.6/test2.py` & `whoisdomain-1.20230424.7/whoisdomain/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 #!/usr/bin/python3
-import whoisdomain as whois
+
 import os
 import re
 import getopt
 import sys
-from typing import Optional, List, Dict
-
-Verbose = False
-PrintGetRawWhoisResult = False
-Ruleset = False
+from typing import (
+    Optional,
+    Tuple,
+    Any,
+    List,
+    Dict,
+)
+
+import whoisdomain as whois  # to be compatible with dannycork
+
+
+Verbose: bool = False
+PrintGetRawWhoisResult: bool = False
+Ruleset: bool = False
 
-Failures = {}
-IgnoreReturncode = False
+Failures: Dict[str, Any] = {}
+IgnoreReturncode: bool = False
 
 
 class ResponseCleaner:
-    data: Optional[str] = None
-    rDict: Dict = {}
+    data: str
+    rDict: Dict[str, Any] = {}
 
-    def __init__(self, pathToTestFile: str):
+    def __init__(
+        self,
+        pathToTestFile: str,
+    ):
         self.data = self.readInputFile(pathToTestFile)
 
-    def readInputFile(self, pathToTestFile: str):
+    def readInputFile(
+        self,
+        pathToTestFile: str,
+    ) -> str:
         if not os.path.exists(pathToTestFile):
-            return None
+            return ""
 
         with open(pathToTestFile, mode="rb") as f:  # switch to binary mode as that is what Popen uses
             # make sure the data is treated exactly the same as the output of Popen
             return f.read().decode(errors="ignore")
 
-    def cleanSection(self, section: List) -> List:
+    def cleanSection(
+        self,
+        section: List[str],
+    ) -> List[str]:
         # cleanup any beginning and ending empty lines from the section
 
         if len(section) == 0:
             return section
 
         rr = r"^\s*$"
         n = 0  # remove empty lines from the start of section
@@ -44,64 +62,67 @@
         n = len(section) - 1  # remove empty lines from the end of the section
         while re.match(rr, section[n]):
             section.pop(n)
             n = len(section) - 1  # remove empty lines from the end of section
 
         return section
 
-    def splitBodyInSections(self, body: List) -> List:
+    def splitBodyInSections(
+        self,
+        body: List[str],
+    ) -> List[str]:
         # split the body on empty line, cleanup all sections, remove empty sections
         # return list of body's
 
-        sections = []
+        sections: List[List[str]] = []
         n = 0
         sections.append([])
         for line in body:
             if re.match(r"^\s*$", line):
                 n += 1
                 sections.append([])
                 continue
             sections[n].append(line)
 
         m = 0
         while m < len(sections):
             sections[m] = self.cleanSection(sections[m])
             m += 1
 
-        # now remove ampty sections and return
-        sections2 = []
+        # now remove empty sections and return
+        sections2: List[str] = []
         m = 0
         while m < len(sections):
             if len(sections[m]) > 0:
                 sections2.append("\n".join(sections[m]))
             m += 1
 
         return sections2
 
     def cleanupWhoisResponse(
         self,
         verbose: bool = False,
         with_cleanup_results: bool = False,
-    ):
-        result = whois._2_parse.cleanupWhoisResponse(
+    ) -> Tuple[str, Dict[Any, Any]]:
+        result = whois.cleanupWhoisResponse(
             self.data,
-            verbose=False,
-            with_cleanup_results=False,
+            verbose,
+            with_cleanup_results,
         )
 
-        self.rDict = {
+        self.rDict: Dict[str, Any] = {
             "BodyHasSections": False,  # if this is true the body is not a list of lines but a list of sections with lines
             "Preamble": [],  # the lines telling what whois servers wwere contacted
             "Percent": [],  # lines staring with %% , often not present but may contain hints
             "Body": [],  # the body of the whois, may be in sections separated by empty lines
             "Postamble": [],  # copyright and other not relevant info for actual parsing whois
         }
-        body = []
+        body: List[str] = []
 
-        rr = []
+        rr: List[str] = []
         z = result.split("\n")
         preambleSeen = False
         postambleSeen = False
         percentSeen = False
         for line in z:
             if preambleSeen is False:
                 if line.startswith("["):
@@ -138,15 +159,15 @@
 
             rr.append(line)
 
         body = self.cleanSection(body)
         self.rDict["Body"] = self.splitBodyInSections(body)
         return "\n".join(rr), self.rDict
 
-    def printMe(self):
+    def printMe(self) -> None:
         zz = ["Preamble", "Percent", "Postamble"]
         for k in zz:
             n = 0
             for lines in self.rDict[k]:
                 tab = " [TAB] " if "\t" in lines else ""  # tabs are present in this section
                 cr = " [CR] " if "\r" in lines else ""  # \r is present in this section
                 print(k, cr, tab, lines)
@@ -159,25 +180,28 @@
                 tab = " [TAB] " if "\t" in lines else ""  # tabs are present in this section
                 cr = " [CR] " if "\r" in lines else ""  # \r is present in this section
                 print(f"# --- {k} Section: {n} {cr}{tab}{ws}")
                 n += 1
                 print(lines)
 
 
-def prepItem(d):
+def prepItem(d: str) -> None:
     print("")
     print(f"test domain: <<<<<<<<<< {d} >>>>>>>>>>>>>>>>>>>>")
 
 
-def xType(x):
+def xType(x: Any) -> str:
     s = f"{type(x)}"
     return s.split("'")[1]
 
 
-def testItem(d: str, printgetRawWhoisResult: bool = False):
+def testItem(
+    d: str,
+    printgetRawWhoisResult: bool = False,
+) -> None:
     global PrintGetRawWhoisResult
 
     timout = 30  # seconds
 
     w = whois.query(
         d,
         ignore_returncode=IgnoreReturncode,
@@ -204,27 +228,27 @@
     for k, v in wd.items():
         ss = "%-18s %-17s "
         if isinstance(v, str):
             print((ss + "'%s'") % (k, xType(v), v))
         else:
             print((ss + "%s") % (k, xType(v), v))
 
-    print("\n", whois.get_last_raw_whois_data())
+    # print("\n", whois.get_last_raw_whois_data())
 
 
-def errorItem(d, e, what="Generic"):
+def errorItem(d: str, e: Any, what: str = "Generic") -> None:
     if what not in Failures:
         Failures[what] = {}
     Failures[what][d] = e
 
     message = f"Domain: {d}; Exception: {what}; Error: {e}"
     print(message)
 
 
-def testDomains(aList):
+def testDomains(aList: List[str]) -> None:
     for d in aList:
 
         # skip empty lines
         if not d:
             continue
 
         if len(d.strip()) == 0:
@@ -255,15 +279,15 @@
             errorItem(d, e, what="WhoisPrivateRegistry")
         except whois.WhoisCommandTimeout as e:
             errorItem(d, e, what="WhoisCommandTimeout")
         # except Exception as e:
         #    errorItem(d, e, what="Generic")
 
 
-def getTestFileOne(fPath, fileData):
+def getTestFileOne(fPath: str, fileData: Dict[str, Any]) -> None:
     if not os.path.isfile(fPath):  # only files
         return
 
     if not fPath.endswith(".txt"):  # ending in .txt
         return
 
     bName = fPath[:-4]
@@ -279,57 +303,65 @@
             aa = re.split(r"\s+", line)
             if aa[0] not in xx:
                 xx.append(aa[0])
 
     return
 
 
-def getTestFilesAll(tDir, fileData):
+def getTestFilesAll(
+    tDir: str,
+    fileData: Dict[str, Any],
+) -> None:
     for item in os.listdir(tDir):
         fPath = f"{tDir}/{item}"
         getTestFileOne(fPath, fileData)
 
 
-def getAllCurrentTld():
+def getAllCurrentTld() -> List[str]:
     return whois.validTlds()
 
 
-def makeMetaAllCurrentTld(allHaving=None, allRegex=None):
-    rr = []
+def makeMetaAllCurrentTld(
+    allHaving: Optional[str] = None,
+    allRegex: Optional[str] = None,
+) -> List[str]:
+    rr: List[str] = []
     for tld in getAllCurrentTld():
         if allRegex:
             if re.search(allRegex, tld):
                 rr.append(f"meta.{tld}")
         else:
             rr.append(f"meta.{tld}")
 
     return rr
 
 
-def showAllCurrentTld():
+def showAllCurrentTld() -> None:
     print("Tld's currently supported")
     for tld in getAllCurrentTld():
         print(tld)
 
 
-def ShowRuleset(tld):
+def ShowRuleset(tld: str) -> None:
     rr = whois.TLD_RE
     if tld in rr:
         for key in sorted(rr[tld].keys()):
             rule = f"{rr[tld][key]}"
             if "re.compile" in rule:
                 rule = rule.split("re.compile(")[1]
                 rule = rule.split(", re.IGNORECASE)")[0]
             print(key, rule, "IGNORECASE")
 
 
-def usage():
+def usage() -> None:
+    name = os.path.basename(sys.argv[0])
+
     print(
-        """
-test.py
+        f"""
+{name}
     [ -v | --verbose ]
         # set verbose to True, this will be forwarded to whois.query
 
     [ -I | --IgnoreReturncode ]
         # sets the IgnoreReturncode to True, this will be forwarded to whois.query
 
     [ -a | --all]
@@ -357,59 +389,61 @@
 
     [ -S | --SupportedTld ]
     print all supported top level domains we know and exit
 
     [ -C <file> | --Cleanup <file> ]
     read the input file specified and run the same cleanup as in whois.query , then exit
 
-    # options are exclusive and without any options the test2 program does nothing
+    # options are exclusive and without any options the {name} program does nothing
 
     # test one specific file with verbose and IgnoreReturncode
-    example: ./test2.py -v -I -f tests/ok-domains.txt 2>2 >out
+    example: {name} -v -I -f tests/ok-domains.txt 2>2 >out
 
     # test one specific directory with verbose and IgnoreReturncode
-    example: ./test2.py -v -I -D tests 2>2 >out
+    example: {name} -v -I -D tests 2>2 >out
 
     # test two domains with verbose and IgnoreReturncode
-    example: ./test2.py -v -I -d meta.org -d meta.com 2>2 >out
+    example: {name} -v -I -d meta.org -d meta.com 2>2 >out
 
     # test all supported tld's with verbose and IgnoreReturncode
-    example: ./test2.py -v -I -a 2>2 >out
+    example: {name} -v -I -a 2>2 >out
 
     # test nothing
-    example: ./test2.py -v -I 2>2 >out
+    example: {name} -v -I 2>2 >out
 """
     )
 
     """
     TODO
     --all --reg <re>
         from all tld a regex match sub selection
 
     --all --having <name>
         from all but only the ones haveing a certain field
     """
+    sys.exit(1)
 
 
-def showFailures():
+def showFailures() -> None:
     if len(Failures):
         print("\n# ========================")
         for i in sorted(Failures.keys()):
             for j in sorted(Failures[i].keys()):
                 print(i, j, Failures[i][j])
 
 
-def main(argv):
+def main() -> None:
     global Verbose
     global IgnoreReturncode
     global PrintGetRawWhoisResult
     global Ruleset
+
     try:
         opts, args = getopt.getopt(
-            argv,
+            sys.argv[1:],
             "RSpvIhaf:d:D:r:H:C:",
             [
                 "Ruleset",
                 "SupportedTld",
                 "print",
                 "verbose",
                 "IgnoreReturncode",
@@ -422,28 +456,29 @@
                 "Cleanup=",
             ],
         )
     except getopt.GetoptError:
         usage()
         sys.exit(2)
 
-    testAllTld = False
-    allHaving = None  # from all supported tld only process the ones having this :: TODO ::
-    allRegex = None  # from all supported tld process only the ones matching this regex
+    testAllTld: bool = False
+
+    allHaving: Optional[str] = None  # from all supported tld only process the ones having this :: TODO ::
+    allRegex: Optional[str] = None  # from all supported tld process only the ones matching this regex
 
-    directory = None
-    dirs = []
+    directory: Optional[str] = None
+    dirs: List[str] = []
 
-    filename = None
-    files = []
+    filename: Optional[str] = None
+    files: List[str] = []
 
-    domain = None
-    domains = []
+    domain: Optional[str] = None
+    domains: List[str] = []
 
-    fileData = {}
+    fileData: Dict[str, Any] = {}
 
     for opt, arg in opts:
         if opt in ("-S", "SupportedTld"):
             for tld in sorted(whois.validTlds()):
                 print(tld)
             sys.exit(0)
 
@@ -452,19 +487,19 @@
             sys.exit(0)
 
         if opt in ("-a", "--all"):
             testAllTld = True
 
         if opt in ("-H", "--having"):
             testAllTld = True
-            allHaving = arg
+            allHaving = str(arg)
 
         if opt in ("-r", "--reg"):
             testAllTld = True
-            allRegex = arg
+            allRegex = str(arg)
 
         if opt in ("-v", "--verbose"):
             Verbose = True
 
         if opt in ("-p", "--print"):
             PrintGetRawWhoisResult = True
 
@@ -541,10 +576,13 @@
         return
 
     if len(domains):
         testDomains(domains)
         showFailures()
         return
 
+    usage()
+    sys.exit(0)
+
 
 if __name__ == "__main__":
-    main(sys.argv[1:])
+    main()
```

### Comparing `whoisdomain-1.20230417.6/test_adjust.py` & `whoisdomain-1.20230424.7/test_adjust.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # from https://github.com/maarten-boot/python-whois-extended
 
 from whoisdomain._3_adjust import str_to_date
 
-TEST_DATETIMES = [
+from typing import (
+    List,
+)
+
+TEST_DATETIMES: List[str] = [
     "02-jan-2000",
     "02.02.2000",
     "01/06/2011",
     "2000-01-02",
     "2000.01.02",
     "2005/05/30",
     "31-01-2000",
```

### Comparing `whoisdomain-1.20230417.6/.github/ISSUE_TEMPLATE/bug_report.md` & `whoisdomain-1.20230424.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.github/workflows/lint.yml` & `whoisdomain-1.20230424.7/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ast.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_ast.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1,
         1,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_codecs.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_codecs.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         4,
         1,
         2,
         3,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_collections_abc.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         32,
         1,
         1
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_ctypes.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1,
         1,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/abc.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/abc.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         1
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/array.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/array.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/array.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         1,
         2,
         6,
         7,
         1,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/builtins.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/builtins.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         30,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/codecs.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/codecs.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/contextlib.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/contextlib.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9555555555555555%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(7, 1)]}',*

 * * "'dep_prios'": '{insert: [(8, 30)]}',*

 * * "'dependencies'": "{insert: [(8, 'os')]}"}*

```diff
@@ -1,38 +1,41 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         5,
         1,
         2,
         3,
         6,
         7,
         8,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
         5,
         5,
         5,
         5,
-        5
+        5,
+        30
     ],
     "dependencies": [
         "collections.abc",
         "abc",
         "sys",
         "_typeshed",
         "types",
         "typing",
         "typing_extensions",
-        "builtins"
+        "builtins",
+        "os"
     ],
     "hash": "48bd9c84f4093e39fcb915605fadeae2429be6aabd9f355f9f72a7690dc6ac5f",
     "id": "contextlib",
     "ignore_all": true,
     "interface_hash": "5904cd9eeb9e37e86b43a16512510d8944642aa6774cf55c704437c00acf1d19",
     "mtime": 1676537402,
     "options": {
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/datetime.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/datetime.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         4,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/enum.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/time.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7451851851851852%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(4, 1), (5, 1)], delete: [7, 6, 5, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 30)], delete: [3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(4, 'builtins'), (5, 'abc')], delete: [5, 4, 2, 0]}",*

 * * "'hash'": "'81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c'",*

 * * "'id'": "'time'",*

 * * "'interface_hash'": "'8f314672fcd922b28b1bc01618687a8a9a53433a789975e9a709b70754450e13'",*

 * * "'path'": "'/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdli […]*

```diff
@@ -1,43 +1,37 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        6,
         1,
         2,
         3,
         4,
-        5,
-        7,
-        8
+        1,
+        1
     ],
     "dep_prios": [
-        5,
-        10,
         10,
         5,
         5,
         5,
         5,
-        5
+        30
     ],
     "dependencies": [
-        "collections.abc",
         "sys",
-        "types",
         "_typeshed",
-        "abc",
-        "builtins",
         "typing",
-        "typing_extensions"
+        "typing_extensions",
+        "builtins",
+        "abc"
     ],
-    "hash": "012147e3892b3d2a985d59171ced67c9aa50834e050353d05cb50cb5398e21b4",
-    "id": "enum",
+    "hash": "81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c",
+    "id": "time",
     "ignore_all": true,
-    "interface_hash": "6acc9fc71d4c9b74c61f9301011d214540213cd05eece97a86738b3d1117b220",
+    "interface_hash": "8f314672fcd922b28b1bc01618687a8a9a53433a789975e9a709b70754450e13",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/enum.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/time.pyi",
     "plugin_data": null,
-    "size": 9967,
+    "size": 3663,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/functools.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/functools.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         4,
         1,
         2,
         3,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/genericpath.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/genericpath.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         1,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/io.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/io.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/io.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         6,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/mmap.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/mmap.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         1,
         2,
         4,
         1,
         1,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/pathlib.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/pathlib.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         13,
         1,
         2,
         14,
         15,
         16,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/pickle.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/pickle.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         1,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/platform.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/platform.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         7,
         1,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/posixpath.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/posixpath.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         1,
         2,
         4,
         17,
         18,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/re.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/re.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/re.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_compile.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7533862433862434%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(2, 6), (3, 1), (4, 3)], delete: [2, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'json.decoder'), (2, 'json.encoder'), "*

 * *                   "(3, '_typeshed')], delete: [2, 1, 0]}",*

 * * "'hash'": "'21bfc4eb15392a97e3f1ffeedd337250fab823a7246015f7df42bbbd4c83b857'",*

 * * "'id'": "'json'",*

 * * "'interface_hash'": "'4d910c236b229d2f343691d41ead3d38e59860e305dd876b3443a059dd068233'",*

 * * "'path'": "'/home/mboot […]*

```diff
@@ -1,37 +1,40 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        1,
         2,
-        4,
         5,
+        6,
+        1,
+        3,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
         5,
+        5,
         30
     ],
     "dependencies": [
-        "re",
-        "sre_constants",
-        "sre_parse",
+        "collections.abc",
+        "json.decoder",
+        "json.encoder",
+        "_typeshed",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "85fe24613b085071a9adfaf390f97bc0722f7ebbb3b5340aee953a407227fdc1",
-    "id": "sre_compile",
+    "hash": "21bfc4eb15392a97e3f1ffeedd337250fab823a7246015f7df42bbbd4c83b857",
+    "id": "json",
     "ignore_all": true,
-    "interface_hash": "f5cb748b952e0951f4e11375600d673b6e8a5f5b1c48d4c8f4496e4511e77868",
+    "interface_hash": "4d910c236b229d2f343691d41ead3d38e59860e305dd876b3443a059dd068233",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/sre_compile.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/__init__.pyi",
     "plugin_data": null,
-    "size": 334,
+    "size": 2027,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_constants.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sre_parse.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         2,
         1,
         3,
         4,
         6,
         7,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/subprocess.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/subprocess.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         6,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/sys.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/sys.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         4,
         5,
         6,
         2,
         3,
         7,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/time.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/time.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7642195767195769%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(4, 5)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'email.message'), (2, 'email.policy')], "*

 * *                   'delete: [1, 0]}',*

 * * "'hash'": "'aae29f136172d174302dc0bad01acd580565bef9a3ab693c168dd7077b8fda50'",*

 * * "'id'": "'email'",*

 * * "'interface_hash'": "'59f9835c8adba5ca5031ddda2e09379f83f5169356cac061657b877e49e4d77d'",*

 * * "'path'": "'/home/mboot/.local/lib/python3.11/site-pa […]*

```diff
@@ -1,37 +1,40 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         4,
+        5,
         1,
         1
     ],
     "dep_prios": [
-        10,
+        5,
+        5,
         5,
         5,
         5,
         5,
         30
     ],
     "dependencies": [
-        "sys",
-        "_typeshed",
+        "collections.abc",
+        "email.message",
+        "email.policy",
         "typing",
         "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c",
-    "id": "time",
+    "hash": "aae29f136172d174302dc0bad01acd580565bef9a3ab693c168dd7077b8fda50",
+    "id": "email",
     "ignore_all": true,
-    "interface_hash": "8f314672fcd922b28b1bc01618687a8a9a53433a789975e9a709b70754450e13",
+    "interface_hash": "59f9835c8adba5ca5031ddda2e09379f83f5169356cac061657b877e49e4d77d",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/time.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/__init__.pyi",
     "plugin_data": null,
-    "size": 3663,
+    "size": 1072,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/types.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/types.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/types.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         3,
         16,
         1,
         2,
         19,
         20,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/typing.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         4,
         6,
         7,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/typing_extensions.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         8,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         10,
         5,
         6,
         7,
         8,
         9,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         11,
         1,
         2,
         3,
         4,
         5,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/collections/abc.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/ctypes/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/header.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7642857142857143%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{delete: [4, 3]}',*

 * * "'dep_prios'": '{delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'email.charset')], delete: [4, 2, 1]}",*

 * * "'hash'": "'f8a86ce2f4b66156b42de2e2042ab58e8264e485e9dc898037a67dc25e80fdf2'",*

 * * "'id'": "'email.header'",*

 * * "'interface_hash'": "'43fb7098b706264f68a3d337bf5e9b0a512c683b5f68f525b5aea9dd7dcf9f28'",*

 * * "'path'": "'/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/header.pyi'",*

 * * "'size'": '1241'}*

```diff
@@ -1,40 +1,34 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
-        4,
-        5,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
-        5,
-        5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "email.message",
-        "email.policy",
+        "email.charset",
         "typing",
-        "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "aae29f136172d174302dc0bad01acd580565bef9a3ab693c168dd7077b8fda50",
-    "id": "email",
+    "hash": "f8a86ce2f4b66156b42de2e2042ab58e8264e485e9dc898037a67dc25e80fdf2",
+    "id": "email.header",
     "ignore_all": true,
-    "interface_hash": "59f9835c8adba5ca5031ddda2e09379f83f5169356cac061657b877e49e4d77d",
+    "interface_hash": "43fb7098b706264f68a3d337bf5e9b0a512c683b5f68f525b5aea9dd7dcf9f28",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -69,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/__init__.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/header.pyi",
     "plugin_data": null,
-    "size": 1072,
+    "size": 1241,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/charset.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/charset.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/contentmanager.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/errors.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/errors.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         1,
         1,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/header.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/policy.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7396296296296296%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(2, 4), (3, 5), (4, 6), (6, 7)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (5, 5), (6, 5), (7, 5)], delete: [4]}',*

 * * "'dependencies'": "{insert: [(1, 'email.contentmanager'), (2, 'email.errors'), (3, "*

 * *                   "'email.header'), (4, 'email.message'), (5, 'abc')], delete: [4, 1]}",*

 * * "'hash'": "'2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4'",*

 * * "'id'": "'email.policy'",*

 * * "'interface_hash'": "'e0627a60d9b3d36960637ed6 […]*

```diff
@@ -1,34 +1,43 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        1,
         2,
         3,
+        4,
+        5,
+        6,
         1,
+        7,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
-        30
+        5,
+        5,
+        5,
+        5
     ],
     "dependencies": [
         "collections.abc",
-        "email.charset",
+        "email.contentmanager",
+        "email.errors",
+        "email.header",
+        "email.message",
+        "abc",
         "typing",
-        "builtins",
-        "abc"
+        "builtins"
     ],
-    "hash": "f8a86ce2f4b66156b42de2e2042ab58e8264e485e9dc898037a67dc25e80fdf2",
-    "id": "email.header",
+    "hash": "2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4",
+    "id": "email.policy",
     "ignore_all": true,
-    "interface_hash": "43fb7098b706264f68a3d337bf5e9b0a512c683b5f68f525b5aea9dd7dcf9f28",
+    "interface_hash": "e0627a60d9b3d36960637ed6b25f3ecef2265f8960c851a02dfbca8db480c91f",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -63,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/header.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/policy.pyi",
     "plugin_data": null,
-    "size": 1241,
+    "size": 3055,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/message.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/message.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         2,
         4,
         5,
         6,
         7,
         1,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/email/policy.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7333333333333333%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(0, 1)], delete: [6, 4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(3, 30)], delete: [4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(3, 'abc')], delete: [5, 4, 3, 2, 1]}",*

 * * "'hash'": "'2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4'",*

 * * "'id'": "'importlib.metadata._meta'",*

 * * "'interface_hash'": "'ba005138f7d1703847dedb1d03c29fae0a8fe68641be3ed97fea905acbac5c23'",*

 * * "'path'": "'/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshe […]*

```diff
@@ -1,43 +1,31 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
+        1,
         2,
-        3,
-        4,
-        5,
-        6,
         1,
-        7,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
-        5
+        30
     ],
     "dependencies": [
         "collections.abc",
-        "email.contentmanager",
-        "email.errors",
-        "email.header",
-        "email.message",
-        "abc",
         "typing",
-        "builtins"
+        "builtins",
+        "abc"
     ],
-    "hash": "2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4",
-    "id": "email.policy",
+    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
+    "id": "importlib.metadata._meta",
     "ignore_all": true,
-    "interface_hash": "e0627a60d9b3d36960637ed6b25f3ecef2265f8960c851a02dfbca8db480c91f",
+    "interface_hash": "ba005138f7d1703847dedb1d03c29fae0a8fe68641be3ed97fea905acbac5c23",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/email/policy.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
     "plugin_data": null,
-    "size": 3055,
+    "size": 842,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1,
         1
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/abc.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9380952380952381%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{delete: [12, 11, 10, 9]}',*

 * * "'dep_prios'": '{delete: [13, 12, 11, 10]}',*

 * * "'dependencies'": '{delete: [13, 12, 11, 10]}'}*

```diff
@@ -1,56 +1,44 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         12,
         13,
         1,
         2,
         3,
         11,
         14,
         15,
         16,
-        1,
-        1,
-        1,
-        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         10,
         10,
         5,
         5,
         5,
         5,
         5,
-        5,
-        30,
-        30,
-        30,
-        30
+        5
     ],
     "dependencies": [
         "collections.abc",
         "importlib.machinery",
         "sys",
         "types",
         "_typeshed",
         "abc",
         "io",
         "typing",
         "typing_extensions",
-        "builtins",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "builtins"
     ],
     "hash": "87680a412f998efe52f43ade822202ee5e74147f77ca226f755058dd85c129c2",
     "id": "importlib.abc",
     "ignore_all": true,
     "interface_hash": "3200c4ec551447a142ba9991d9aa5ff6d62347cc096cccab4e2c75a8331190e1",
     "mtime": 1676537402,
     "options": {
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/machinery.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7371212121212121%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(0, 23), (1, 30), (4, 21), (5, 22), (6, 24), (7, 25), (8, 26), (9, 27), '*

 * *                '(10, 28), (11, 33)], delete: [9, 8, 7, 6, 5, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(6, 5), (7, 5), (8, 5), (9, 5), (10, 5), (11, 5)], delete: [9, 3, 1, '*

 * *                '0]}',*

 * * "'dependencies'": "{insert: [(1, 'os.path'), (5, 'builtins'), (6, 'contextlib'), (7, 'io'), (8, "*

 * *                   "'subprocess'), (9, 'typing'), (10, 'typing_extensions'), (11, 'typ […]*

```diff
@@ -1,61 +1,67 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        1,
-        5,
-        9,
+        23,
+        30,
         1,
         2,
-        3,
-        4,
-        6,
-        1,
-        1,
+        21,
+        22,
+        24,
+        25,
+        26,
+        27,
+        28,
+        33,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
         5,
-        20,
         10,
         10,
         5,
         5,
         5,
-        30,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "importlib.abc",
         "collections.abc",
-        "importlib.metadata",
-        "importlib",
+        "os.path",
         "sys",
-        "types",
         "_typeshed",
-        "typing",
-        "builtins",
         "abc",
+        "builtins",
+        "contextlib",
+        "io",
+        "subprocess",
+        "typing",
+        "typing_extensions",
+        "types",
         "array",
         "ctypes",
         "mmap",
         "pickle"
     ],
-    "hash": "a601f02927fc655baeb22d9e11677857e6141618829ae1fab8cb90d78757326b",
-    "id": "importlib.machinery",
+    "hash": "8fd495b40c54c92e0ac8e555ba1f72b83260e8dcc4a2ff328cd47dc0563c0ca9",
+    "id": "os",
     "ignore_all": true,
-    "interface_hash": "71603eaeca07ac4aa59c442977cddd0deb1b5b2e435d383e1a1bff9abca71326",
+    "interface_hash": "2a240d1e6e2e82440be18a4d12c71f3f0287ca634821a5ee11affc0a8a09ebef",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -90,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
     "plugin_data": null,
-    "size": 5603,
+    "size": 36795,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         30,
         5,
         6,
         7,
         1,
         2,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7285714285714285%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 5), (2, 9), (5, 3), (6, 4), (7, 6), (8, 1), (9, 1), (10, '*

 * *                '1), (11, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 5), (2, 5), (3, 20), (4, 10), (5, 10), (9, 30), (10, 30), '*

 * *                '(11, 30), (12, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'importlib.abc'), (2, 'importlib.metadata'), (3, 'importlib'), "*

 * *                   "(4, 'sys'), (5, 'types'), (6, '_typeshed'), (10, 'array'), (11, 'ctypes'), "*

 * *               […]*

```diff
@@ -1,31 +1,61 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
+        5,
+        9,
+        1,
         2,
+        3,
+        4,
+        6,
+        1,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
+        5,
+        20,
+        10,
+        10,
         5,
         5,
         5,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
+        "importlib.abc",
         "collections.abc",
+        "importlib.metadata",
+        "importlib",
+        "sys",
+        "types",
+        "_typeshed",
         "typing",
         "builtins",
-        "abc"
+        "abc",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
-    "id": "importlib.metadata._meta",
+    "hash": "a601f02927fc655baeb22d9e11677857e6141618829ae1fab8cb90d78757326b",
+    "id": "importlib.machinery",
     "ignore_all": true,
-    "interface_hash": "ba005138f7d1703847dedb1d03c29fae0a8fe68641be3ed97fea905acbac5c23",
+    "interface_hash": "71603eaeca07ac4aa59c442977cddd0deb1b5b2e435d383e1a1bff9abca71326",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -60,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi",
     "plugin_data": null,
-    "size": 842,
+    "size": 5603,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7505952380952381%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(1, 2)], delete: [4, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [2, 1, 0]}',*

 * * "'dependencies'": '{delete: [3, 2, 1]}',*

 * * "'hash'": "'94d69bd74fbb9158ed4d0253c7134792103ba5d53da327b8fda39343b4082490'",*

 * * "'id'": "'json.decoder'",*

 * * "'interface_hash'": "'0d9d1e2e302db4d060f5434b6cca8ed925ac4380822e8f2600badc3a5e79d2c4'",*

 * * "'path'": "'/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/decoder.pyi'",*

 * * "'size'": '1113'}*

```diff
@@ -1,40 +1,31 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        2,
-        5,
-        6,
         1,
-        3,
+        2,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        5,
-        5,
-        5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "json.decoder",
-        "json.encoder",
-        "_typeshed",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "21bfc4eb15392a97e3f1ffeedd337250fab823a7246015f7df42bbbd4c83b857",
-    "id": "json",
+    "hash": "94d69bd74fbb9158ed4d0253c7134792103ba5d53da327b8fda39343b4082490",
+    "id": "json.decoder",
     "ignore_all": true,
-    "interface_hash": "4d910c236b229d2f343691d41ead3d38e59860e305dd876b3443a059dd068233",
+    "interface_hash": "0d9d1e2e302db4d060f5434b6cca8ed925ac4380822e8f2600badc3a5e79d2c4",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -69,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/__init__.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/decoder.pyi",
     "plugin_data": null,
-    "size": 2027,
+    "size": 1113,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/decoder.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/getopt.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7516666666666667%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{delete: [1]}',*

 * * "'dep_prios'": '{insert: [(1, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [1, 0]}",*

 * * "'hash'": "'55041139e9f30b9e34c79ecae62a2940dfdd0d1af8c3b8125431c124c778c172'",*

 * * "'id'": "'getopt'",*

 * * "'interface_hash'": "'a917a119b9e3f7f7e9d5c25482575952445085f04b97dd656131e8681f7e3782'",*

 * * "'path'": "'/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/getopt.pyi'",*

 * * "'size'": '442'}*

```diff
@@ -1,31 +1,28 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
-        2,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "typing",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "94d69bd74fbb9158ed4d0253c7134792103ba5d53da327b8fda39343b4082490",
-    "id": "json.decoder",
+    "hash": "55041139e9f30b9e34c79ecae62a2940dfdd0d1af8c3b8125431c124c778c172",
+    "id": "getopt",
     "ignore_all": true,
-    "interface_hash": "0d9d1e2e302db4d060f5434b6cca8ed925ac4380822e8f2600badc3a5e79d2c4",
+    "interface_hash": "a917a119b9e3f7f7e9d5c25482575952445085f04b97dd656131e8681f7e3782",
     "mtime": 1676537402,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -60,13 +57,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/json/decoder.pyi",
+    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/getopt.pyi",
     "plugin_data": null,
-    "size": 1113,
+    "size": 442,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/json/encoder.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6646919191919192%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(0, 13), (1, 15), (4, 4), (5, 1), (6, 1), (7, 1), (8, 1), (9, 1), (10, '*

 * *                '1)], delete: [11, 10, 9, 8, 7, 6, 5, 4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (6, 30), (7, 30), (8, 30), (9, 30), (10, 30)], delete: [9, 8, '*

 * *                '7, 6, 5, 4, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'whoisdomain._0_init_tld'), (1, 'whoisdomain.exceptions'), (2, "*

 * *                   "'re'), (4, 'typing'), (5, 'builtins'), (6, '_collections_abc') […]*

```diff
@@ -1,68 +1,65 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        23,
-        30,
+        13,
+        15,
         1,
         2,
-        21,
-        22,
-        24,
-        25,
-        26,
-        27,
-        28,
-        33,
+        4,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
         10,
         10,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
+        30,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "os.path",
+        "whoisdomain._0_init_tld",
+        "whoisdomain.exceptions",
+        "re",
         "sys",
+        "typing",
+        "builtins",
+        "_collections_abc",
         "_typeshed",
         "abc",
-        "builtins",
-        "contextlib",
-        "io",
-        "subprocess",
-        "typing",
-        "typing_extensions",
-        "types",
         "array",
         "ctypes",
+        "enum",
         "mmap",
-        "pickle"
+        "pickle",
+        "typing_extensions"
     ],
-    "hash": "8fd495b40c54c92e0ac8e555ba1f72b83260e8dcc4a2ff328cd47dc0563c0ca9",
-    "id": "os",
-    "ignore_all": true,
-    "interface_hash": "2a240d1e6e2e82440be18a4d12c71f3f0287ca634821a5ee11affc0a8a09ebef",
-    "mtime": 1676537402,
+    "hash": "e928486addfb59b7e60c5566d8699a5b7a2ff03a30f525e8de245b7dc25ec2f0",
+    "id": "whoisdomain._2_parse",
+    "ignore_all": false,
+    "interface_hash": "a23c60234e2359272fcd528311d9baa51dddbe67c4c7aa4fd8cb0809a8c8ac78",
+    "mtime": 1682337273,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -96,13 +93,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/mboot/.local/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
+    "path": "whoisdomain/_2_parse.py",
     "plugin_data": null,
-    "size": 36795,
+    "size": 9035,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/os/path.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/os/path.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1682344859'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         7,
         1,
         1,
         1
     ],
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_0_init_tld.data.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285230010759336%*

 * *Differences: {"'names'": "{'REG_COLLECTION_BY_KEY': {'node': {'type': {'args': {1: {'type_of_any': 2}, insert: "*

 * *            "[(0, 'builtins.str')], delete: [0]}}}}, 'TLD_RE': {'node': {'type': {'args': {1: "*

 * *            "{'.class': 'Instance', 'args': ['builtins.str', OrderedDict([('.class', 'AnyType'), "*

 * *            "('missing_import_name', None), ('source_any', None), ('type_of_any', 2)])], "*

 * *            "'type_ref': 'builtins.dict', delete: ['missing_import_name', 'source_any', "*

 * *            "'type_of_any']}}}}}, 'V […]*

```diff
@@ -31,25 +31,20 @@
                     "has_explicit_value"
                 ],
                 "fullname": "whoisdomain._0_init_tld.REG_COLLECTION_BY_KEY",
                 "name": "REG_COLLECTION_BY_KEY",
                 "type": {
                     ".class": "Instance",
                     "args": [
+                        "builtins.str",
                         {
                             ".class": "AnyType",
                             "missing_import_name": null,
                             "source_any": null,
-                            "type_of_any": 4
-                        },
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 4
+                            "type_of_any": 2
                         }
                     ],
                     "type_ref": "builtins.dict"
                 }
             }
         },
         "TLD_RE": {
@@ -64,18 +59,25 @@
                 "fullname": "whoisdomain._0_init_tld.TLD_RE",
                 "name": "TLD_RE",
                 "type": {
                     ".class": "Instance",
                     "args": [
                         "builtins.str",
                         {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 2
+                            ".class": "Instance",
+                            "args": [
+                                "builtins.str",
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
+                                }
+                            ],
+                            "type_ref": "builtins.dict"
                         }
                     ],
                     "type_ref": "builtins.dict"
                 }
             }
         },
         "UnknownTld": {
@@ -86,15 +88,14 @@
         "Verbose": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready",
-                    "is_inferred",
                     "has_explicit_value"
                 ],
                 "fullname": "whoisdomain._0_init_tld.Verbose",
                 "name": "Verbose",
                 "type": "builtins.bool"
             }
         },
@@ -203,25 +204,20 @@
                     "arg_names": [
                         "zz"
                     ],
                     "arg_types": [
                         {
                             ".class": "Instance",
                             "args": [
+                                "builtins.str",
                                 {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
+                                    "type_of_any": 2
                                 }
                             ],
                             "type_ref": "builtins.dict"
                         }
                     ],
                     "bound_args": [],
                     "def_extras": {
@@ -229,18 +225,25 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "buildRegCollection",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str",
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
+                            }
+                        ],
+                        "type_ref": "builtins.dict"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -339,18 +342,25 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "get_tld_re",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 2
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str",
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
+                            }
+                        ],
+                        "type_ref": "builtins.dict"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -361,15 +371,35 @@
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [],
                 "arg_names": [],
                 "flags": [],
                 "fullname": "whoisdomain._0_init_tld.initOnImport",
                 "name": "initOnImport",
-                "type": null
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [],
+                    "arg_names": [],
+                    "arg_types": [],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "initOnImport",
+                    "ret_type": {
+                        ".class": "NoneType"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
             }
         },
         "initOne": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
@@ -392,36 +422,28 @@
                         1
                     ],
                     "arg_names": [
                         "tld",
                         "override"
                     ],
                     "arg_types": [
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 1
-                        },
+                        "builtins.str",
                         "builtins.bool"
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "initOne",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "NoneType"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -448,25 +470,20 @@
                     "arg_names": [
                         "aDict"
                     ],
                     "arg_types": [
                         {
                             ".class": "Instance",
                             "args": [
+                                "builtins.str",
                                 {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
+                                    "type_of_any": 2
                                 }
                             ],
                             "type_ref": "builtins.dict"
                         }
                     ],
                     "bound_args": [],
                     "def_extras": {
@@ -474,18 +491,15 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "mergeExternalDictWithRegex",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "NoneType"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -506,13 +520,37 @@
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [],
                 "arg_names": [],
                 "flags": [],
                 "fullname": "whoisdomain._0_init_tld.validTlds",
                 "name": "validTlds",
-                "type": null
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [],
+                    "arg_names": [],
+                    "arg_types": [],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "validTlds",
+                    "ret_type": {
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str"
+                        ],
+                        "type_ref": "builtins.list"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
             }
         }
     },
-    "path": "whoisdomain/_0_init_tld.py"
+    "path": "/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/_0_init_tld.py"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/whoisdomain.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7187777777777777%*

 * *Differences: {"'data_mtime'": '1682326841',*

 * * "'dep_lines'": '{insert: [(1, 3), (3, 5), (4, 6), (5, 15), (6, 1), (7, 1), (8, 1), (9, 1), (10, '*

 * *                '1), (11, 1)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (5, 10), (7, 30), (8, 30), (9, 30), (10, 30), (11, '*

 * *                '30), (12, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'os'), (2, 'getopt'), (5, 'whoisdomain'), (13, 'io'), (17, "*

 * *                   "'typing_extensions'), (18, 'whoisdomain._0_init_tld'), (19, "*

 * *     […]*

```diff
@@ -1,65 +1,86 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682326841,
     "dep_lines": [
-        10,
-        11,
-        1,
         2,
+        3,
         4,
+        5,
+        6,
+        15,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        5,
+        10,
+        10,
         10,
         10,
         5,
+        10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "whoisdomain.tld_regexpr",
-        "whoisdomain.exceptions",
+        "os",
         "re",
+        "getopt",
         "sys",
         "typing",
+        "whoisdomain",
         "builtins",
         "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "enum",
+        "io",
         "mmap",
         "pickle",
-        "types"
+        "types",
+        "typing_extensions",
+        "whoisdomain._0_init_tld",
+        "whoisdomain._2_parse",
+        "whoisdomain._3_adjust",
+        "whoisdomain.exceptions"
     ],
-    "hash": "beb0fbfc8849a98adea48266a50473f40e26cc8a6038150caaefe352248dfcba",
-    "id": "whoisdomain._0_init_tld",
+    "hash": "0bb3d2f98302f655d6c88fbfe2adc9c88b676b42b74aa19a42cc54c2a8743507",
+    "id": "whoisdomain.whoisdomain",
     "ignore_all": false,
-    "interface_hash": "97f7005623fab9ee3542c1d4377173245fe43a98ebb829ffb42c271b9432eb75",
-    "mtime": 1681288053,
+    "interface_hash": "525e9962f9ada65627f296dd96e21bbde410d78d6a952e4ea264d775aa938cfa",
+    "mtime": 1682326800,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -93,13 +114,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/_0_init_tld.py",
+    "path": "whoisdomain/whoisdomain.py",
     "plugin_data": null,
-    "size": 4420,
+    "size": 16115,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_1_query.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285706350682634%*

 * *Differences: {"'names'": "{'makeWhoisCommandToRun': {'node': {'type': {'ret_type': {'.class': 'Instance', "*

 * *            "'args': ['builtins.str'], 'type_ref': 'builtins.list', delete: "*

 * *            "['missing_import_name', 'source_any', 'type_of_any']}}}}, "*

 * *            "'tryInstallMissingWhoisOnWindows': {'node': {'type': {'ret_type': {'.class': "*

 * *            "'NoneType', delete: ['missing_import_name', 'source_any', 'type_of_any']}}}}}",*

 * * "'path'": "'/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/_ […]*

```diff
@@ -542,18 +542,19 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "makeWhoisCommandToRun",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str"
+                        ],
+                        "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -685,21 +686,18 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "tryInstallMissingWhoisOnWindows",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "NoneType"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         }
     },
-    "path": "whoisdomain/_1_query.py"
+    "path": "/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/_1_query.py"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_1_query.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_0_init_tld.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7265769496204278%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(0, 10), (1, 11)], delete: [8, 7, 6, 5, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 5)], delete: [9, 4, 3, 2, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'whoisdomain.tld_regexpr'), (2, 're'), (6, '_collections_abc'), "*

 * *                   "(11, 'enum')], delete: [15, 14, 13, 6, 5, 4, 2, 1]}",*

 * * "'hash'": "'77d19b3e4069ba734dd08f8c9a2dd3b3303327635e9c9ab0566c8f2270cbadcb'",*

 * * "'id'": "'whoisdomain._0_init_tld'",*

 * * "'interface_hash'": "'afde3e7efce6a4ed7bd2b7e58c […]*

```diff
@@ -1,77 +1,65 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        7,
+        10,
+        11,
         1,
         2,
-        3,
         4,
-        5,
-        6,
-        9,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        10,
-        10,
-        10,
+        5,
         10,
         10,
         5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
         30
     ],
     "dependencies": [
+        "whoisdomain.tld_regexpr",
         "whoisdomain.exceptions",
-        "subprocess",
-        "time",
+        "re",
         "sys",
-        "os",
-        "platform",
-        "json",
         "typing",
         "builtins",
+        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
-        "io",
-        "json.decoder",
-        "json.encoder",
+        "enum",
         "mmap",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "343e77056a215375f7380992e01b3e5d349c6f7dbd38b207a3aef5e7a545a127",
-    "id": "whoisdomain._1_query",
+    "hash": "77d19b3e4069ba734dd08f8c9a2dd3b3303327635e9c9ab0566c8f2270cbadcb",
+    "id": "whoisdomain._0_init_tld",
     "ignore_all": false,
-    "interface_hash": "5d9f218e895566945384cc21d442853ccc57cc47776484c5716ecc773fe7d3f4",
-    "mtime": 1681731613,
+    "interface_hash": "afde3e7efce6a4ed7bd2b7e58c5388dc8c2b79f9bff4062b39708c8cfc89c0e3",
+    "mtime": 1682337976,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -105,13 +93,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/_1_query.py",
+    "path": "whoisdomain/_0_init_tld.py",
     "plugin_data": null,
-    "size": 5759,
+    "size": 4549,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_2_parse.data.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9263155478018302%*

 * *Differences: {"'names'": "{'NONESTRINGS': {'node': {'type': {'args': ['builtins.str']}}}, 'NoneStrings': "*

 * *            "{'node': {'type': {'ret_type': {'args': ['builtins.str']}}}}, 'NoneStringsAdd': "*

 * *            "{'node': {'type': {'ret_type': {'.class': 'NoneType', delete: ['missing_import_name', "*

 * *            "'source_any', 'type_of_any']}}}}, 'QUOTASTRINGS': {'node': {'flags': {insert: [(0, "*

 * *            "'is_ready')], delete: [0]}}}, 'QuotaStrings': {'node': {'type': {'ret_type': {'args': "*

 * *            "['builtins […]*

```diff
@@ -36,20 +36,15 @@
                     "has_explicit_value"
                 ],
                 "fullname": "whoisdomain._2_parse.NONESTRINGS",
                 "name": "NONESTRINGS",
                 "type": {
                     ".class": "Instance",
                     "args": [
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 4
-                        }
+                        "builtins.str"
                     ],
                     "type_ref": "builtins.list"
                 }
             }
         },
         "NoneStrings": {
             ".class": "SymbolTableNode",
@@ -75,20 +70,15 @@
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "NoneStrings",
                     "ret_type": {
                         ".class": "Instance",
                         "args": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 4
-                            }
+                            "builtins.str"
                         ],
                         "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
@@ -126,18 +116,15 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "NoneStringsAdd",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "NoneType"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -148,15 +135,15 @@
         },
         "QUOTASTRINGS": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_inferred",
+                    "is_ready",
                     "has_explicit_value"
                 ],
                 "fullname": "whoisdomain._2_parse.QUOTASTRINGS",
                 "name": "QUOTASTRINGS",
                 "type": {
                     ".class": "Instance",
                     "args": [
@@ -190,20 +177,15 @@
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "QuotaStrings",
                     "ret_type": {
                         ".class": "Instance",
                         "args": [
-                            {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 4
-                            }
+                            "builtins.str"
                         ],
                         "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
@@ -241,18 +223,15 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "QuotaStringsAdd",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "NoneType"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -269,15 +248,14 @@
         "Verbose": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready",
-                    "is_inferred",
                     "has_explicit_value"
                 ],
                 "fullname": "whoisdomain._2_parse.Verbose",
                 "name": "Verbose",
                 "type": "builtins.bool"
             }
         },
@@ -359,14 +337,19 @@
                     "is_ready"
                 ],
                 "fullname": "whoisdomain._2_parse.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
+        "cast": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.cast",
+            "kind": "Gdef"
+        },
         "cleanupWhoisResponse": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -493,25 +476,20 @@
                         "verbose"
                     ],
                     "arg_types": [
                         "builtins.str",
                         {
                             ".class": "Instance",
                             "args": [
+                                "builtins.str",
                                 {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
+                                    "type_of_any": 2
                                 }
                             ],
                             "type_ref": "builtins.dict"
                         },
                         "builtins.str",
                         "builtins.bool"
                     ],
@@ -521,18 +499,25 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "doExtractPattensFromWhoisString",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str",
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
+                            }
+                        ],
+                        "type_ref": "builtins.dict"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -572,25 +557,20 @@
                         "verbose"
                     ],
                     "arg_types": [
                         "builtins.str",
                         {
                             ".class": "Instance",
                             "args": [
+                                "builtins.str",
                                 {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
+                                    "type_of_any": 2
                                 }
                             ],
                             "type_ref": "builtins.dict"
                         },
                         "builtins.str",
                         "builtins.bool"
                     ],
@@ -600,18 +580,25 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "doExtractPattensIanaFromWhoisString",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str",
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
+                            }
+                        ],
+                        "type_ref": "builtins.dict"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -698,25 +685,20 @@
                         "verbose"
                     ],
                     "arg_types": [
                         "builtins.str",
                         {
                             ".class": "Instance",
                             "args": [
+                                "builtins.str",
                                 {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
+                                    "type_of_any": 2
                                 }
                             ],
                             "type_ref": "builtins.dict"
                         },
                         "builtins.str",
                         "builtins.bool"
                     ],
@@ -821,20 +803,15 @@
                             ".class": "Instance",
                             "args": [
                                 "builtins.str"
                             ],
                             "type_ref": "builtins.list"
                         },
                         "builtins.bool",
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 1
-                        }
+                        "builtins.bool"
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
@@ -904,20 +881,15 @@
                         "verbose"
                     ],
                     "arg_types": [
                         "builtins.str",
                         {
                             ".class": "Instance",
                             "args": [
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
-                                }
+                                "builtins.str"
                             ],
                             "type_ref": "builtins.list"
                         },
                         "builtins.str",
                         "builtins.bool"
                     ],
                     "bound_args": [],
@@ -926,18 +898,15 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "handleShortResponse",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "NoneType"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -948,9 +917,9 @@
         },
         "sys": {
             ".class": "SymbolTableNode",
             "cross_ref": "sys",
             "kind": "Gdef"
         }
     },
-    "path": "whoisdomain/_2_parse.py"
+    "path": "/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/_2_parse.py"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_2_parse.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7312693498452012%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(2, 2), (3, 3), (4, 6)], delete: [6, 5, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10)], delete: [8, 7, 6, 0]}',*

 * * "'dependencies'": "{insert: [(3, 'datetime')], delete: [14, 11, 6, 0]}",*

 * * "'hash'": "'36a769e4c39cdae2f7a3923ddf25f8202aca11c0860877c906241b02a5c67b4d'",*

 * * "'id'": "'whoisdomain._3_adjust'",*

 * * "'interface_hash'": "'aa54805cde802baeee9046a4853ce480b34cc99d85193f0576bcca4bcec92b5d'",*

 * * "'mtime'": '1682337299',*

 * * "'path'": "'whoisdomain/_3_ad […]*

```diff
@@ -1,68 +1,59 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        12,
-        14,
-        1,
-        2,
         4,
         1,
-        1,
-        1,
+        2,
+        3,
+        6,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
+        10,
         10,
         10,
         5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "whoisdomain._0_init_tld",
         "whoisdomain.exceptions",
         "re",
         "sys",
+        "datetime",
         "typing",
         "builtins",
-        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
-        "enum",
         "mmap",
         "pickle",
-        "types",
         "typing_extensions"
     ],
-    "hash": "45e6e9e386cc90dc0b2e1660189f63759bc2038cda06a63637d71f01d3244b0d",
-    "id": "whoisdomain._2_parse",
+    "hash": "36a769e4c39cdae2f7a3923ddf25f8202aca11c0860877c906241b02a5c67b4d",
+    "id": "whoisdomain._3_adjust",
     "ignore_all": false,
-    "interface_hash": "e49d2f96d2efa686d2ddb0dfa389f5635aadeae321b3e3ba4797cf02ef5951a7",
-    "mtime": 1681288053,
+    "interface_hash": "aa54805cde802baeee9046a4853ce480b34cc99d85193f0576bcca4bcec92b5d",
+    "mtime": 1682337299,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -96,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/_2_parse.py",
+    "path": "whoisdomain/_3_adjust.py",
     "plugin_data": null,
-    "size": 8571,
+    "size": 8544,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/_3_adjust.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714274836396%*

 * *Differences: {"'names'": "{'Domain': {'node': {'names': {'name_servers': {'node': {'type': {'args': "*

 * *            "['builtins.str']}}}, 'statuses': {'node': {'type': {'args': ['builtins.str']}}}}}}}",*

 * * "'path'": "'/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/_3_adjust.py'"}*

```diff
@@ -390,20 +390,15 @@
                                 "has_explicit_value"
                             ],
                             "fullname": "whoisdomain._3_adjust.Domain.name_servers",
                             "name": "name_servers",
                             "type": {
                                 ".class": "Instance",
                                 "args": [
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 4
-                                    }
+                                    "builtins.str"
                                 ],
                                 "type_ref": "builtins.list"
                             }
                         }
                     },
                     "owner": {
                         ".class": "SymbolTableNode",
@@ -574,20 +569,15 @@
                                 "has_explicit_value"
                             ],
                             "fullname": "whoisdomain._3_adjust.Domain.statuses",
                             "name": "statuses",
                             "type": {
                                 ".class": "Instance",
                                 "args": [
-                                    {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 4
-                                    }
+                                    "builtins.str"
                                 ],
                                 "type_ref": "builtins.list"
                             }
                         }
                     },
                     "text": {
                         ".class": "SymbolTableNode",
@@ -820,9 +810,9 @@
         },
         "sys": {
             ".class": "SymbolTableNode",
             "cross_ref": "sys",
             "kind": "Gdef"
         }
     },
-    "path": "whoisdomain/_3_adjust.py"
+    "path": "/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/_3_adjust.py"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/_3_adjust.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/main.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7168803418803419%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(1, 4), (2, 5), (4, 7), (5, 15), (6, 1), (7, 1), (8, 1), (9, 1), (10, '*

 * *                '1), (11, 1), (12, 1)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (5, 10), (7, 30), (8, 30), (9, 30), (10, 30), (11, 30), (12, '*

 * *                '30), (13, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'os'), (2, 'getopt'), (5, 'whoisdomain'), (7, "*

 * *                   "'_collections_abc'), (13, 'genericpath'), (14, 'io'), (17, 'posixpath'), […]*

```diff
@@ -1,65 +1,89 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        4,
-        1,
-        2,
         3,
+        4,
+        5,
         6,
+        7,
+        15,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
+        10,
         10,
         10,
         10,
         5,
+        10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "whoisdomain.exceptions",
+        "os",
         "re",
+        "getopt",
         "sys",
-        "datetime",
         "typing",
+        "whoisdomain",
         "builtins",
+        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "enum",
+        "genericpath",
+        "io",
         "mmap",
         "pickle",
-        "types",
-        "typing_extensions"
+        "posixpath",
+        "typing_extensions",
+        "whoisdomain._0_init_tld",
+        "whoisdomain._2_parse",
+        "whoisdomain._3_adjust",
+        "whoisdomain.exceptions"
     ],
-    "hash": "aaa2898a60970d5207f0dfdb5ffb9302f197e36f8c9a3b880c1d69b08d90833f",
-    "id": "whoisdomain._3_adjust",
+    "hash": "a2dcb5528aa637a9b79ff8dbc1602b912e107a00fb1b76d8ccf3150694d3fa09",
+    "id": "whoisdomain.main",
     "ignore_all": false,
-    "interface_hash": "0b5adf5388d2b9fcf64d59ec8edd3b69ad3c421c7882289e42454c662e5d9b4d",
-    "mtime": 1681742061,
+    "interface_hash": "00fbeb10a6bef74d26f14650208a62286684c08290329ef29363c85d9a2d71b5",
+    "mtime": 1682344568,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -93,13 +117,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/_3_adjust.py",
+    "path": "whoisdomain/main.py",
     "plugin_data": null,
-    "size": 8534,
+    "size": 16746,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/__init__.data.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9019304567695723%*

 * *Differences: {"'names'": "{'FailedParsingWhoisOutput': {delete: ['module_public']}, 'LastWhois': {'node': "*

 * *            "{'type': {'args': {1: {'type_of_any': 2}, insert: [(0, 'builtins.str')], delete: "*

 * *            "[0]}}}}, 'NoneStrings': {'module_public': False}, 'NoneStringsAdd': {'module_public': "*

 * *            "False}, 'QuotaStrings': {'module_public': False}, 'QuotaStringsAdd': "*

 * *            "{'module_public': False}, 'TLD_RE': {delete: ['module_public']}, 'UnknownDateFormat': "*

 * *            "{delete: ['module_publ […]*

```diff
@@ -2,14 +2,20 @@
     ".class": "MypyFile",
     "_fullname": "whoisdomain",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
+        "Any": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Any",
+            "kind": "Gdef",
+            "module_public": false
+        },
         "CACHE_FILE": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
@@ -19,14 +25,20 @@
                 "fullname": "whoisdomain.CACHE_FILE",
                 "name": "CACHE_FILE",
                 "type": {
                     ".class": "NoneType"
                 }
             }
         },
+        "Callable": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Callable",
+            "kind": "Gdef",
+            "module_public": false
+        },
         "Dict": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.Dict",
             "kind": "Gdef",
             "module_public": false
         },
         "Domain": {
@@ -34,16 +46,15 @@
             "cross_ref": "whoisdomain._3_adjust.Domain",
             "kind": "Gdef",
             "module_public": false
         },
         "FailedParsingWhoisOutput": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.exceptions.FailedParsingWhoisOutput",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "LastWhois": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "Var",
@@ -52,25 +63,20 @@
                     "has_explicit_value"
                 ],
                 "fullname": "whoisdomain.LastWhois",
                 "name": "LastWhois",
                 "type": {
                     ".class": "Instance",
                     "args": [
+                        "builtins.str",
                         {
                             ".class": "AnyType",
                             "missing_import_name": null,
                             "source_any": null,
-                            "type_of_any": 4
-                        },
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 4
+                            "type_of_any": 2
                         }
                     ],
                     "type_ref": "builtins.dict"
                 }
             }
         },
         "List": {
@@ -78,36 +84,40 @@
             "cross_ref": "typing.List",
             "kind": "Gdef",
             "module_public": false
         },
         "NoneStrings": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain._2_parse.NoneStrings",
-            "kind": "Gdef"
+            "kind": "Gdef",
+            "module_public": false
         },
         "NoneStringsAdd": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain._2_parse.NoneStringsAdd",
-            "kind": "Gdef"
+            "kind": "Gdef",
+            "module_public": false
         },
         "Optional": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.Optional",
             "kind": "Gdef",
             "module_public": false
         },
         "QuotaStrings": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain._2_parse.QuotaStrings",
-            "kind": "Gdef"
+            "kind": "Gdef",
+            "module_public": false
         },
         "QuotaStringsAdd": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain._2_parse.QuotaStringsAdd",
-            "kind": "Gdef"
+            "kind": "Gdef",
+            "module_public": false
         },
         "SLOW_DOWN": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "Var",
@@ -120,58 +130,51 @@
                 "name": "SLOW_DOWN",
                 "type": "builtins.int"
             }
         },
         "TLD_RE": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain._0_init_tld.TLD_RE",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "Tuple": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.Tuple",
             "kind": "Gdef",
             "module_public": false
         },
         "UnknownDateFormat": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.exceptions.UnknownDateFormat",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "UnknownTld": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.exceptions.UnknownTld",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "WhoisCommandFailed": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.exceptions.WhoisCommandFailed",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "WhoisCommandTimeout": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.exceptions.WhoisCommandTimeout",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "WhoisPrivateRegistry": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.exceptions.WhoisPrivateRegistry",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "WhoisQuotaExceeded": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.exceptions.WhoisQuotaExceeded",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         },
         "ZZ": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain.tld_regexpr.ZZ",
             "kind": "Gdef",
             "module_public": false
         },
@@ -294,15 +297,15 @@
                     "args": [
                         "builtins.str"
                     ],
                     "type_ref": "builtins.list"
                 }
             }
         },
-        "doServerHintsForThisTld": {
+        "_doServerHintsForThisTld": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -314,16 +317,16 @@
                 "arg_names": [
                     "tld",
                     "thisTld",
                     "server",
                     "verbose"
                 ],
                 "flags": [],
-                "fullname": "whoisdomain.doServerHintsForThisTld",
-                "name": "doServerHintsForThisTld",
+                "fullname": "whoisdomain._doServerHintsForThisTld",
+                "name": "_doServerHintsForThisTld",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0,
                         0,
                         0,
                         1
@@ -335,25 +338,20 @@
                         "verbose"
                     ],
                     "arg_types": [
                         "builtins.str",
                         {
                             ".class": "Instance",
                             "args": [
+                                "builtins.str",
                                 {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
+                                    "type_of_any": 2
                                 }
                             ],
                             "type_ref": "builtins.dict"
                         },
                         {
                             ".class": "UnionType",
                             "items": [
@@ -369,28 +367,31 @@
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "doServerHintsForThisTld",
+                    "name": "_doServerHintsForThisTld",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "UnionType",
+                        "items": [
+                            "builtins.str",
+                            {
+                                ".class": "NoneType"
+                            }
+                        ]
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "doSlowdownHintForThisTld": {
+        "_doSlowdownHintForThisTld": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -402,16 +403,16 @@
                 "arg_names": [
                     "tld",
                     "thisTld",
                     "slow_down",
                     "verbose"
                 ],
                 "flags": [],
-                "fullname": "whoisdomain.doSlowdownHintForThisTld",
-                "name": "doSlowdownHintForThisTld",
+                "fullname": "whoisdomain._doSlowdownHintForThisTld",
+                "name": "_doSlowdownHintForThisTld",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0,
                         0,
                         0,
                         1
@@ -421,39 +422,46 @@
                         "thisTld",
                         "slow_down",
                         "verbose"
                     ],
                     "arg_types": [
                         "builtins.str",
                         {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 1
+                            ".class": "Instance",
+                            "args": [
+                                "builtins.str",
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
+                                }
+                            ],
+                            "type_ref": "builtins.dict"
                         },
                         "builtins.int",
                         "builtins.bool"
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "doSlowdownHintForThisTld",
+                    "name": "_doSlowdownHintForThisTld",
                     "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "doUnsupportedTldAnyway": {
+        "_doUnsupportedTldAnyway": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -471,16 +479,16 @@
                     "ignore_returncode",
                     "slow_down",
                     "server",
                     "verbose",
                     "wh"
                 ],
                 "flags": [],
-                "fullname": "whoisdomain.doUnsupportedTldAnyway",
-                "name": "doUnsupportedTldAnyway",
+                "fullname": "whoisdomain._doUnsupportedTldAnyway",
+                "name": "_doUnsupportedTldAnyway",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0,
                         0,
                         1,
                         1,
@@ -524,46 +532,31 @@
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "doUnsupportedTldAnyway",
+                    "name": "_doUnsupportedTldAnyway",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "UnionType",
+                        "items": [
+                            "whoisdomain._3_adjust.Domain",
+                            {
+                                ".class": "NoneType"
+                            }
+                        ]
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "do_parse": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "whoisdomain._2_parse.do_parse",
-            "kind": "Gdef",
-            "module_public": false
-        },
-        "do_query": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "whoisdomain._1_query.do_query",
-            "kind": "Gdef",
-            "module_public": false
-        },
-        "filterTldToSupportedPattern": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "whoisdomain._0_init_tld.filterTldToSupportedPattern",
-            "kind": "Gdef",
-            "module_public": false
-        },
-        "fromDomainStringToTld": {
+        "_fromDomainStringToTld": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
@@ -573,16 +566,16 @@
                 ],
                 "arg_names": [
                     "domain",
                     "internationalized",
                     "verbose"
                 ],
                 "flags": [],
-                "fullname": "whoisdomain.fromDomainStringToTld",
-                "name": "fromDomainStringToTld",
+                "fullname": "whoisdomain._fromDomainStringToTld",
+                "name": "_fromDomainStringToTld",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0,
                         0,
                         1
                     ],
@@ -600,124 +593,399 @@
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "fromDomainStringToTld",
+                    "name": "_fromDomainStringToTld",
                     "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
+                        ".class": "TupleType",
+                        "implicit": false,
+                        "items": [
+                            {
+                                ".class": "UnionType",
+                                "items": [
+                                    "builtins.str",
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
+                            },
+                            {
+                                ".class": "UnionType",
+                                "items": [
+                                    {
+                                        ".class": "Instance",
+                                        "args": [
+                                            "builtins.str"
+                                        ],
+                                        "type_ref": "builtins.list"
+                                    },
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
+                            }
+                        ],
+                        "partial_fallback": {
+                            ".class": "Instance",
+                            "args": [
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 6
+                                }
+                            ],
+                            "type_ref": "builtins.tuple"
+                        }
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "get": {
+        "_internationalizedDomainNameToPunyCode": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
-                ".class": "Var",
-                "flags": [
-                    "is_inferred",
-                    "has_explicit_value"
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0
                 ],
-                "fullname": "whoisdomain.get",
-                "name": "get",
+                "arg_names": [
+                    "d"
+                ],
+                "flags": [],
+                "fullname": "whoisdomain._internationalizedDomainNameToPunyCode",
+                "name": "_internationalizedDomainNameToPunyCode",
                 "type": {
-                    ".class": "AnyType",
-                    "missing_import_name": null,
-                    "source_any": null,
-                    "type_of_any": 1
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        "d"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "Instance",
+                            "args": [
+                                "builtins.str"
+                            ],
+                            "type_ref": "builtins.list"
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "_internationalizedDomainNameToPunyCode",
+                    "ret_type": {
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str"
+                        ],
+                        "type_ref": "builtins.list"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
                 }
             }
         },
-        "get_last_raw_whois_data": {
+        "_result2dict": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
-                "arg_kinds": [],
-                "arg_names": [],
+                "arg_kinds": [
+                    0
+                ],
+                "arg_names": [
+                    "func"
+                ],
                 "flags": [],
-                "fullname": "whoisdomain.get_last_raw_whois_data",
-                "name": "get_last_raw_whois_data",
-                "type": null
+                "fullname": "whoisdomain._result2dict",
+                "name": "_result2dict",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        "func"
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "_result2dict",
+                    "ret_type": {
+                        ".class": "AnyType",
+                        "missing_import_name": null,
+                        "source_any": null,
+                        "type_of_any": 2
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
             }
         },
-        "internationalizedDomainNameToPunyCode": {
+        "_validateWeKnowTheToplevelDomain": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_public": false,
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    1
+                ],
+                "arg_names": [
+                    "tld",
+                    "return_raw_text_for_unsupported_tld"
+                ],
+                "flags": [],
+                "fullname": "whoisdomain._validateWeKnowTheToplevelDomain",
+                "name": "_validateWeKnowTheToplevelDomain",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        1
+                    ],
+                    "arg_names": [
+                        "tld",
+                        "return_raw_text_for_unsupported_tld"
+                    ],
+                    "arg_types": [
+                        "builtins.str",
+                        "builtins.bool"
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "_validateWeKnowTheToplevelDomain",
+                    "ret_type": {
+                        ".class": "UnionType",
+                        "items": [
+                            {
+                                ".class": "Instance",
+                                "args": [
+                                    "builtins.str",
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
+                                ],
+                                "type_ref": "builtins.dict"
+                            },
+                            {
+                                ".class": "NoneType"
+                            }
+                        ]
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "_verifyPrivateREgistry": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
                     0
                 ],
                 "arg_names": [
-                    "d"
+                    "thisTld"
                 ],
                 "flags": [],
-                "fullname": "whoisdomain.internationalizedDomainNameToPunyCode",
-                "name": "internationalizedDomainNameToPunyCode",
+                "fullname": "whoisdomain._verifyPrivateREgistry",
+                "name": "_verifyPrivateREgistry",
                 "type": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0
                     ],
                     "arg_names": [
-                        "d"
+                        "thisTld"
                     ],
                     "arg_types": [
                         {
                             ".class": "Instance",
                             "args": [
-                                "builtins.str"
+                                "builtins.str",
+                                {
+                                    ".class": "AnyType",
+                                    "missing_import_name": null,
+                                    "source_any": null,
+                                    "type_of_any": 2
+                                }
                             ],
-                            "type_ref": "builtins.list"
+                            "type_ref": "builtins.dict"
                         }
                     ],
                     "bound_args": [],
                     "def_extras": {
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
-                    "name": "internationalizedDomainNameToPunyCode",
+                    "name": "_verifyPrivateREgistry",
+                    "ret_type": {
+                        ".class": "NoneType"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "cast": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.cast",
+            "kind": "Gdef",
+            "module_public": false
+        },
+        "cleanupWhoisResponse": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "whoisdomain._2_parse.cleanupWhoisResponse",
+            "kind": "Gdef"
+        },
+        "do_parse": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "whoisdomain._2_parse.do_parse",
+            "kind": "Gdef",
+            "module_public": false
+        },
+        "do_query": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "whoisdomain._1_query.do_query",
+            "kind": "Gdef",
+            "module_public": false
+        },
+        "filterTldToSupportedPattern": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "whoisdomain._0_init_tld.filterTldToSupportedPattern",
+            "kind": "Gdef",
+            "module_public": false
+        },
+        "get": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_public": false,
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "whoisdomain.get",
+                "name": "get",
+                "type": {
+                    ".class": "AnyType",
+                    "missing_import_name": null,
+                    "source_any": null,
+                    "type_of_any": 2
+                }
+            }
+        },
+        "get_last_raw_whois_data": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [],
+                "arg_names": [],
+                "flags": [],
+                "fullname": "whoisdomain.get_last_raw_whois_data",
+                "name": "get_last_raw_whois_data",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [],
+                    "arg_names": [],
+                    "arg_types": [],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "get_last_raw_whois_data",
                     "ret_type": {
                         ".class": "Instance",
                         "args": [
-                            "builtins.str"
+                            "builtins.str",
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
+                            }
                         ],
-                        "type_ref": "builtins.list"
+                        "type_ref": "builtins.dict"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "mergeExternalDictWithRegex": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain._0_init_tld.mergeExternalDictWithRegex",
-            "kind": "Gdef"
+            "kind": "Gdef",
+            "module_public": false
         },
         "query": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
                 ".class": "FuncDef",
                 "abstract_status": 0,
                 "arg_kinds": [
                     0,
                     1,
                     1,
@@ -807,20 +1075,15 @@
                                 "builtins.str",
                                 {
                                     ".class": "NoneType"
                                 }
                             ]
                         },
                         "builtins.bool",
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 1
-                        },
+                        "builtins.bool",
                         "builtins.bool",
                         "builtins.bool",
                         "builtins.bool",
                         {
                             ".class": "UnionType",
                             "items": [
                                 "builtins.float",
@@ -851,169 +1114,27 @@
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
-        "result2dict": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "module_public": false,
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0
-                ],
-                "arg_names": [
-                    "func"
-                ],
-                "flags": [],
-                "fullname": "whoisdomain.result2dict",
-                "name": "result2dict",
-                "type": null
-            }
-        },
         "sys": {
             ".class": "SymbolTableNode",
             "cross_ref": "sys",
             "kind": "Gdef",
             "module_public": false
         },
         "validTlds": {
             ".class": "SymbolTableNode",
             "cross_ref": "whoisdomain._0_init_tld.validTlds",
             "kind": "Gdef"
         },
-        "validateWeKnowTheToplevelDomain": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "module_public": false,
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    1
-                ],
-                "arg_names": [
-                    "tld",
-                    "return_raw_text_for_unsupported_tld"
-                ],
-                "flags": [],
-                "fullname": "whoisdomain.validateWeKnowTheToplevelDomain",
-                "name": "validateWeKnowTheToplevelDomain",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0,
-                        1
-                    ],
-                    "arg_names": [
-                        "tld",
-                        "return_raw_text_for_unsupported_tld"
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 1
-                        },
-                        "builtins.bool"
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "validateWeKnowTheToplevelDomain",
-                    "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
-        "verifyPrivateREgistry": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "module_public": false,
-            "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0
-                ],
-                "arg_names": [
-                    "thisTld"
-                ],
-                "flags": [],
-                "fullname": "whoisdomain.verifyPrivateREgistry",
-                "name": "verifyPrivateREgistry",
-                "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0
-                    ],
-                    "arg_names": [
-                        "thisTld"
-                    ],
-                    "arg_types": [
-                        {
-                            ".class": "Instance",
-                            "args": [
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
-                                },
-                                {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 4
-                                }
-                            ],
-                            "type_ref": "builtins.dict"
-                        }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "verifyPrivateREgistry",
-                    "ret_type": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 1
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
-                }
-            }
-        },
         "wraps": {
             ".class": "SymbolTableNode",
             "cross_ref": "functools.wraps",
             "kind": "Gdef",
             "module_public": false
         }
     },
-    "path": "whoisdomain/__init__.py"
+    "path": "/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/__init__.py"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/__init__.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/test_adjust.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6962962962962963%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(0, 6), (1, 8)], delete: [12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [13, 12, 11, 10, 9, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(5, 'datetime'), (6, 'whoisdomain')], delete: [17, 16, 15, 14, 13, "*

 * *                   '12, 9, 6, 5, 4, 3, 1, 0]}',*

 * * "'hash'": "'d59f8f43d406d6ef9aca3f624f0d44b68fd1a9f89f6b8124f1e264499dc86a01'",*

 * * "'id'": "'test_adjust'",*

 * * "'interface_hash'": "'4c6234e8ce89a6f9a851a30a715064e1b3351e3 […]*

```diff
@@ -1,74 +1,41 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
-        10,
-        11,
-        19,
-        20,
-        28,
-        1,
-        2,
-        3,
-        1,
-        1,
-        1,
-        1,
-        1,
+        6,
+        8,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
-        5,
-        5,
-        10,
-        5,
-        5,
-        5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "whoisdomain._1_query",
-        "whoisdomain._2_parse",
         "whoisdomain._3_adjust",
-        "whoisdomain._0_init_tld",
-        "whoisdomain.exceptions",
-        "sys",
-        "functools",
         "typing",
         "builtins",
-        "_collections_abc",
         "_typeshed",
         "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
-        "types",
-        "typing_extensions"
+        "datetime",
+        "whoisdomain"
     ],
-    "hash": "7f7744135845346fec47d3d4974d55b6c55b6f02573afd23cc9e9ec9749f155c",
-    "id": "whoisdomain",
+    "hash": "d59f8f43d406d6ef9aca3f624f0d44b68fd1a9f89f6b8124f1e264499dc86a01",
+    "id": "test_adjust",
     "ignore_all": false,
-    "interface_hash": "7719e2ed6e68e8615500df58f7abc240f811681ac1499467f869b3c2487edd48",
-    "mtime": 1681721103,
+    "interface_hash": "4c6234e8ce89a6f9a851a30a715064e1b3351e349f774cd4e8c43f5b46dd23cd",
+    "mtime": 1682344065,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -102,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/__init__.py",
+    "path": "test_adjust.py",
     "plugin_data": null,
-    "size": 10048,
+    "size": 1385,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/exceptions.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'path'": "'/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/exceptions.py'"}*

```diff
@@ -360,9 +360,9 @@
                 ],
                 "fullname": "whoisdomain.exceptions.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         }
     },
-    "path": "whoisdomain/exceptions.py"
+    "path": "/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/exceptions.py"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/exceptions.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/exceptions.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'interface_hash'": "'414f6a4513798e734f317ee991ac8823cd34ddce19eb54face6931444000bb6f'",*

 * * "'mtime'": '1681904065'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
@@ -14,16 +14,16 @@
         "builtins",
         "abc",
         "typing"
     ],
     "hash": "543b6b1d6e7d76da1abbae4c0ccf3cba0c585b69afb7146a2c26c3c1c1c23f27",
     "id": "whoisdomain.exceptions",
     "ignore_all": false,
-    "interface_hash": "225b0a51098ebe930ee480a7372baa086b96777d25d32194baf0ea590fd21ae1",
-    "mtime": 1681288053,
+    "interface_hash": "414f6a4513798e734f317ee991ac8823cd34ddce19eb54face6931444000bb6f",
+    "mtime": 1681904065,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/whoisdomain/tld_regexpr.data.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9206271127278072%*

 * *Differences: {"'names'": "{'ZZ': {'node': {'type': {'args': {1: {'type_of_any': 2}, insert: [(0, "*

 * *            "'builtins.str')], delete: [0]}}}}, 'Any': OrderedDict([('.class', 'SymbolTableNode'), "*

 * *            "('cross_ref', 'typing.Any'), ('kind', 'Gdef')])}",*

 * * "'path'": "'/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/tld_regexpr.py'"}*

```diff
@@ -2,14 +2,19 @@
     ".class": "MypyFile",
     "_fullname": "whoisdomain.tld_regexpr",
     "future_import_flags": [],
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
+        "Any": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing.Any",
+            "kind": "Gdef"
+        },
         "Dict": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.Dict",
             "kind": "Gdef"
         },
         "ZZ": {
             ".class": "SymbolTableNode",
@@ -21,25 +26,20 @@
                     "has_explicit_value"
                 ],
                 "fullname": "whoisdomain.tld_regexpr.ZZ",
                 "name": "ZZ",
                 "type": {
                     ".class": "Instance",
                     "args": [
+                        "builtins.str",
                         {
                             ".class": "AnyType",
                             "missing_import_name": null,
                             "source_any": null,
-                            "type_of_any": 4
-                        },
-                        {
-                            ".class": "AnyType",
-                            "missing_import_name": null,
-                            "source_any": null,
-                            "type_of_any": 4
+                            "type_of_any": 2
                         }
                     ],
                     "type_ref": "builtins.dict"
                 }
             }
         },
         "__annotations__": {
@@ -116,9 +116,9 @@
                 ],
                 "fullname": "whoisdomain.tld_regexpr.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         }
     },
-    "path": "whoisdomain/tld_regexpr.py"
+    "path": "/home/mboot/DEV/00-github.com/mboot-github/WhoisDomain/whoisdomain/tld_regexpr.py"
 }
```

### Comparing `whoisdomain-1.20230417.6/.mypy_cache/3.11/whoisdomain/tld_regexpr.meta.json` & `whoisdomain-1.20230424.7/.mypy_cache/3.11/test2.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7177777777777777%*

 * *Differences: {"'data_mtime'": '1682344859',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 1)]}',*

 * * "'dep_prios'": '{insert: [(2, 30), (3, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'whoisdomain.main'), (3, 'typing'), (4, 'whoisdomain')], delete: "*

 * *                   '[0]}',*

 * * "'hash'": "'1ae168f64958fa1793d1aa90d039fa9a94dda886e63dd33884ec6ca2a7fd50f1'",*

 * * "'id'": "'test2'",*

 * * "'interface_hash'": "'7e6bb333051637b5a0491d6fa877488e5ed6d76644b09ef7354c787a1f54ca7d'",*

 * * "'mtime'": '1682342282',*

 * * "'path'": "'test2.py'",*

 * * "'size'": '67'}*

```diff
@@ -1,29 +1,35 @@
 {
-    "data_mtime": 1681721902,
+    "data_mtime": 1682344859,
     "dep_lines": [
+        3,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "typing",
+        "whoisdomain.main",
         "builtins",
-        "abc"
+        "abc",
+        "typing",
+        "whoisdomain"
     ],
-    "hash": "8acc57a8a0aa84441542714dfef5903f5066551b5a508c631744465debaaa182",
-    "id": "whoisdomain.tld_regexpr",
+    "hash": "1ae168f64958fa1793d1aa90d039fa9a94dda886e63dd33884ec6ca2a7fd50f1",
+    "id": "test2",
     "ignore_all": false,
-    "interface_hash": "bf7372147a4626bd2dd8b6ab9bf5efa08c63feda6d91f0c0719cbdc05d64fe46",
-    "mtime": 1681740226,
+    "interface_hash": "7e6bb333051637b5a0491d6fa877488e5ed6d76644b09ef7354c787a1f54ca7d",
+    "mtime": 1682342282,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -57,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "whoisdomain/tld_regexpr.py",
+    "path": "test2.py",
     "plugin_data": null,
-    "size": 104888,
+    "size": 67,
     "suppressed": [],
     "version_id": "1.0.0"
 }
```

### Comparing `whoisdomain-1.20230417.6/Old/DONE` & `whoisdomain-1.20230424.7/Old/DONE`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/analize_patterns.py` & `whoisdomain-1.20230424.7/Old/analize_patterns.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/compare_known_tld.py` & `whoisdomain-1.20230424.7/Old/compare_known_tld.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/makeTestdataAll.sh` & `whoisdomain-1.20230424.7/Old/makeTestdataAll.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/test.py` & `whoisdomain-1.20230424.7/Old/test.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/test.sh` & `whoisdomain-1.20230424.7/test.sh`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/test3.py` & `whoisdomain-1.20230424.7/Old/test3.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/testExtend.py` & `whoisdomain-1.20230424.7/Old/testExtend.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/tests/new-test.txt` & `whoisdomain-1.20230424.7/Old/tests/new-test.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/Old/tests/ok-domains.txt` & `whoisdomain-1.20230424.7/Old/tests/ok-domains.txt`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/make_testdata.sh` & `whoisdomain-1.20230424.7/testdata/make_testdata.sh`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 {
     DOMAINS=(
         example.net # has iana source
         example.com # has iana source
         example.org # has no iana source
         meta.co.uk # has multiline for all relevant fields and 4 nameservers; should be fixed output has only 2
         xs4all.nl # has multiline nameserver and multiline registrar; outout has no nameservers should be 2
-        meta.com.sg # has mail
         meta.com # have emails
-        google.com # have emails
         meta.jp # jp has [registrar] type keywords not registrar:
         meta.co.jp # jp has [registrar] type keywords not registrar:
         meta.kr # has both korean and english text
         meta.com.tr # has utf 8 response text and different formatting style
         hello.xyz # has sometimes IANA Source beginning on mac
     )
 }
@@ -23,14 +21,15 @@
 {
     local str="$1"
 
     grep name_servers  "./$str/output" | awk '{ $1 = $2 = ""; print }' | awk -F, '{print NF}'
     grep "name server" "./$str/nameservers" | wc -l
 
 }
+
 makeDataForDomain()
 {
     local str="$1"
 
     # create one dir for each domain we will test
     mkdir -p "$str"
```

### Comparing `whoisdomain-1.20230417.6/testdata/example.com/output` & `whoisdomain-1.20230424.7/testdata/example.com/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/example.net/output` & `whoisdomain-1.20230424.7/testdata/example.net/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/example.org/input` & `whoisdomain-1.20230424.7/testdata/example.org/input`

 * *Files 2% similar despite different names*

```diff
@@ -54,12 +54,12 @@
 Tech Fax: REDACTED FOR PRIVACY
 Tech Fax Ext: REDACTED FOR PRIVACY
 Tech Email: Please query the RDDS service of the Registrar of Record identified in this output for information on how to contact the Registrant, Admin, or Tech contact of the queried domain name.
 Name Server: a.iana-servers.net
 Name Server: b.iana-servers.net
 DNSSEC: signedDelegation
 URL of the ICANN Whois Inaccuracy Complaint Form: https://www.icann.org/wicf/
->>> Last update of WHOIS database: 2023-01-27T13:06:45Z <<<
+>>> Last update of WHOIS database: 2023-04-24T13:35:47Z <<<
 
 For more information on Whois status codes, please visit https://icann.org/epp
 
 Terms of Use: Access to Public Interest Registry WHOIS information is provided to assist persons in determining the contents of a domain name registration record in the Public Interest Registry registry database. The data in this record is provided by Public Interest Registry for informational purposes only, and Public Interest Registry does not guarantee its accuracy. This service is intended only for query-based access. You agree that you will use this data only for lawful purposes and that, under no circumstances will you use this data to (a) allow, enable, or otherwise support the transmission by e-mail, telephone, or facsimile of mass unsolicited, commercial advertising or solicitations to entities other than the data recipient's own existing customers; or (b) enable high volume, automated, electronic processes that send queries or data to the systems of Registry Operator, a Registrar, or Identity Digital except as reasonably necessary to register domain names or modify existing registrations. All rights reserved. Public Interest Registry reserves the right to modify these terms at any time. By submitting this query, you agree to abide by this policy.  The Registrar of Record identified in this output may have an RDDS service that can be queried for additional information on how to contact the Registrant, Admin, or Tech contact of the queried domain name.
```

### Comparing `whoisdomain-1.20230417.6/testdata/example.org/output` & `whoisdomain-1.20230424.7/testdata/example.org/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/google.com/input` & `whoisdomain-1.20230424.7/testdata/meta.com/input`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,88 @@
 [Querying whois.verisign-grs.com]
-[Redirected to whois.markmonitor.com]
-[Querying whois.markmonitor.com]
-[whois.markmonitor.com]
-Domain Name: google.com
-Registry Domain ID: 2138514_DOMAIN_COM-VRSN
-Registrar WHOIS Server: whois.markmonitor.com
-Registrar URL: http://www.markmonitor.com
-Updated Date: 2019-09-09T15:39:04+0000
-Creation Date: 1997-09-15T07:00:00+0000
-Registrar Registration Expiration Date: 2028-09-13T07:00:00+0000
-Registrar: MarkMonitor, Inc.
-Registrar IANA ID: 292
-Registrar Abuse Contact Email: abusecomplaints@markmonitor.com
-Registrar Abuse Contact Phone: +1.2086851750
-Domain Status: clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)
-Domain Status: clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)
-Domain Status: clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)
-Domain Status: serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)
-Domain Status: serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)
-Domain Status: serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)
-Registrant Organization: Google LLC
+[Redirected to whois.registrarsafe.com]
+[Querying whois.registrarsafe.com]
+[whois.registrarsafe.com]
+Domain Name: META.COM
+Registry Domain ID: 1433704_DOMAIN_COM-VRSN
+Registrar WHOIS Server: whois.registrarsafe.com
+Registrar URL: https://www.registrarsafe.com
+Updated Date: 2023-01-25T20:09:06Z
+Creation Date: 1991-01-21T05:00:00Z
+Registrar Registration Expiration Date: 2032-01-22T05:00:00Z
+Registrar: RegistrarSafe, LLC
+Registrar IANA ID: 3237
+Registrar Abuse Contact Email: abusecomplaints@registrarsafe.com
+Registrar Abuse Contact Phone: +1.6503087004
+Domain Status: clientDeleteProhibited https://www.icann.org/epp#clientDeleteProhibited
+Domain Status: clientTransferProhibited https://www.icann.org/epp#clientTransferProhibited
+Domain Status: clientUpdateProhibited https://www.icann.org/epp#clientUpdateProhibited
+Domain Status: serverDeleteProhibited https://www.icann.org/epp#serverDeleteProhibited
+Domain Status: serverTransferProhibited https://www.icann.org/epp#serverTransferProhibited
+Domain Status: serverUpdateProhibited https://www.icann.org/epp#serverUpdateProhibited
+Registry Registrant ID: 
+Registrant Name: Domain Admin
+Registrant Organization: Meta Platforms, Inc.
+Registrant Street: 1601 Willow Rd 
+Registrant City: Menlo Park
 Registrant State/Province: CA
+Registrant Postal Code: 94025
 Registrant Country: US
-Registrant Email: Select Request Email Form at https://domains.markmonitor.com/whois/google.com
-Admin Organization: Google LLC
+Registrant Phone: +1.6505434800
+Registrant Phone Ext:
+Registrant Fax: 
+Registrant Fax Ext:
+Registrant Email: domain@fb.com
+Registry Admin ID: 
+Admin Name: Domain Admin
+Admin Organization: Meta Platforms, Inc.
+Admin Street: 1601 Willow Rd 
+Admin City: Menlo Park
 Admin State/Province: CA
+Admin Postal Code: 94025
 Admin Country: US
-Admin Email: Select Request Email Form at https://domains.markmonitor.com/whois/google.com
-Tech Organization: Google LLC
+Admin Phone: +1.6505434800
+Admin Phone Ext:
+Admin Fax: 
+Admin Fax Ext:
+Admin Email: domain@fb.com
+Registry Tech ID: 
+Tech Name: Domain Admin
+Tech Organization: Meta Platforms, Inc.
+Tech Street: 1601 Willow Rd 
+Tech City: Menlo Park
 Tech State/Province: CA
+Tech Postal Code: 94025
 Tech Country: US
-Tech Email: Select Request Email Form at https://domains.markmonitor.com/whois/google.com
-Name Server: ns1.google.com
-Name Server: ns4.google.com
-Name Server: ns3.google.com
-Name Server: ns2.google.com
+Tech Phone: +1.6505434800
+Tech Phone Ext:
+Tech Fax: 
+Tech Fax Ext:
+Tech Email: domain@fb.com
+Name Server: D.NS.FACEBOOK.COM
+Name Server: A.NS.FACEBOOK.COM
+Name Server: C.NS.FACEBOOK.COM
+Name Server: B.NS.FACEBOOK.COM
 DNSSEC: unsigned
 URL of the ICANN WHOIS Data Problem Reporting System: http://wdprs.internic.net/
->>> Last update of WHOIS database: 2023-01-27T13:04:53+0000 <<<
+>>> Last update of WHOIS database: 2023-04-24T13:35:49Z <<<
 
-For more information on WHOIS status codes, please visit:
-  https://www.icann.org/resources/pages/epp-status-codes
+Search results obtained from the RegistrarSafe, LLC WHOIS database are
+provided by RegistrarSafe, LLC for information purposes only, to assist
+users in obtaining information concerning a domain name registration record.
+The information contained therein is provided on an "as is" and "as available"
+basis and RegistrarSafe, LLC does not guarantee the accuracy or completeness
+of any information provided through the WHOIS database.  By submitting a WHOIS query,
+you agree to the following: (1) that you will use any information provided through
+the WHOIS only for lawful purposes; (2) that you will comply with all ICANN rules
+and regulations governing use of the WHOIS; (3)  that you will not use any information
+provided through the WHOIS to  enable, or otherwise cause the transmission of mass
+unsolicited, commercial advertising or solicitations via e-mail (i.e., spam); or
+(4) that you will not use the WHOIS to enable or otherwise utilize high volume,
+automated, electronic processes that apply to or attach to RegistrarSafe, LLC or
+its systems. RegistrarSafe, LLC reserves the right to modify these terms
+at any time and to take any other appropriate actions, including but not limited to
+restricting any access that violates these terms and conditions. By submitting this
+query, you acknowledge and agree to abide by the foregoing terms, conditions and policies.
 
-If you wish to contact this domain’s Registrant, Administrative, or Technical
-contact, and such email address is not visible above, you may do so via our web
-form, pursuant to ICANN’s Temporary Specification. To verify that you are not a
-robot, please enter your email address to receive a link to a page that
-facilitates email communication with the relevant contact(s).
-
-Web-based WHOIS:
-  https://domains.markmonitor.com/whois
-
-If you have a legitimate interest in viewing the non-public WHOIS details, send
-your request and the reasons for your request to whoisrequest@markmonitor.com
-and specify the domain name in the subject line. We will review that request and
-may ask for supporting documentation and explanation.
-
-The data in MarkMonitor’s WHOIS database is provided for information purposes,
-and to assist persons in obtaining information about or related to a domain
-name’s registration record. While MarkMonitor believes the data to be accurate,
-the data is provided "as is" with no guarantee or warranties regarding its
-accuracy.
-
-By submitting a WHOIS query, you agree that you will use this data only for
-lawful purposes and that, under no circumstances will you use this data to:
-  (1) allow, enable, or otherwise support the transmission by email, telephone,
-or facsimile of mass, unsolicited, commercial advertising, or spam; or
-  (2) enable high volume, automated, or electronic processes that send queries,
-data, or email to MarkMonitor (or its systems) or the domain name contacts (or
-its systems).
-
-MarkMonitor reserves the right to modify these terms at any time.
-
-By submitting this query, you agree to abide by this policy.
-
-MarkMonitor Domain Management(TM)
-Protecting companies and consumers in a digital world.
-
-Visit MarkMonitor at https://www.markmonitor.com
-Contact us at +1.8007459229
-In Europe, at +44.02032062220
---
+For more information on Whois status codes, please visit
+    https://www.icann.org/resources/pages/epp-status-codes-2014-06-16-en.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `whoisdomain-1.20230417.6/testdata/google.com/output` & `whoisdomain-1.20230424.7/testdata/meta.com/output`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
-test domain: <<<<<<<<<< google.com >>>>>>>>>>>>>>>>>>>>
-name               str               'google.com'
+test domain: <<<<<<<<<< meta.com >>>>>>>>>>>>>>>>>>>>
+name               str               'meta.com'
 tld                str               'com'
-registrar          str               'MarkMonitor, Inc.'
+registrar          str               'RegistrarSafe, LLC'
 registrant_country str               'US'
-creation_date      datetime.datetime 1997-09-15 09:00:00
-expiration_date    NoneType          None
-last_updated       datetime.datetime 2019-09-09 17:39:04
-status             str               'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)'
-statuses           list              ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)']
+creation_date      datetime.datetime 1991-01-21 05:00:00
+expiration_date    datetime.datetime 2032-01-22 05:00:00
+last_updated       datetime.datetime 2023-01-25 20:09:06
+status             str               'clientDeleteProhibited https://www.icann.org/epp#clientDeleteProhibited'
+statuses           list              ['clientDeleteProhibited https://www.icann.org/epp#clientDeleteProhibited', 'clientTransferProhibited https://www.icann.org/epp#clientTransferProhibited', 'clientUpdateProhibited https://www.icann.org/epp#clientUpdateProhibited', 'serverDeleteProhibited https://www.icann.org/epp#serverDeleteProhibited', 'serverTransferProhibited https://www.icann.org/epp#serverTransferProhibited', 'serverUpdateProhibited https://www.icann.org/epp#serverUpdateProhibited']
 dnssec             bool              False
-name_servers       list              ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com']
-registrant         str               'Google LLC'
-emails             list              ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
+name_servers       list              ['a.ns.facebook.com', 'b.ns.facebook.com', 'c.ns.facebook.com', 'd.ns.facebook.com']
+registrant         str               'Meta Platforms, Inc.'
+emails             list              ['abusecomplaints@registrarsafe.com', 'domain@fb.com']
```

### Comparing `whoisdomain-1.20230417.6/testdata/hello.xyz/input` & `whoisdomain-1.20230424.7/testdata/hello.xyz/input`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [Querying whois.nic.xyz]
 [whois.nic.xyz]
 Domain Name: HELLO.XYZ
 Registry Domain ID: D2208533-CNIC
 Registrar WHOIS Server: whois.namecheap.com
 Registrar URL: https://namecheap.com
-Updated Date: 2022-03-14T11:17:22.0Z
+Updated Date: 2023-03-14T09:24:32.0Z
 Creation Date: 2014-03-20T15:01:22.0Z
-Registry Expiry Date: 2023-03-20T23:59:59.0Z
+Registry Expiry Date: 2024-03-20T23:59:59.0Z
 Registrar: Namecheap
 Registrar IANA ID: 1068
 Domain Status: clientTransferProhibited https://icann.org/epp#clientTransferProhibited
 Registrant Organization: Privacy service provided by Withheld for Privacy ehf
 Registrant State/Province: Capital Region
 Registrant Country: IS
 Registrant Email: Please query the RDDS service of the Registrar of Record identified in this output for information on how to contact the Registrant, Admin, or Tech contact of the queried domain name.
@@ -19,15 +19,15 @@
 Name Server: DNS1.REGISTRAR-SERVERS.COM
 Name Server: DNS2.REGISTRAR-SERVERS.COM
 DNSSEC: unsigned
 Billing Email: Please query the RDDS service of the Registrar of Record identified in this output for information on how to contact the Registrant, Admin, or Tech contact of the queried domain name.
 Registrar Abuse Contact Email: abuse@namecheap.com
 Registrar Abuse Contact Phone: +1.9854014545
 URL of the ICANN Whois Inaccuracy Complaint Form: https://www.icann.org/wicf/
->>> Last update of WHOIS database: 2023-01-27T13:06:56.0Z <<<
+>>> Last update of WHOIS database: 2023-04-24T13:36:01.0Z <<<
 
 For more information on Whois status codes, please visit https://icann.org/epp
 
 >>> IMPORTANT INFORMATION ABOUT THE DEPLOYMENT OF RDAP: please visit
 https://www.centralnic.com/support/rdap <<<
 
 The Whois and RDAP services are provided by CentralNic, and contain
```

### Comparing `whoisdomain-1.20230417.6/testdata/hello.xyz/output` & `whoisdomain-1.20230424.7/testdata/hello.xyz/output`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 test domain: <<<<<<<<<< hello.xyz >>>>>>>>>>>>>>>>>>>>
 name               str               'hello.xyz'
 tld                str               'xyz'
 registrar          str               'Namecheap'
 registrant_country str               'IS'
 creation_date      datetime.datetime 2014-03-20 15:01:22
-expiration_date    datetime.datetime 2023-03-20 23:59:59
-last_updated       datetime.datetime 2022-03-14 11:17:22
+expiration_date    datetime.datetime 2024-03-20 23:59:59
+last_updated       datetime.datetime 2023-03-14 09:24:32
 status             str               'clientTransferProhibited https://icann.org/epp#clientTransferProhibited'
 statuses           list              ['clientTransferProhibited https://icann.org/epp#clientTransferProhibited']
 dnssec             bool              False
 name_servers       list              ['dns1.registrar-servers.com', 'dns2.registrar-servers.com']
 registrant         str               'Privacy service provided by Withheld for Privacy ehf'
 emails             list              ['abuse@namecheap.com']
```

### Comparing `whoisdomain-1.20230417.6/testdata/meta.co.jp/input` & `whoisdomain-1.20230424.7/testdata/meta.co.jp/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/meta.co.jp/output` & `whoisdomain-1.20230424.7/testdata/meta.co.jp/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/meta.co.uk/input` & `whoisdomain-1.20230424.7/testdata/meta.co.uk/input`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     Name servers:
         a.ns.facebook.com
         b.ns.facebook.com
         c.ns.facebook.com
         d.ns.facebook.com
 
-    WHOIS lookup made at 13:06:46 27-Jan-2023
+    WHOIS lookup made at 14:35:48 24-Apr-2023
 
 -- 
 This WHOIS information is provided for free by Nominet UK the central registry
 for .uk domain names. This information and the .uk WHOIS are:
 
     Copyright Nominet UK 1996 - 2023.
```

### Comparing `whoisdomain-1.20230417.6/testdata/meta.co.uk/output` & `whoisdomain-1.20230424.7/testdata/meta.co.uk/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/meta.com.tr/input` & `whoisdomain-1.20230424.7/testdata/meta.com.tr/input`

 * *Files 18% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
 ** Additional Info:
 Created on..............: 2006-Dec-28.
 Expires on..............: 2026-Dec-27.
 
 
 ** Whois Server:
-Last Update Time: 2023-01-27T16:04:30+03:00
+Last Update Time: 2023-04-24T16:22:51+03:00
```

### Comparing `whoisdomain-1.20230417.6/testdata/meta.com.tr/output` & `whoisdomain-1.20230424.7/testdata/meta.com.tr/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/meta.jp/input` & `whoisdomain-1.20230424.7/testdata/meta.jp/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/meta.jp/output` & `whoisdomain-1.20230424.7/testdata/meta.jp/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/meta.kr/input` & `whoisdomain-1.20230424.7/testdata/meta.kr/input`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/meta.kr/output` & `whoisdomain-1.20230424.7/testdata/meta.kr/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/testdata/xs4all.nl/input` & `whoisdomain-1.20230424.7/testdata/xs4all.nl/input`

 * *Files 11% similar despite different names*

```diff
@@ -18,28 +18,25 @@
 
 DNSSEC:      yes
 
 Domain nameservers:
    ns1.kpn.net
    ns11.kpn.net
 
-Record maintained by: NL Domain Registry
+Record maintained by: SIDN BV
 
 Copyright notice
 No part of this publication may be reproduced, published, stored in a
 retrieval system, or transmitted, in any form or by any means,
 electronic, mechanical, recording, or otherwise, without prior
-permission of the Foundation for Internet Domain Registration in the
-Netherlands (SIDN).
+permission of SIDN.
 These restrictions apply equally to registrars, except in that
 reproductions and publications are permitted insofar as they are
 reasonable, necessary and solely in the context of the registration
 activities referred to in the General Terms and Conditions for .nl
 Registrars.
 Any use of this material for advertising, targeting commercial offers or
 similar activities is explicitly forbidden and liable to result in legal
 action. Anyone who is aware or suspects that such activities are taking
-place is asked to inform the Foundation for Internet Domain Registration
-in the Netherlands.
-(c) The Foundation for Internet Domain Registration in the Netherlands
-(SIDN) Dutch Copyright Act, protection of authors' rights (Section 10,
-subsection 1, clause 1).
+place is asked to inform SIDN.
+(c) SIDN BV, Dutch Copyright Act, protection of authors' rights
+(Section 10, subsection 1, clause 1).
```

### Comparing `whoisdomain-1.20230417.6/testdata/xs4all.nl/output` & `whoisdomain-1.20230424.7/testdata/xs4all.nl/output`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230424.7/whoisdomain/_0_init_tld.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 )
 
 from .tld_regexpr import ZZ
 from .exceptions import (
     UnknownTld,
 )
 
-Verbose = False
-TLD_RE: Dict[str, Any] = {}
-REG_COLLECTION_BY_KEY: Dict = {}
+Verbose: bool = False
+TLD_RE: Dict[str, Dict[str, Any]] = {}
+REG_COLLECTION_BY_KEY: Dict[str, Any] = {}
 
 
-def validTlds():
+def validTlds() -> List[str]:
     return sorted(TLD_RE.keys())
 
 
 def filterTldToSupportedPattern(
     domain: str,
     d: List[str],
     verbose: bool = False,
@@ -46,15 +46,15 @@
     # if not fail
     a = f"The TLD {tld} is currently not supported by this package."
     b = "Use validTlds() to see what toplevel domains are supported."
     msg = f"{a} {b}"
     raise UnknownTld(msg)
 
 
-def get_tld_re(tld: str, override: bool = False) -> Any:
+def get_tld_re(tld: str, override: bool = False) -> Dict[str, Any]:
     if override is False:
         if tld in TLD_RE:
             return TLD_RE[tld]
 
     v = ZZ[tld]
 
     extend = v.get("extend")
@@ -83,26 +83,26 @@
     # meta domains start with _: examples _centralnic and _donuts
     if tld[0] != "_":
         TLD_RE[tld] = tld_re
 
     return tld_re
 
 
-def mergeExternalDictWithRegex(aDict: Dict = {}):
+def mergeExternalDictWithRegex(aDict: Dict[str, Any] = {}) -> None:
     # merge in ZZ, this extends ZZ with new tld's and overrides existing tld's
     for tld in aDict.keys():
         ZZ[tld] = aDict[tld]
 
     # reprocess te regexes we newly defined or overrode
     override = True
     for tld in aDict.keys():
         initOne(tld, override)
 
 
-def initOne(tld, override: bool = False):
+def initOne(tld: str, override: bool = False) -> None:
     if tld[0] == "_":  # skip meta domain patterns , these are not domains just handles we reuse
         return
 
     what = get_tld_re(tld, override)
 
     # test if the string is identical after idna conversion
     d = tld.split(".")
@@ -113,16 +113,17 @@
 
     # also automatically see if we can internationalize the domains to the official ascii string
     TLD_RE[tld2] = what
     if Verbose:
         print(f"{tld} -> {tld2}", file=sys.stderr)
 
 
-def buildRegCollection(zz: Dict):
-    regCollection: Dict = {}
+def buildRegCollection(zz: Dict[str, Any]) -> Dict[str, Any]:
+    regCollection: Dict[str, Any] = {}
+
     # get all regexes
     for name in zz:
         # print(name)
         z = zz[name]
         for key in z:
             if key is None:
                 continue
@@ -147,15 +148,15 @@
             regCollection[key][reg] = None
             if isinstance(reg, str):
                 regCollection[key][reg] = re.compile(reg, flags=re.IGNORECASE)
 
     return regCollection
 
 
-def initOnImport():
+def initOnImport() -> None:
     global REG_COLLECTION_BY_KEY
     # here we run the import processing
     # we load all tld's on import so we dont lose time later
     # we keep ZZ so we can later reuse it if we want to aoverrid or update tld's
     REG_COLLECTION_BY_KEY = buildRegCollection(ZZ)
     override = False
     for tld in ZZ.keys():
```

### Comparing `whoisdomain-1.20230417.6/whoisdomain/_1_query.py` & `whoisdomain-1.20230424.7/whoisdomain/_1_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     force: bool = False,
     cache_file: Optional[str] = None,
     cache_age: int = CACHE_MAX_AGE,
     slow_down: int = 0,
     ignore_returncode: bool = False,
     server: Optional[str] = None,
     verbose: bool = False,
-    timeout: float = None,
+    timeout: Optional[float] = None,
     wh: str = "whois",
 ) -> str:
     k = ".".join(dl)
 
     if cache_file:
         if verbose:
             print(f"using cache file: {cache_file}", file=sys.stderr)
@@ -81,15 +81,17 @@
 
         if cache_file:
             cache_save(cache_file)
 
     return CACHE[k][1]
 
 
-def tryInstallMissingWhoisOnWindows(verbose: bool = False):
+def tryInstallMissingWhoisOnWindows(
+    verbose: bool = False,
+) -> None:
     """
     Windows 'whois' command wrapper
     https://docs.microsoft.com/en-us/sysinternals/downloads/whois
     """
     folder = os.getcwd()
     copy_command = r"copy \\live.sysinternals.com\tools\whois.exe " + folder
     if verbose:
@@ -105,15 +107,15 @@
 
 
 def makeWhoisCommandToRun(
     dl: List[str],
     server: Optional[str] = None,
     verbose: bool = False,
     wh: str = "whois",
-):
+) -> List[str]:
     domain = ".".join(dl)
 
     if platform.system() == "Windows":
         # Usage: whois [-v] domainname [whois.server]
 
         if os.path.exists("whois.exe"):
             wh = r".\whois.exe"
@@ -158,15 +160,15 @@
 
 
 def _do_whois_query(
     dl: List[str],
     ignore_returncode: bool,
     server: Optional[str] = None,
     verbose: bool = False,
-    timeout: float = None,
+    timeout: Optional[float] = None,
     wh: str = "whois",
 ) -> str:
     # if getenv[TEST_WHOIS_PYTON] fake whois by reading static data from a file
     # this wasy we can actually implemnt a test run with known data in and expected data out
     if os.getenv("TEST_WHOIS_PYTHON"):
         return testWhoisPythonFromStaticTestData(dl, ignore_returncode, server, verbose)
```

### Comparing `whoisdomain-1.20230417.6/whoisdomain/_2_parse.py` & `whoisdomain-1.20230424.7/whoisdomain/_2_parse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import re
 import sys
 
 from typing import (
+    cast,
     Any,
     Dict,
     Optional,
     List,
     Tuple,
 )
 
 from ._0_init_tld import TLD_RE
 
 from .exceptions import FailedParsingWhoisOutput
 from .exceptions import WhoisQuotaExceeded
 
-Verbose = True
+Verbose: bool = True
 
-NONESTRINGS: List = [
+NONESTRINGS: List[str] = [
     "the domain has not been registered",
     "no match found for",
     "no matching record",
     "not found",
     "no data found",
     "no entries found",
     "status: free",
@@ -33,60 +34,60 @@
     "malformed request",  # this means this domain is not in whois as it is on top of a registered domain
     "no match",
     "registration of this domain is restricted",
     "restricted",
     "this domain is currently available",
 ]
 
-QUOTASTRINGS = [
+QUOTASTRINGS: List[str] = [
     "limit exceeded",
     "quota exceeded",
     "try again later",
     "please try again",
     "exceeded the maximum allowable number",
     "can temporarily not be answered",
     "please try again.",
     "queried interval is too short",
     "number of allowed queries exceeded",
 ]
 
 
-def NoneStrings() -> List:
+def NoneStrings() -> List[str]:
     return sorted(NONESTRINGS)
 
 
-def NoneStringsAdd(aString: str):
+def NoneStringsAdd(aString: str) -> None:
     if aString and isinstance(aString, str) and len(aString) > 0:
         NONESTRINGS.append(aString)
 
 
-def QuotaStrings() -> List:
+def QuotaStrings() -> List[str]:
     return sorted(QUOTASTRINGS)
 
 
-def QuotaStringsAdd(aString: str):
+def QuotaStringsAdd(aString: str) -> None:
     if aString and isinstance(aString, str) and len(aString) > 0:
         NONESTRINGS.append(aString)
 
 
 def cleanupWhoisResponse(
     whois_str: str,
     verbose: bool = False,
     with_cleanup_results: bool = False,
 ) -> str:
-    tmp2 = []
+    tmp2: List[str] = []
 
     # note we cannot do yet rstrip() on the lines as many registrars use \r and even trailing whitespace after entries
     # as the resulting matches are all stripped of leading and trailing whitespace this currently is fixed there
     # and relaxes the regexes: you will often see a capture with (.*)
     # we would have to fix all regexes to allow stripping all trailing whitespace
     # it would make many matches easier though.
 
     skipFromHere = False
-    tmp: List = whois_str.split("\n")
+    tmp: List[str] = whois_str.split("\n")
     for line in tmp:
         if skipFromHere is True:
             continue
 
         # some servers respond with: % Quota exceeded in the comment section (lines starting with %)
         if "quota exceeded" in line.lower():
             raise WhoisQuotaExceeded(whois_str)
@@ -116,18 +117,19 @@
         tmp2.append(line.strip("\r"))
 
     return "\n".join(tmp2)
 
 
 def handleShortResponse(
     tld: str,
-    dl: List,
+    dl: List[str],
     whois_str: str,
     verbose: bool = False,
-):  # returns None or raises one of (WhoisQuotaExceeded, FailedParsingWhoisOutput)
+) -> None:
+    # returns None or raises one of (WhoisQuotaExceeded, FailedParsingWhoisOutput)
     if verbose:
         d = ".".join(dl)
         print(f"line count < 5:: {tld} {d} {whois_str}", file=sys.stderr)
 
     # TODO: some short responses are actually valid:
     # lookfor Domain: and Status but all other fields are missing so the regexec could fail
     # this domain is taken already or reserved
@@ -159,34 +161,44 @@
     for i in quotaStrings:
         if i in s:
             raise WhoisQuotaExceeded(whois_str)
 
     raise FailedParsingWhoisOutput(whois_str)
 
 
-def doDnsSec(whois_str: str) -> bool:
+def doDnsSec(
+    whois_str: str,
+) -> bool:
     whois_dnssec: Any = whois_str.split("DNSSEC:")
     if len(whois_dnssec) >= 2:
         whois_dnssec = whois_dnssec[1].split("\n")[0]
         if whois_dnssec.strip() == "signedDelegation" or whois_dnssec.strip() == "yes":
             return True
     return False
 
 
-def doIfServerNameLookForDomainName(whois_str: str, verbose: bool = False) -> str:
+def doIfServerNameLookForDomainName(
+    whois_str: str,
+    verbose: bool = False,
+) -> str:
     # not often available anymore
     if re.findall(r"Server Name:\s?(.+)", whois_str, re.IGNORECASE):
         if verbose:
             msg = "i have seen Server Name:, looking for Domain Name:"
             print(msg, file=sys.stderr)
         whois_str = whois_str[whois_str.find("Domain Name:") :]
     return whois_str
 
 
-def doExtractPattensIanaFromWhoisString(tld: str, r: Dict, whois_str: str, verbose: bool = False):
+def doExtractPattensIanaFromWhoisString(
+    tld: str,
+    r: Dict[str, Any],
+    whois_str: str,
+    verbose: bool = False,
+) -> Dict[str, Any]:
     # now handle the actual format if this whois response
     iana = {
         "domain_name": r"domain:\s?([^\n]+)",
         "registrar": r"organisation:\s?([^\n]+)",
         "creation_date": r"created:\s?([^\n]+)",
     }
     for k, v in iana.items():
@@ -194,15 +206,39 @@
         if zz:
             if verbose:
                 print(f"parsing iana data only for tld: {tld}, {zz}", file=sys.stderr)
             r[k] = zz
     return r
 
 
-def doSourceIana(tld: str, r: Dict, whois_str: str, verbose: bool = False) -> Tuple[str, Optional[Dict[str, Any]]]:
+def doExtractPattensFromWhoisString(
+    tld: str,
+    r: Dict[str, Any],
+    whois_str: str,
+    verbose: bool = False,
+) -> Dict[str, Any]:
+    for k, v in TLD_RE.get(tld, TLD_RE["com"]).items():  # use TLD_RE["com"] as default if a regex is missing
+        if k.startswith("_"):  # skip meta element like: _server or _privateRegistry
+            continue
+
+        # Historical: here we use 'empty string' as default, not None
+        if v is None:
+            r[k] = [""]
+        else:
+            r[k] = v.findall(whois_str) or [""]
+
+    return r
+
+
+def doSourceIana(
+    tld: str,
+    r: Dict[str, Any],
+    whois_str: str,
+    verbose: bool = False,
+) -> Tuple[str, Optional[Dict[str, Any]]]:
     # here we can handle the example.com and example.net permanent IANA domains
     k = "source:       IANA"
 
     if verbose:
         msg = f"i have seen {k}"
         print(msg, file=sys.stderr)
 
@@ -216,60 +252,59 @@
         if verbose:
             msg = f"after: {k} we see not only whitespace: {whois_splitted[1]}"
             print(msg, file=sys.stderr)
 
         return whois_splitted[1], None
 
     # try to parse this as a IANA domain as after is only whitespace
-    r = doExtractPattensFromWhoisString(tld, r, whois_str, verbose)  # set default values
+    r = doExtractPattensFromWhoisString(
+        tld,
+        r,
+        whois_str,
+        verbose,
+    )  # set default values
 
     # now handle the actual format if this whois response
-    r = doExtractPattensIanaFromWhoisString(tld, r, whois_str, verbose)
+    r = doExtractPattensIanaFromWhoisString(
+        tld,
+        r,
+        whois_str,
+        verbose,
+    )
 
     return whois_str, r
 
 
-def doExtractPattensFromWhoisString(tld: str, r: Dict, whois_str: str, verbose: bool = False):
-    for k, v in TLD_RE.get(tld, TLD_RE["com"]).items():  # use TLD_RE["com"] as default if a regex is missing
-        if k.startswith("_"):  # skip meta element like: _server or _privateRegistry
-            continue
-
-        # Historical: here we use 'empty string' as default, not None
-        if v is None:
-            r[k] = [""]
-        else:
-            r[k] = v.findall(whois_str) or [""]
-
-    return r
-
-
 def do_parse(
     whois_str: str,
     tld: str,
     dl: List[str],
     verbose: bool = False,
-    with_cleanup_results=False,
+    with_cleanup_results: bool = False,
 ) -> Optional[Dict[str, Any]]:
 
     whois_str = cleanupWhoisResponse(
         whois_str=whois_str,
         verbose=verbose,
         with_cleanup_results=with_cleanup_results,
     )
 
     if whois_str.count("\n") < 5:
-        return handleShortResponse(tld, dl, whois_str, verbose)
+        # return handleShortResponse(tld, dl, whois_str, verbose)
+        handleShortResponse(tld, dl, whois_str, verbose)
+        return None
 
     r: Dict[str, Any] = {
         "tld": tld,
         "DNSSEC": doDnsSec(whois_str),
     }
 
     if "source:       IANA" in whois_str:  # prepare for handling historical IANA domains
         whois_str, ianaDomain = doSourceIana(tld, r, whois_str, verbose)
         if ianaDomain is not None:
+            ianaDomain = cast(Optional[Dict[str, Any]], ianaDomain)
             return ianaDomain
 
     if "Server Name" in whois_str:  # handle old type Server Name (not very common anymore)
         whois_str = doIfServerNameLookForDomainName(whois_str, verbose)
 
     return doExtractPattensFromWhoisString(tld, r, whois_str, verbose)
```

### Comparing `whoisdomain-1.20230417.6/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230424.7/whoisdomain/_3_adjust.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     registrant_country: Optional[str] = None
 
     creation_date = None
     expiration_date = None
     last_updated = None
 
     status: Optional[str] = None
-    statuses: List = []
+    statuses: List[str] = []
 
     dnssec: bool = False
-    name_servers: List = []
+    name_servers: List[str] = []
     owner: Optional[str] = None
     abuse_contact = None
     reseller = None
     registrant = None
     admin = None
 
     def __init__(
```

### Comparing `whoisdomain-1.20230417.6/whoisdomain/__init__.py` & `whoisdomain-1.20230424.7/whoisdomain/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import sys
 from functools import wraps
 from typing import (
+    cast,
     Optional,
     List,
     Dict,
     Tuple,
+    Any,
+    Callable,
 )
 
 from ._1_query import do_query
 from ._2_parse import (
     do_parse,
     NoneStrings,
     NoneStringsAdd,
     QuotaStrings,
     QuotaStringsAdd,
+    cleanupWhoisResponse,
 )
 
-from ._3_adjust import Domain
-from ._0_init_tld import (
+from ._3_adjust import (
+    Domain,
+)
+
+from .tld_regexpr import (
     ZZ,
+)
+
+from ._0_init_tld import (
     TLD_RE,
     validTlds,
     filterTldToSupportedPattern,
     mergeExternalDictWithRegex,
 )
 
 from .exceptions import (
@@ -31,74 +41,57 @@
     UnknownDateFormat,
     WhoisCommandFailed,
     WhoisPrivateRegistry,
     WhoisQuotaExceeded,
     WhoisCommandTimeout,
 )
 
-"""
-    Python module/library for retrieving WHOIS information of domains.
-
-    By DDarko.org  ddarko@ddarko.org  http://ddarko.org/
-    License MIT  http://www.opensource.org/licenses/mit-license.php
-
-    Usage example
-    >>> import whois
-    >>> domain = whois.query('google.com')
-    >>> print(domain.__dict__)  # print(whois.get('google.com'))
-
-    {
-        'expiration_date':  datetime.datetime(2020, 9, 14, 0, 0),
-        'last_updated':     datetime.datetime(2011, 7, 20, 0, 0),
-        'registrar':        'MARKMONITOR INC.',
-        'name':             'google.com',
-        'creation_date':    datetime.datetime(1997, 9, 15, 0, 0)
-    }
-
-    >>> print(domain.name)
-    google.com
-
-    >>> print(domain.expiration_date)
-    2020-09-14 00:00:00
-
-"""
 __all__ = [
-    "query",
-    "get",
+    "UnknownTld",
+    "FailedParsingWhoisOutput",
+    "UnknownDateFormat",
+    "WhoisCommandFailed",
+    "WhoisPrivateRegistry",
+    "WhoisQuotaExceeded",
+    "WhoisCommandTimeout",
+    "cleanupWhoisResponse",
     "validTlds",
-    "mergeExternalDictWithRegex",
-    "NoneStrings",
-    "NoneStringsAdd",
-    "QuotaStrings",
-    "QuotaStringsAdd",
+    "TLD_RE",
+    "get_last_raw_whois_data",
 ]
 
-
 CACHE_FILE = None
 SLOW_DOWN = 0
 
+LastWhois: Dict[str, Any] = {
+    "Try": [],
+}
+
+
+# PRIVATE
 
-def internationalizedDomainNameToPunyCode(d: List[str]) -> List[str]:
+
+def _internationalizedDomainNameToPunyCode(d: List[str]) -> List[str]:
     return [k.encode("idna").decode() or k for k in d]
 
 
-def result2dict(func):
+def _result2dict(func: Any) -> Any:
     @wraps(func)
-    def _inner(*args, **kw):
+    def _inner(*args: str, **kw: Any) -> Dict[str, Any]:
         r = func(*args, **kw)
         return r and vars(r) or {}
 
     return _inner
 
 
-def fromDomainStringToTld(
+def _fromDomainStringToTld(
     domain: str,
     internationalized: bool,
     verbose: bool = False,
-):
+) -> Tuple[Optional[str], Optional[List[str]]]:
     domain = domain.lower().strip().rstrip(".")  # Remove the trailing dot to support FQDN.
     d: List[str] = domain.split(".")
     if verbose:
         print(d, file=sys.stderr)
 
     if d[0] == "www":
         d = d[1:]
@@ -107,69 +100,88 @@
         return None, None
 
     tld: str = filterTldToSupportedPattern(domain, d, verbose)
     if verbose:
         print(f"filterTldToSupportedPattern returns tld: {tld}", file=sys.stderr)
 
     if internationalized and isinstance(internationalized, bool):
-        d = internationalizedDomainNameToPunyCode(d)
+        d = _internationalizedDomainNameToPunyCode(d)
 
     if verbose:
         print(tld, d, file=sys.stderr)
 
     return tld, d
 
 
-def validateWeKnowTheToplevelDomain(tld, return_raw_text_for_unsupported_tld: bool = False):  # may raise UnknownTld
+def _validateWeKnowTheToplevelDomain(
+    tld: str,
+    return_raw_text_for_unsupported_tld: bool = False,
+) -> Optional[Dict[str, Any]]:
+    # may raise UnknownTld
     if tld not in TLD_RE.keys():
         if return_raw_text_for_unsupported_tld:
             return None
+
         a = f"The TLD {tld} is currently not supported by this package."
         b = "Use validTlds() to see what toplevel domains are supported."
         msg = f"{a} {b}"
         raise UnknownTld(msg)
+
     return TLD_RE.get(tld)
 
 
-def verifyPrivateREgistry(thisTld: Dict):  # may raise WhoisPrivateRegistry
+def _verifyPrivateREgistry(
+    thisTld: Dict[str, Any],
+) -> None:
+    # may raise WhoisPrivateRegistry
     # signal we know the tld but it has no whos or does not respond with any information
     if thisTld.get("_privateRegistry"):
         msg = "This tld has either no whois server or responds only with minimal information"
         raise WhoisPrivateRegistry(msg)
 
 
-def doServerHintsForThisTld(tld: str, thisTld: Dict, server: Optional[str], verbose: bool = False):
+def _doServerHintsForThisTld(
+    tld: str,
+    thisTld: Dict[str, Any],
+    server: Optional[str],
+    verbose: bool = False,
+) -> Optional[str]:
     # allow server hints using "_server" from the tld_regexpr.py file
     thisTldServer = thisTld.get("_server")
     if server is None and thisTldServer:
         server = thisTldServer
         if verbose:
             print(f"using _server hint {server} for tld: {tld}", file=sys.stderr)
     return server
 
 
-def doSlowdownHintForThisTld(tld: str, thisTld, slow_down: int, verbose: bool = False) -> int:
+def _doSlowdownHintForThisTld(
+    tld: str,
+    thisTld: Dict[str, Any],
+    slow_down: int,
+    verbose: bool = False,
+) -> int:
     # allow a configrable slowdown for some tld's
     slowDown = thisTld.get("_slowdown")
     if slow_down == 0 and slowDown and slowDown > 0:
         slow_down = slowDown
         if verbose:
             print(f"using _slowdown hint {slowDown} for tld: {tld}", file=sys.stderr)
     return slow_down
 
 
-def doUnsupportedTldAnyway(
+def _doUnsupportedTldAnyway(
     tld: str,
     dl: List[str],
     ignore_returncode: bool = False,
     slow_down: int = 0,
     server: Optional[str] = None,
     verbose: bool = False,
     wh: str = "whois",
-):
+) -> Optional[Domain]:
     include_raw_whois_text = True
 
     # we will not hunt for possible valid first level domains as we have no actual feedback
 
     whois_str = do_query(
         dl=dl,
         slow_down=slow_down,
@@ -194,38 +206,36 @@
         whois_str=whois_str,
         verbose=verbose,
         include_raw_whois_text=include_raw_whois_text,
         return_raw_text_for_unsupported_tld=True,
     )
 
 
-LastWhois: Dict = {
-    "Try": [],
-}
+# PUBLIC
 
 
-def get_last_raw_whois_data():
+def get_last_raw_whois_data() -> Dict[str, Any]:
     global LastWhois
     return LastWhois
 
 
 def query(
     domain: str,
     force: bool = False,
     cache_file: Optional[str] = None,
     cache_age: int = 60 * 60 * 48,
     slow_down: int = 0,
     ignore_returncode: bool = False,
     server: Optional[str] = None,
     verbose: bool = False,
-    with_cleanup_results=False,
+    with_cleanup_results: bool = False,
     internationalized: bool = False,
     include_raw_whois_text: bool = False,
     return_raw_text_for_unsupported_tld: bool = False,
-    timeout: float = None,
+    timeout: Optional[float] = None,
     cmd: str = "whois",
 ) -> Optional[Domain]:
     """
     force=True          Don't use cache.
     cache_file=<path>   Use file to store cache not only memory.
     cache_age=172800    Cache expiration time for given domain, in seconds
     slow_down=0         Time [s] it will wait after you query WHOIS database.
@@ -248,35 +258,43 @@
     LastWhois["Try"] = []  # init on start of query
 
     wh: str = cmd  # make it compatible with python-whois-extended
 
     assert isinstance(domain, str), Exception("`domain` - must be <str>")
     return_raw_text_for_unsupported_tld = bool(return_raw_text_for_unsupported_tld)
 
-    tld, dl = fromDomainStringToTld(domain, internationalized, verbose)
+    tld, dl = _fromDomainStringToTld(
+        domain,
+        internationalized,
+        verbose,
+    )
     if tld is None:
         return None
 
-    thisTld = validateWeKnowTheToplevelDomain(tld, return_raw_text_for_unsupported_tld)  # may raise UnknownTld
+    dl = cast(List[str], dl)
+    thisTld = _validateWeKnowTheToplevelDomain(
+        tld,
+        return_raw_text_for_unsupported_tld,
+    )  # may raise UnknownTld
     if thisTld is None:
-        return doUnsupportedTldAnyway(
+        return _doUnsupportedTldAnyway(
             tld,
             dl,
             ignore_returncode=ignore_returncode,
             slow_down=slow_down,
             server=server,
             verbose=verbose,
             wh=wh,
         )
 
-    verifyPrivateREgistry(thisTld)  # may raise WhoisPrivateRegistry
-    server = doServerHintsForThisTld(tld, thisTld, server, verbose)
+    _verifyPrivateREgistry(thisTld)  # may raise WhoisPrivateRegistry
+    server = _doServerHintsForThisTld(tld, thisTld, server, verbose)
 
     slow_down = slow_down or SLOW_DOWN
-    slow_down = doSlowdownHintForThisTld(tld, thisTld, slow_down, verbose)
+    slow_down = _doSlowdownHintForThisTld(tld, thisTld, slow_down, verbose)
 
     # if the tld is a multi level we should not move further down than the tld itself
     # we currently allow progressive lookups until we find something:
     # so xxx.yyy.zzz will try both xxx.yyy.zzz and yyy.zzz
     # but if the tld is yyy.zzz we should only try xxx.yyy.zzz
 
     cache_file = cache_file or CACHE_FILE
@@ -326,8 +344,8 @@
         # no result or no domain but we can not reduce any further so we have None
         return None
 
     return None
 
 
 # Add get function to support return result in dictionary form
-get = result2dict(query)
+get = _result2dict(query)
```

### Comparing `whoisdomain-1.20230417.6/whoisdomain/exceptions.py` & `whoisdomain-1.20230424.7/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230424.7/whoisdomain/tld_regexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from typing import Dict
+from typing import (
+    Dict,
+    Any,
+)
 
-ZZ: Dict = {}
+ZZ: Dict[str, Any] = {}
 
 # elements starting with _
 # are meta patterns and are not processed as domains
 # examples:  _donuts, _centralnic
 
 # elements ending in _
 # like id_ , is_, if_, in_, global_ are conflicting words in python without a trailing _
```

### Comparing `whoisdomain-1.20230417.6/.gitignore` & `whoisdomain-1.20230424.7/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230417.6/pyproject.toml` & `whoisdomain-1.20230424.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "whoisdomain"
-version = "1.20230417.6"
+version = "1.20230424.7"
 authors = [
   { name="DannyCork"},
 ]
 
 maintainers = [
   { name="Maarten Boot", email="mboot.github@gmail.com" },
 ]
@@ -43,11 +43,15 @@
     "tld",
     "domain",
     "expiration",
     "cctld",
     "registrar",
 ]
 
+[project.scripts]
+whoisdomain = 'whoisdomain.main:main'
+
 [project.urls]
 "Bug Tracker" = "https://github.com/mboot-github/WhoisDomain/issues"
 "Home Page" = "https://github.com/mboot-github/WhoisDomain/"
 "Repository" = "https://github.com/mboot-github/WhoisDomain/"
+
```

### Comparing `whoisdomain-1.20230417.6/PKG-INFO` & `whoisdomain-1.20230424.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230417.6
+Version: 1.20230424.7
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <mboot.github@gmail.com>
 License-Expression: MIT
@@ -45,14 +45,16 @@
  * Possibility to cache results.
  * Verbose output on stderr during debugging to see how the internal functions are doing their work
  * raise a exception on Quota ecceeded type responses
  * raise a exception on PrivateRegistry tld's where we know the tld and know we don't know anything
  * allow for optional cleaning the response before extracting information
  * optionally allow IDN's to be translated to Punycode
  * optional specify the whois command on query(...,cmd="whois") as in: https://github.com/gen1us2k/python-whois/
+ * the module is now 'mypy --strict' clean
+ * the module now also exports a cli command domainwhois
 
 ## Dependencies
   * please install also the command line "whois" of your distribution
   * this library parses the output of the "whois" cli command of your operating system
 
 ## Usage example
 
@@ -92,17 +94,73 @@
 status             str               'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)'
 statuses           list              ['clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)']
 dnssec             bool              False
 name_servers       list              ['ns1.google.com', 'ns2.google.com', 'ns3.google.com', 'ns4.google.com']
 registrant         str               'Google LLC'
 emails             list              ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com']
 
- {'Try': [{'Domain': 'google.com', 'rawData': '[Querying whois.verisign-grs.com]\n[Redirected to whois.markmonitor.com]\n[Querying whois.markmonitor.com]\n[whois.markmonitor.com]\nDomain Name: google.com\nRegistry Domain ID: 2138514_DOMAIN_COM-VRSN\nRegistrar WHOIS Server: whois.markmonitor.com\nRegistrar URL: http://www.markmonitor.com\nUpdated Date: 2019-09-09T15:39:04+0000\nCreation Date: 1997-09-15T07:00:00+0000\nRegistrar Registration Expiration Date: 2028-09-13T07:00:00+0000\nRegistrar: MarkMonitor, Inc.\nRegistrar IANA ID: 292\nRegistrar Abuse Contact Email: abusecomplaints@markmonitor.com\nRegistrar Abuse Contact Phone: +1.2086851750\nDomain Status: clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)\nDomain Status: clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)\nDomain Status: clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)\nDomain Status: serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)\nDomain Status: serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)\nDomain Status: serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)\nRegistrant Organization: Google LLC\nRegistrant State/Province: CA\nRegistrant Country: US\nRegistrant Email: Select Request Email Form at https://domains.markmonitor.com/whois/google.com\nAdmin Organization: Google LLC\nAdmin State/Province: CA\nAdmin Country: US\nAdmin Email: Select Request Email Form at https://domains.markmonitor.com/whois/google.com\nTech Organization: Google LLC\nTech State/Province: CA\nTech Country: US\nTech Email: Select Request Email Form at https://domains.markmonitor.com/whois/google.com\nName Server: ns1.google.com\nName Server: ns3.google.com\nName Server: ns2.google.com\nName Server: ns4.google.com\nDNSSEC: unsigned\nURL of the ICANN WHOIS Data Problem Reporting System: http://wdprs.internic.net/\n>>> Last update of WHOIS database: 2023-04-17T08:13:22+0000 <<<\n\nFor more information on WHOIS status codes, please visit:\n  https://www.icann.org/resources/pages/epp-status-codes\n\nIf you wish to contact this domain’s Registrant, Administrative, or Technical\ncontact, and such email address is not visible above, you may do so via our web\nform, pursuant to ICANN’s Temporary Specification. To verify that you are not a\nrobot, please enter your email address to receive a link to a page that\nfacilitates email communication with the relevant contact(s).\n\nWeb-based WHOIS:\n  https://domains.markmonitor.com/whois\n\nIf you have a legitimate interest in viewing the non-public WHOIS details, send\nyour request and the reasons for your request to whoisrequest@markmonitor.com\nand specify the domain name in the subject line. We will review that request and\nmay ask for supporting documentation and explanation.\n\nThe data in MarkMonitor’s WHOIS database is provided for information purposes,\nand to assist persons in obtaining information about or related to a domain\nname’s registration record. While MarkMonitor believes the data to be accurate,\nthe data is provided "as is" with no guarantee or warranties regarding its\naccuracy.\n\nBy submitting a WHOIS query, you agree that you will use this data only for\nlawful purposes and that, under no circumstances will you use this data to:\n  (1) allow, enable, or otherwise support the transmission by email, telephone,\nor facsimile of mass, unsolicited, commercial advertising, or spam; or\n  (2) enable high volume, automated, or electronic processes that send queries,\ndata, or email to MarkMonitor (or its systems) or the domain name contacts (or\nits systems).\n\nMarkMonitor reserves the right to modify these terms at any time.\n\nBy submitting this query, you agree to abide by this policy.\n\nMarkMonitor Domain Management(TM)\nProtecting companies and consumers in a digital world.\n\nVisit MarkMonitor at https://www.markmonitor.com\nContact us at +1.8007459229\nIn Europe, at +44.02032062220\n--\n', 'server': None}]}
  ```
 
+A short intro into the cli whoisdomain command
+```
+whoisdomain
+    [ -v | --verbose ]
+        # set verbose to True, this will be forwarded to whois.query
+
+    [ -I | --IgnoreReturncode ]
+        # sets the IgnoreReturncode to True, this will be forwarded to whois.query
+
+    [ -a | --all]
+        # test all existing tld currently supported,
+
+    [ -d <domain> | --domain = <domain> " ]
+        # only analyze the given domains
+        # the option can be repeated to specify more then one domain
+
+    [ -f <filename> | --file = <filename> " ]
+        # use the named file to test all domains (one domain per line)
+        # lines starting with # or empty lines are skipped, anything after the domain is ignored
+        # the option can be repeated to specify more then one file
+
+    [ -D <directory> | --Directory = <directory> " ]
+        # use the named directory, ald use all files ending in .txt as files containing domains
+        # files are processed as in the -f option so comments and empty lines are skipped
+        # the option can be repeated to specify more then one directory
+
+    [ -p | --print ]
+    also print text containing the raw output of whois
+
+    [ -R | --Ruleset ]
+    dump the ruleset for the tld and exit
+
+    [ -S | --SupportedTld ]
+    print all supported top level domains we know and exit
+
+    [ -C <file> | --Cleanup <file> ]
+    read the input file specified and run the same cleanup as in whois.query , then exit
+
+    # options are exclusive and without any options the whoisdomain program does nothing
+
+    # test one specific file with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -f tests/ok-domains.txt 2>2 >out
+
+    # test one specific directory with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -D tests 2>2 >out
+
+    # test two domains with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -d meta.org -d meta.com 2>2 >out
+
+    # test all supported tld's with verbose and IgnoreReturncode
+    example: whoisdomain -v -I -a 2>2 >out
+
+    # test nothing
+    example: whoisdomain -v -I 2>2 >out
+
+```
+
 ## ccTLD & TLD support
 see the file: ./whoisdomain/tld_regexpr.py
 or call whoisdomain.validTlds()
 
 ## Support
  * Python 3.x is supported for x >= 6
  * Python 2.x IS NOT supported.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

