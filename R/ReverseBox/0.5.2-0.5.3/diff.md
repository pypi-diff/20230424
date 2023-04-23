# Comparing `tmp/ReverseBox-0.5.2.tar.gz` & `tmp/ReverseBox-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.5.2.tar", last modified: Sun Apr 23 22:22:54 2023, max compression
+gzip compressed data, was "ReverseBox-0.5.3.tar", last modified: Sun Apr 23 22:39:17 2023, max compression
```

## Comparing `ReverseBox-0.5.2.tar` & `ReverseBox-0.5.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.389977 ReverseBox-0.5.2/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.5.2/LICENSE
--rw-rw-rw-   0        0        0     5602 2023-04-23 22:22:54.389977 ReverseBox-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4340 2023-04-22 15:45:22.000000 ReverseBox-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.340765 ReverseBox-0.5.2/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     5602 2023-04-23 22:22:54.000000 ReverseBox-0.5.2/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1805 2023-04-23 22:22:54.000000 ReverseBox-0.5.2/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 22:22:54.000000 ReverseBox-0.5.2/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-23 22:22:54.000000 ReverseBox-0.5.2/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 22:22:54.000000 ReverseBox-0.5.2/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.341765 ReverseBox-0.5.2/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.5.2/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.345870 ReverseBox-0.5.2/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.2/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.5.2/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.5.2/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.5.2/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.348871 ReverseBox-0.5.2/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.5.2/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-15 13:54:42.000000 ReverseBox-0.5.2/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.5.2/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.353055 ReverseBox-0.5.2/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.2/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-23 00:00:01.000000 ReverseBox-0.5.2/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.5.2/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.5.2/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.361223 ReverseBox-0.5.2/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.5.2/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.5.2/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.5.2/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.5.2/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.5.2/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.5.2/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.5.2/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.5.2/reversebox/crc/crc32_iso_hdlc.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.365510 ReverseBox-0.5.2/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.2/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.5.2/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.5.2/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.5.2/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.369511 ReverseBox-0.5.2/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.2/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.5.2/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.5.2/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.5.2/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.373695 ReverseBox-0.5.2/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.5.2/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.5.2/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:01.000000 ReverseBox-0.5.2/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.5.2/reversebox/image/psp_swizzle.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.378813 ReverseBox-0.5.2/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.2/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-23 15:32:28.000000 ReverseBox-0.5.2/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:49.000000 ReverseBox-0.5.2/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:41.000000 ReverseBox-0.5.2/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     6667 2023-04-23 22:20:53.000000 ReverseBox-0.5.2/reversebox/io_files/translation_text_handler.py
--rw-rw-rw-   0        0        0       42 2023-04-23 22:22:54.390977 ReverseBox-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1825 2023-04-23 22:21:32.000000 ReverseBox-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.380813 ReverseBox-0.5.2/tests/
--rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.5.2/tests/__init__.py
--rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.5.2/tests/common.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:22:54.388977 ReverseBox-0.5.2/tests/tests_crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.5.2/tests/tests_crc/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.5.2/tests/tests_crc/test_crc16_arc.py
--rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.5.2/tests/tests_crc/test_crc16_ccitt.py
--rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.5.2/tests/tests_crc/test_crc16_dnp.py
--rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.5.2/tests/tests_crc/test_crc16_kermit.py
--rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.5.2/tests/tests_crc/test_crc16_modbus.py
--rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.5.2/tests/tests_crc/test_crc16_sick.py
--rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:01.000000 ReverseBox-0.5.2/tests/tests_crc/test_crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.088637 ReverseBox-0.5.3/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     5602 2023-04-23 22:39:17.088637 ReverseBox-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2023-04-22 15:45:22.000000 ReverseBox-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.040468 ReverseBox-0.5.3/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     5602 2023-04-23 22:39:16.000000 ReverseBox-0.5.3/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1805 2023-04-23 22:39:16.000000 ReverseBox-0.5.3/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 22:39:16.000000 ReverseBox-0.5.3/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-23 22:39:16.000000 ReverseBox-0.5.3/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 22:39:16.000000 ReverseBox-0.5.3/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.041469 ReverseBox-0.5.3/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.5.3/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.045609 ReverseBox-0.5.3/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.3/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.5.3/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.5.3/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.5.3/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.048610 ReverseBox-0.5.3/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.5.3/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-15 13:54:42.000000 ReverseBox-0.5.3/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.5.3/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.052694 ReverseBox-0.5.3/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.3/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-23 00:00:01.000000 ReverseBox-0.5.3/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.5.3/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.5.3/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.060890 ReverseBox-0.5.3/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.5.3/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.5.3/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.5.3/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.5.3/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.5.3/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.5.3/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.5.3/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.5.3/reversebox/crc/crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.065220 ReverseBox-0.5.3/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.3/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.5.3/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.5.3/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.5.3/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.069221 ReverseBox-0.5.3/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.3/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.5.3/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.5.3/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.5.3/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.073222 ReverseBox-0.5.3/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.5.3/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.5.3/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:01.000000 ReverseBox-0.5.3/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.5.3/reversebox/image/psp_swizzle.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.078591 ReverseBox-0.5.3/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.3/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-23 15:32:28.000000 ReverseBox-0.5.3/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:49.000000 ReverseBox-0.5.3/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:41.000000 ReverseBox-0.5.3/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     7061 2023-04-23 22:36:29.000000 ReverseBox-0.5.3/reversebox/io_files/translation_text_handler.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 22:39:17.088637 ReverseBox-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2023-04-23 22:37:07.000000 ReverseBox-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.080591 ReverseBox-0.5.3/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.5.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.5.3/tests/common.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:39:17.088637 ReverseBox-0.5.3/tests/tests_crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.5.3/tests/tests_crc/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.5.3/tests/tests_crc/test_crc16_arc.py
+-rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.5.3/tests/tests_crc/test_crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.5.3/tests/tests_crc/test_crc16_dnp.py
+-rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.5.3/tests/tests_crc/test_crc16_kermit.py
+-rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.5.3/tests/tests_crc/test_crc16_modbus.py
+-rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.5.3/tests/tests_crc/test_crc16_sick.py
+-rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:01.000000 ReverseBox-0.5.3/tests/tests_crc/test_crc32_iso_hdlc.py
```

### Comparing `ReverseBox-0.5.2/LICENSE` & `ReverseBox-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/PKG-INFO` & `ReverseBox-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.5.2
+Version: 0.5.3
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ReverseBox-0.5.2/README.md` & `ReverseBox-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.5.3/ReverseBox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.5.2
+Version: 0.5.3
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ReverseBox-0.5.2/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.5.3/ReverseBox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/common/logger.py` & `ReverseBox-0.5.3/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/crc/crc16_arc.py` & `ReverseBox-0.5.3/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.5.3/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.5.3/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.5.3/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.5.3/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/crc/crc16_sick.py` & `ReverseBox-0.5.3/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.5.3/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.5.3/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.5.3/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.5.3/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/image/image_finder_gui.py` & `ReverseBox-0.5.3/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/image/image_finder_main.py` & `ReverseBox-0.5.3/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/image/psp_swizzle.py` & `ReverseBox-0.5.3/reversebox/image/psp_swizzle.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.5.3/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/io_files/check_file.py` & `ReverseBox-0.5.3/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/io_files/file_handler.py` & `ReverseBox-0.5.3/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.5.3/reversebox/io_files/translation_text_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,16 +107,27 @@
                 logger.error(
                     f"Couldn't decode entry at offset {translation_entry.text_offset}. "
                     f"Error: {error}"
                 )
                 self.close()
                 return False
 
