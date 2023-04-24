# Comparing `tmp/monobit-0.39.3.tar.gz` & `tmp/monobit-0.40.0.tar.gz`

## Comparing `monobit-0.39.3.tar` & `monobit-0.40.0.tar`

### file list

```diff
@@ -1,500 +1,510 @@
--rw-r--r--   0        0        0    26365 2020-02-02 00:00:00.000000 monobit-0.39.3/YAFF.md
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.39.3/banner.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.39.3/convert.py
--rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.39.3/explore.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/__init__.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/basetypes.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/binary.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/canvas.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/chart.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/constants.py
--rw-r--r--   0        0        0    57985 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/encoding.py
--rw-r--r--   0        0        0    47781 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/font.py
--rw-r--r--   0        0        0    29683 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/glyph.py
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/labels.py
--rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/magic.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/pack.py
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/properties.py
--rw-r--r--   0        0        0    20080 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/raster.py
--rw-r--r--   0        0        0    13621 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/renderer.py
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripting.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/storage.py
--rw-r--r--   0        0        0     7711 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/streams.py
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/struct.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/taggers.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/vector.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/__init__.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/ReadMe.txt
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/stdenc.txt
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/symbol.txt
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/adobe/zdingbat.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/LICENSE.md
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/README.md
--rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/aglfn.txt
--rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/agl/glyphlist.txt
--rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ARABIC.TXT
--rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CELTIC.TXT
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CENTEURO.TXT
--rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CHINSIMP.TXT
--rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CHINTRAD.TXT
--rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CORPCHAR.TXT
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CROATIAN.TXT
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/CYRILLIC.TXT
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/DEVANAGA.TXT
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/DINGBATS.TXT
--rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/FARSI.TXT
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GAELIC.TXT
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GREEK.TXT
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GUJARATI.TXT
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/GURMUKHI.TXT
--rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/HEBREW.TXT
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ICELAND.TXT
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/INUIT.TXT
--rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/JAPANESE.TXT
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/KEYBOARD.TXT
--rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/KOREAN.TXT
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ROMAN.TXT
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ROMANIAN.TXT
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/ReadMe.txt
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/SYMBOL.TXT
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/THAI.TXT
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/TURKISH.TXT
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/apple/UKRAINE.TXT
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/README.md
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/bulgarian-mik.txt
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/cp866.txt
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/gost19768-87.txt
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/hp-roman8.txt
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi-0.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi-7.txt
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-a.txt
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-b.txt
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-e.txt
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-f.txt
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-r.txt
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/czyborra/koi8-u.txt
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca2
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-cn
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-cu
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-de
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-dk
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-es
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-es2
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-fr
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-gb
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-hu
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-it
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp-ocr-b
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-kr
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-us
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/iso646-yu
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/jis_x0201
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/dkuug/x0201-7
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-ethiopic.map
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-ipa.map
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-is13194.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-lviscii.map
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-sisheng.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-tibetan.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/MULE-uviscii.map
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/emacs/README.md
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/evertype/ARMENIAN.TXT
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/evertype/GEORGIAN.TXT
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/evertype/README.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1116.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1117.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1118.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1119.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1125.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/113.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/1131.ucp
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30000.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30001.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30002.ucp
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30003.ucp
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30004.ucp
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30005.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30006.ucp
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30007.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30008.ucp
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30009.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30010.ucp
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30011.ucp
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30013.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30014.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30015.ucp
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30016.ucp
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30017.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30018.ucp
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30019.ucp
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30020.ucp
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30021.ucp
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30022.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30023.ucp
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30024.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30025.ucp
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30026.ucp
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30027.ucp
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30028.ucp
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30029.ucp
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30030.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30031.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30032.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30033.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30034.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30039.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/30040.ucp
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3021.ucp
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3845.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3846.ucp
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/3848.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/437.ucp
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/57781.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/58152.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/58210.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/58335.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/59234.ucp
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/59829.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/60258.ucp
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/60853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/61282.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/62306.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/667.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/668.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/737.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/770.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/771.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/772.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/773.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/774.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/775.ucp
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/777.ucp
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/778.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/790.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/808.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/848.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/849.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/850.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/851.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/852.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/855.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/856.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/857.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/858.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/859.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/860.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/861.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/862.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/863.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/864.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/865.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/866.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/867.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/869.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/872.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/895.ucp
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/899.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/991.ucp
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/freedos/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iana/Amiga-1251
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iana/PTCP154
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iana/README.md
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
--rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
--rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/ibm-cdra/readme.txt
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/README.md
--rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
--rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/cns-11643-1992.ucm
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
--rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-720_P100-1997.ucm
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-806_P100-1998.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-851_P100-1995.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-858_P100-1997.ucm
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-868_P100-1995.ucm
--rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/ibm-932_P120-1999.ucm
--rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/windows-1361-2000.ucm
--rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/icu/windows-936-2000.ucm
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-1.TXT
--rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-10.TXT
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-11.TXT
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-13.TXT
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-14.TXT
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-15.TXT
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-16.TXT
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-2.TXT
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-3.TXT
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-4.TXT
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-5.TXT
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-6.TXT
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-7.TXT
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-8.TXT
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/8859-9.TXT
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/iso-8859/ReadMe.txt
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMOS7.TXT
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPC.TXT
--rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPM.TXT
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT1.TXT
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT2.TXT
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ICHG.TXT
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/APL2PRIM.TXT
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8IG.TXT
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8II.TXT
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VG.TXT
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VI.TXT
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTI.TXT
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTV.TXT
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64IALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64IPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64VALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/C64VPRI.TXT
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/COCOICHG.TXT
--rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR4.TXT
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR6.TXT
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIALT.TXT
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIPRI.TXT
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVALT.TXT
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVPRI.TXT
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVPRI.TXT
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCICH.TXT
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCVID.TXT
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG0.TXT
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG1.TXT
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/MSX.TXT
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG0.TXT
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG1.TXT
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCEFF.TXT
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSB.TXT
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSI.TXT
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSV.TXT
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ReadMe.txt
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/SINCLRQL.TXT
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG0.TXT
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG1.TXT
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG2.TXT
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG3.TXT
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TI994A.TXT
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1REV.TXT
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZX80.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZX81.TXT
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/currency-sign-0x9c.ucp
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/currency-sign-0xdb.ucp
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/dec-vt100.ucp
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/hp48.txt
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/ibm897graph.ucp
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/mac-system.ucp
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/ms-linedraw.txt
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/russup3.ucp
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/russup4ac.ucp
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/russup4na.ucp
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/windows-1.0.txt
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/windows-2.0.txt
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/manual/windows-3.1.txt
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/GREEK.TXT
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/ICELAND.TXT
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/LATIN2.TXT
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/ROMAN.TXT
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/MAC/TURKISH.TXT
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP437.TXT
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP737.TXT
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP775.TXT
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP850.TXT
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP852.TXT
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP855.TXT
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP857.TXT
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP860.TXT
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP861.TXT
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP862.TXT
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP863.TXT
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP864.TXT
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP865.TXT
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP866.TXT
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP869.TXT
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/PC/CP874.TXT
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
--rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
--rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
--rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
--rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/APL-ISO-IR-68.TXT
--rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/ATARIST.TXT
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/CP1006.TXT
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/CP424.TXT
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/CP856.TXT
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/GSM0338.TXT
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/IBMGRAPH.TXT
--rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/JIS0208.TXT
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KOI8-R.TXT
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KOI8-U.TXT
--rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KPS9566.TXT
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/KZ1048.TXT
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/NEXTSTEP.TXT
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/README.md
--rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/SGML.TXT
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/dashen-map.txt
--rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/misc/ibm-ugl.txt
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ALTVAR.TXT
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-7.TXT
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8.TXT
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8A.TXT
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/DECMCS.TXT
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/GEO-ITA.TXT
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/GEO-PS.TXT
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/IRANSYSTEM.TXT
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/KOI8RU.TXT
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/OSNOVAR.TXT
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/README.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/mleisher/TIS620.TXT
--rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/moztw/big5_2003-b2u.txt
--rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/moztw/eten.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/moztw/url
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/README.md
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/TCVN5712-1.TXT
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/TCVN5712-2.TXT
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/python/TCVN5712-3.TXT
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/vietstd/unicode.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/vietstd/url
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/vietstd/viscii1.1.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/README.md
--rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/abicomp.html
--rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/brascii.html
--rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/cp853.html
--rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/cwi2.html
--rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/dec-special.html
--rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/dec-technical.html
--rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/gem.html
--rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/kamenicky.html
--rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/lics.html
--rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/mattel-aquarius.html
--rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/mazovia.html
--rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/pascii.html
--rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/ventura.html
--rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/windows-1252.html
--rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/wingdings.html
--rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/wikipedia/wiscii.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/README.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-0.enc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-1.enc
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-2.enc
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/mulelao-1.enc
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/suneu-greek.enc
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/charmaps/xfonts/viscii1.1-1.enc
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/compressors.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/container.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/directory.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/mac.py
--rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/source.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/tar.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/containers/zip.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/__init__.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/amiga.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/bbc.py
--rw-r--r--   0        0        0    41624 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/bdf.py
--rw-r--r--   0        0        0    41746 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/bmfont.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/borland.py
--rw-r--r--   0        0        0    22614 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/cpi.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/daisydot.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/dashen.py
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/dec.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/dosstart.py
--rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/figlet.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/fontx.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/fzx.py
--rw-r--r--   0        0        0    26397 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/gdos.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/geos.py
--rw-r--r--   0        0        0    18471 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hbf.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hex.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hexdraw.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/hurt.py
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/image.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mousegraphics.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mzfon.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/nearlyraw.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/palm.py
--rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pcl.py
--rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pcpaint.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pdf.py
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/pkfont.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/printshop.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/psf.py
--rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/raw.py
--rw-r--r--   0        0        0    28660 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/sfnt.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/signum.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/svg.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/vfont.py
--rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/yaff.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/dfont.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/fond.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/iigs.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/lisa.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/mac/nfnt.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/__init__.py
--rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/gpifont.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/lx.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/os2/ne.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/LICENSE.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/__init__.py
--rw-r--r--   0        0        0    33202 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/fnt.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/mz.py
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/ne.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/formats/windows/pe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripts/__init__.py
--rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripts/banner.py
--rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.39.3/monobit/scripts/convert.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.39.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.39.3/LICENSE
--rw-r--r--   0        0        0    17179 2020-02-02 00:00:00.000000 monobit-0.39.3/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.39.3/pyproject.toml
--rw-r--r--   0        0        0    19132 2020-02-02 00:00:00.000000 monobit-0.39.3/PKG-INFO
+-rw-r--r--   0        0        0    26847 2020-02-02 00:00:00.000000 monobit-0.40.0/YAFF.md
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.40.0/banner.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.40.0/convert.py
+-rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.40.0/explore.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/__init__.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/basetypes.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/binary.py
+-rw-r--r--   0        0        0     7452 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/cachedprops.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/canvas.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/chart.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/constants.py
+-rw-r--r--   0        0        0    57985 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/encoding.py
+-rw-r--r--   0        0        0    48755 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/font.py
+-rw-r--r--   0        0        0    31744 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/glyph.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/labels.py
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/magic.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/pack.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/properties.py
+-rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/raster.py
+-rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/renderer.py
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripting.py
+-rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/storage.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/streams.py
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/struct.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/taggers.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/vector.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/__init__.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/ReadMe.txt
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/stdenc.txt
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/symbol.txt
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/adobe/zdingbat.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/LICENSE.md
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/README.md
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/aglfn.txt
+-rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/agl/glyphlist.txt
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ARABIC.TXT
+-rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CELTIC.TXT
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CENTEURO.TXT
+-rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CHINSIMP.TXT
+-rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CHINTRAD.TXT
+-rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CORPCHAR.TXT
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CROATIAN.TXT
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/CYRILLIC.TXT
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/DEVANAGA.TXT
+-rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/DINGBATS.TXT
+-rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/FARSI.TXT
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GAELIC.TXT
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GREEK.TXT
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GUJARATI.TXT
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/GURMUKHI.TXT
+-rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/HEBREW.TXT
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ICELAND.TXT
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/INUIT.TXT
+-rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/JAPANESE.TXT
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/KEYBOARD.TXT
+-rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/KOREAN.TXT
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ROMAN.TXT
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ROMANIAN.TXT
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/ReadMe.txt
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/SYMBOL.TXT
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/THAI.TXT
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/TURKISH.TXT
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/apple/UKRAINE.TXT
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/README.md
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/bulgarian-mik.txt
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/cp866.txt
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/gost19768-87.txt
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/hp-roman8.txt
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi-0.txt
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi-7.txt
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-a.txt
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-b.txt
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-e.txt
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-f.txt
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-r.txt
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/czyborra/koi8-u.txt
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca2
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-cn
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-cu
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-de
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-dk
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-es
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-es2
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-fr
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-gb
+-rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-hu
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-it
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp-ocr-b
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-kr
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-us
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/iso646-yu
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/jis_x0201
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/dkuug/x0201-7
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-ethiopic.map
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-ipa.map
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-is13194.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-lviscii.map
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-sisheng.map
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-tibetan.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/MULE-uviscii.map
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/emacs/README.md
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/evertype/ARMENIAN.TXT
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/evertype/GEORGIAN.TXT
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/evertype/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1116.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1117.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1118.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1119.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1125.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/113.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/1131.ucp
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30000.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30001.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30002.ucp
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30003.ucp
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30004.ucp
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30005.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30006.ucp
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30007.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30008.ucp
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30009.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30010.ucp
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30011.ucp
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30013.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30014.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30015.ucp
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30016.ucp
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30017.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30018.ucp
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30019.ucp
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30020.ucp
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30021.ucp
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30022.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30023.ucp
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30024.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30025.ucp
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30026.ucp
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30027.ucp
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30028.ucp
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30029.ucp
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30030.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30031.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30032.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30033.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30034.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30039.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/30040.ucp
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3021.ucp
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3845.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3846.ucp
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/3848.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/437.ucp
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/57781.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/58152.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/58210.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/58335.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/59234.ucp
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/59829.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/60258.ucp
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/60853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/61282.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/62306.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/667.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/668.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/737.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/770.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/771.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/772.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/773.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/774.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/775.ucp
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/777.ucp
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/778.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/790.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/808.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/848.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/849.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/850.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/851.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/852.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/855.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/856.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/857.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/858.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/859.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/860.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/861.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/862.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/863.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/864.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/865.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/866.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/867.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/869.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/872.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/895.ucp
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/899.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/991.ucp
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/README.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/freedos/__init__.py
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iana/Amiga-1251
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iana/PTCP154
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iana/README.md
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
+-rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
+-rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/ibm-cdra/readme.txt
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/README.md
+-rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
+-rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/cns-11643-1992.ucm
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
+-rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm
+-rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm
+-rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/windows-1361-2000.ucm
+-rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/icu/windows-936-2000.ucm
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-1.TXT
+-rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-10.TXT
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-11.TXT
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-13.TXT
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-14.TXT
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-15.TXT
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-16.TXT
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-2.TXT
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-3.TXT
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-4.TXT
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-5.TXT
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-6.TXT
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-7.TXT
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-8.TXT
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/8859-9.TXT
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/iso-8859/ReadMe.txt
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPC.TXT
+-rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPM.TXT
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8II.TXT
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTI.TXT
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTV.TXT
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64IALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64IPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64VALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/C64VPRI.TXT
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/COCOICHG.TXT
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIALT.TXT
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVALT.TXT
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG0.TXT
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG1.TXT
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/MSX.TXT
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG0.TXT
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG1.TXT
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCEFF.TXT
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSB.TXT
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSI.TXT
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSV.TXT
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ReadMe.txt
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TI994A.TXT
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZX80.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZX81.TXT
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/currency-sign-0x9c.ucp
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/currency-sign-0xdb.ucp
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/dec-vt100.ucp
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/hp48.txt
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/ibm897graph.ucp
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/mac-system.ucp
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/ms-linedraw.txt
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/russup3.ucp
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/russup4ac.ucp
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/russup4na.ucp
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/windows-1.0.txt
+-rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/windows-2.0.txt
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/manual/windows-3.1.txt
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/GREEK.TXT
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP437.TXT
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP737.TXT
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP775.TXT
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP850.TXT
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP852.TXT
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP855.TXT
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP857.TXT
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP860.TXT
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP861.TXT
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP862.TXT
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP863.TXT
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP864.TXT
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP865.TXT
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP866.TXT
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP869.TXT
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/PC/CP874.TXT
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
+-rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
+-rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
+-rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
+-rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/ATARIST.TXT
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/CP1006.TXT
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/CP424.TXT
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/CP856.TXT
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/GSM0338.TXT
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/IBMGRAPH.TXT
+-rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/JIS0208.TXT
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KOI8-R.TXT
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KOI8-U.TXT
+-rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KPS9566.TXT
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/KZ1048.TXT
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/NEXTSTEP.TXT
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/README.md
+-rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/SGML.TXT
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/dashen-map.txt
+-rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/misc/ibm-ugl.txt
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ALTVAR.TXT
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-7.TXT
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8.TXT
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/DECMCS.TXT
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/GEO-ITA.TXT
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/GEO-PS.TXT
+-rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/KOI8RU.TXT
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/OSNOVAR.TXT
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/README.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/mleisher/TIS620.TXT
+-rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/moztw/big5_2003-b2u.txt
+-rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/moztw/eten.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/moztw/url
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/README.md
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/TCVN5712-1.TXT
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/TCVN5712-2.TXT
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/python/TCVN5712-3.TXT
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/vietstd/unicode.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/vietstd/url
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/vietstd/viscii1.1.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/README.md
+-rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/abicomp.html
+-rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/brascii.html
+-rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/cp853.html
+-rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/cwi2.html
+-rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/dec-special.html
+-rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/dec-technical.html
+-rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/gem.html
+-rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/kamenicky.html
+-rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/lics.html
+-rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/mattel-aquarius.html
+-rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/mazovia.html
+-rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/pascii.html
+-rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/ventura.html
+-rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/windows-1252.html
+-rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/wingdings.html
+-rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/wikipedia/wiscii.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/README.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-0.enc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-1.enc
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-2.enc
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/mulelao-1.enc
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/suneu-greek.enc
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/charmaps/xfonts/viscii1.1-1.enc
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/__init__.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/compressors.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/container.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/directory.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/mac.py
+-rw-r--r--   0        0        0    14707 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/source.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/tar.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/containers/zip.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/__init__.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/amiga.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/bbc.py
+-rw-r--r--   0        0        0    41746 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/bmfont.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/borland.py
+-rw-r--r--   0        0        0    22614 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/cpi.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/daisydot.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/dashen.py
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/dec.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/dosstart.py
+-rw-r--r--   0        0        0    11129 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/figlet.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/fontx.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/fzx.py
+-rw-r--r--   0        0        0    26402 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/gdos.py
+-rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/geos.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/hurt.py
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/image.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mousegraphics.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mzfon.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/nearlyraw.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/palm.py
+-rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pcl.py
+-rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pcpaint.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pdf.py
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/pkfont.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/printshop.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/psf.py
+-rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/raw.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/signum.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/svg.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/vfont.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/__init__.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/dfont.py
+-rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/fond.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/iigs.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/lisa.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/mac/nfnt.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/__init__.py
+-rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/gpifont.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/lx.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/os2/ne.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/__init__.py
+-rw-r--r--   0        0        0    30773 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/sfnt.py
+-rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/sfnt_writer.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/E_B_S_C_.py
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/_b_d_a_t.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/_b_h_e_d.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/sfnt/fonttools/_b_l_o_c.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/__init__.py
+-rw-r--r--   0        0        0    15992 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/draw.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/hex.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/text/yaff.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/LICENSE.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/__init__.py
+-rw-r--r--   0        0        0    33222 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/fnt.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/mz.py
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/ne.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/windows/pe.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/xlfd/__init__.py
+-rw-r--r--   0        0        0    41619 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/xlfd/bdf.py
+-rw-r--r--   0        0        0    18491 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/formats/xlfd/hbf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripts/__init__.py
+-rwxr-xr-x   0        0        0     9148 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripts/banner.py
+-rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.40.0/monobit/scripts/convert.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.40.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.40.0/LICENSE
+-rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 monobit-0.40.0/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.40.0/pyproject.toml
+-rw-r--r--   0        0        0    19692 2020-02-02 00:00:00.000000 monobit-0.40.0/PKG-INFO
```

### Comparing `monobit-0.39.3/YAFF.md` & `monobit-0.40.0/YAFF.md`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,15 @@
   - `proportional`: glyphs have different advance widths, e.g. `M` is wider than `i`.
   - `monospace`: all glyphs have the same advance width.
   - `character-cell`: all glyphs can be defined on a raster of fixed size and displayed without overlap.
   - `multi-cell`: like `character-cell`, but some glyphs may take up two cells.
 
 Characteristics that give a font's identity are:
 - `family`: typeface or font family name
+- `subfamily`: additional font name components; usually style, weight, slant
 - `point-size`: nominal size of the font in points
 - `name`: full name of the font
 - `revision`: version
 
 Font description characteristics that can be used to compare different fonts in a family:
 - `style`: e.g. `serif`, `sans`, ...
 - `weight`: e.g. `bold`, `normal`, `light`, ...
@@ -392,17 +393,26 @@
 Or they can be related to processing:
 - `converter`: software used to produce the present file, e.g. `monobit`.
 - `source-name`: file name from which the font was originally extracted.
 - `source-format`: file format from which the font was originally extracted.
 - `history`: summary of processing steps applied since extraction.
 
 
+##### Encoding parameters
+
+_Encoding parameters_ affect how text is converted into glyphs.
+
+- `encoding`: name of the codepage or encoding that matches codepoints to characters, e.g. `unicode`, `oem-437`.
+- `default-char`: label indicating the glyph to be used as the _missing_, _undefined_ or _default_ glyph
+- `word-boundary`: label indicating the glyph to be used as a word boundary. Usually u+0020 (space).
+
+
 ##### Stroke definitions
 
-- `path` is a special glyph property that contains a stroke sequence describing
+- `path` is a glyph property that contains a stroke sequence describing
     how to draw the glyph. The stroke path is defined as a sequence of straight lines
     and moves to be applied sequentially, starting from the glyph origin.
     Path elements are given as a keyword followed by relative x,y offsets where the x coordinate
     increases rightward and the y coordinate increases upward.
         `m` _x_ _y_ moves _x_ design units to the right and _y_ design units up
         `l` _x_ _y_ draws a line _x_ design units to the right and _y_ design units up
     Stroke definitions are scalable and can be converted to pixel values by applying
```

### Comparing `monobit-0.39.3/explore.py` & `monobit-0.40.0/explore.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/__init__.py` & `monobit-0.40.0/monobit/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/basetypes.py` & `monobit-0.40.0/monobit/basetypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 def passthrough(var):
     """Passthrough type."""
     return var
 
 def to_int(int_str):
     """Convert from int-like or string in any representation."""
