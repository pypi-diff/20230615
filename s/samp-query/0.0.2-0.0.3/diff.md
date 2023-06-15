# Comparing `tmp/samp_query-0.0.2.tar.gz` & `tmp/samp_query-0.0.3.tar.gz`

## Comparing `samp_query-0.0.2.tar` & `samp_query-0.0.3.tar`

### file list

```diff
@@ -1,162 +1,14 @@
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 samp_query-0.0.2/main.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 samp_query-0.0.2/requirements-test.txt
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.0.2/requirements.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 samp_query-0.0.2/setup.cfg
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193664 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57284 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19757 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   186597 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_random.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_random.meta.json
--rw-r--r--   0        0        0   148438 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_socket.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_socket.meta.json
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66369 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1141201 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134205 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113663 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    41312 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextvars.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextvars.meta.json
--rw-r--r--   0        0        0    63243 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    66832 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    95774 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/fractions.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/fractions.meta.json
--rw-r--r--   0        0        0   131240 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/functools.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/functools.meta.json
--rw-r--r--   0        0        0    24392 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93251 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/main.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/main.meta.json
--rw-r--r--   0        0        0    31498 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    90192 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mypy_extensions.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mypy_extensions.meta.json
--rw-r--r--   0        0        0    86256 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0    96566 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48532 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82100 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0    45089 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/random.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/random.meta.json
--rw-r--r--   0        0        0   182913 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    23917 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/select.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/select.meta.json
--rw-r--r--   0        0        0    53813 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/signal.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/signal.meta.json
--rw-r--r--   0        0        0   125399 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/socket.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/socket.meta.json
--rw-r--r--   0        0        0    15195 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30249 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53699 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   204969 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ssl.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ssl.meta.json
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/struct.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/struct.meta.json
--rw-r--r--   0        0        0   173165 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152142 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   248499 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444944 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73947 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    96967 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446258 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140931 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13270 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26983 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86486 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33569 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75523 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69924 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97890 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   382581 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0    26165 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/outcome/__init__.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/outcome/__init__.meta.json
--rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/samp_query/__init__.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/samp_query/__init__.meta.json
--rw-r--r--   0        0        0   346581 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/__init__.data.json
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/__init__.meta.json
--rw-r--r--   0        0        0    58434 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/abc.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/abc.meta.json
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/from_thread.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/from_thread.meta.json
--rw-r--r--   0        0        0    96361 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/lowlevel.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/lowlevel.meta.json
--rw-r--r--   0        0        0    85329 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/socket.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/socket.meta.json
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/to_thread.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/to_thread.meta.json
--rw-r--r--   0        0        0    38045 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio_typing/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio_typing/__init__.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 samp_query-0.0.2/samp_query/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.2/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.2/test/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.2/test/test_client.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.0.2/LICENSE
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.0.2/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 samp_query-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 samp_query-0.0.3/.coverage
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 samp_query-0.0.3/main.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 samp_query-0.0.3/requirements-test.txt
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 samp_query-0.0.3/samp_query/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.3/test/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 samp_query-0.0.3/test/test_client.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.0.3/LICENSE
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.0.3/README.md
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 samp_query-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.0.3/PKG-INFO
```

### Comparing `samp_query-0.0.2/.github/workflows/ci.yml` & `samp_query-0.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.2/samp_query/__init__.py` & `samp_query-0.0.3/samp_query/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import random
 from dataclasses import dataclass, field
 
 import cchardet as chardet  # type: ignore
 import trio
 
 
-def unpack_string(data: bytes) -> tuple[str, bytes]:
-    str_len, data = *struct.unpack_from('<I', data), data[4:]
+def unpack_string(data: bytes, len_type: str = 'I') -> tuple[str, bytes]:
+    format = f'<{len_type}'
+    size = struct.calcsize(format)
+    str_len, data = *struct.unpack_from(format, data), data[size:]
     string, data = data[:str_len], data[str_len:]
     encoding: str = chardet.detect(string)['encoding']
     return string.decode(encoding), data
 
 
 @dataclass
 class ServerInfo:
@@ -40,14 +42,50 @@
             max_players=max_players,
             gamemode=gamemode,
             language=language,
         )
 
 
 @dataclass
+class PlayerInfo:
+    name: str
+    score: int
+
+    @classmethod
+    def from_data(cls, data: bytes) -> tuple[PlayerInfo, bytes]:
+        name, data = unpack_string(data, 'B')
+        score = struct.unpack_from('<i', data)[0]
+        data = data[4:]  # int, see above
+
+        return cls(
+            name=name,
+            score=score,
+        ), data
+
+
+@dataclass
+class PlayerList:
+    players: list[PlayerInfo]
+
+    @classmethod
+    def from_data(cls, data: bytes) -> PlayerList:
+        player_count = struct.unpack_from('<H', data)[0]
+        data = data[2:]  # short, see above
+        players = []
+
+        for _ in range(player_count):
+            player, data = PlayerInfo.from_data(data)
+            players.append(player)
+
+        assert not data  # We consumed all the buffer
+
+        return cls(players=players)
+
+
+@dataclass
 class Client:
     ip: str
     port: int
     rcon_password: str | None = field(default=None, repr=False)
 
     _socket: trio.socket.SocketType | None = field(default=None, repr=False)
     _prefix: bytes | None = field(default=None, repr=False)
@@ -94,7 +132,13 @@
         return trio.current_time() - start_time
 
     async def info(self) -> ServerInfo:
         await self.send(b'i')
         assert self._prefix
         data = await self.receive(header=self._prefix + b'i')
         return ServerInfo.from_data(data)
+
+    async def players(self) -> PlayerList:
+        await self.send(b'c')
+        assert self._prefix
+        data = await self.receive(header=self._prefix + b'c')
+        return PlayerList.from_data(data)
```

### Comparing `samp_query-0.0.2/LICENSE` & `samp_query-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.2/PKG-INFO` & `samp_query-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samp_query
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SAMP query/RCON client for Python using trio.
 Project-URL: Homepage, https://github.com/Cheaterman/samp-query
 Project-URL: Bug Tracker, https://github.com/Cheaterman/samp-query/issues
 Author-email: The Cheaterman <the.cheaterman@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