+            comment_text: str = (
+                f"text_offset={translation_entry.text_offset} | "
+                f"export_length={translation_entry.text_export_length} | "
+                f"import_length={translation_entry.text_import_length}"
+            )
+
             output_po_file.append(
-                polib.POEntry(msgctxt=text_entry_key, msgid=text_entry_str, msgstr="")
+                polib.POEntry(
+                    msgctxt=text_entry_key,
+                    msgid=text_entry_str,
+                    msgstr="",
+                    comment=comment_text,
+                )
             )
         try:
             output_po_file.save(output_po_file_path)
         except Exception:
             logger.error(f"Couldn't save po file to path: {output_po_file_path}")
             self.close()
             return False
```

### Comparing `ReverseBox-0.5.2/setup.py` & `ReverseBox-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.5.2"
+VERSION_NUM = "0.5.3"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

### Comparing `ReverseBox-0.5.2/tests/common.py` & `ReverseBox-0.5.3/tests/common.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/tests/tests_crc/test_crc16_arc.py` & `ReverseBox-0.5.3/tests/tests_crc/test_crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/tests/tests_crc/test_crc16_ccitt.py` & `ReverseBox-0.5.3/tests/tests_crc/test_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/tests/tests_crc/test_crc16_dnp.py` & `ReverseBox-0.5.3/tests/tests_crc/test_crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/tests/tests_crc/test_crc16_kermit.py` & `ReverseBox-0.5.3/tests/tests_crc/test_crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/tests/tests_crc/test_crc16_modbus.py` & `ReverseBox-0.5.3/tests/tests_crc/test_crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/tests/tests_crc/test_crc16_sick.py` & `ReverseBox-0.5.3/tests/tests_crc/test_crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.5.2/tests/tests_crc/test_crc32_iso_hdlc.py` & `ReverseBox-0.5.3/tests/tests_crc/test_crc32_iso_hdlc.py`

 * *Files identical despite different names*