+    if isinstance(int_str, int):
+        return int_str
     try:
         # '0xFF' - hex
         # '0o77' - octal
         # '99' - decimal
         return int(int_str, 0)
     except (TypeError, ValueError):
         # '099' - ValueError above, OK as decimal
```

### Comparing `monobit-0.39.3/monobit/binary.py` & `monobit-0.40.0/monobit/binary.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/canvas.py` & `monobit-0.40.0/monobit/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 
 from .raster import Raster, blockstr
 
 
 class Canvas(Raster):
     """Mutable raster."""
 
-    _sequence = list
+    _inner = list
+    _outer = list
+    _0 = 0
+    _1 = 1
+    _itemtype = int
 
     @classmethod
     def blank(cls, width, height, fill=-1):
         """Create a canvas in background colour."""
         canvas = [[fill]*width for _ in range(height)]
         # setting 0 and 1 will make Raster init leave the input alone
         return cls(canvas, _0=0, _1=1)
```

### Comparing `monobit-0.39.3/monobit/chart.py` & `monobit-0.40.0/monobit/chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 def grid_map(
         font,
         columns=32, margin=(0, 0), padding=(0, 0),
         order='row-major', direction=(1, -1),
     ):
     """Create glyph map for font chart matrix."""
-    font = font.equalise_horizontal()
     padding = Coord(*padding)
     margin = Coord(*margin)
     # work out image geometry
     step_x = font.raster_size.x + padding.x
     step_y = font.raster_size.y + padding.y
     rows = ceildiv(len(font.glyphs), columns)
     # output glyph map
```

### Comparing `monobit-0.39.3/monobit/encoding.py` & `monobit-0.40.0/monobit/encoding.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/font.py` & `monobit-0.40.0/monobit/font.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,40 +15,40 @@
 from .raster import turn_method
 from .basetypes import Coord, Bounds
 from .basetypes import to_int
 from .encoding import charmaps, encoder
 from .taggers import tagger
 from .labels import Tag, Char, Codepoint, Label, to_label
 from .binary import ceildiv
-from .properties import (
-    extend_string, DefaultProps, normalise_property, as_tuple,
-    writable_property, checked_property
-)
+from .properties import normalise_property, extend_string
+from .cachedprops import DefaultProps, writable_property, as_tuple, checked_property
 from .taggers import tagmaps
 
 
 # sentinel object
 NOT_SET = object()
 
 
-# pylint: disable=redundant-keyword-arg, no-member
-
 ###############################################################################
-# property management
+# font class
 
+# pylint: disable=redundant-keyword-arg, no-member
+class Font(DefaultProps):
+    """Representation of font, including glyphs and metadata."""
 
-# recognised yaff properties and converters from str
-# this also defines the default order in yaff files
-class FontProperties(DefaultProps):
+    # recognised properties and converters from str
+    # this also defines the default order in yaff files
 
     # naming - can be determined from source file if needed
     # full human name
     name: str
     # typeface/font family
     family: str
+    # further specifiers
+    subfamily: str
     # unique id
     font_id: str
 
     # font metadata
     # can't be calculated
     # author or issuer
     author: str
@@ -131,15 +131,15 @@
     # can't be calculated, affect rendering
 
     # vertical distance between consecutive baselines, in pixels
     line_height: int
     # horizontal distance between consecutive baselines, in pixels
     line_width: int
 
-    # character properties
+    # encoding parameters
     # can't be calculated, affect rendering
 
     # character map, stored as normalised name
     encoding: charmaps.normalise
     # replacement for missing glyph
     default_char: Label
     # word-break character (usually space)
@@ -190,36 +190,48 @@
     history: str
 
     # type converters for compatibility synonyms
     average_advance: float
     max_advance: int
     cap_advance: int
 
+    # non-overridable, for pylint's benefit
+    raster: Bounds
+
+    __properties_start__ = True
+
     @writable_property
     def name(self):
         """Full human-friendly name."""
+        if self.spacing in ('character-cell', 'multi-cell'):
+            size = 'x'.join(str(_x) for _x in self.cell_size)
+        else:
+            size = str(self.point_size)
+        return ' '.join(
+            _x for _x in (self.family, self.subfamily, size) if _x
+        )
+
+    @writable_property
+    def subfamily(self):
+        """Font additional names."""
         if self.slant == self._get_default('slant'):
             slant = ''
         else:
             # title-case
             slant = self.slant.title()
         if self.setwidth == self._get_default('setwidth'):
             setwidth = ''
         else:
             setwidth = self.setwidth.title()
         if (slant or setwidth) and self.weight == self._get_default('weight'):
             weight = ''
         else:
             weight = self.weight.title()
-        if self.spacing in ('character-cell', 'multi-cell'):
-            size = 'x'.join(str(_x) for _x in self.cell_size)
-        else:
-            size = str(self.point_size)
         return ' '.join(
-            str(_x) for _x in (self.family, setwidth, weight, slant, size) if _x
+            _x for _x in (setwidth, weight, slant) if _x
         )
 
     @writable_property
     def family(self):
         """Name of font family."""
         # use source name if no family name defined
         stem = PurePath(self.source_name).stem
@@ -256,25 +268,25 @@
         # stretch/shrink dpi.x if aspect ratio is not square
         return Coord((dpi*self.pixel_aspect.x)//self.pixel_aspect.y, dpi)
 
     @writable_property
     def encoding(self):
         """Encoding."""
         # if we have no codepoints, we can always assume unicode encoding
-        if self._font.get_chars() and not self._font.get_codepoints():
+        if self.get_chars() and not self.get_codepoints():
             return charmaps.normalise('unicode')
         return ''
 
     ##########################################################################
     # metrics
 
     @writable_property
     def line_height(self):
         """Vertical distance between consecutive baselines, in pixels."""
-        if 'leading' in vars(self):
+        if self._defined('leading') is not None:
             return self.pixel_size + self.leading
         return max(self.raster_size.y, self.pixel_size)
 
     @writable_property
     def line_width(self):
         """Horizontal distance between consecutive baselines, in pixels."""
         return self.max_width
@@ -285,47 +297,47 @@
 
     @writable_property
     def ascent(self):
         """
         Recommended typographic ascent relative to baseline.
         Defaults to ink-top.
         """
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 0
         return max(0, self.ink_bounds.top)
 
     @writable_property
     def descent(self):
         """
         Recommended typographic descent relative to baseline.
         Defaults to ink-bottom.
         """
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 0
         # if ink bounds go below the baseline, use them as descent
         return max(0, -self.ink_bounds.bottom)
 
 
     @writable_property
     def right_extent(self):
         """
         Horizontal ascent relative to baseline for vertical rendering.
         Defaults to ink-right.
         """
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 0
         return max(0, self.ink_bounds.right)
 
     @writable_property
     def left_extent(self):
         """
         Horizontal descent relative to baseline for vertical rendering.
         Defaults to ink-left.
         """
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 0
         # if ink bounds go below the baseline, use them as descent
         return max(0, -self.ink_bounds.left)
 
 
     @checked_property
     def pixel_size(self):
@@ -360,82 +372,86 @@
         # - there is no kerning
         #
         # a special case is the _multi-cell_ font,
         # where a glyph may take up 0, 1 or 2 cells.
         #
         # a _monospace_ font is a font where all glyphs have equal advance_width.
         #
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 'character-cell'
         if any(
                 _glyph.advance_width < 0 or _glyph.right_kerning
-                for _glyph in self._font.glyphs
+                for _glyph in self.glyphs
             ):
             return 'proportional'
         # don't count void glyphs (0 width and/or height)
         # to determine whether it's monospace
         advances = set(
             _glyph.advance_width
-            for _glyph in self._font.glyphs if _glyph.advance_width
+            for _glyph in self.glyphs if _glyph.advance_width
         )
+        if len(set(advances)) > 2:
+            return 'proportional'
         monospaced = len(set(advances)) == 1
-        bispaced = len(set(advances)) == 2
-        ink_contained_y = self.line_height >= self.bounding_box.y
-        ink_contained_x = all(
-            _glyph.advance_width >= _glyph.bounding_box.x
-            for _glyph in self._font.glyphs
-        )
-        if ink_contained_x and ink_contained_y:
-            if monospaced:
-                return 'character-cell'
-            if bispaced:
-                return 'multi-cell'
-        if monospaced:
-            return 'monospace'
-        return 'proportional'
+        negative = tuple(
+            _g for _g in self.glyphs
+            if _g.left_bearing < 0 or _g.right_bearing < 0
+            or _g.top_bearing < 0 or _g.bottom_bearing < 0
+        )
+        if not negative:
+            return 'character-cell' if monospaced else 'multi-cell'
+        # we have negative bearings; need to check if there's ink in them
+        # this should be rare (monospaced/bispaced with negative bearings)
+        if all(
+                (_g.advance_width >= _g.bounding_box.x)
+                and (_g.advance_height >= _g.bounding_box.y)
+                for _g in negative
+            ):
+            return 'character-cell' if monospaced else 'multi-cell'
+        return 'monospace' if monospaced else 'proportional'
 
     @checked_property
     def raster(self):
         """
         Minimum box encompassing all glyph matrices overlaid at fixed origin,
         bottom-left origin coordinates.
         """
-        if not self._font.glyphs:
+        if not self.glyphs:
             return Bounds(0, 0, 0, 0)
-        return Glyph._get_common_raster(*self._font.glyphs)
+        return Glyph._get_common_raster(*self.glyphs)
 
     @checked_property
     def raster_size(self):
         """Minimum box encompassing all glyph matrices overlaid at fixed origin."""
         return Coord(
             self.raster.right - self.raster.left,
             self.raster.top - self.raster.bottom
         )
 
     @checked_property
     def cell_size(self):
         """Width, height of the character cell."""
-        if not self._font.glyphs or self.spacing == 'proportional':
+        if not self.glyphs or self.spacing == 'proportional':
             return Coord(0, 0)
         # smaller of the (at most two) advance widths is the cell size
         # in a multi-cell font, some glyphs may take up two cells.
-        cell_x = min(
-            _glyph.advance_width
-            for _glyph in self._font.glyphs if _glyph.advance_width
+        cells = tuple(
+            (_g.advance_width, _g.advance_height)
+            for _g in self.glyphs
         )
-        return Coord(cell_x, self.line_height)
+        return Coord(*min(_c for _c in cells if all(_c)))
 
     @checked_property
     def ink_bounds(self):
         """
         Minimum bounding box encompassing all glyphs at fixed origin,
         bottom-left origin cordinates.
         """
         nonempty = [
-            _glyph for _glyph in self._font.glyphs
+            _glyph for _glyph in self.glyphs
             if _glyph.bounding_box.x and _glyph.bounding_box.y
         ]
         if not nonempty:
             return Bounds(0, 0, 0, 0)
         lefts, bottoms, rights, tops = zip(*(
             _glyph.ink_bounds
             for _glyph in nonempty
@@ -467,58 +483,58 @@
             self.raster.right - self.ink_bounds.right,
             self.raster.top - self.ink_bounds.top,
         )
 
     @writable_property
     def average_width(self):
         """Get average glyph advance width."""
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 0
         return (
-            sum(_glyph.advance_width for _glyph in self._font.glyphs)
-            / len(self._font.glyphs)
+            sum(_glyph.advance_width for _glyph in self.glyphs)
+            / len(self.glyphs)
         )
 
     @writable_property
     def max_width(self):
         """Maximum glyph advance width."""
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 0
-        return max(_glyph.advance_width for _glyph in self._font.glyphs)
+        return max(_glyph.advance_width for _glyph in self.glyphs)
 
     @writable_property
     def cap_width(self):
         """Advance width of uppercase X."""
         try:
-            return self._font.get_glyph(char='X').advance_width
+            return self.get_glyph(char='X').advance_width
         except KeyError:
             return 0
 
     @writable_property
     def x_height(self):
         """Ink height of lowercase x."""
         try:
-            return self._font.get_glyph(char='x').bounding_box.y
+            return self.get_glyph(char='x').bounding_box.y
         except KeyError:
             return 0
 
     @writable_property
     def cap_height(self):
         """Ink height of uppercase X."""
         try:
-            return self._font.get_glyph(char='X').bounding_box.y
+            return self.get_glyph(char='X').bounding_box.y
         except KeyError:
             return 0
 
     @writable_property
     def digit_width(self):
         """Advance width of digits, if fixed."""
         try:
             widths = set(
-                self._font.get_glyph(char=_d).advance_width
+                self.get_glyph(char=_d).advance_width
                 for _d in '$0123456789'
             )
         except KeyError:
             return 0
         if len(widths) == 1:
             return widths.pop()
         return 0
@@ -529,62 +545,66 @@
 
     @writable_property
     def underline_descent(self):
         """
         Position of underline below baseline.
         0 means underline on baseline itself.
         """
-        if not self._font.glyphs:
+        if not self.glyphs:
             return 0
         max_descent = -min(
             _glyph.shift_up + _glyph.padding.bottom
-            for _glyph in self._font.glyphs
+            for _glyph in self.glyphs
         )
         # XLFD calculation says round(max_descent/2) but I think they mean this
         # they may meam something else with the 'top of the baseline'?
         return 1 + ceildiv(max_descent, 2)
 
     @writable_property
     def superscript_size(self):
         """Recommended superscript size in pixels."""
         return round(self.pixel_size * 0.6)
 
     @writable_property
     def superscript_offset(self):
         """Recommended superscript horizontal, vertical offset in pixels."""
         shift = round(self.pixel_size * 0.4)
-        return Coord(shift, shift)
+        return Coord(0, shift)
 
     @writable_property
     def subscript_size(self):
         """Recommended subscript size in pixels."""
         return round(self.pixel_size * 0.6)
 
     @writable_property
     def subscript_offset(self):
         """Recommended subscript horizontal, vertical offset in pixels."""
         shift = round(self.pixel_size * 0.4)
-        return Coord(shift, shift)
+        return Coord(0, shift)
 
     @writable_property
     def small_cap_size(self):
         """Recommended small-capital size in pixels."""
+        if not self.cap_height:
+            return 0
         return round(
             self.pixel_size * (
                 (self.x_height + (self.cap_height - self.x_height) / 3)
                 / self.cap_height
             )
         )
 
     @writable_property
     def word_space(self):
         """Recommended space between words, in pixels."""
         try:
-            return self._font.get_glyph(char=' ').advance_width
+            return self.get_glyph(char=' ').advance_width
         except KeyError:
+            if self.spacing in ('character-cell', 'multi-cell'):
+                return self.cell_size.x
             # convoluted XLFD calc just boils down to this?
             return round(self.pixel_size / 3)
 
     @writable_property
     def min_word_space(self):
         """Recommended minimum space between words, in pixels."""
         return round(0.75 * self.word_space)
@@ -603,15 +623,15 @@
     ##########################################################################
     # character properties
 
     @writable_property
     def default_char(self):
         """Label for default character."""
         repl = '\ufffd'
-        if repl not in self._font.get_chars():
+        if repl not in self.get_chars():
             repl = ''
         return Char(repl)
 
 
     ##########################################################################
     # deprecated compatibility synonyms
 
@@ -627,43 +647,37 @@
 
     @writable_property('cap_width')
     def cap_advance(self):
         """Advance width of LATIN CAPITAL LETTER X."""
         return self.cap_width
 
 
-###############################################################################
-# Font class
+    __properties_end__ = True
 
+    ###########################################################################
 
-class Font:
-    """Representation of font glyphs and metadata."""
 
     def __init__(self, glyphs=(), *, comment=None, **properties):
         """Create new font."""
         self._glyphs = tuple(glyphs)
         # construct lookup tables
         self._labels = {
             _label: _index
             for _index, _glyph in enumerate(self._glyphs)
             for _label in _glyph.get_labels()
         }
         # comment can be str (just global comment) or mapping of property comments
-        if not comment:
-            pass
-        elif isinstance(comment, str):
-            properties['#'] = comment
-        else:
-            properties.update({f'#{_k}': _v for _k, _v in comment.items()})
+        if isinstance(comment, str):
+            comment = {'': comment}
         self._glyphs, properties = self._apply_metrics(self._glyphs, properties)
         # update properties
         # set encoding first so we can set labels
         # NOTE - we must be careful NOT TO ACCESS CACHED PROPERTIES
         #        until the constructor is complete
-        self._props = FontProperties(_font=self, **properties)
+        super().__init__(**properties, _comments=comment)
 
     @staticmethod
     def _apply_metrics(glyphs, props):
         """Apply globally specified glyph metrics."""
         glyph_metrics = {
             _k: props[_k]
             for _k in (
@@ -722,19 +736,15 @@
             glyphs = self._glyphs
         old_comment = self._get_comment_dict()
         if isinstance(comment, str):
             old_comment[''] = comment
         elif comment is not NOT_SET:
             old_comment.update(comment)
         # comment and properties are replaced keyword by keyword
-        properties = {
-            _k: _v
-            for _k, _v in vars(self._props).items()
-            if not _k.startswith('_') and not _k.startswith('#')
-        }
+        properties = {**self._props}
         properties.update({
             normalise_property(_k): _v
             for _k, _v in kwargs.items()
         })
         return Font(
             tuple(glyphs),
             comment=old_comment,
@@ -749,15 +759,15 @@
         if not comment:
             comment = {}
         for key, comment in comment.items():
             old_comment = self.get_comment(key)
             if old_comment:
                 comment[key] = extend_string(old_comment, comment)
         for key, value in properties.items():
-            if key in self._props:
+            if self._defined(key):
                 properties[key] = extend_string(self._props[key], value)
         if glyphs:
             glyphs = (*self.glyphs, *glyphs)
         else:
             glyphs = NOT_SET
         return self.modify(glyphs, comment={**comment}, **properties)
 
@@ -783,69 +793,66 @@
             comment=comment,
             **none_args,
         )
 
     ##########################################################################
     # property access
 
-    def __getattr__(self, attr):
-        """Take property from property table."""
-        if '_props' not in vars(self):
-            logging.error(type(self).__name__ + '._props not defined')
-            raise AttributeError(attr)
-        if attr.startswith('_'):
-            # don't delegate private members
-            raise AttributeError(attr)
-        return getattr(self._props, attr)
-
     def get_comment(self, key=''):
         """Get global or property comment."""
         key = normalise_property(key)
-        return getattr(self._props, f'#{key}', '')
+        return self._comments.get(key, '')
 
     def _get_comment_dict(self):
         """Get all global and property comments as a dict."""
-        return {
-            _k[1:]: self._props[_k]
-            for _k in self._props
-            if _k.startswith('#')
-        }
+        return self._comments
 
     @property
     def properties(self):
         """Non-defaulted properties in order of default definition list."""
-        return {
-            _k.replace('_', '-'): self._props[_k]
-            for _k in self._props
-            if not _k.startswith('_') and not _k.startswith('#')
-            and self._props[_k] != self._props._get_default(_k)
-        }
+        return {_k.replace('_', '-'): _v for _k, _v in self._props.items()}
 
     def is_known_property(self, key):
         """Field is a recognised property."""
-        return self._props._known(key)
+        return self._known(key)
 
     def get_property(self, key):
         """Get value for property."""
-        key = normalise_property(key)
-        return getattr(self._props, key, '')
+        try:
+            return self._get_property(key)
+        except KeyError:
+            return None
+
+    def get_default(self, property):
+        """Default value for a property."""
+        return self._get_default(property)
 
     def format_properties(self, template, **kwargs):
         """Format a string template using font properties."""
         from string import Formatter
 
         # pylint: disable=no-self-argument
         class FontFormatter(Formatter):
             def get_value(inner_self, key, inner_args, inner_kwargs):
                 if key in inner_kwargs:
                     return inner_kwargs[key]
                 return getattr(self, key)
 
         return FontFormatter().format(template, **kwargs)
 
+    def get_features(self):
+        """Get set of special features for this font."""
+        feats = set.union(*(_g.features for _g in self.glyphs))
+        if any(
+                self._defined(_p)
+                for _p in ('line_width', 'left-extent', 'right-extent')
+            ):
+            feats.add('vertical')
+        return feats
+
 
     ##########################################################################
     # glyph access
 
     @property
     def glyphs(self):
         return self._glyphs
@@ -884,14 +891,16 @@
                 char = Char(label)
             if char:
                 try:
                     return self._compose_glyph(char)
                 except KeyError:
                     pass
             if missing == 'default':
+                if label == self.word_boundary:
+                    return self.get_space_glyph()
                 return self.get_default_glyph()
             if missing == 'empty':
                 return self.get_empty_glyph()
             if missing is None or isinstance(missing, Glyph):
                 return missing
             raise
 
@@ -919,19 +928,32 @@
         except KeyError:
             pass
         raise KeyError(f'No glyph found matching label={label}')
 
     @cache
     def get_default_glyph(self):
         """Get default glyph; empty if not defined."""
-        return self.get_glyph(self.default_char, missing='empty')
+        try:
+            return self.get_glyph(self.default_char, missing='raise')
+        except KeyError:
+            # use fully inked space-sized block if default glyph undefined
+            return self.get_space_glyph().invert()
+
+
+    @cache
+    def get_space_glyph(self):
+        """Get blank glyph with advance width defined by word-space property."""
+        return Glyph.blank(
+            width=self.word_space, height=self.pixel_size,
+            shift_up=-self.descent
+        )
 
     @cache
     def get_empty_glyph(self):
-        """Get blank glyph with zero advance_width and advance_height"""
+        """Get blank glyph with zero advance_width and advance_height."""
         return Glyph.blank()
 
 
     ##########################################################################
     # label access
 
     @cache
@@ -1019,15 +1041,14 @@
         else:
             return self
         return self.modify(encoding=encoding, glyphs=tuple(
             _glyph.label(**kwargs)
             for _glyph in self.glyphs
         ))
 
-    # need converter from string to set of labels to script this
     @scriptable
     def subset(
             self, labels:tuple[Label]=(), *,
             chars:tuple[Char]=(), codepoints:tuple[Codepoint]=(), tags:tuple[Tag]=(),
         ):
         """
         Return a subset of the font.
@@ -1070,17 +1091,15 @@
             _glyph
             for _glyph in self.glyphs
             if not (set(_glyph.get_labels()) & set(labels))
         ]
         return self.modify(glyphs)
 
 
-    # WARNING: this shadows builtin set() in any annotations for method definitions below
-    @scriptable(script_args=FontProperties.__annotations__.items())
-    def set(self, **kwargs):
+    def _set(self, **kwargs):
         """Return a copy of the font with one or more recognised properties changed."""
         kwargs = {
             _k: (_v if _v != '' else None)
             for _k, _v in kwargs.items()
         }
         return self.modify(**kwargs)
 
@@ -1247,30 +1266,36 @@
         # fix line-advances to ensure they remain unchanged
         return font.modify(
             line_height=self.line_height,
             line_width=self.line_width,
         )
 
     @scriptable
-    def reduce(self, *, adjust_metrics:bool=True):
+    def reduce(self, *, adjust_metrics:bool=True, create_vertical_metrics:bool=False):
         """
         Reduce glyphs to their bounding box.
 
         adjust_metrics: make the operation render-invariant (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
+        create_vertical_metrics = (
+            create_vertical_metrics or 'vertical' in self.get_features()
+        )
         font = self._apply_to_all_glyphs(
             Glyph.reduce,
             adjust_metrics=adjust_metrics,
+            create_vertical_metrics=create_vertical_metrics,
         )
         if not adjust_metrics:
             return font
-        # fix line-advances to ensure they remain unchanged
+        if not create_vertical_metrics:
+            # fix line-advances to ensure they remain unchanged
+            return font.modify(line_height=self.line_height)
         return font.modify(
-            line_height=self.line_height,
-            line_width=self.line_width,
+            line_height=self.line_height, line_width=self.line_width
         )
 
     @scriptable
     def equalise_horizontal(self):
         """
         Pad glyphs to include positive horizontal bearings and line height.
         Negative bearings and upshifts are equalised.
@@ -1438,9 +1463,12 @@
             @wraps(_func)
             def _modify_glyphs(self, _func=_func, **kwargs):
                 return self._apply_to_all_glyphs(_func, **kwargs)
 
             locals()[_name] = _modify_glyphs
 
 
+# set properties from script
+Font.set = scriptable(script_args=Font.__annotations__.items())(Font._set)
+
 # scriptable font/glyph operations
 operations = get_scriptables(Font)
```

### Comparing `monobit-0.39.3/monobit/glyph.py` & `monobit-0.40.0/monobit/glyph.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 
 import logging
 from functools import cache
 
 from .encoding import is_graphical, is_blank
 from .labels import Codepoint, Char, Tag, to_label
 from .raster import Raster, NOT_SET, turn_method
-from .properties import (
-    DefaultProps, normalise_property, extend_string,
-    writable_property, as_tuple, checked_property
-)
+from .properties import Props, normalise_property, extend_string
+from .cachedprops import DefaultProps, writable_property, as_tuple, checked_property
 from .basetypes import Coord, Bounds, to_number
 from .scripting import scriptable
 from .vector import StrokePath
 
 
 ##############################################################################
 # kerning table
@@ -62,16 +60,16 @@
         # no kerning is zero kerning
         return 0
 
 
 ##############################################################################
 # glyph properties
 
-class GlyphProperties(DefaultProps):
-    """Recognised properties for Glyph."""
+class Glyph(DefaultProps):
+    """Single glyph including raster and properties."""
 
     # horizontal offset from leftward origin to matrix left edge
     left_bearing: int
     # horizontal offset from matrix right edge to rightward origin
     right_bearing: int
     # upward offset from origin to matrix bottom
     shift_up: int
@@ -92,34 +90,40 @@
     kern_to: KernTable
     tracking: int
     offset: Coord
 
     # path segments for stroke fonts
     path: StrokePath
 
+    # non-overridable, hinted for pylint
+    padding: Bounds
+    height: int
+
+    # sentinel to help build the list of calculated properties
+    __properties_start__ = True
 
     @checked_property
     def advance_width(self):
         """Internal advance width of glyph, including internal bearings."""
         return self.left_bearing + self.width + self.right_bearing
 
     @checked_property
     def advance_height(self):
         """Internal advance width of glyph, including internal bearings."""
         return self.top_bearing + self.height + self.bottom_bearing
 
     @checked_property
     def width(self):
         """Raster width of glyph."""
-        return self._glyph._pixels.width
+        return self._pixels.width
 
     @checked_property
     def height(self):
         """Raster height of glyph."""
-        return self._glyph._pixels.height
+        return self._pixels.height
 
     @checked_property
     def ink_bounds(self):
         """Minimum box encompassing all ink, relative to bottom left."""
         # pylint: disable=no-member
         bounds = Bounds(
             self.raster.left + self.padding.left,
@@ -140,15 +144,15 @@
             self.ink_bounds.right - self.ink_bounds.left,
             self.ink_bounds.top - self.ink_bounds.bottom
         )
 
     @checked_property
     def padding(self):
         """Offset from raster sides to bounding box. Left, bottom, right, top."""
-        return self._glyph._pixels.padding
+        return self._pixels.padding
 
     @checked_property
     def raster(self):
         """Raster bounds, from bottom left."""
         return Bounds(
             left=self.left_bearing,
             bottom=self.shift_up,
@@ -182,59 +186,59 @@
     def offset(self):
         """
         (horiz, vert) offset from origin to matrix start
         Deprecated synonym for left-bearing, shift-up.
         """
 
 
-##############################################################################
-# glyph
+    __properties_end__ = True
 
-class Glyph:
-    """Single glyph."""
+    ##########################################################################
+    # dunder methods
 
     def __init__(
             self, pixels=(), *,
             labels=(), codepoint=b'', char='', tag='', comment='',
-            _0=NOT_SET, _1=NOT_SET,
+            _0=NOT_SET, _1=NOT_SET, _trustme=False,
             **properties
         ):
         """Create glyph from tuple of tuples."""
+        if _trustme:
+            self._pixels = Raster(pixels, _0=_0, _1=_1)
+            self._labels = labels
+            self._comment = comment
+            super().__init__(**properties)
+            return
         # raster data
         self._pixels = Raster(pixels, _0=_0, _1=_1)
         # labels
         labels = (
             Char(char), Codepoint(codepoint), Tag(tag),
             *(to_label(_l) for _l in labels)
         )
         self._labels = tuple(_l for _l in labels if _l)
         # comment
         if not isinstance(comment, str):
             raise TypeError('Glyph comment must be a single string.')
         self._comment = comment
         # recognised properties
-        # access needed for calculated properties
-        self._props = GlyphProperties(_glyph=self, **properties)
+        super().__init__(**properties)
 
     def __eq__(self, other):
         """Equality."""
         if not isinstance(other, type(self)):
             return False
         if (self.width, self.height) != (other.width, other.height):
             return False
         for p in (*self.properties.keys(), *other.properties.keys()):
             p = normalise_property(p)
             if not getattr(self, p) == getattr(other, p):
                 return False
         return self.as_matrix() == other.as_matrix()
 
-
-    ##########################################################################
-    # representation
-
     def __repr__(self):
         """Text representation."""
         elements = (
             f"labels={repr(self._labels)}" if self._labels else '',
             "comment=({})".format(
                 "\n  '" + "\n',\n  '".join(self.comment.splitlines()) + "'"
             ) if self._comment else '',
@@ -260,52 +264,41 @@
             **kwargs
         ):
         """Return a copy of the glyph with changes."""
         if pixels is NOT_SET:
             pixels = self._pixels
         if labels is NOT_SET:
             labels = self._labels
-        if tag is NOT_SET:
-            tag = ''
-        else:
-            labels = tuple(
-                _l for _l in labels if not isinstance(_l, Tag)
-            )
-        if codepoint is NOT_SET:
-            codepoint = b''
         else:
-            labels = tuple(
-                _l for _l in labels if not isinstance(_l, Codepoint)
-            )
-        if char is NOT_SET:
-            char = ''
-        else:
-            labels = tuple(
-                _l for _l in labels if not isinstance(_l, Char)
-            )
+            labels = tuple(to_label(_l) for _l in labels)
+        if tag is not NOT_SET:
+            labels = [_l for _l in labels if not isinstance(_l, Tag)]
+            if tag:
+                labels.append(Tag(tag))
+        if codepoint is not NOT_SET:
+            labels = [_l for _l in labels if not isinstance(_l, Codepoint)]
+            if codepoint or codepoint == 0:
+                labels.append(Codepoint(codepoint))
+        if char is not NOT_SET:
+            labels = [_l for _l in labels if not isinstance(_l, Char)]
+            if char:
+                labels.append(Char(char))
         if comment is NOT_SET:
             comment = self._comment
-        properties = {
-            _k: _v
-            for _k, _v in vars(self._props).items()
-            if not _k.startswith('_') and not _k.startswith('#')
-        }
+        properties = {**self._props}
         properties.update({
             normalise_property(_k): _v
             for _k, _v in kwargs.items()
         })
         return type(self)(
             pixels,
             labels=labels,
-            codepoint=codepoint,
-            char=char,
-            tag=tag,
             comment=comment or '',
-            _0=_0, _1=_1,
-            **properties
+            **properties,
+            _trustme=True,
         )
 
     def label(
             self, codepoint_from=None, char_from=None,
             tag_from=None, comment_from=None,
             overwrite=False, match_whitespace=True, match_graphical=True,
         ):
@@ -352,17 +345,17 @@
             self, *,
             comment=None, **properties
         ):
         """Return a copy of the glyph with changes."""
         if not comment:
             comment = ''
         comment = extend_string(self._comment, comment)
-        for property, value in properties.items():
-            if property in self._props:
-                properties[property] = extend_string(self._props[property], value)
+        for key, value in properties.items():
+            if self._defined(key):
+                properties[key] = extend_string(self._props[key], value)
         # do not record glyph history
         try:
             history = properties.pop('history')
             #logging.debug("Ignoring glyph history '%s'", history)
         except KeyError:
             pass
         return self.modify(
@@ -396,49 +389,61 @@
             **none_args
         )
 
 
     ##########################################################################
     # property access
 
-    def __getattr__(self, attr):
-        """Take attribute from property table if not defined here."""
-        if '_props' not in vars(self):
-            logging.error(type(self).__name__ + '._props not defined')
-            raise AttributeError(attr)
-        if attr.startswith('_'):
-            # don't delegate private members
-            raise AttributeError(attr)
-        return getattr(self._props, attr)
-
     @property
     def comment(self):
         return self._comment
 
-    @classmethod
-    def default(cls, property):
+    def get_default(self, property):
         """Default value for a property."""
-        return vars(GlyphProperties).get(normalise_property(property), '')
+        return self._get_default(property)
 
     @property
     def properties(self):
         """Non-defaulted properties in order of default definition list."""
-        return {
-            _k.replace('_', '-'): self._props[_k]
-            for _k in self._props
-            if not _k.startswith('_')
-            and self._props[_k] != self._props._get_default(_k)
-        }
+        return {_k.replace('_', '-'): _v for _k, _v in self._props.items()}
 
     def get_property(self, key):
         """Get value for property."""
-        key = normalise_property(key)
-        return getattr(self._props, key, '')
+        try:
+            return self._get_property(key)
+        except KeyError:
+            return None
 
+    def get_defined(self, key):
+        """Get value for property, if explicitly defined."""
+        return self._defined(key)
 
+    @property
+    def features(self):
+        """Get set of special features for this glyph."""
+        feats = set()
+        if any(
+                self._defined(_p)
+                for _p in ('top-bearing', 'bottom-bearing', 'shift-left')
+            ):
+            feats.add('vertical')
+        if any(
+                self._defined(_p)
+                for _p in ('left-kerning', 'right-kerning')
+            ):
+            feats.add('kerning')
+        if any(
+                self._get_property(_p) < 0
+                for _p in (
+                    'left-bearing', 'right-bearing',
+                    'top-bearing', 'bottom-bearing'
+                )
+            ):
+            feats.add('overlap')
+        return feats
 
     ##########################################################################
     # label access
 
     @property
     def tags(self):
         return tuple(_l for _l in self._labels if isinstance(_l, Tag))
@@ -504,15 +509,15 @@
         """Create glyph from hex string."""
         pixels = Raster.from_hex(hexstr, width, height, align=align)
         return cls(pixels, **kwargs)
 
     @classmethod
     def from_path(cls, strokepath, *, advance_width=None, **kwargs):
         """Draw the StrokePath and create a Glyph."""
-        raster = strokepath.draw()
+        raster = Raster(strokepath.draw())
         if advance_width is None:
             advance_width = strokepath.bounds.right
         return cls(
             raster, path=strokepath,
             right_bearing=advance_width-strokepath.bounds.right,
             left_bearing=strokepath.bounds.left,
             shift_up=strokepath.bounds.bottom,
@@ -542,14 +547,18 @@
         """Convert glyph to a string of quadrant block characters."""
         return self._pixels.as_blocks()
 
     def as_vector(self, ink=1, paper=0):
         """Return flat tuple of user-specified foreground and background objects."""
         return self._pixels.as_vector(ink=ink, paper=paper)
 
+    def as_byterows(self, *, align='left'):
+        """Convert glyph to rows of bytes."""
+        return self._pixels.as_byterows(align=align)
+
     def as_bytes(self, *, align='left'):
         """Convert glyph to flat bytes."""
         return self._pixels.as_bytes(align=align)
 
     def as_hex(self, *, align='left'):
         """Convert glyph to hex string."""
         return self._pixels.as_hex(align=align)
@@ -621,40 +630,57 @@
     turn = scriptable(turn_method)
 
     # raster resizing
 
     @scriptable
     def crop(
             self, left:int=0, bottom:int=0, right:int=0, top:int=0,
-            *, adjust_metrics:bool=True
+            *, adjust_metrics:bool=True, create_vertical_metrics:bool=False
         ):
         """
         Crop the raster.
 
         left: number of columns to remove from left
         bottom: number of rows to remove from bottom
         right: number of columns to remove from right
         top: number of rows to remove from top
         adjust_metrics: make the operation render-invariant (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
+        if not any((left, bottom, right, top)):
+            return self
+        create_vertical_metrics = (
+            create_vertical_metrics or 'vertical' in self.features
+        )
         # reduce raster
         pixels = self._pixels.crop(left, bottom, right, top)
-        if adjust_metrics:
-            return self.modify(
-                pixels,
-                # horizontal metrics
-                left_bearing=self.left_bearing + left,
-                right_bearing=self.right_bearing + right,
-                shift_up=self.shift_up + bottom,
-                # vertical metrics
-                top_bearing=self.top_bearing + top,
-                bottom_bearing=self.bottom_bearing + bottom,
-                shift_left=self.shift_left + self.width//2 - pixels.width//2,
-            )
-        return self.modify(pixels)
+        if not adjust_metrics:
+            return self.modify(pixels)
+        else:
+            # shift-left adjustment rounds differently for odd-width than even width
+            sign = 1 if (self.width%2) else -1
+            if not create_vertical_metrics:
+                return self.modify(
+                    pixels,
+                    left_bearing=self.left_bearing + left,
+                    right_bearing=self.right_bearing + right,
+                    shift_up=self.shift_up + bottom,
+                )
+            else:
+                return self.modify(
+                    pixels,
+                    # horizontal metrics
+                    left_bearing=self.left_bearing + left,
+                    right_bearing=self.right_bearing + right,
+                    shift_up=self.shift_up + bottom,
+                    # vertical metrics
+                    top_bearing=self.top_bearing + top,
+                    bottom_bearing=self.bottom_bearing + bottom,
+                    shift_left=self.shift_left + sign*((sign*(right-left))//2),
+                )
 
     @scriptable
     def expand(
             self, left:int=0, bottom:int=0, right:int=0, top:int=0,
             *, adjust_metrics:bool=True
         ):
         """
@@ -662,38 +688,47 @@
 
         left: number of columns to add on left
         bottom: number of rows to add on bottom
         right: number of columns to add on right
         top: number of rows to add on top
         adjust_metrics: make the operation render-invariant (default: True)
         """
+        if not any((left, bottom, right, top)):
+            return self
         # reduce raster
         pixels = self._pixels.expand(left, bottom, right, top)
         if adjust_metrics:
+            # shift-left adjustment rounds differently for odd-width than even width
+            sign = 1 if (self.width%2) else -1
             return self.modify(
                 pixels,
                 # horizontal metrics
                 left_bearing=self.left_bearing - left,
                 right_bearing=self.right_bearing - right,
                 shift_up=self.shift_up - bottom,
                 # vertical metrics
                 top_bearing=self.top_bearing - top,
                 bottom_bearing=self.bottom_bearing - bottom,
-                shift_left=self.shift_left + self.width//2 - pixels.width//2,
+                # for shift-left, expand left is like crop right, and v.v.
+                shift_left=self.shift_left + sign*((sign*(left-right))//2),
             )
         return self.modify(pixels)
 
     @scriptable
-    def reduce(self, *, adjust_metrics:bool=True):
+    def reduce(self, *, adjust_metrics:bool=True, create_vertical_metrics:bool=False):
         """
         Return a glyph reduced to the bounding box.
 
         adjust_metrics: make the operation render-invariant (default: True)
+        create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
-        return self.crop(*self.padding, adjust_metrics=adjust_metrics)
+        return self.crop(
+            *self.padding, adjust_metrics=adjust_metrics,
+            create_vertical_metrics=create_vertical_metrics,
+        )
 
 
     # scaling
 
     @scriptable
     def stretch(
             self, factor_x:int=1, factor_y:int=1,
@@ -702,14 +737,16 @@
         """
         Stretch glyph by repeating rows and/or columns.
 
         factor_x: number of times to repeat horizontally
         factor_y: number of times to repeat vertically
         adjust_metrics: also stretch metrics (default: True)
         """
+        if factor_x == factor_y == 1:
+            return self
         pixels = self._pixels.stretch(factor_x, factor_y)
         if adjust_metrics:
             return self.modify(
                 pixels,
                 left_bearing=factor_x*self.left_bearing,
                 right_bearing=factor_x*self.right_bearing,
                 top_bearing=factor_y*self.top_bearing,
@@ -727,14 +764,16 @@
         """
         Shrink by removing rows and/or columns.
 
         factor_x: factor to shrink horizontally
         factor_y: factor to shrink vertically
         adjust_metrics: also stretch metrics (default: True)
         """
+        if factor_x == factor_y == 1:
+            return self
         pixels = self._pixels.shrink(factor_x, factor_y)
         if adjust_metrics:
             return self.modify(
                 pixels,
                 left_bearing=self.left_bearing // factor_x,
                 right_bearing=self.right_bearing // factor_x,
                 top_bearing=self.top_bearing // factor_y,
@@ -764,20 +803,22 @@
         modulo = pitch_y - (-self.shift_up*pitch_x) % pitch_y
         # adjust for shift at baseline height, to keep it fixed
         pre = (-self.shift_up * pitch_x + modulo) // pitch_y - (modulo==pitch_y)
         if direction == 'r':
             work = self.modify(
                 left_bearing=self.left_bearing-pre,
                 right_bearing=self.right_bearing+pre,
+                shift_left=self.shift_left+pre,
             )
             work = work.expand(right=extra_width)
         elif direction == 'l':
             work = self.modify(
                 left_bearing=self.left_bearing+pre,
                 right_bearing=self.right_bearing-pre,
+                shift_left=self.shift_left-pre,
             )
             work = work.expand(left=extra_width)
         else:
             raise ValueError(
                 f'Shear direction must be `left` or `right`, not `{direction}`'
             )
         pixels = work._pixels.shear(
```

### Comparing `monobit-0.39.3/monobit/labels.py` & `monobit-0.40.0/monobit/labels.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/magic.py` & `monobit-0.40.0/monobit/magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         ):
         """Decorator to register converter for file type."""
 
         def _decorator(converter):
             if not name:
                 raise ValueError('No registration name given')
             if name in self._names:
-                raise ValueError('Registration name `{name} already in use')
+                raise ValueError(f'Registration name `{name}` already in use for {self._names[name]}')
             if not isinstance(magic, (list, tuple)):
                 raise TypeError('Registration parameter `magic` must be list or tuple')
             if not isinstance(patterns, (list, tuple)):
                 raise TypeError('Registration parameter `patterns` must be list or tuple')
             converter.format = name
             self._names[name] = converter
             ## magic signatures
```

### Comparing `monobit-0.39.3/monobit/pack.py` & `monobit-0.40.0/monobit/pack.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from .font import Font, FontProperties
+from .font import Font
 from .scripting import scriptable, get_scriptables
 
 
 class Pack:
     """Holds one or more potentially unrelated fonts."""
 
     def __init__(self, fonts=()):
@@ -43,15 +43,15 @@
 
         index: which font to pick; 0 is first, -1 is last (default: zero)
         """
         return self[index]
 
     @scriptable(
         pack_operation=True,
-        script_args=FontProperties.__annotations__.items()
+        script_args=Font.__annotations__.items()
     )
     def select(self, **properties):
         """Get a subset of fonts from the pack by property. E.g. select(name='Times')."""
         return Pack(
             _font
             for _font in self
             if all(
```

### Comparing `monobit-0.39.3/monobit/properties.py` & `monobit-0.40.0/monobit/cachedprops.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,276 +1,193 @@
 """
-monobit.properties - property structures
+monobit.cachedprops - defaultable, cached property sets with type conversion
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 
 import logging
 from types import SimpleNamespace
 from functools import partial, wraps, cache
 from itertools import chain
 from textwrap import indent, wrap
 
 from .basetypes import CONVERTERS
+from .properties import Props, normalise_property
 
 
-def reverse_dict(orig_dict):
-    """Reverse a dict."""
-    return {_v: _k for _k, _v in orig_dict.items()}
 
-
-##############################################################################
-# property sets
-
-def extend_string(string, line):
-    """Add a line to a multiline string."""
-    return '\n'.join(
-        _line
-        for _line in string.split('\n') + [line]
-        if _line
-    )
-
-def normalise_property(field):
-    # preserve distinction between starting underscore (internal) and starting dash (user property)
-    return field[:1] + field[1:].replace('-', '_')
-
-
-class Props(SimpleNamespace):
-    """
-    SimpleNamespace with the dunder methods of a dict
-    Not a mapping but allows both key-style and attribute-style access
-    """
-
-    # don't pollute the object namespace
-    # we only have __dunder__ methods
-
-    def __init__(self, *args, **kwargs):
-        # convert from string representation
-        if len(args) == 1 and isinstance(args[0], str):
-            kwargs = dict(
-                _line.strip().split(':', 1)
-                for _line in args[0].splitlines()
-            )
-            args = ()
-        super().__init__(*args, **kwargs)
-
-    def __getitem__(self, field):
-        try:
-            return getattr(self, normalise_property(field))
-        except AttributeError as e:
-            raise KeyError(field) from e
-
-    def __setitem__(self, field, value):
-        try:
-            setattr(self, normalise_property(field), value)
-        except AttributeError as e:
-            raise KeyError(field) from e
-
-    def __delitem__(self, field):
-        try:
-            delattr(self, normalise_property(field))
-        except AttributeError as e:
-            raise KeyError(field) from e
-
-    def __len__(self):
-        return len(vars(self))
-
-    def __iter__(self):
-        return iter(vars(self))
-
-    def __str__(self):
-        strs = tuple(
-            (str(_k), str(_v))
-            for _k, _v in vars(self).items()
-        )
-        return '\n'.join(
-            f'{_k}: ' + (indent('\n' + _v, '    ') if '\n' in _v else _v)
-            for _k, _v in strs
-        )
-
-    def __repr__(self):
-        return (
-            type(self).__name__
-            + '(\n' +
-            indent(
-                '\n'.join(f'{_k}={_v!r},' for _k, _v in vars(self).items()),
-                '    '
-            )
-            + '\n)'
-        )
-
-    def __ior__(self, rhs):
-        """Update with other Properties object."""
-        self.__dict__.update(vars(rhs))
-        return self
-
-    def __or__(self, rhs):
-        """Combine with other Properties object."""
-        new = Props(**vars(self))
-        new |= rhs
-        return new
-
-
-##############################################################################
-# property sets with default values, override policy and type conversion
-
-
-def delayed_cache(fn):
-    """Cache only once _frozen attribute is set."""
-    field = normalise_property(fn.__name__)
-
-    @wraps(fn)
-    def _getter(self):
-        if not self._frozen:
-            return fn(self)
-        try:
-            return self._cache[field]
-        except KeyError:
-            pass
-        self._cache[field] = fn(self)
-        return self._cache[field]
-
-    return _getter
-
-
-class DefaultProps(Props):
+class DefaultProps:
     """
     Namespace with recognised fields and defaults.
     Define field types (converters) and defaults in class definition.
     >>> class MyProps(DefaultProps)
     >>>    field_1: int
     >>>    field_2: int = 2
     >>> p = MyProps()
     >>> p.field_2
     >>> 2
     >>> p.field_1
     >>> 0
     where field_1 has an implied default, int() == 0
     """
 
-    # set to True when defaults have been set for a given type
-    # on first instatntiation
-    _init = False
-
-    def __init__(self, *args, **kwargs):
+    def __init__(self, _comments=None, **kwargs):
         # disable cacheing while building the object
-        self._frozen = False
-        super().__init__(*args)
-        # if a type constructor is given in the annotations, use that to set the default
-        # note that we're changing the *class* namespace on the *instance* initialiser
-        # which feels a bit hacky
-        # but this will be a no-op after the first instance has initialised
-        if not type(self)._init:
-            self._set_defaults()
-            type(self)._init = True
-        # use Props.__setitem__ for value conversion
-        # we use None to *unset* properties
+        self._set_defaults()
+        self._props = {}
         [
-            setattr(self, normalise_property(field), value)
-            for field, value in kwargs.items()
-            if value is not None
+            setattr(self, _field, _value)
+            for _field, _value in kwargs.items()
+            #if not _field.startswith('_')
         ]
+        _comments = _comments or {}
+        self._comments = {
+            normalise_property(_k): _v
+            for _k, _v in _comments.items()
+        }
         # enable cacheing
         self._cache = {}
-        self._frozen = True
 
     def __repr__(self):
         return (
             type(self).__name__
             + '(\n    ' +
             '\n    '.join(
-                f'{_k}={_v!r},' for _k, _v in vars(self).items()
+                f'{_k}={_v!r},' for _k, _v in self._props.items()
                 if not _k.startswith('_')
             )
             + '\n)'
         )
 
-    def _set_defaults(self):
+    @classmethod
+    def _set_defaults(cls):
         """If a type constructor is given in the annotations, use that to set the default."""
-        cls = type(self)
-        for field, field_type in cls.__annotations__.items():
-            if field not in vars(cls):
-                setattr(cls, field, field_type())
+        # if a type constructor is given in the annotations, use that to set the default
+        # note that we're changing the *class* namespace on the *instance* initialiser
+        # which feels a bit hacky
+        # but this will be a no-op after the first instance has initialised
+        if not hasattr(cls, '_init'):
+            # type's attributes - these are the calculated properties
+            cls._attribs = list(vars(cls))
+            try:
+                start = cls._attribs.index('__properties_start__')
+                end = cls._attribs.index('__properties_end__')
+            except ValueError:
+                pass
+            else:
+                # cut back the list, speeds up setattr
+                cls._attribs = cls._attribs[start+1:end]
+            cls._attribs = set(cls._attribs)
+            # types, converters and default values for overriding/custom properties
+            cls._types = {**cls.__annotations__}
+            cls._converters = {
+                _field: CONVERTERS.get(_type, _type)
+                for _field, _type in cls._types.items()
+            }
+            cls._defaults = {
+                # can't use .get() as _type() would fail for some defaulted fields
+                _field: vars(cls)[_field] if _field in vars(cls) else _type()
+                #CONVERTERS(_type, _type)()
+                for _field, _type in cls.__annotations__.items()
+                if _field not in cls._attribs
+            }
+            cls._init = True
 
     @classmethod
     def _get_default(cls, field):
         """Default value for a property."""
-        return vars(cls).get(normalise_property(field), None)
+        return cls._defaults.get(normalise_property(field), None)
 
     def _defined(self, field):
         """Writable property has been explicitly set."""
-        return vars(self).get(normalise_property(field), None)
+        return self._props.get(normalise_property(field), None)
 
     @classmethod
     def _known(cls, field):
         """Field is a writable property."""
         # note that checked_properties are not included, writable_properties and regular fields are
-        return normalise_property(field) in vars(cls)
+        field = normalise_property(field)
+        return field in cls._defaults or field in cls._attribs
 
-    def __setattr__(self, field, value):
-        if field != '_frozen' and self._frozen:
-            raise ValueError('Cannot set property on frozen object.')
+    def __getattr__(self, field):
+        if field.startswith('_'):
+            raise AttributeError(field)
+        try:
+            return self._get_property(field)
+        except KeyError as e:
+            raise AttributeError(e)
+
+    def _get_property(self, field):
+        field = normalise_property(field)
         try:
-            converter = type(self).__annotations__[field]
-            converter = CONVERTERS.get(converter, converter)
+            return self._props[field]
         except KeyError:
             pass
-        else:
-            value = converter(value)
-        super().__setattr__(field, value)
+        return self._defaults[field]
 
-    def __iter__(self):
-        """Iterate on default definition order first, then remaining keys."""
-        keys = vars(super()).keys()
-        have_defaults = (_k for _k in type(self).__annotations__ if _k in keys)
-        others = (_k for _k in keys if _k not in type(self).__annotations__)
-        return chain(have_defaults, others)
+    def __setattr__(self, field, value):
+        if field.startswith('_'):
+            return super().__setattr__(field, value)
+        field = normalise_property(field)
+        if field in self._attribs:
+            self._cache = {}
+            return super().__setattr__(field, value)
+        return self._set_property(field, value)
+
+    def _set_property(self, field, value):
+        field = normalise_property(field)
+        if value is None:
+            self._props.pop(field, None)
+        else:
+            # this fails because not all our annotations are actual types
+            #field_type = self._types.get(field, None)
+            #if field_type and not isinstance(field, field_type):
+            converter = self._converters.get(field, None)
+            if converter:
+                value = converter(value)
+            self._props[field] = value
+        self._cache = {}
 
 
 def writable_property(arg=None, *, field=None):
     """Decorator to take property from property table, if defined; calculate otherwise."""
     if not callable(arg):
         return partial(writable_property, field=arg)
     fn = arg
     field = field or fn.__name__
     field = normalise_property(field)
     cached_fn = delayed_cache(fn)
 
     @wraps(fn)
     def _getter(self):
         try:
-            # get property through vars()
             # only use if explicitly set on the instance
-            return vars(self)[field]
+            return self._props[field]
         except KeyError:
             pass
         return cached_fn(self)
 
     @wraps(fn)
     def _setter(self, value):
-        if self._frozen:
-            raise ValueError('Cannot set property on frozen object.')
         #logging.debug(f'Setting overridable property {field}={value}.')
-        vars(self)[field] = value
+        self._set_property(field, value)
 
     return property(_getter, _setter)
 
 
 def checked_property(fn):
     """Non-overridable property, attempted writes will be logged and dropped."""
     field = normalise_property(fn.__name__)
 
     _getter = delayed_cache(fn)
 
     @wraps(fn)
     def _setter(self, value):
-        if self._frozen:
-            raise ValueError('Cannot set property on frozen object.')
         logging.info(f'Non-overridable property {field} cannot be set to {value}; ignored.')
 
     return property(_getter, _setter)
 
 
 def as_tuple(arg=None, *, fields=None, tuple_type=None):
     """
@@ -286,17 +203,34 @@
 
     tuple_type = tuple_type or tuple
 
     @wraps(fn)
     def _getter(self):
         # in this case, always use the fields, whether defaulted or set
         return tuple_type(tuple(
-            self[normalise_property(_field)]
+            getattr(self, _field)
             for _field in fields
         ))
 
     @wraps(fn)
     def _setter(self, value):
         for field, element in zip(fields, tuple_type(value)):
-            self[normalise_property(field)] = element
+            self._set_property(field, element)
 
     return property(_getter, _setter)
+
+
+def delayed_cache(fn):
+    """Cache only once _frozen attribute is set."""
+    field = normalise_property(fn.__name__)
+
+    @wraps(fn)
+    def _getter(self):
+        try:
+            return self._cache[field]
+        except KeyError:
+            pass
+        value = fn(self)
+        self._cache[field] = value
+        return value
+
+    return _getter
```

### Comparing `monobit-0.39.3/monobit/raster.py` & `monobit-0.40.0/monobit/raster.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,53 +54,59 @@
 
 
 # immutable bit matrix
 
 class Raster:
     """Bit matrix."""
 
-    _0 = False
-    _1 = True
-    _sequence = tuple
+    _0 = '0'
+    _1 = '1'
+    _inner = ''.join
+    _outer = tuple
+    _itemtype = str
 
     def __init__(self, pixels=(), *, width=NOT_SET, _0=NOT_SET, _1=NOT_SET):
         """Create glyph from tuple of tuples."""
         if isinstance(pixels, type(self)):
             if _0 is NOT_SET:
                 _0 = pixels._0
             if _1 is NOT_SET:
                 _1 = pixels._1
-            self._pixels = pixels._pixels
-            self._width = pixels._width
+            if width is NOT_SET:
+                width = pixels.width
+            pixels = pixels._pixels
+        if (
+                _0 is NOT_SET or _1 is NOT_SET
+                or not isinstance(_0, self._itemtype)
+                or not isinstance(_1, self._itemtype)
+            ):
+            if _1 is NOT_SET:
+                _1 = True
+            # glyph data
+            self._pixels = self._outer(
+                self._inner(self._1 if _bit == _1 else self._0 for _bit in _row)
+                for _row in pixels
+            )
+            # check pixel matrix geometry
+            if len(set(len(_r) for _r in self._pixels)) > 1:
+                raise ValueError(
+                    f"All rows in raster must be of the same width: {repr(self)}"
+                )
+        else:
+            # if _0 and _1 provided, we don't check the pixel matrix
+            self._pixels = pixels
             self._0 = _0
             self._1 = _1
-        else:
-            if _0 is NOT_SET or _1 is NOT_SET:
-                # glyph data
-                self._pixels = self._sequence(
-                    self._sequence(bool(_bit) for _bit in _row)
-                    for _row in pixels
-                )
-                # check pixel matrix geometry
-                if len(set(len(_r) for _r in self._pixels)) > 1:
-                    raise ValueError(
-                        f"All rows in raster must be of the same width: {repr(self)}"
-                    )
-            else:
-                # if _0 and _1 provided, we don't check the pixel matrix
-                self._pixels = pixels
-                self._0 = _0
-                self._1 = _1
-            if not self._pixels:
-                if width is not NOT_SET:
-                    self._width = width
-                else:
-                    self._width = 0
+        if not self._pixels:
+            if width is not NOT_SET:
+                self._width = width
             else:
-                self._width = len(self._pixels[0])
+                self._width = 0
+        else:
+            self._width = len(self._pixels[0])
 
 
     # NOTE - these following are shadowed in GlyphProperties
 
     @property
     def width(self):
         """Raster width of glyph."""
@@ -162,19 +168,32 @@
         return tuple(
             tuple(ink if _c == self._1 else paper for _c in _row)
             for _row in self._pixels
         )
 
     def as_text(self, *, ink='@', paper='.', start='', end='\n'):
         """Convert raster to text."""
+        def _get_unused(startval):
+            charset = (self._0, self._1, start, end, ink, paper)
+            for _i in range(startval, startval+len(charset)+1):
+                unused = chr(_i)
+                if unused not in charset:
+                    return unused
+
         if not self.height:
             return ''
-        contents = (end + start).join(
-            ''.join(_row)
-            for _row in self.as_matrix(ink=ink, paper=paper)
+        delim = _get_unused(0)
+        contents = delim.join(self._pixels)
+        if paper in (self._1, start, end):
+            swap = _get_unused(7)
+        else:
+            swap = paper
+        contents = (
+            contents.replace(self._0, swap).replace(self._1, ink)
+            .replace(swap, paper).replace(delim, end+start)
         )
         return blockstr(''.join((start, contents, end)))
 
     def as_blocks(self, *, ink='@', paper='.', start='', end='\n'):
         """Convert glyph to a string of quadrant block characters."""
         if not self.height:
             return ''
@@ -295,36 +314,50 @@
                 int.from_bytes(byteseq, 'big'))[2:].zfill(8*len(byteseq)
             )
         return cls.from_vector(
             bitseq, width=width, height=height, stride=stride, align=align,
             _0='0', _1='1',
         )
 
-    def as_bytes(self, *, align='left'):
+    def as_byterows(self, *, align='left'):
         """
-        Convert raster to flat bytes.
+        Convert raster to bytes, by row
 
-        align: 'left' or 'right' for byte-alignment; 'bit' for bit-alignment
+        align: 'left' or 'right'
         """
         if not self.height or not self.width:
-            return b''
+            return ()
         rows = (
             ''.join(_row)
             for _row in self.as_matrix(paper='0', ink='1')
         )
+        bytewidth = ceildiv(self.width, 8)
+        if align.startswith('l'):
+            rows = (_row.ljust(8*bytewidth, '0') for _row in rows)
+        byterows = (int(_row, 2).to_bytes(bytewidth, 'big') for _row in rows)
+        return byterows
+
+    def as_bytes(self, *, align='left'):
+        """
+        Convert raster to flat bytes.
+
+        align: 'left' or 'right' for byte-alignment; 'bit' for bit-alignment
+        """
+        if not self.height or not self.width:
+            return b''
         if align.startswith('b'):
-            bits = ''.join(rows)
+            bits = ''.join(
+                ''.join(_row)
+                for _row in self.as_matrix(paper='0', ink='1')
+            )
             bytesize = ceildiv(len(bits), 8)
             byterow = int(bits, 2).to_bytes(bytesize, 'big')
             return byterow
         else:
-            bytewidth = ceildiv(self.width, 8)
-            if align.startswith('l'):
-                rows = (_row.ljust(8*bytewidth, '0') for _row in rows)
-            byterows = (int(_row, 2).to_bytes(bytewidth, 'big') for _row in rows)
+            byterows = self.as_byterows(align=align)
             return b''.join(byterows)
 
     @classmethod
     def from_hex(cls, hexstr, width, height=NOT_SET, *, align='left'):
         """Create raster from hex string."""
         byteseq = bytes.fromhex(hexstr)
         return cls.from_bytes(byteseq, width, height, align=align)
@@ -360,29 +393,29 @@
     # transformations
 
     # orthogonal transformations
 
     def mirror(self):
         """Reverse pixels horizontally."""
         return type(self)(
-            self._sequence(_row[::-1] for _row in self._pixels),
+            self._outer(_row[::-1] for _row in self._pixels),
             _0=self._0, _1=self._1
         )
 
     def flip(self):
         """Reverse pixels vertically."""
         return type(self)(
             self._pixels[::-1],
             _0=self._0, _1=self._1
         )
 
     def transpose(self):
         """Transpose glyph."""
         return type(self)(
-            self._sequence(zip(*self._pixels)),
+            self._outer(self._inner(_r) for _r in zip(*self._pixels)),
             _0=self._0, _1=self._1
         )
 
     turn = turn_method
 
     # ink shifts on constant raster size
 
@@ -394,15 +427,15 @@
         right: number of columns to roll (to right if positive, to left if negative)
         """
         rolled = self
         rows, columns = down, right
         if self.height > 1 and rows:
             rolled = rolled._pixels[-rows:] + rolled._pixels[:-rows]
         if self.width > 1 and columns:
-            rolled = self._sequence(
+            rolled = self._outer(
                 _row[-columns:] + _row[:-columns]
                 for _row in rolled._pixels
             )
         return type(self)(rolled, _0=self._0, _1=self._1)
 
     def shift(self, *, left:int=0, down:int=0, right:int=0, up:int=0):
         """
@@ -425,20 +458,20 @@
         empty_row = _0 * self.width
         if rows > 0:
             shifted = (empty_row,) * rows + pixels[:-rows]
         else:
             shifted = pixels[-rows:] + (empty_row,) * -rows
         if columns > 0:
             return type(self)(
-                self._sequence(_0 * columns + _row[:-columns] for _row in shifted),
+                self._outer(_0 * columns + _row[:-columns] for _row in shifted),
                 _0=_0, _1=_1
             )
         else:
             return type(self)(
-                self._sequence(_row[-columns:] + _0 * -columns for _row in shifted),
+                self._outer(_row[-columns:] + _0 * -columns for _row in shifted),
                 _0=_0, _1=_1
             )
 
     # raster size changes
 
     def crop(self, left:int=0, bottom:int=0, right:int=0, top:int=0):
         """
@@ -449,15 +482,15 @@
         right: number of columns to remove from right
         top: number of rows to remove from top
         """
         if min(left, bottom, right, top) < 0:
             raise ValueError('Can only crop glyph by a positive amount.')
         if self.height-top-bottom <= 0:
             return type(self).blank(width=max(0, self.width-right-left))
-        return type(self)(self._sequence(
+        return type(self)(self._outer(
                 _row[left : (-right if right else None)]
                 for _row in self._pixels[top : (-bottom if bottom else None)]
             ),
             _0=self._0, _1=self._1
         )
 
     def expand(self, left:int=0, bottom:int=0, right:int=0, top:int=0):
@@ -470,54 +503,52 @@
         top: number of rows to add on top
         """
         if min(left, bottom, right, top) < 0:
             raise ValueError('Can only expand glyph by a positive amount.')
         if not top+self.height+bottom:
             return type(self).blank(width=right+self.width+left)
         new_width = left + self.width + right
-        _0, _1 = '0', '1'
-        pixels = (
-            ''.join(_row)
-            for _row in self.as_matrix(paper=_0, ink=_1)
-        )
-        empty_row = _0 * new_width
+        empty_row = self._0 * new_width
         pixels = (
-            self._sequence((empty_row,)) * top
-            + self._sequence(_0 * left + _row + _0 * right for _row in pixels)
-            + self._sequence((empty_row,)) * bottom
+            self._outer((empty_row,)) * top
+            + self._outer(
+                self._0 * left + _row + self._0 * right
+                for _row in self._pixels
+            )
+            + self._outer((empty_row,)) * bottom
         )
-        return type(self)(pixels, _0=_0, _1=_1)
+        return type(self)(pixels, _0=self._0, _1=self._1)
 
     def stretch(self, factor_x:int=1, factor_y:int=1):
         """
         Repeat rows and/or columns.
 
         factor_x: number of times to repeat horizontally
         factor_y: number of times to repeat vertically
         """
         # vertical stretch
         pixels = (_row for _row in self._pixels for _ in range(factor_y))
         # horizontal stretch
         pixels = (
-            self._sequence(_col for _col in _row for _ in range(factor_x))
+            self._inner(_col for _col in _row for _ in range(factor_x))
             for _row in pixels
         )
-        return type(self)(self._sequence(pixels), _0=self._0, _1=self._1)
+        return type(self)(self._outer(pixels), _0=self._0, _1=self._1)
 
     def shrink(self, factor_x:int=1, factor_y:int=1):
         """
         Remove rows and/or columns.
 
         factor_x: factor to shrink horizontally
         factor_y: factor to shrink vertically
         """
         # vertical shrink
         shrunk = self._pixels[::factor_y]
         # horizontal shrink
-        shrunk = self._sequence(_row[::factor_x] for _row in shrunk)
+        shrunk = self._outer(_row[::factor_x] for _row in shrunk)
         return type(self)(shrunk, _0=self._0, _1=self._1)
 
     # effects
 
     # pylint: disable=no-method-argument
     def overlay(*others, operator=any):
         """
@@ -526,16 +557,19 @@
         operator: aggregation function, callable on iterable on bool/int.
                   Use any for additive, all for masking.
         """
         self = others[0]
         # use as instance method or class method
         matrices = tuple(_r.as_matrix() for _r in others)
         rows = tuple(zip(*_row) for _row in zip(*matrices))
-        combined = self._sequence(self._sequence(operator(_item) for _item in _row) for _row in rows)
-        return type(self)(combined, _0=False, _1=True)
+        combined = self._outer(
+            self._inner(self._1 if operator(_item) else self._0 for _item in _row)
+            for _row in rows
+        )
+        return type(self)(combined, _0=self._0, _1=self._1)
 
     def invert(self):
         """Reverse video."""
         return type(self)(self._pixels, _0=self._1, _1=self._0)
 
     def smear(self, *, left:int=0, right:int=0, up:int=0, down:int=0):
         """
@@ -556,52 +590,47 @@
     def shear(
             self, direction:str='right',
             pitch:Coord=(1, 1), modulo:int=0,
         ):
         """Transform raster by shearing diagonally."""
         direction = direction[0].lower()
         xpitch, ypitch = pitch
-        _0, _1 = '0', '1'
         shiftrange = range(self.height)[::-1]
         shiftrange = (
             (_y*xpitch + modulo)//ypitch - (modulo==ypitch)
             for _y in shiftrange
         )
-        pixels = (
-            ''.join(_row)
-            for _row in self.as_matrix(paper=_0, ink=_1)
-        )
-        empty = _0 * self.width
+        empty = self._0 * self.width
         if direction == 'l':
             return type(self)(
-                self._sequence(
+                self._outer(
                     _row[_y:] + empty[:_y]
-                    for _row, _y in zip(pixels, shiftrange)
+                    for _row, _y in zip(self._pixels, shiftrange)
                 ),
-                _0=_0, _1=_1
+                _0=self._0, _1=self._1
             )
         elif direction == 'r':
             return type(self)(
-                self._sequence(
+                self._outer(
                     empty[:_y] + _row[:self.width-_y]
-                    for _row, _y in zip(pixels, shiftrange)
+                    for _row, _y in zip(self._pixels, shiftrange)
                 ),
-                _0=_0, _1=_1
+                _0=self._0, _1=self._1
             )
         raise ValueError(
             f'Shear direction must be `left` or `right`, not `{direction}`'
         )
 
     def underline(self, top_height:int=0, bottom_height:int=0):
         """Return a raster with a line added."""
         _0, _1 = '0', '1'
         if bottom_height > top_height:
             return self
         top_height = min(self.height, max(0, top_height))
         bottom_height = min(self.height, max(0, bottom_height))
-        pixels = self._sequence(
+        pixels = self._outer(
             _1 * self.width
             if top_height >= self.height-_line-1 >= bottom_height
             else ''.join(_row)
             for _line, _row in enumerate(self.as_matrix(paper=_0, ink=_1))
         )
         return type(self)(pixels, _0=_0, _1=_1)
```

### Comparing `monobit-0.39.3/monobit/renderer.py` & `monobit-0.40.0/monobit/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,18 @@
         for func, args, kwargs in transformations:
             rfont = func(rfont, *args, **kwargs)
         # get glyph rows again, from transformed font
         glyphs = _get_text_glyphs(
             rfont, text, direction, line_direction, base_direction, missing
         )
     # reduce all glyphs to avoid creating overwide margins
-    glyphs = tuple(tuple(_g.reduce() for _g in _row) for _row in glyphs)
+    glyphs = tuple(
+        tuple(_g.reduce(create_vertical_metrics=True) for _g in _row)
+        for _row in glyphs
+    )
     if direction in ('top-to-bottom', 'bottom-to-top'):
         _render = _render_vertical
         min_margin = 0, _adjust_margins_vertical(glyphs)
     else:
         _render = _render_horizontal
         min_margin = _adjust_margins_horizontal(glyphs), 0
     margin_x, margin_y = margin or min_margin
@@ -181,23 +184,23 @@
         grid_x, grid_y = [], []
         for count, glyph in enumerate(glyph_row):
             # advance origin to next glyph
             if count:
                 y -= adjust_bearings
             y -= glyph.advance_height
             grid_y.append(y + glyph.bottom_bearing)
-            grid_x.append(baseline - glyph.width // 2 - glyph.shift_left)
+            grid_x.append(baseline - (glyph.width//2) - glyph.shift_left)
         if align == 'bottom':
             start = margin_y - y
         else:
             start = -margin_y
         # append empty glyph at start and end for margins
         glyph_map.append(Props(
             glyph=Glyph(), sheet=0,
-            x=baseline+(font.line_width+1)//2+margin_x*2,
+            x=baseline + (font.line_width+1)//2 + margin_x*2,
             y=start+y-margin_y
         ))
         for glyph, x, y in zip(glyph_row, grid_x, grid_y):
             glyph_map.append(Props(glyph=glyph, sheet=0, x=margin_x+x, y=start+y))
         # move to next line
         baseline += font.line_width
     return glyph_map
```

### Comparing `monobit-0.39.3/monobit/scripting.py` & `monobit-0.40.0/monobit/scripting.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/storage.py` & `monobit-0.40.0/monobit/storage.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/streams.py` & `monobit-0.40.0/monobit/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def get_bytesio(bytestring):
     """Workaround as our streams objects require a buffer."""
     return io.BufferedReader(io.BytesIO(bytestring))
 
 def get_stringio(string):
-    """Workaround as our streams objetcs require a buffer."""
+    """Workaround as our streams objects require a buffer."""
     return io.TextIOWrapper(get_bytesio(string.encode()))
 
 
 class StreamBase:
     """Base class for streams."""
 
     def __init__(self, stream, mode='', name='', where=None):
@@ -208,14 +208,16 @@
         mode = mode[:1]
         if isinstance(file, DirectoryStream):
             file = file.name
         if not isinstance(file, (str, Path)):
             raise TypeError(
                 'DirectoryStream initialiser must be DirectoryStream, Path or str.'
             )
+        # path is what should be used to open the actual directory
+        self.path = Path(file)
         dummystream = open(os.devnull, mode + 'b')
         # initialise wrapper
         super().__init__(dummystream, mode=mode, name=name, where=where)
 
 
 ###############################################################################
```

### Comparing `monobit-0.39.3/monobit/struct.py` & `monobit-0.40.0/monobit/struct.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/taggers.py` & `monobit-0.40.0/monobit/taggers.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,20 +86,24 @@
 
 
 class CodepointTagger(Tagger):
     """Tag with codepoint numbers."""
 
     name = 'codepoint'
 
+    def __init__(self, prefix=''):
+        """Create codepoint tagger with prefix"""
+        self._prefix = prefix
+
     def comment(self, *labels):
         """Get codepoint string."""
         cp = _get_codepoint(labels)
         if not cp:
             return ''
-        return str(cp)
+        return f'{self._prefix}{cp}'
 
 
 class MappingTagger(Tagger):
     """Tag on the basis of a mapping table."""
 
     def __init__(self, mapping, name=''):
         """Set up mapping."""
@@ -203,9 +207,14 @@
 
 tagmaps = {
     'char': CharTagger(),
     'codepoint': CodepointTagger(),
     'name': UnicodeTagger(),
     'desc': UnicodeTagger(include_char=True),
     'adobe': AdobeTagger.load('charmaps/agl/aglfn.txt', separator=';', unicode_column=0, tag_column=1),
+    'truetype': AdobeTagger.load('charmaps/agl/aglfn.txt', separator=';', unicode_column=0, tag_column=1),
     'sgml': SGMLTagger.load('charmaps/misc/SGML.TXT', separator='\t', unicode_column=2),
 }
+
+# truetype mapping is adobe mapping *but* with .null for NUL
+# https://developer.apple.com/fonts/TrueType-Reference-Manual/RM06/Chap6post.html
+tagmaps['truetype']._chr2tag['\0'] = '.null'
```

### Comparing `monobit-0.39.3/monobit/vector.py` & `monobit-0.40.0/monobit/vector.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/adobe/ReadMe.txt` & `monobit-0.40.0/monobit/charmaps/adobe/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/adobe/stdenc.txt` & `monobit-0.40.0/monobit/charmaps/adobe/stdenc.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/adobe/symbol.txt` & `monobit-0.40.0/monobit/charmaps/adobe/symbol.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/adobe/zdingbat.txt` & `monobit-0.40.0/monobit/charmaps/adobe/zdingbat.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/agl/LICENSE.md` & `monobit-0.40.0/monobit/charmaps/agl/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/agl/README.md` & `monobit-0.40.0/monobit/charmaps/agl/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/agl/aglfn.txt` & `monobit-0.40.0/monobit/charmaps/agl/aglfn.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/agl/glyphlist.txt` & `monobit-0.40.0/monobit/charmaps/agl/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/ARABIC.TXT` & `monobit-0.40.0/monobit/charmaps/apple/ARABIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/CELTIC.TXT` & `monobit-0.40.0/monobit/charmaps/apple/CELTIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/CENTEURO.TXT` & `monobit-0.40.0/monobit/charmaps/apple/CENTEURO.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/CHINSIMP.TXT` & `monobit-0.40.0/monobit/charmaps/apple/CHINSIMP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/CHINTRAD.TXT` & `monobit-0.40.0/monobit/charmaps/apple/CHINTRAD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/CORPCHAR.TXT` & `monobit-0.40.0/monobit/charmaps/apple/CORPCHAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/CROATIAN.TXT` & `monobit-0.40.0/monobit/charmaps/apple/CROATIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/CYRILLIC.TXT` & `monobit-0.40.0/monobit/charmaps/apple/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/DEVANAGA.TXT` & `monobit-0.40.0/monobit/charmaps/apple/DEVANAGA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/DINGBATS.TXT` & `monobit-0.40.0/monobit/charmaps/apple/DINGBATS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/FARSI.TXT` & `monobit-0.40.0/monobit/charmaps/apple/FARSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/GAELIC.TXT` & `monobit-0.40.0/monobit/charmaps/apple/GAELIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/GREEK.TXT` & `monobit-0.40.0/monobit/charmaps/apple/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/GUJARATI.TXT` & `monobit-0.40.0/monobit/charmaps/apple/GUJARATI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/GURMUKHI.TXT` & `monobit-0.40.0/monobit/charmaps/apple/GURMUKHI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/HEBREW.TXT` & `monobit-0.40.0/monobit/charmaps/apple/HEBREW.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/ICELAND.TXT` & `monobit-0.40.0/monobit/charmaps/apple/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/INUIT.TXT` & `monobit-0.40.0/monobit/charmaps/apple/INUIT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/JAPANESE.TXT` & `monobit-0.40.0/monobit/charmaps/apple/JAPANESE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/KEYBOARD.TXT` & `monobit-0.40.0/monobit/charmaps/apple/KEYBOARD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/KOREAN.TXT` & `monobit-0.40.0/monobit/charmaps/apple/KOREAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/ROMAN.TXT` & `monobit-0.40.0/monobit/charmaps/apple/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/ROMANIAN.TXT` & `monobit-0.40.0/monobit/charmaps/apple/ROMANIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/ReadMe.txt` & `monobit-0.40.0/monobit/charmaps/apple/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/SYMBOL.TXT` & `monobit-0.40.0/monobit/charmaps/apple/SYMBOL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/THAI.TXT` & `monobit-0.40.0/monobit/charmaps/apple/THAI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/TURKISH.TXT` & `monobit-0.40.0/monobit/charmaps/apple/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/apple/UKRAINE.TXT` & `monobit-0.40.0/monobit/charmaps/apple/UKRAINE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/README.md` & `monobit-0.40.0/monobit/charmaps/czyborra/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/bulgarian-mik.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/bulgarian-mik.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/cp866.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/cp866.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/gost19768-87.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/gost19768-87.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/hp-roman8.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/hp-roman8.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi-0.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi-0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi-7.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi-7.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi8-a.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi8-a.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi8-b.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi8-b.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi8-e.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi8-e.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi8-f.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi8-f.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi8-r.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi8-r.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/czyborra/koi8-u.txt` & `monobit-0.40.0/monobit/charmaps/czyborra/koi8-u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-ca2` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-ca2`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-cn` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-cn`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-cu` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-cu`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-de` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-de`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-dk` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-dk`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-es` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-es`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-es2` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-es2`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-fr` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-fr`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-gb` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-gb`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-hu` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-hu`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-it` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-it`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-jp-ocr-b` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-jp-ocr-b`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-kr` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-kr`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-us` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-us`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/iso646-yu` & `monobit-0.40.0/monobit/charmaps/dkuug/iso646-yu`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/jis_x0201` & `monobit-0.40.0/monobit/charmaps/dkuug/jis_x0201`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/dkuug/x0201-7` & `monobit-0.40.0/monobit/charmaps/dkuug/x0201-7`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/MULE-ethiopic.map` & `monobit-0.40.0/monobit/charmaps/emacs/MULE-ethiopic.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/MULE-ipa.map` & `monobit-0.40.0/monobit/charmaps/emacs/MULE-ipa.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/MULE-is13194.map` & `monobit-0.40.0/monobit/charmaps/emacs/MULE-is13194.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/MULE-lviscii.map` & `monobit-0.40.0/monobit/charmaps/emacs/MULE-lviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/MULE-sisheng.map` & `monobit-0.40.0/monobit/charmaps/emacs/MULE-sisheng.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/MULE-tibetan.map` & `monobit-0.40.0/monobit/charmaps/emacs/MULE-tibetan.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/MULE-uviscii.map` & `monobit-0.40.0/monobit/charmaps/emacs/MULE-uviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/emacs/README.md` & `monobit-0.40.0/monobit/charmaps/emacs/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/evertype/ARMENIAN.TXT` & `monobit-0.40.0/monobit/charmaps/evertype/ARMENIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/evertype/GEORGIAN.TXT` & `monobit-0.40.0/monobit/charmaps/evertype/GEORGIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/evertype/README.md` & `monobit-0.40.0/monobit/charmaps/evertype/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/1116.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/1116.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/1117.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/1117.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/1118.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/1118.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/1119.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/1119.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/1125.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/1125.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/113.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/113.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/1131.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/1131.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30000.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30000.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30001.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30001.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30002.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30002.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30003.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30003.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30004.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30004.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30005.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30005.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30006.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30006.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30007.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30007.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30008.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30008.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30009.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30009.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30010.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30010.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30011.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30011.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30012.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30013.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30013.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30014.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30014.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30015.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30015.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30016.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30016.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30017.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30017.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30018.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30018.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30019.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30019.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30020.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30020.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30021.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30022.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30022.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30023.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30023.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30024.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30024.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30025.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30025.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30026.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30026.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30027.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30027.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30028.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30028.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30029.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30029.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30030.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30030.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30031.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30031.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30032.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30032.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30033.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30033.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30034.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30034.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30039.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30039.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/30040.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/30040.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/3012.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/3012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/3021.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/3021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/3845.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/3845.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/3846.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/3846.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/3848.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/3848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/437.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/437.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/57781.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/57781.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/58152.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/58152.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/58210.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/58210.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/58335.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/58335.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/59234.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/59234.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/59829.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/59829.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/60258.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/60258.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/60853.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/60853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/61282.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/61282.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/62306.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/62306.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/667.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/667.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/668.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/668.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/737.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/737.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/770.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/770.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/771.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/771.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/772.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/772.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/773.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/773.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/774.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/774.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/775.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/775.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/777.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/777.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/778.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/778.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/790.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/790.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/808.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/808.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/848.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/849.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/849.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/850.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/850.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/851.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/851.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/852.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/852.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/853.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/855.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/855.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/856.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/856.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/857.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/857.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/858.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/858.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/859.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/859.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/860.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/860.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/861.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/861.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/862.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/862.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/863.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/863.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/864.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/864.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/865.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/865.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/866.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/866.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/867.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/867.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/869.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/869.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/872.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/872.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/895.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/895.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/899.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/899.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/991.ucp` & `monobit-0.40.0/monobit/charmaps/freedos/991.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/freedos/README.md` & `monobit-0.40.0/monobit/charmaps/freedos/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iana/Amiga-1251` & `monobit-0.40.0/monobit/charmaps/iana/Amiga-1251`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iana/PTCP154` & `monobit-0.40.0/monobit/charmaps/iana/PTCP154`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100` & `monobit-0.40.0/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/ibm-cdra/038834B0.UPMAP100` & `monobit-0.40.0/monobit/charmaps/ibm-cdra/038834B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101` & `monobit-0.40.0/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100` & `monobit-0.40.0/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/ibm-cdra/readme.txt` & `monobit-0.40.0/monobit/charmaps/ibm-cdra/readme.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/README.md` & `monobit-0.40.0/monobit/charmaps/icu/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm` & `monobit-0.40.0/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/cns-11643-1992.ucm` & `monobit-0.40.0/monobit/charmaps/icu/cns-11643-1992.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-1125_P100-1997.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-1125_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-1375_P100-2008.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-1375_P100-2008.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-720_P100-1997.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-720_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-806_P100-1998.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-806_P100-1998.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-851_P100-1995.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-851_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-858_P100-1997.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-858_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-868_P100-1995.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-868_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/ibm-932_P120-1999.ucm` & `monobit-0.40.0/monobit/charmaps/icu/ibm-932_P120-1999.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/windows-1361-2000.ucm` & `monobit-0.40.0/monobit/charmaps/icu/windows-1361-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/icu/windows-936-2000.ucm` & `monobit-0.40.0/monobit/charmaps/icu/windows-936-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-1.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-10.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-10.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-11.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-11.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-13.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-13.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-14.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-14.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-15.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-15.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-16.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-16.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-2.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-3.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-4.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-5.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-6.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-7.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-8.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/8859-9.TXT` & `monobit-0.40.0/monobit/charmaps/iso-8859/8859-9.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/iso-8859/ReadMe.txt` & `monobit-0.40.0/monobit/charmaps/iso-8859/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMOS7.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMOS7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ADAMSWTR.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ADAMSWTR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPC.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/AMSCPM.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/AMSCPM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT1.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ALT2.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ALT2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2ICHG.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2ICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/APL2PRIM.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/APL2PRIM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8IG.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8IG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8II.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8II.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VG.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARI8VI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARI8VI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ATARISTV.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ATARISTV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/C64IALT.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/C64IALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/C64IPRI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/C64IPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/C64VALT.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/C64VALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/C64VPRI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/C64VPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/COCOICHG.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/COCOICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR4.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/COCOSGR6.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/COCOSGR6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIALT.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETIPRI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVALT.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CPETVPRI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CPETVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIALT.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICIPRI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVALT.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/CVICVPRI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/CVICVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCICH.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/IBMPCVID.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/IBMPCVID.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG0.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/MINITLG1.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/MINITLG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/MSX.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/MSX.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG0.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ORICG1.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ORICG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCEFF.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCEFF.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSB.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSB.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/RISCOSV.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/RISCOSV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ReadMe.txt` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/SINCLRQL.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/SINCLRQL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG0.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG1.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG2.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TELTXTG3.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TELTXTG3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TI994A.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TI994A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ICH.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1ORG.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1ORG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM1REV.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM1REV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IIN.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IJP.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3IRV.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3IRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VIN.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VJP.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM3VRV.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM3VRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIA.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIP.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AIR.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AIR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVA.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVP.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/TRSM4AVR.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/TRSM4AVR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZX80.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZX80.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZX81.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZX81.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXDESKTP.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXDESKTP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT` & `monobit-0.40.0/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/dec-vt100.ucp` & `monobit-0.40.0/monobit/charmaps/manual/dec-vt100.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/hp48.txt` & `monobit-0.40.0/monobit/charmaps/manual/hp48.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/ibm897graph.ucp` & `monobit-0.40.0/monobit/charmaps/manual/ibm897graph.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/mac-system.ucp` & `monobit-0.40.0/monobit/charmaps/manual/mac-system.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/ms-linedraw.txt` & `monobit-0.40.0/monobit/charmaps/manual/ms-linedraw.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/russup3.ucp` & `monobit-0.40.0/monobit/charmaps/manual/russup3.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/russup4ac.ucp` & `monobit-0.40.0/monobit/charmaps/manual/russup4ac.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/russup4na.ucp` & `monobit-0.40.0/monobit/charmaps/manual/russup4na.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/windows-1.0.txt` & `monobit-0.40.0/monobit/charmaps/manual/windows-1.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/windows-2.0.txt` & `monobit-0.40.0/monobit/charmaps/manual/windows-2.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/manual/windows-3.1.txt` & `monobit-0.40.0/monobit/charmaps/manual/windows-3.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP037.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP037.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP500.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP500.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/EBCDIC/CP875.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/EBCDIC/CP875.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/MAC/GREEK.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/MAC/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/MAC/ICELAND.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/MAC/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/MAC/LATIN2.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/MAC/LATIN2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/MAC/ROMAN.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/MAC/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/MAC/TURKISH.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/MAC/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP437.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP437.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP737.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP737.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP775.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP775.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP850.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP850.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP852.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP852.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP855.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP855.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP857.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP857.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP860.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP860.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP861.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP861.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP862.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP862.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP863.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP863.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP864.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP864.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP865.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP865.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP866.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP866.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP869.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP869.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/PC/CP874.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/PC/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP874.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP932.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP932.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP936.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP936.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP949.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP949.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/microsoft/WINDOWS/CP950.TXT` & `monobit-0.40.0/monobit/charmaps/microsoft/WINDOWS/CP950.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/APL-ISO-IR-68.TXT` & `monobit-0.40.0/monobit/charmaps/misc/APL-ISO-IR-68.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/ATARIST.TXT` & `monobit-0.40.0/monobit/charmaps/misc/ATARIST.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/CP1006.TXT` & `monobit-0.40.0/monobit/charmaps/misc/CP1006.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/CP424.TXT` & `monobit-0.40.0/monobit/charmaps/misc/CP424.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/CP856.TXT` & `monobit-0.40.0/monobit/charmaps/misc/CP856.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/GSM0338.TXT` & `monobit-0.40.0/monobit/charmaps/misc/GSM0338.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/IBMGRAPH.TXT` & `monobit-0.40.0/monobit/charmaps/misc/IBMGRAPH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/JIS0208.TXT` & `monobit-0.40.0/monobit/charmaps/misc/JIS0208.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/KOI8-R.TXT` & `monobit-0.40.0/monobit/charmaps/misc/KOI8-R.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/KOI8-U.TXT` & `monobit-0.40.0/monobit/charmaps/misc/KOI8-U.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/KPS9566.TXT` & `monobit-0.40.0/monobit/charmaps/misc/KPS9566.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/KZ1048.TXT` & `monobit-0.40.0/monobit/charmaps/misc/KZ1048.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/NEXTSTEP.TXT` & `monobit-0.40.0/monobit/charmaps/misc/NEXTSTEP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/SGML.TXT` & `monobit-0.40.0/monobit/charmaps/misc/SGML.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/US-ASCII-QUOTES.TXT` & `monobit-0.40.0/monobit/charmaps/misc/US-ASCII-QUOTES.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/dashen-map.txt` & `monobit-0.40.0/monobit/charmaps/misc/dashen-map.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/misc/ibm-ugl.txt` & `monobit-0.40.0/monobit/charmaps/misc/ibm-ugl.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/ALTVAR.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/ALTVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-7.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/ARMSCII-8A.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/ARMSCII-8A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/DECMCS.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/DECMCS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/GEO-ITA.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/GEO-ITA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/GEO-PS.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/GEO-PS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/IRANSYSTEM.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/IRANSYSTEM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/KOI8RU.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/KOI8RU.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/OSNOVAR.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/OSNOVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/README.md` & `monobit-0.40.0/monobit/charmaps/mleisher/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/mleisher/TIS620.TXT` & `monobit-0.40.0/monobit/charmaps/mleisher/TIS620.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/moztw/big5_2003-b2u.txt` & `monobit-0.40.0/monobit/charmaps/moztw/big5_2003-b2u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/moztw/eten.txt` & `monobit-0.40.0/monobit/charmaps/moztw/eten.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/python/TCVN5712-1.TXT` & `monobit-0.40.0/monobit/charmaps/python/TCVN5712-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/python/TCVN5712-2.TXT` & `monobit-0.40.0/monobit/charmaps/python/TCVN5712-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/python/TCVN5712-3.TXT` & `monobit-0.40.0/monobit/charmaps/python/TCVN5712-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/vietstd/unicode.html` & `monobit-0.40.0/monobit/charmaps/vietstd/unicode.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/vietstd/viscii1.1.txt` & `monobit-0.40.0/monobit/charmaps/vietstd/viscii1.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/abicomp.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/abicomp.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/brascii.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/brascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/cp853.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/cp853.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/cwi2.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/cwi2.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/dec-special.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/dec-special.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/dec-technical.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/dec-technical.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/gem.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/gem.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/kamenicky.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/kamenicky.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/lics.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/lics.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/mattel-aquarius.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/mattel-aquarius.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/mazovia.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/mazovia.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/pascii.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/pascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/ventura.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/ventura.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/windows-1252.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/windows-1252.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/wingdings.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/wingdings.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/wikipedia/wiscii.html` & `monobit-0.40.0/monobit/charmaps/wikipedia/wiscii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-1.enc` & `monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/xfonts/mulearabic-2.enc` & `monobit-0.40.0/monobit/charmaps/xfonts/mulearabic-2.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/xfonts/mulelao-1.enc` & `monobit-0.40.0/monobit/charmaps/xfonts/mulelao-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/xfonts/suneu-greek.enc` & `monobit-0.40.0/monobit/charmaps/xfonts/suneu-greek.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/charmaps/xfonts/viscii1.1-1.enc` & `monobit-0.40.0/monobit/charmaps/xfonts/viscii1.1-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/containers/compressors.py` & `monobit-0.40.0/monobit/containers/compressors.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/containers/container.py` & `monobit-0.40.0/monobit/containers/container.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/containers/directory.py` & `monobit-0.40.0/monobit/containers/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self, path='', mode='r', ignore_case=True):
         """Create directory wrapper."""
         # if empty path, this refers to the whole filesystem
         if not path:
             self._path = Path('/')
         elif isinstance(path, DirectoryStream):
             # directory 'streams'
-            self._path = Path(path.name)
+            self._path = Path(path.path)
         elif isinstance(path, Directory):
             self._path = Path(path._path)
         else:
             self._path = Path(path)
         # mode really should just be 'r' or 'w'
         mode = mode[:1]
         if mode == 'w':
```

### Comparing `monobit-0.39.3/monobit/containers/mac.py` & `monobit-0.40.0/monobit/containers/mac.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/containers/source.py` & `monobit-0.40.0/monobit/containers/source.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/containers/tar.py` & `monobit-0.40.0/monobit/containers/tar.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/containers/zip.py` & `monobit-0.40.0/monobit/containers/zip.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/amiga.py` & `monobit-0.40.0/monobit/formats/amiga.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/bbc.py` & `monobit-0.40.0/monobit/formats/bbc.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/bdf.py` & `monobit-0.40.0/monobit/formats/xlfd/bdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..binary import int_to_bytes, bytes_to_int, ceildiv
-from ..properties import normalise_property
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..font import Font, Coord
-from ..glyph import Glyph
-from ..encoding import charmaps, NotFoundError
-from ..taggers import tagmaps
-from ..labels import Char
+from ...binary import int_to_bytes, bytes_to_int, ceildiv
+from ...properties import normalise_property
+from ...storage import loaders, savers
+from ...magic import FileFormatError
+from ...font import Font, Coord
+from ...glyph import Glyph
+from ...encoding import charmaps, NotFoundError
+from ...taggers import tagmaps
+from ...labels import Char
 
 
 @loaders.register(
     name='bdf',
     magic=(b'STARTFONT ',),
     patterns=('*.bdf',),
 )
@@ -1006,14 +1006,17 @@
     has_vertical_metrics = any(
         _k in _g.properties
         for _g in font.glyphs
         for _k in vertical_metrics
     )
     if has_vertical_metrics:
         bdf_props.append(('METRICSSET', '2'))
+    # minimize glyphs to ink-bounds (BBX) before storing, except "cell" fonts
+    if font.spacing not in ('character-cell', 'multi-cell'):
+        font = font.reduce()
     # labels
     # get glyphs for encoding values
     encoded_glyphs = []
     for glyph in font.glyphs:
         if charmaps.is_unicode(font.encoding):
             if len(glyph.codepoint) == 1:
                 encoding, = glyph.codepoint
@@ -1041,17 +1044,14 @@
                 logging.warning(
                     f'Multi-codepoint glyph {glyph.codepoint}'
                     "can't be stored as no name or character available."
                 )
         encoded_glyphs.append((encoding, name, glyph))
     glyphs = []
     for encoding, name, glyph in encoded_glyphs:
-        # minimize glyphs to ink-bounds (BBX) before storing, except "cell" fonts
-        if font.spacing not in ('character-cell', 'multi-cell'):
-            glyph = glyph.reduce()
         swidth_y, dwidth_y = 0, 0
         # SWIDTH = DWIDTH / ( points/1000 * dpi / 72 )
         # DWIDTH specifies the widths in x and y, dwx0 and dwy0, in device pixels.
         # Like SWIDTH , this width information is a vector indicating the position of
         # the next glyph’s origin relative to the origin of this glyph.
         dwidth_x = glyph.advance_width
         swidth_x = _swidth(dwidth_x, font.point_size, font.dpi.x)
```

### Comparing `monobit-0.39.3/monobit/formats/bmfont.py` & `monobit-0.40.0/monobit/formats/bmfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/borland.py` & `monobit-0.40.0/monobit/formats/borland.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/cpi.py` & `monobit-0.40.0/monobit/formats/cpi.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/daisydot.py` & `monobit-0.40.0/monobit/formats/daisydot.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/dashen.py` & `monobit-0.40.0/monobit/formats/dashen.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/dec.py` & `monobit-0.40.0/monobit/formats/dec.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/dosstart.py` & `monobit-0.40.0/monobit/formats/dosstart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/figlet.py` & `monobit-0.40.0/monobit/formats/figlet.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/fontx.py` & `monobit-0.40.0/monobit/formats/fontx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/fzx.py` & `monobit-0.40.0/monobit/formats/fzx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/gdos.py` & `monobit-0.40.0/monobit/formats/gdos.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,15 +585,15 @@
         compressed=0,
         dbcs_flag=0,
         use_full_id=0,
     )
     header = _FNT_HEADER[endian](
         font_id=add_props.get('font-id', 255),
         point=font.point_size,
-        name=font.name.encode('ascii', 'replace'),
+        name=font.name.encode('ascii', 'replace')[:32],
         first_ade=int(min(font.get_codepoints())),
         last_ade=int(max(font.get_codepoints())),
         top=font.raster_size.y+add_shift_up,
         ascent=font.ascent-1,
         # Half line distance expressed as a positive offset from baseline.
         # interpreting as x-height
         half=font.x_height,
```

### Comparing `monobit-0.39.3/monobit/formats/geos.py` & `monobit-0.40.0/monobit/formats/geos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/hbf.py` & `monobit-0.40.0/monobit/formats/xlfd/hbf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
-monobit.formats.hbf - Hanzi Bitmap File Format
+monobit.formats.xlfd.hbf - Hanzi Bitmap File Format
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from pathlib import Path
 
-from ..properties import normalise_property
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..font import Font, Coord
-from ..glyph import Glyph
-from ..binary import ceildiv
+from ...properties import normalise_property
+from ...storage import loaders, savers
+from ...magic import FileFormatError
+from ...font import Font, Coord
+from ...glyph import Glyph
+from ...binary import ceildiv
 
 from .bdf import read_props, _parse_xlfd_properties, _create_xlfd_properties
 from .bdf import _create_xlfd_name
-from .yaff import _globalise_glyph_metrics
-from .windows import _normalise_metrics
+# from ..text.yaff import _globalise_glyph_metrics
+from ..windows import _normalise_metrics
 
 
 @loaders.register(
     name='hbf',
     magic=(b'HBF_START_FONT ',),
     patterns=('*.hbf',),
 )
```

### Comparing `monobit-0.39.3/monobit/formats/hurt.py` & `monobit-0.40.0/monobit/formats/hurt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/image.py` & `monobit-0.40.0/monobit/formats/image.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/mousegraphics.py` & `monobit-0.40.0/monobit/formats/mousegraphics.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/mzfon.py` & `monobit-0.40.0/monobit/formats/mzfon.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/nearlyraw.py` & `monobit-0.40.0/monobit/formats/nearlyraw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/palm.py` & `monobit-0.40.0/monobit/formats/palm.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/pcl.py` & `monobit-0.40.0/monobit/formats/pcl.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/pcpaint.py` & `monobit-0.40.0/monobit/formats/pcpaint.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/pdf.py` & `monobit-0.40.0/monobit/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/pkfont.py` & `monobit-0.40.0/monobit/formats/pkfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/printshop.py` & `monobit-0.40.0/monobit/formats/printshop.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/psf.py` & `monobit-0.40.0/monobit/formats/psf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/raw.py` & `monobit-0.40.0/monobit/formats/raw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/sfnt.py` & `monobit-0.40.0/monobit/formats/sfnt/sfnt.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,52 +5,44 @@
 licence: https://opensource.org/licenses/MIT
 """
 
 import sys
 import logging
 import json
 import math
+import re
 from unicodedata import bidirectional
 
-try:
-    from fontTools import ttLib
-except ImportError:
-    ttLib = None
-else:
-    from fontTools.ttLib import TTLibError
-    from fontTools.ttLib.ttFont import TTFont
-    from fontTools.ttLib.ttCollection import TTCollection
-
-from ..properties import Props
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..labels import Tag, Char
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from .windows.fnt import _WEIGHT_MAP
+from . import fonttools
+from .fonttools import check_fonttools
+
+from ...properties import Props
+from ...font import Font
+from ...glyph import Glyph
+from ...raster import Raster
+from ...labels import Tag, Char, Codepoint
+from ...storage import loaders, savers
+from ...magic import FileFormatError
+from ..windows.fnt import _WEIGHT_MAP, CHARSET_MAP
 
 
 # errors that invalidate only one strike or resource, not the whole file
 
 class ResourceFormatError(FileFormatError):
     """Unsupported parameters in resource."""
 
 class StrikeFormatError(ResourceFormatError):
     """Unsupported parameters in bitmap strike."""
 
 
-# must be importable by mac module
-load_sfnt = None
-
 # resource header
 SFNT_MAGIC = b'\0\1\0\0'
 
 
-if ttLib:
+if fonttools.loaded:
     @loaders.register(
         name='sfnt',
         magic=(
             SFNT_MAGIC,
             # alternative headers which also occur:
             # TrueType
             b'true',
@@ -62,26 +54,27 @@
         patterns=('*.otb', '*.ttf', '*.otf', '*.woff', '*.tte',),
     )
     # pylint: disable=function-redefined
     def load_sfnt(
             infile,
             hmtx:bool=False, vmtx:bool=False,
             hhea:bool=False, vhea:bool=False,
-            os_2:bool=True
+            os_2:bool=True, post:bool=True,
         ):
         """
         Load an SFNT resource and convert to Font.
 
         hmtx: override horizontal bitmap metrics with `hmtx` table (default: False)
         vmtx: override vertical bitmap metrics with `vmtx` table (default: False)
         hhea: include horizontal line metrics from `hhea` table (default: False)
         vhea: include vertical line metrics from `vhea` table (default: False)
-        os_2: include metrics from OS/2 table (default: True)
+        os_2: include metrics from `OS/2` table (default: True)
+        post: include metrics from `post` table (default: True)
         """
-        tags = _get_tags(hmtx, vmtx, hhea, vhea, os_2)
+        tags = _get_tags(hmtx, vmtx, hhea, vhea, os_2, post)
         sfnt = _read_sfnt(infile, tags)
         logging.debug(str(sfnt))
         fonts = _convert_sfnt(sfnt)
         return fonts
 
 
     @loaders.register(
@@ -92,159 +85,209 @@
         ),
         patterns=('*.ttc', '*.otc'),
     )
     def load_collection(
             infile,
             hmtx:bool=False, vmtx:bool=False,
             hhea:bool=False, vhea:bool=False,
-            os_2:bool=True
+            os_2:bool=True, post:bool=True,
         ):
         """
         Load a TrueType/OpenType Collection file.
 
         hmtx: override horizontal bitmap metrics with `hmtx` table (default: False)
         vmtx: override vertical bitmap metrics with `vmtx` table (default: False)
         hhea: include horizontal line metrics from `hhea` table (default: False)
         vhea: include vertical line metrics from `vhea` table (default: False)
-        os_2: include metrics from OS/2 table (default: True)
+        os_2: include metrics from `OS/2` table (default: True)
+        post: include metrics from `post` table (default: True)
         """
-        tags = _get_tags(hmtx, vmtx, hhea, vhea, os_2)
+        tags = _get_tags(hmtx, vmtx, hhea, vhea, os_2, post)
         sfnts = _read_collection(infile, tags)
         fonts = []
         for _sfnt in sfnts:
             fonts.extend(_convert_sfnt(_sfnt))
         return fonts
 
+else:
+    # ensure names are importable; sfnt used by mac, win modules
+    load_sfnt = check_fonttools
+    load_collection = check_fonttools
+
 
 ###############################################################################
-# fontTools extensions
+# common encoding tables
 
-# bdat/bloc tables are Apple's version of EBDT/EBLC.
-# They have the same structure but a different tag.
-table__b_h_e_d = None
-table__b_l_o_c = None
-table__b_d_a_t = None
-
-def _init_fonttools():
-    """Register extension classes for fontTools."""
-    if not ttLib:
-        raise FileFormatError(
-            'Parsing `sfnt` resources requires module `fontTools`, '
-            'which is not available.'
-        )
-    global table__b_h_e_d, table__b_l_o_c, table__b_d_a_t
-    if table__b_d_a_t:
-        return
-
-    from fontTools.ttLib.tables._h_e_a_d import table__h_e_a_d
-    from fontTools.ttLib.tables.E_B_L_C_ import table_E_B_L_C_
-    from fontTools.ttLib.tables.E_B_D_T_ import table_E_B_D_T_
-
-    class table__b_h_e_d(table__h_e_a_d): pass
-    class table__b_l_o_c(table_E_B_L_C_): pass
-
-    class table__b_d_a_t(table_E_B_D_T_):
-        locatorName = "bloc"
-
-    ttLib.registerCustomTableClass('bhed', 'monobit.formats.sfnt')
-    ttLib.registerCustomTableClass('bloc', 'monobit.formats.sfnt')
-    ttLib.registerCustomTableClass('bdat', 'monobit.formats.sfnt')
+# shared with mac
 
+# based on:
+# [1] Apple Technotes (As of 2002)/te/te_02.html
+# [2] https://developer.apple.com/library/archive/documentation/mac/Text/Text-367.html#HEADING367-0
+MAC_ENCODING = {
+    0: 'mac-roman',
+    1: 'mac-japanese',
+    2: 'mac-trad-chinese',
+    3: 'mac-korean',
+    4: 'mac-arabic',
+    5: 'mac-hebrew',
+    6: 'mac-greek',
+    7: 'mac-cyrillic', # [1] russian
+    # 8: [2] right-to-left symbols
+    9: 'mac-devanagari',
+    10: 'mac-gurmukhi',
+    11: 'mac-gujarati',
+    12: 'mac-oriya',
+    13: 'mac-bengali',
+    14: 'mac-tamil',
+    15: 'mac-telugu',
+    16: 'mac-kannada',
+    17: 'mac-malayalam',
+    18: 'mac-sinhalese',
+    19: 'mac-burmese',
+    20: 'mac-khmer',
+    21: 'mac-thai',
+    22: 'mac-laotian',
+    23: 'mac-georgian',
+    24: 'mac-armenian',
+    25: 'mac-simp-chinese', # [1] maldivian
+    26: 'mac-tibetan',
+    27: 'mac-mongolian',
+    28: 'mac-ethiopic', # [2] == geez
+    29: 'mac-centraleurope', # [1] non-cyrillic slavic
+    30: 'mac-vietnamese',
+    31: 'mac-sindhi', # [2] == ext-arabic
+    #32: [1] [2] 'uninterpreted symbols'
+}
+
+WIN_ENCODING = {
+    # Symbol, but apparently not windows-symbol but any undefined encoding
+    0: '',
+    1: 'utf-16le', # unicode bmp
+    2: 'ms932', # shift-jis
+    3: 'ms936', # PRC
+    4: 'ms950', # Big-5
+    5: 'ms949', # Wansung
+    6: 'ms1361', # Johab
+    10: 'utf-16le', # Unicode full repertoire
+}
+
+ISO_ENCODING = {
+    0: 'ascii',
+    # unicode
+    1: 'iso-10646',
+    # latin-1
+    2: 'iso-8859-1',
+}
+
+PLATFORM_ENCODING = {
+    # macintosh platform
+    1: MAC_ENCODING,
+    # ISO platform
+    2: ISO_ENCODING,
+    # Windows platform
+    3: WIN_ENCODING,
+    # legacy windows charset value
+    4: CHARSET_MAP,
+}
 
 ###############################################################################
 # sfnt resource reader
 
-
 # tags we will decompile and process
 _TAGS = (
     # check `maxp` first to catch any assertion errors on decompile
     'maxp',
     # core bitmap tables
-    'bhed', 'head',
+    'head', 'bhed',
     'EBLC', 'bloc',
     'EBDT', 'bdat',
+    'EBSC',
     # sbix: currently just warn we don't parse it
     'sbix',
     # metrics
     'hmtx', 'hhea',
     'vmtx', 'vhea',
     'OS/2',
+    # underline metrics and glyph name tags
+    'post',
     # metadata
     'name',
     # kerning information
     'kern',
     'GPOS',
     # encoding
     'cmap',
 )
 
-def _get_tags(hmtx, vmtx, hhea, vhea, os_2):
+def _get_tags(hmtx, vmtx, hhea, vhea, os_2, post):
     """Get list of tables to extract."""
     tags = list(_TAGS)
     if not hmtx:
         tags.remove('hmtx')
     if not vmtx:
         tags.remove('vmtx')
     if not hhea:
         tags.remove('hhea')
     if not vhea:
         tags.remove('vhea')
     if not os_2:
         tags.remove('OS/2')
+    if not post:
+        tags.remove('post')
     return tags
 
 
 def _read_sfnt(instream, tags):
     """Read an SFNT resource into data structure."""
     # let fonttools parse the SFNT
-    _init_fonttools()
+    check_fonttools()
     try:
-        ttf = TTFont(instream)
-    except (TTLibError, AssertionError) as e:
+        ttf = fonttools.TTFont(instream)
+    except (fonttools.TTLibError, AssertionError) as e:
         raise FileFormatError(f'Could not read sfnt file: {e}')
     return _sfnt_props(ttf, tags)
 
 def _read_collection(instream, tags):
     """Read a collection into data structures."""
     # let fonttools parse the SFNT
-    _init_fonttools()
+    check_fonttools()
     try:
-        ttfc = TTCollection(instream)
-    except (TTLibError, AssertionError) as e:
+        ttcf = fonttools.TTCollection(instream)
+    except (fonttools.TTLibError, AssertionError) as e:
         raise FileFormatError(f'Could not read collection file: {e}')
-    ttfc_data = []
-    for ttf in ttfc:
+    ttcf_data = []
+    for ttf in ttcf:
         try:
-            ttfc_data.append(_sfnt_props(ttf, tags))
+            ttcf_data.append(_sfnt_props(ttf, tags))
         except ResourceFormatError as e:
             logging.debug(e)
-    return ttfc_data
+    return ttcf_data
 
 
 def _sfnt_props(ttf, tags):
     """Decompile tables and convert from fontTools objects to data structure."""
     tables = {}
     for tag in _TAGS:
         if tag not in tags:
             tables[tag] = None
             continue
         try:
             # __getitem__ forces a decompilation of the table
             tables[tag] = ttf.get(tag, None)
-        except (TTLibError, AssertionError) as e:
+        except (fonttools.TTLibError, AssertionError) as e:
             if not str(e):
                 e = f'{type(e).__name__} in fontTools library.'
             logging.debug('Could not read `%s` table in sfnt: %s', tag, e)
     return Props(**_to_props(tables))
 
 
 def _to_props(obj):
     """Recursively convert fontTools objects to namespaces."""
     # avoid infinite recursion
-    if isinstance(obj, TTFont):
+    if isinstance(obj, fonttools.TTFont):
         return str(obj)
     if obj is None:
         return obj
     if isinstance(obj, dict):
         return {
             _k: _to_props(_v)
             for _k, _v in obj.items()
@@ -288,21 +331,33 @@
             'Bitmap strikes in `sbix` format not supported.'
         )
     if not sfnt.bdat or not sfnt.bloc:
         raise ResourceFormatError(
             'No `EBDT` or `bdat` bitmap strikes found in sfnt resource.'
         )
     fonts = []
+    unitable = _get_unicode_table(sfnt)
+    enctable, encoding = _get_encoding_table(sfnt)
     for i_strike in range(sfnt.bloc.numSizes):
         try:
             props = _convert_props(sfnt, i_strike)
-            glyphs = _convert_glyphs(sfnt, i_strike, props._hfupp, props._vfupp)
+            glyphs = _convert_glyphs(
+                sfnt, i_strike, props._hfupp, props._vfupp, unitable, enctable
+            )
             del props._hfupp
             del props._vfupp
-            fonts.append(Font(glyphs, source_format=source_format, **vars(props)))
+            # disabled - if we remove tags we break kerning (can label() adjust kerning too?)
+            # # remove temporary names created by fontTools
+            # # if there's no post table or it is empty
+            # if not sfnt.post or sfnt.post.formatType == 3.0:
+            #     glyphs = (_g.modify(tag=None) if _g.char else _g for _g in glyphs)
+            fonts.append(Font(
+                glyphs, source_format=source_format, encoding=encoding or None,
+                **vars(props)
+            ))
         except StrikeFormatError:
             pass
     return fonts
 
 
 def _convert_props(sfnt, i_strike):
     """Build font properties from sfnt data."""
@@ -313,23 +368,22 @@
     # we also had pixels per em in the EBLC table, so now we know units per pixel
     props = _convert_bloc_props(sfnt.bloc, i_strike)
     props |= _convert_head_props(sfnt.head)
     props |= _convert_name_props(sfnt.name)
     props |= _convert_os_2_props(getattr(sfnt, 'OS/2'), vert_fu_p_pix, hori_fu_p_pix)
     props |= _convert_hhea_props(sfnt.hhea, vert_fu_p_pix)
     props |= _convert_vhea_props(sfnt.vhea, hori_fu_p_pix)
+    props |= _convert_post_props(sfnt.post, vert_fu_p_pix)
     props._hfupp = hori_fu_p_pix
     props._vfupp = vert_fu_p_pix
     return props
 
 
-def _convert_glyphs(sfnt, i_strike, hori_fu_p_pix, vert_fu_p_pix):
+def _convert_glyphs(sfnt, i_strike, hori_fu_p_pix, vert_fu_p_pix, unitable, enctable):
     """Build glyphs and glyph properties from sfnt data."""
-    unitable = _get_unicode_table(sfnt)
-    enctable = _get_encoding_table(sfnt)
     glyphs = []
     strike = sfnt.bdat.strikeData[i_strike]
     blocstrike = sfnt.bloc.strikes[i_strike]
     for subtable in blocstrike.indexSubTables:
         # some formats are byte aligned, others bit-aligned
         if subtable.imageFormat in (1, 6):
             align = 'left'
@@ -384,15 +438,15 @@
             # hori
             left_bearing=metrics.horiBearingX,
             right_bearing=(
                 metrics.horiAdvance - metrics.width - metrics.horiBearingX
             ),
             shift_up=metrics.horiBearingY - metrics.height,
             # vert
-            shift_left=metrics.vertBearingX,
+            shift_left=metrics.vertBearingX - metrics.width//2,
             top_bearing=metrics.vertBearingY,
             bottom_bearing=(
                 metrics.vertAdvance - metrics.height
                 - metrics.vertBearingY
             ),
         )
     elif not small_is_vert:
@@ -401,15 +455,15 @@
             left_bearing=metrics.BearingX,
             right_bearing=metrics.Advance - metrics.width - metrics.BearingX,
             shift_up=metrics.BearingY - metrics.height,
         )
     else:
         # small metrics, interpret as vert
         return dict(
-            shift_left=metrics.BearingX,
+            shift_left=metrics.BearingX - metrics.width//2,
             top_bearing=metrics.BearingY,
             bottom_bearing=(
                 metrics.Advance - metrics.height - metrics.BearingY
             ),
         )
 
 
@@ -430,17 +484,16 @@
     # ISO platform (deprecated), ISO 10646
     (2, 1),
 )
 
 def _get_unicode_table(sfnt):
     """Get unicode mapping from sfnt data."""
     # find unicode encoding
-    known_tables = tuple(_t for _t in sfnt.cmap.tables)
     for id_pair in _UNICODE_CHOICES:
-        for table in known_tables:
+        for table in sfnt.cmap.tables:
             if (int(table.platformID), int(table.platEncID)) == id_pair:
                 unitable = {
                     _name: chr(int(_ord))
                     for _ord, _name in table.cmap.items()
                 }
                 break
         else:
@@ -448,30 +501,36 @@
         break
     else:
         unitable = {}
     return unitable
 
 def _get_encoding_table(sfnt):
     """Get non-unicode encoding from sfnt data."""
-    known_tables = tuple(_t for _t in sfnt.cmap.tables)
     # get the largest table for non-unicode mappings
     non_unicode_tables = (
-        _t.cmap for _t in known_tables
+        _t for _t in sfnt.cmap.tables
         if (int(_t.platformID), int(_t.platEncID)) not in _UNICODE_CHOICES
     )
     non_unicode_tables = sorted(
-        ((len(_t), _t) for _t in non_unicode_tables),
+        ((len(_t.cmap), _t) for _t in non_unicode_tables),
         reverse=True
     )
-    enctable = non_unicode_tables[0][1] if non_unicode_tables else {}
+    if not non_unicode_tables:
+        return {}, ''
+    largest_table = non_unicode_tables[0][1]
+    encoding = (
+        PLATFORM_ENCODING
+        .get(largest_table.platformID, {})
+        .get(largest_table.platEncID, '')
+    )
     enctable = {
         _name: int(_ord)
-        for _ord, _name in enctable.items()
+        for _ord, _name in largest_table.cmap.items()
     }
-    return enctable
+    return enctable, encoding
 
 
 ###############################################################################
 # 'hmtx' table
 
 def _convert_hmtx_metrics(hmtx, glyph_name, hori_fu_p_pix, width):
     """Convert horizontal metrics from hmtx table."""
@@ -505,21 +564,21 @@
 
 ###############################################################################
 # 'kern' table
 
 def _convert_kern_metrics(glyphs, kern, hori_fu_p_pix):
     """Convert kerning values form kern table."""
     if kern:
-        if kern.version != 0:
-            logging.warning(f'`kern` table version {kern.version} not supported.')
-            return {}
         glyph_props = {}
         for table in kern.kernTables:
+            if not hasattr(table, 'coverage') or not hasattr(table, 'kernTable'):
+                logging.warning('Kerning subtable format not supported')
+                continue
             if table.coverage != 1:
-                logging.warning('Vertical or cross-stream kerning not supported.')
+                logging.warning('Vertical or cross-stream kerning not supported')
                 continue
             for pair, kern_value in table.kernTable.items():
                 left, right = pair
                 ktable = glyph_props.get(Tag(left), {})
                 ktable[Tag(right)]  = kern_value / hori_fu_p_pix
                 glyph_props[Tag(left)] = ktable
         glyphs = tuple(
@@ -541,15 +600,15 @@
         llist = gpos.table.LookupList.Lookup
         glyph_props = {}
         for lookup in llist:
             for subtable in lookup.SubTable:
                 if subtable._type != 'PairPos':
                     continue
                 # per the docs, in logical order
-                # i.e first is left for LTR, first is right ror RTL
+                # i.e first is left for LTR, first is right for RTL
                 # presumably to be determined from glyph unicode properties?
                 # what happens if one glyph is LTR and the other RTL is unclear
                 # the one RTL file I have does things differently,
                 # and in line with this comment:
                 # https://fontforge-devel.narkive.com/s9C4jFO9/patch-1-2-fix-right-to-left-kerning
                 # i.e. the second glyph's Xadvance is adjusted by a negative number
                 # is this a hack to compensate for LTR-focussed real-world implementations?
@@ -615,15 +674,15 @@
     if bmst.flags not in (1, 2):
         logging.warning(
             f'Unsupported metric flag value {bmst.flags}, '
             'using 1 (horizontal) instead.'
         )
         bmst.flags = 1
     props = Props()
-    # asppect ratio is the inverse of pixels-per-em ratio
+    # aspect ratio is the inverse of pixels-per-em ratio
     den = math.gcd(bmst.ppemY, bmst.ppemX)
     props.pixel_aspect = (bmst.ppemY//den, bmst.ppemX//den)
     small_metrics_are_vert = bmst.flags == 2
     # horizontal line metrics
     # according to the EBLC spec the sbit metrics also define the linegap
     # but I don't see it. widthMax looks like a max advance
     props.ascent = bmst.hori.ascender
@@ -657,15 +716,15 @@
 
 def _convert_head_props(head):
     """Convert font properties from head/bhed table."""
     if not head:
         return Props()
     props = Props(
         revision=head.fontRevision,
-        style=mac_style_name(head.macStyle),
+        style=mac_style_name(head.macStyle) or None,
     )
     return props
 
 
 ###############################################################################
 # 'hhea' table
 
@@ -694,73 +753,24 @@
     props = Props(
         # > from the centerline to the previous line’s descent
         # > assuming top-to-bottom right-to-left
         right_extent=vhea.ascent // horiz_fu_p_pix,
         # > from the centerline to the next line’s descent
         left_extent=abs(vhea.descent) // horiz_fu_p_pix,
         line_width=(
-            (vhea.ascender + abs(vhea.descender) + vhea.lineGap)
+            (vhea.ascent + abs(vhea.descent) + vhea.lineGap)
             // horiz_fu_p_pix
         ),
     )
     return props
 
 
 ###############################################################################
 # 'name' table
 
-# based on:
-# [1] Apple Technotes (As of 2002)/te/te_02.html
-# [2] https://developer.apple.com/library/archive/documentation/mac/Text/Text-367.html#HEADING367-0
-MAC_ENCODING = {
-    0: 'mac-roman',
-    1: 'mac-japanese',
-    2: 'mac-trad-chinese',
-    3: 'mac-korean',
-    4: 'mac-arabic',
-    5: 'mac-hebrew',
-    6: 'mac-greek',
-    7: 'mac-cyrillic', # [1] russian
-    # 8: [2] right-to-left symbols
-    9: 'mac-devanagari',
-    10: 'mac-gurmukhi',
-    11: 'mac-gujarati',
-    12: 'mac-oriya',
-    13: 'mac-bengali',
-    14: 'mac-tamil',
-    15: 'mac-telugu',
-    16: 'mac-kannada',
-    17: 'mac-malayalam',
-    18: 'mac-sinhalese',
-    19: 'mac-burmese',
-    20: 'mac-khmer',
-    21: 'mac-thai',
-    22: 'mac-laotian',
-    23: 'mac-georgian',
-    24: 'mac-armenian',
-    25: 'mac-simp-chinese', # [1] maldivian
-    26: 'mac-tibetan',
-    27: 'mac-mongolian',
-    28: 'mac-ethiopic', # [2] == geez
-    29: 'mac-centraleurope', # [1] non-cyrillic slavic
-    30: 'mac-vietnamese',
-    31: 'mac-sindhi', # [2] == ext-arabic
-    #32: [1] [2] 'uninterpreted symbols'
-}
-#
-# WIN_ENCODING = {
-#     0: 'windows-symbol',
-#     1: 'utf-16le', # unicode bmp
-#     2: 'ms932', # shift-jis
-#     3: 'ms936', # PRC
-#     4: 'ms950', # Big-5
-#     5: 'ms949', # Wansung
-#     6: 'ms1361', # Johab
-#     10: 'utf-16le', # Unicode full repertoire
-# }
 def _decode_name(namerecs, nameid):
     for namerec in namerecs:
         if namerec.nameID != nameid:
             continue
         if namerec.platformID == 1:
             # mac
             encoding = MAC_ENCODING.get(namerec.platEncID, 'mac-roman')
@@ -769,49 +779,70 @@
             # > All string data for platform 3 must be encoded in UTF-16BE.
             encoding = 'utf-16be'
             #WIN_ENCODING.get(namerec.platEncID, 'utf-16le')
         elif namerec.platformID == 0:
             # unicode platform
             encoding = 'utf-16be'
         try:
-            return namerec.string.decode(encoding)
+            return namerec.string.decode(encoding) or None
         except UnicodeError:
             pass
         # not all these encodings will be recognised by Python
         # fallback to latin-1
-        return namerec.string.decode('latin-1')
+        return namerec.string.decode('latin-1') or None
     return None
 
+
+def _convert_version_string(version_string):
+    """Convert standard sfnt version string to something more like ours."""
+    # version is encoded as 'Version x.y', optionally followed by non-numeric info
+    # split by non-(digit or dot)
+    groups = re.split(r'([\d\.]+)', version_string)
+    if len(groups) < 2 or groups[0].lower() != 'version ':
+        # non-compliant version string, preserve as is
+        pass
+    else:
+        version_number = str(float(groups[1]))
+        if len(groups) == 2:
+            return version_number
+        version_string = ''.join(groups[2:])
+        if version_number not in version_string:
+            version_string = version_number + version_string
+        # non-alpha separator
+        if not version_string[0].isalnum():
+            version_string = version_string[1:]
+    return version_string.strip().rstrip('0').rstrip('.')
+
 def _convert_name_props(name):
     """Convert font properties from name table."""
     if not name:
         return Props()
     props = Props(
         copyright=_decode_name(name.names, 0),
         family=_decode_name(name.names, 1),
         # weight or slant or both
-        #subfamily=_decode_name(name.names, 2),
+        subfamily=_decode_name(name.names, 2),
         font_id=_decode_name(name.names, 3),
         name=_decode_name(name.names, 4),
         #
-        revision=_decode_name(name.names, 5),
+        revision=_convert_version_string(_decode_name(name.names, 5)),
         #
         #postscript_name
         #
-        trademark=_decode_name(name.names, 7),
+        #trademark=_decode_name(name.names, 7),
         foundry=_decode_name(name.names, 8),
         author=_decode_name(name.names, 9),
         #
-        description=_decode_name(name.names, 10),
+        #description=_decode_name(name.names, 10),
         #
-        vendor_url=_decode_name(name.names, 11),
+        #vendor_url=_decode_name(name.names, 11),
         #
-        author_url=_decode_name(name.names, 12),
+        #author_url=_decode_name(name.names, 12),
         notice=_decode_name(name.names, 13),
-        license_url=_decode_name(name.names, 14),
+        #license_url=_decode_name(name.names, 14),
     )
     return props
 
 
 ###############################################################################
 # 'OS/2' table
 
@@ -849,22 +880,42 @@
         superscript_offset=(
             int(os_2.ySuperscriptXOffset // hori_fu_p_pix),
             int(os_2.ySuperscriptYOffset // vert_fu_p_pix)
         ),
         #ascent=os_2.sTypoAscender // vert_fu_p_pix,
         # the spec states sTypoDescender is 'usually' negative,
         # but fonttosfnt produces + values while fontforge -
-        # abs should be fine as I have nno interpretation for a negative descent
+        # abs should be fine as I have no interpretation for a negative descent
         # note the sign also affects int division
         #descent=abs(os_2.sTypoDescender // vert_fu_p_pix),
         line_height=(
             os_2.sTypoAscender + abs(os_2.sTypoDescender) + os_2.sTypoLineGap
         ) // vert_fu_p_pix,
     )
     if os_2.version > 1:
         props |= Props(
             x_height=os_2.sxHeight // vert_fu_p_pix,
             cap_height=os_2.sCapHeight // vert_fu_p_pix,
             default_char=Char(chr(os_2.usDefaultChar)),
             word_boundary=Char(chr(os_2.usBreakChar)),
         )
+        # > This is the Unicode code point, in UTF-16 encoding, of a character
+        # > that can be used for a default glyph if a requested character is not
+        # > supported in the font. If the value of this field is zero,
+        # > glyph ID 0 is to be used for the default character.
+        if props.default_char == Char('\0'):
+            props.default_char = Tag('.notdef')
+    return props
+
+
+###############################################################################
+# 'post' table
+
+def _convert_post_props(post, vert_fu_p_pix):
+    """Convert font properties from `post` table."""
+    if not post:
+        return Props()
+    props = Props(
+        underline_descent=-post.underlinePosition // vert_fu_p_pix or None,
+        underline_thickness=post.underlineThickness // vert_fu_p_pix or None,
+    )
     return props
```

### Comparing `monobit-0.39.3/monobit/formats/signum.py` & `monobit-0.40.0/monobit/formats/signum.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/svg.py` & `monobit-0.40.0/monobit/formats/svg.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/vfont.py` & `monobit-0.40.0/monobit/formats/vfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/yaff.py` & `monobit-0.40.0/monobit/formats/text/yaff.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 """
-monobit.formats.yaff - monobit-yaff format
+monobit.formats.text.yaff - monobit-yaff format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 import string
 from dataclasses import dataclass, field
 from itertools import count, zip_longest
 from collections import deque
+from functools import cached_property
 
-from ..storage import loaders, savers
-from ..encoding import charmaps
-from ..magic import FileFormatError
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..labels import Label, strip_matching
-from ..properties import normalise_property
-from ..basetypes import passthrough
+from ...storage import loaders, savers
+from ...encoding import charmaps
+from ...magic import FileFormatError
+from ...font import Font
+from ...glyph import Glyph
+from ...raster import Raster
+from ...labels import Label, strip_matching
+from ...properties import Props, normalise_property
+from ...basetypes import passthrough
+from .draw import NonEmptyBlock, DrawComment, Empty, Unparsed, iter_blocks
+from .draw import format_comment
 
 
 ##############################################################################
 # interface
 
-
 @loaders.register(
     name='yaff',
     # maybe, if multi-section
     magic=(b'---',),
     patterns=('*.yaff', '*.yaffs',),
 )
 def load_yaff(instream, allow_empty:bool=False):
     """
     Load font from a monobit .yaff file.
 
     allow_empty: allow files with no glyphs (default: False)
     """
-    return _load_yaff(instream.text, allow_empty)
+    return _load_yaffs(instream.text, allow_empty)
 
 
 @savers.register(
     linked=load_yaff,
 )
 def save_yaff(fonts, outstream):
     """Write fonts to a monobit .yaff file."""
@@ -71,244 +73,238 @@
     paper = '.'
     empty = '-'
 
     # string to be quoted if one of these chars at start and/or end
     quotable = (':', ' ')
     glyphchars = (ink, paper, empty)
 
-##############################################################################
+
 ##############################################################################
 # read file
 
 
-def _load_yaff(text_stream, allow_empty):
-    """Parse a yaff/yaffs file."""
-    reader = YaffReader()
+def _load_yaffs(text_stream, allow_empty):
+    """Parse a yaff or yaffs file."""
     fonts = []
-    has_next_section = True
-    while has_next_section:
-        reader = YaffReader()
-        has_next_section = reader.parse_section(text_stream)
-        font = reader.get_font()
+    reader = SectionIterator(text_stream)
+    while not reader.eof:
+        font = _read_yaff(reader)
         # if no glyphs, ignore it - may not be yaff at all
         if font.glyphs or allow_empty:
             fonts.append(font)
     return fonts
 
 
-@dataclass
-class YaffElement:
-    keys: list = field(default_factory=list)
-    value: list = field(default_factory=list)
-    comment: list = field(default_factory=list)
-    indent: int = 0
-
-
-class YaffReader:
-    """Parser for text-based font file."""
-
-    def __init__(self):
-        """Set up text reader."""
-        # current element appending to
-        # elements done
-        self._elements = deque()
-
-    # first pass: lines to elements
-
-    def _yield_element(self, current):
-        """Close and append current element and start a new one."""
-        if current.keys or current.value or current.comment:
-            self._elements.append(current)
-        return YaffElement()
-
-    def parse_section(self, text_stream):
-        """Parse a single yaff section."""
-        current = YaffElement()
-        for line in text_stream:
-            # strip trailing whitespace
-            contents = line.rstrip()
-            if contents == BOUNDARY_MARKER:
-                self._yield_element(current)
-                # ignore empty sections
-                if self._elements:
-                    return True
-            if not contents:
-                # ignore empty lines except while already parsing comments
-                if (
-                        current.comment
-                        and not current.value
-                        and not current.keys
-                    ):
-                    current.comment.append('')
-            else:
-                startchar = contents[:1]
-                if startchar == YaffParams.comment:
-                    if current.keys or current.value:
-                        # new comment starts new element
-                        current = self._yield_element(current)
-                    current.comment.append(contents[1:])
-                elif startchar not in YaffParams.whitespace:
-                    if current.value:
-                        # new key when we have a value starts a new element
-                        current = self._yield_element(current)
-                    # note that we don't use partition() for the first check
-                    # as we have to allow for : inside (quoted) glyph labels
-                    if contents[-1:] == YaffParams.separator:
-                        current.keys.append(contents[:-1])
-                    else:
-                        # this must be a property key, not a glyph label
-                        # new key, separate at the first :
-                        # prop keys must be alphanum so no need to worry about quoting
-                        key, sep, value = contents.partition(YaffParams.separator)
-                        # yield key and value
-                        # yaff does not allow multiline values starting on the key line
-                        current.keys.append(key.rstrip())
-                        current.value.append(value.lstrip())
-                        current = self._yield_element(current)
-                else:
-                    # first line in value
-                    if not current.value:
-                        current.indent = len(contents) - len(contents.lstrip())
-                    # continue building value
-                    # do not strip all whitespace as we need it for multiline glyph props
-                    # but strip the first line's indent
-                    current.value.append(contents[current.indent:])
-        self._yield_element(current)
-        return False
-
-    # second pass: top comment
-
-    def get_clusters(self):
-        """Convert top comment cluster and return."""
-        clusters = self._elements
-        # separate out global top comment
-        if clusters and clusters[0]:
-            top = clusters[0]
-            comments = top.comment
-            # find last empty line which separates global from prop comment
-            try:
-                index = len(comments) - comments[::-1].index('')
-            except ValueError:
-                index = len(comments) + 1
-            if len(comments) > 1:
-                global_comment = YaffElement(comment=comments[:index-1])
-                top.comment = comments[index:]
-                clusters.appendleft(global_comment)
-        return clusters
-
-
-    # third pass: interpret clusters
-
-    def get_font(self):
-        """Get clusters from reader and convert to Font."""
-        clusters = self.get_clusters()
-        # recursive call
-        glyphs, props, comments = convert_clusters(clusters)
-        return Font(glyphs, comment=comments, **props)
-
-
-def convert_clusters(clusters):
-    """Convert cluster."""
-    props = {}
-    comments = {}
-    glyphs = []
-    for cluster in clusters:
-        if not cluster.keys:
-            # global comment
-            comments[''] = normalise_comment(cluster.comment)
-        elif not set(cluster.value[0]) - set(YaffParams.glyphchars):
-            # if first line in the value consists of glyph symbols, it's a glyph
-            # note that the set diff is significantly faster than all() on a genexp
-            glyphs.append(_convert_glyph(cluster))
+class SectionIterator:
+
+    def __init__(self, textstream):
+        self._stream = textstream
+        self.eof = False
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self.eof:
+            raise StopIteration()
+        line = self._stream.readline()
+        if not line:
+            self.eof = True
+            raise StopIteration()
+        if line[:3] == BOUNDARY_MARKER:
+            raise StopIteration()
         else:
-            key, value, comment = convert_property(cluster)
-            if value:
-                props[key] = value
-            # property comments
-            if comment:
-                comments[key] = comment
-    return glyphs, props, comments
-
-def convert_property(cluster):
-    """Convert property cluster."""
-    # there should not be multiple keys for a property
-    key = cluster.keys.pop(0)
-    if cluster.keys:
-        logging.warning('ignored excess keys: %s', cluster.keys)
-    # Props object converts only non-leading underscores
-    # so we need to make sure we turn those into dashes
-    key = key.replace('_', '-')
-    value = '\n'.join(strip_matching(_line, '"') for _line in cluster.value)
-    comment = normalise_comment(cluster.comment)
-    return key, value, comment
-
-def _convert_glyph(cluster):
-    """Parse single glyph."""
-    keys = cluster.keys
-    lines = cluster.value
-    comment = normalise_comment(cluster.comment)
-    # find first property row
-    # note empty lines have already been dropped by reader
-    is_prop = tuple(YaffParams.separator in _line for _line in lines)
-    try:
-        first_prop = is_prop.index(True)
-    except ValueError:
-        first_prop = len(lines)
-    raster = lines[:first_prop]
-    prop_lines = lines[first_prop:]
-    if all(set(_line) == set([YaffParams.empty]) for _line in raster):
-        raster = Raster.blank(width=len(raster[0])-1, height=len(raster)-1)
-    # new text reader on glyph property lines
-    reader = YaffReader()
-    reader.parse_section(prop_lines)
-    # ignore in-glyph comments
-    props = dict(
-        convert_property(cluster)[:2]
-        for cluster in reader.get_clusters()
-        if cluster.keys
+            return line
+
+
+def _read_yaff(text_stream):
+    """Parse a monobit yaff file."""
+    blocktypes = (
+        YaffComment, YaffProperty, YaffGlyph, YaffPropertyOrGlyph,
+        Empty, Unparsed
     )
-    # labels
-    glyph = Glyph(
-        raster, _0=YaffParams.paper, _1=YaffParams.ink,
-        labels=keys, comment=comment, **props
+    glyphs = []
+    font_comments = []
+    font_props = {}
+    font_prop_comms = {}
+    current_comment = []
+    for block in iter_blocks(text_stream, blocktypes):
+        if isinstance(block, (YaffGlyph, YaffPropertyOrGlyph)) and block.is_glyph():
+            glyphs.append(block.get_glyph_value() | Props(
+                comment='\n\n'.join(current_comment),
+            ))
+            current_comment = []
+        elif isinstance(block, (YaffProperty, YaffPropertyOrGlyph)):
+            key = block.get_key()
+            font_props[key] = block.get_value()
+            font_prop_comms[key] = '\n\n'.join(current_comment)
+            current_comment = []
+        if not glyphs and not font_props:
+            font_comments.extend(current_comment)
+            current_comment = []
+        if isinstance(block, YaffComment):
+            current_comment.append(block.get_value())
+        elif not isinstance(block, (YaffProperty, YaffGlyph, YaffPropertyOrGlyph)):
+            logging.debug('Unparsed lines: %s', block.get_value())
+    font_comments.extend(current_comment)
+    return Font(
+        (Glyph(**vars(_g)) for _g in glyphs), **font_props,
+        comment={'': '\n\n'.join(font_comments), **font_prop_comms},
     )
-    return glyph
 
 
-def normalise_comment(lines):
-    """Remove common single leading space"""
-    if all(_line[0] == ' ' for _line in lines if _line):
-        return '\n'.join(_line[1:] for _line in lines)
-    return '\n'.join(lines)
+class YaffComment(DrawComment):
 
+    def starts(self, line):
+        return line[:1] == YaffParams.comment
+
+
+class YaffMultiline(NonEmptyBlock, YaffParams):
+
+    def __init__(self, line):
+        self.indent = 0
+        super().__init__(line)
+
+    def ends(self, line):
+        if self.indent:
+            # dedent
+            return line and line[:1] not in self.whitespace
+        if line and line[:1] in self.whitespace:
+            return False
+        # gather multiple labels without values, but break on line with value
+        return line.rstrip()[-1:] != self.separator
+
+    def append(self, line):
+        line = line.rstrip()
+        self.lines.append(line)
+        if not self.indent and line and line[:1] in self.whitespace:
+            self.indent = len(line) - len(line.lstrip())
+
+
+class YaffGlyph(YaffMultiline):
+
+    label_chars = tuple('"' + "'" + string.digits)
+
+    def starts(self, line):
+        return line and (line[:1] in self.label_chars) or '+' in line
+
+    def get_value(self):
+        labels = tuple(_l[:-1] for _l in self.lines[:self.n_keys])
+        lines = (_l[self.indent:] for _l in self.lines[self.n_keys:])
+        lines = tuple(_l for _l in lines if _l)
+        # locate glyph properties
+        for i, line in enumerate(lines):
+            if line[:1] not in (self.paper, self.ink) and set(line) != set(self.empty):
+                break
+        else:
+            i += 1
+        raster = lines[:i]
+        properties = {}
+        key = None
+        for line in lines[i:]:
+            if line[:1] in self.whitespace:
+                # multiline glyph properties
+                if not properties[key]:
+                    properties[key] = line.strip()
+                else:
+                    properties[key] = '\n'.join((properties[key], line.strip()))
+            else:
+                # one-line glyph properties
+                key, _, value = line.partition(self.separator)
+                value = value.strip()
+                properties[key] = value.strip()
+        # deal with sized empties (why?)
+        if all(set(_line) == set([self.empty]) for _line in raster):
+            raster = Raster.blank(width=len(raster[0])-1, height=len(raster)-1)
+        return Props(
+            pixels=Raster(raster, _0=self.paper, _1=self.ink),
+            labels=labels, **properties
+        )
+
+    def _count_keys(self):
+        return sum(
+            _line[-1:] == self.separator and _line[:1] not in self.whitespace
+            for _line in self.lines
+        )
+    n_keys = cached_property(_count_keys)
+
+    def is_glyph(self):
+        return True
+
+    get_glyph_value = get_value
+
+
+class YaffProperty(NonEmptyBlock, YaffParams):
+
+    def starts(self, line):
+        return (
+            line[:1] not in self.whitespace
+            and line[-1:] != self.separator
+            and self.separator in line
+        )
+
+    def get_value(self):
+        _, _, value = self.lines[0].partition(self.separator)
+        return _strip_quotes(value)
+
+    def get_key(self):
+        key, _, _ = self.lines[0].partition(self.separator)
+        return key
+
+
+def _strip_quotes(line):
+    line = line.strip()
+    if len(line) > 1 and line[0] == line[-1] == '"':
+        return line[1:-1]
+    return line
+
+
+class YaffPropertyOrGlyph(YaffMultiline):
+
+    def starts(self, line):
+        return line[:1] not in self.whitespace and line[-1:] == self.separator
+
+    def get_value(self):
+        return '\n'.join(_strip_quotes(_l) for _l in self.lines[1:])
+
+    def get_key(self):
+        return self.lines[0][:-1]
+
+    # glyph block with plain label
+
+    get_glyph_value = YaffGlyph.get_value
+    n_keys = cached_property(YaffGlyph._count_keys)
+
+    def is_glyph(self):
+        if self.n_keys > 1:
+            return True
+        # n_keys == 1, so first non-key line is 1
+        first = self.lines[1].lstrip()
+        # multiline block with single key
+        # may be property or (deprecated) glyph with plain label
+        # we need to check the contents
+        return first[:1] in (self.ink, self.paper) or set(first) == set(self.empty)
 
 
-##############################################################################
 ##############################################################################
 # write file
 
-
-def _globalise_glyph_metrics(mod_glyphs):
+def _globalise_glyph_metrics(glyphs):
     """If all glyph props are equal, take them global."""
     properties = {}
     for key in (
-            'shift-up', 'left-bearing', 'right-bearing',
-            'shift-left', 'top-bearing', 'bottom-bearing',
+            'shift_up', 'left_bearing', 'right_bearing',
+            'shift_left', 'top_bearing', 'bottom_bearing',
         ):
-        distinct = set(
-            getattr(_g, normalise_property(key))
-            for _g in mod_glyphs
-        )
+        distinct = set(_g.get_defined(key) for _g in glyphs)
         if len(distinct) == 1:
-            mod_glyphs = tuple(_g.drop(key) for _g in mod_glyphs)
             value = distinct.pop()
-            # NOTE - these all have zero defaults
-            if value != 0:
+            if value is not None:
                 properties[key] = value
-    return mod_glyphs, properties
+    return properties
 
 
 def _save_yaff(fonts, outstream):
     """Write fonts to a plaintext stream as yaff."""
     for number, font in enumerate(fonts):
         if len(fonts) > 1:
             outstream.write(BOUNDARY_MARKER + '\n')
@@ -326,55 +322,55 @@
             'spacing': font.spacing,
         }
         if font.spacing in ('character-cell', 'multi-cell'):
             props['cell_size'] = font.cell_size
         else:
             props['bounding_box'] = font.bounding_box
         props.update(font.properties)
-        glyphs, global_metrics = _globalise_glyph_metrics(font.glyphs)
+        global_metrics = _globalise_glyph_metrics(font.glyphs)
         props.update(global_metrics)
         if props:
             # write recognised yaff properties first, in defined order
             for key, value in props.items():
-                _write_property(outstream, key, value, font.get_comment(key))
+                if value != font.get_default(key):
+                    _write_property(outstream, key, value, font.get_comment(key))
             outstream.write('\n')
-        for glyph in glyphs:
-            _write_glyph(outstream, glyph)
+        for glyph in font.glyphs:
+            _write_glyph(outstream, glyph, global_metrics)
 
-def _write_glyph(outstream, glyph, label=None):
+def _write_glyph(outstream, glyph, global_metrics):
     """Write out a single glyph in text format."""
     # glyph comments
     if glyph.comment:
         outstream.write(
             '\n' + format_comment(glyph.comment, YaffParams.comment) + '\n'
         )
-    if label:
-        labels = [label]
-    else:
-        labels = glyph.get_labels()
-    if not labels:
-        outstream.write(f'{YaffParams.separator}\n')
+    labels = glyph.get_labels() or ['']
     for _label in labels:
         outstream.write(f'{str(_label)}{YaffParams.separator}\n')
     # glyph matrix
     # empty glyphs are stored as 0x0, not 0xm or nx0
-    if not glyph.width or not glyph.height:
+    if not glyph.pixels.width or not glyph.pixels.height:
         glyphtxt = f'{YaffParams.tab}{YaffParams.empty}\n'
     else:
-        glyphtxt = glyph.as_text(
+        glyphtxt = glyph.pixels.as_text(
             start=YaffParams.tab,
             ink=YaffParams.ink, paper=YaffParams.paper,
             end='\n'
         )
     outstream.write(glyphtxt)
-    if glyph.properties:
+    properties = glyph.properties
+    for key in global_metrics:
+        properties.pop(key.replace('_', '-'), None)
+    if properties:
         outstream.write(f'\n')
-    for key, value in glyph.properties.items():
-        _write_property(outstream, key, value, None, indent=YaffParams.tab)
-    if glyph.properties:
+    for key, value in properties.items():
+        if value != glyph.get_default(key):
+            _write_property(outstream, key, value, None, indent=YaffParams.tab)
+    if properties:
         outstream.write('\n')
     outstream.write('\n')
 
 def _write_property(outstream, key, value, comments, indent=''):
     """Write out a property."""
     if value is None:
         return
@@ -414,15 +410,7 @@
             or value[0] in YaffParams.quotable
             or value[-1] in YaffParams.quotable
             or value[0] == value[-1] == '"'
             or all(_c in YaffParams.glyphchars for _c in value)
         ):
         return f'"{value}"'
     return value
-
-
-def format_comment(comments, comment_char):
-    """Format a multiline comment."""
-    return '\n'.join(
-        f'{comment_char} {_line}'
-        for _line in comments.splitlines()
-    )
```

### Comparing `monobit-0.39.3/monobit/formats/mac/__init__.py` & `monobit-0.40.0/monobit/formats/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/mac/dfont.py` & `monobit-0.40.0/monobit/formats/mac/dfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/mac/fond.py` & `monobit-0.40.0/monobit/formats/mac/fond.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/mac/iigs.py` & `monobit-0.40.0/monobit/formats/mac/iigs.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/mac/lisa.py` & `monobit-0.40.0/monobit/formats/mac/lisa.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/mac/nfnt.py` & `monobit-0.40.0/monobit/formats/mac/nfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/os2/__init__.py` & `monobit-0.40.0/monobit/formats/os2/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/os2/gpifont.py` & `monobit-0.40.0/monobit/formats/os2/gpifont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/os2/lx.py` & `monobit-0.40.0/monobit/formats/os2/lx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/os2/ne.py` & `monobit-0.40.0/monobit/formats/os2/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/windows/LICENSE.md` & `monobit-0.40.0/monobit/formats/windows/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/windows/__init__.py` & `monobit-0.40.0/monobit/formats/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/windows/fnt.py` & `monobit-0.40.0/monobit/formats/windows/fnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,21 +563,21 @@
     if win_props.dfStrikeOut:
         deco.append('strikethrough')
     if deco:
         properties['decoration'] = ' '.join(deco)
     weight = win_props.dfWeight
     if weight:
         weight = max(100, min(900, weight))
-        properties['weight'] = _WEIGHT_MAP[round(weight, -2)]
+        properties['weight'] = _WEIGHT_MAP.get(round(weight, -2), None)
     charset = win_props.dfCharSet
     if charset in CHARSET_MAP:
         properties['encoding'] = CHARSET_MAP[charset]
     else:
         properties['windows.dfCharSet'] = str(charset)
-    properties['style'] = _STYLE_MAP[win_props.dfPitchAndFamily & 0xff00]
+    properties['style'] = _STYLE_MAP.get(win_props.dfPitchAndFamily & 0xff00, None)
     if win_props.dfBreakChar:
         properties['word-boundary'] = win_props.dfFirstChar + win_props.dfBreakChar
     properties['device'] = bytes_to_str(data[win_props.dfDevice:])
     # unparsed properties: dfMaxWidth - but this can be calculated from the matrices
     if version == 0x300:
         # https://github.com/letolabs/fontforge/blob/master/fontforge/winfonts.c
         # /* These fields are not present in 2.0 and are not meaningful in 3.0 */
```

### Comparing `monobit-0.39.3/monobit/formats/windows/mz.py` & `monobit-0.40.0/monobit/formats/windows/mz.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/windows/ne.py` & `monobit-0.40.0/monobit/formats/windows/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/formats/windows/pe.py` & `monobit-0.40.0/monobit/formats/windows/pe.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/scripts/banner.py` & `monobit-0.40.0/monobit/scripts/banner.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/monobit/scripts/convert.py` & `monobit-0.40.0/monobit/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/LICENSE` & `monobit-0.40.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monobit-0.39.3/README.md` & `monobit-0.40.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 | Amiga Font Contents   | `amiga-fc` | `.font`                     | ✔     |       |
 | Amiga font            | `amiga`    |                             | ✔     |       |
 | BBC soft font         | `bbc`      |                             | ✔     | ✔     |
 | X11/Adobe BDF         | `bdf`      | `.bdf`                      | ✔     | ✔     |
 | AngelCode BMFont [P]  | `bmfont` | `.fnt` `.xml` `.json` + images | ✔    | ✔     |
 | Raw binary            | `raw`      | `.fnt` `.rom` [*]           | ✔     | ✔     |
 | Codepage Information  | `cpi`      | `.cpi`                      | ✔     | ✔     |
+| Consoleet / vfontas   | `consoleet`| `.txt`                      | ✔     |       |
 | Daisy-Dot             | `daisy`    | `.nlq` `.nl2` `.nl3` `.nl4` | ✔     |       |
 | Dashen                | `dashen`   | `.pft`                      | ✔     |       |
 | DEC DRCS soft font    | `dec`      |                             | ✔     | ✔     |
 | DosStart!             | `dosstart` | `.dsf`                      | ✔     |       |
 | FZX font              | `fzx`      | `.fzx`                      | ✔     | ✔     |
 | Figlet font           | `figlet`   | `.flf`                      | ✔     | ✔     |
 | Windows or OS/2 font  | `mzfon`    | `.fon` `.exe` `.dll`        | ✔     | ✔ (16-bit Windows) |
@@ -117,26 +118,29 @@
 | hexdraw               | `hexdraw`  | `.draw`                     | ✔     | ✔     |
 | Bitmap image [P]      | `image`    | `.png` `.gif` `.bmp`        | ✔     | ✔     |
 | Apple IIgs font       | `iigs`     | `.fon`                      | ✔     | ✔     |
 | Bare codepage         | `kbd`      | `.cp`                       | ✔     | ✔     |
 | REXXCOM Font Mania    | `mania`    | `.com`                      | ✔     |       |
 | LISA font library     | `lisa`     | `.bin`                      | ✔     |       |
 | MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     |       |
-| MouseGraphics         | `mgtk`     |                             | ✔     |       |
+| mkwinfon text format  | `mkwinfon` | `.fd`                       | ✔     |       |
+| PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | Bare NFNT resource    | `nfnt`     | `.f`                        | ✔     | ✔     |
 | Palm OS font (v1/NFNT)| `palm`     | `.pdb`                      | ✔     |       |
 | Optiks PCR Font       | `pcr`      | `.pcr`                      | ✔     |       |
 | PCPaint, GRASP, ChiWriter | `pcpaint` | `.set` `.fnt`  `.sft` `.pft` `.eft` ... | ✔ |  |
 | PDF chart [R]         | `pdf`      | `.pdf`                      |       | ✔     |
 | TeX PKFONT            | `pkfont`   | `.pk`                       | ✔     |       |
 | The Print Shop        | `printshop`| `.pnf`                      | ✔     |       |
 | PC Screen Font        | `psf`      | `.psf` `.psfu`              | ✔     | ✔ (version 2) |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
-| SFNT embedded bitmap  | `sfnt`     | `.otb` `.ttf` `.otf` [F] [**] | ✔   |       |
+| PSF2TXT               | `psf2txt`  | `.txt`                      | ✔     |       |
 | Signum! 2             | `signum`   | `.e24` `.p9` `.p24` `.l30`  | ✔     |       |
+| SFNT embedded bitmap  | `sfnt`     | `.otb` `.ttf` `.otf` [F] [**] | ✔   | ✔ (OTB) |
+| SFNT collection       | `ttcf`     | `.otc` `.ttc` [F] [**]      | ✔     | ✔ (OTB) |
 | vfont                 | `vfont`    |                             | ✔     | ✔     |
 | Bare GEOS resource    | `vlir`     |                             | ✔     |       |
 | Windows FNT resource  | `win`      | `.fnt`                      | ✔     | ✔     |
 | XBIN font section     | `xbin`     | `.xb`                       | ✔     | ✔     |
 | monobit yaff          | `yaff`     | `.yaff`                     | ✔     | ✔     |
 
 
@@ -177,23 +181,27 @@
 and only exceptionally embed bitmaps to improve rendering on low-resolution displays.
 
 _The vast majority of `.ttf`, `.otf`, `.dfont` etc. files do not contain bitmaps at all_.
 This is true even for fonts with a pixelised look.
 To convert these you first need to _rasterise_ them, which `monobit` does not do.
 Some of the other font tools linked below do have rasterising features.
 
+`monobit` can experimentally output OpenType Bitmap (`.otb`) files, a bitmap-only
+file format supported by Linux desktops.
+
 
 Font format features
 --------------------
 
 Here is a comparison of what you can and cannot store in selected formats supported by `monobit`.
 
 | Format        | Unicode | Unicode sequences | Encoding | MBCS | Multiple fonts | Cell size | Proportional | Kerning | Colour/antialiasing | Glyph representation
 |---------------|---|---|---|---|---|------|---|---|---|--------------
 | `yaff`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ |   | visual text
+| `sfnt`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
 | `bmfont`      | ✔ |   | ✔ | ✔ |   | any  | ✔ | ✔ | ✔ | image
 | `bdf`         | ✔ |   | ✔ | ✔ |   | any  | ✔ |   |   | hex
 | `nfnt`        |   |   | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
 | `win`         |   |   | ✔ | ✔ | ✔ | any  | ✔ |   |   | binary
 | `hexdraw`     | ✔ |   |   |   |   | any  | ✔ |   |   | visual text
 | `amiga`       |   |   |   |   | ✔ | any  | ✔ |   | ✔ | binary
 | `gdos`        |   |   |   |   |   | any  | ✔ |   |   | binary
```

### Comparing `monobit-0.39.3/pyproject.toml` & `monobit-0.40.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "monobit"
-version = "0.39.3"
+version = "0.40.0"
 authors = [
     { name = "Rob Hagemans", email = "rob.hagemans@hotmail.com" },
 ]
 description = "Tools for working with monochrome bitmap fonts."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `monobit-0.39.3/PKG-INFO` & `monobit-0.40.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monobit
-Version: 0.39.3
+Version: 0.40.0
 Summary: Tools for working with monochrome bitmap fonts.
 Project-URL: Homepage, https://github.com/robhagemans/monobit
 Author-email: Rob Hagemans <rob.hagemans@hotmail.com>
 License: MIT License
         
         Copyright (c) 2019--2023 Rob Hagemans
         
@@ -134,14 +134,15 @@
 | Amiga Font Contents   | `amiga-fc` | `.font`                     | ✔     |       |
 | Amiga font            | `amiga`    |                             | ✔     |       |
 | BBC soft font         | `bbc`      |                             | ✔     | ✔     |
 | X11/Adobe BDF         | `bdf`      | `.bdf`                      | ✔     | ✔     |
 | AngelCode BMFont [P]  | `bmfont` | `.fnt` `.xml` `.json` + images | ✔    | ✔     |
 | Raw binary            | `raw`      | `.fnt` `.rom` [*]           | ✔     | ✔     |
 | Codepage Information  | `cpi`      | `.cpi`                      | ✔     | ✔     |
+| Consoleet / vfontas   | `consoleet`| `.txt`                      | ✔     |       |
 | Daisy-Dot             | `daisy`    | `.nlq` `.nl2` `.nl3` `.nl4` | ✔     |       |
 | Dashen                | `dashen`   | `.pft`                      | ✔     |       |
 | DEC DRCS soft font    | `dec`      |                             | ✔     | ✔     |
 | DosStart!             | `dosstart` | `.dsf`                      | ✔     |       |
 | FZX font              | `fzx`      | `.fzx`                      | ✔     | ✔     |
 | Figlet font           | `figlet`   | `.flf`                      | ✔     | ✔     |
 | Windows or OS/2 font  | `mzfon`    | `.fon` `.exe` `.dll`        | ✔     | ✔ (16-bit Windows) |
@@ -159,26 +160,29 @@
 | hexdraw               | `hexdraw`  | `.draw`                     | ✔     | ✔     |
 | Bitmap image [P]      | `image`    | `.png` `.gif` `.bmp`        | ✔     | ✔     |
 | Apple IIgs font       | `iigs`     | `.fon`                      | ✔     | ✔     |
 | Bare codepage         | `kbd`      | `.cp`                       | ✔     | ✔     |
 | REXXCOM Font Mania    | `mania`    | `.com`                      | ✔     |       |
 | LISA font library     | `lisa`     | `.bin`                      | ✔     |       |
 | MacOS font            | `mac`      | `.dfont` `.suit`            | ✔     |       |
-| MouseGraphics         | `mgtk`     |                             | ✔     |       |
+| mkwinfon text format  | `mkwinfon` | `.fd`                       | ✔     |       |
+| PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
 | Bare NFNT resource    | `nfnt`     | `.f`                        | ✔     | ✔     |
 | Palm OS font (v1/NFNT)| `palm`     | `.pdb`                      | ✔     |       |
 | Optiks PCR Font       | `pcr`      | `.pcr`                      | ✔     |       |
 | PCPaint, GRASP, ChiWriter | `pcpaint` | `.set` `.fnt`  `.sft` `.pft` `.eft` ... | ✔ |  |
 | PDF chart [R]         | `pdf`      | `.pdf`                      |       | ✔     |
 | TeX PKFONT            | `pkfont`   | `.pk`                       | ✔     |       |
 | The Print Shop        | `printshop`| `.pnf`                      | ✔     |       |
 | PC Screen Font        | `psf`      | `.psf` `.psfu`              | ✔     | ✔ (version 2) |
 | PSF2AMS PSFCOM        | `psfcom`   | `.com`                      | ✔     |       |
-| SFNT embedded bitmap  | `sfnt`     | `.otb` `.ttf` `.otf` [F] [**] | ✔   |       |
+| PSF2TXT               | `psf2txt`  | `.txt`                      | ✔     |       |
 | Signum! 2             | `signum`   | `.e24` `.p9` `.p24` `.l30`  | ✔     |       |
+| SFNT embedded bitmap  | `sfnt`     | `.otb` `.ttf` `.otf` [F] [**] | ✔   | ✔ (OTB) |
+| SFNT collection       | `ttcf`     | `.otc` `.ttc` [F] [**]      | ✔     | ✔ (OTB) |
 | vfont                 | `vfont`    |                             | ✔     | ✔     |
 | Bare GEOS resource    | `vlir`     |                             | ✔     |       |
 | Windows FNT resource  | `win`      | `.fnt`                      | ✔     | ✔     |
 | XBIN font section     | `xbin`     | `.xb`                       | ✔     | ✔     |
 | monobit yaff          | `yaff`     | `.yaff`                     | ✔     | ✔     |
 
 
@@ -219,23 +223,27 @@
 and only exceptionally embed bitmaps to improve rendering on low-resolution displays.
 
 _The vast majority of `.ttf`, `.otf`, `.dfont` etc. files do not contain bitmaps at all_.
 This is true even for fonts with a pixelised look.
 To convert these you first need to _rasterise_ them, which `monobit` does not do.
 Some of the other font tools linked below do have rasterising features.
 
+`monobit` can experimentally output OpenType Bitmap (`.otb`) files, a bitmap-only
+file format supported by Linux desktops.
+
 
 Font format features
 --------------------
 
 Here is a comparison of what you can and cannot store in selected formats supported by `monobit`.
 
 | Format        | Unicode | Unicode sequences | Encoding | MBCS | Multiple fonts | Cell size | Proportional | Kerning | Colour/antialiasing | Glyph representation
 |---------------|---|---|---|---|---|------|---|---|---|--------------
 | `yaff`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ |   | visual text
+| `sfnt`        | ✔ | ✔ | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
 | `bmfont`      | ✔ |   | ✔ | ✔ |   | any  | ✔ | ✔ | ✔ | image
 | `bdf`         | ✔ |   | ✔ | ✔ |   | any  | ✔ |   |   | hex
 | `nfnt`        |   |   | ✔ | ✔ | ✔ | any  | ✔ | ✔ | ✔ | binary
 | `win`         |   |   | ✔ | ✔ | ✔ | any  | ✔ |   |   | binary
 | `hexdraw`     | ✔ |   |   |   |   | any  | ✔ |   |   | visual text
 | `amiga`       |   |   |   |   | ✔ | any  | ✔ |   | ✔ | binary
 | `gdos`        |   |   |   |   |   | any  | ✔ |   |   | binary
```

