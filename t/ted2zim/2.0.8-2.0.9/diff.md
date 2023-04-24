# Comparing `tmp/ted2zim-2.0.8.tar.gz` & `tmp/ted2zim-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ted2zim-2.0.8.tar", last modified: Sat Oct  3 19:26:57 2020, max compression
+gzip compressed data, was "dist/ted2zim-2.0.9.tar", last modified: Thu Jun 10 13:36:50 2021, max compression
```

## Comparing `ted2zim-2.0.8.tar` & `ted2zim-2.0.9.tar`

### file list

```diff
@@ -1,215 +1,223 @@
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:57.081232 ted2zim-2.0.8/
--rw-r--r--   0 reg        (501) staff       (20)     2049 2020-10-03 19:25:49.000000 ted2zim-2.0.8/CHANGELOG.md
--rw-r--r--   0 reg        (501) staff       (20)       89 2020-08-27 16:19:06.000000 ted2zim-2.0.8/MANIFEST.in
--rw-r--r--   0 reg        (501) staff       (20)     5268 2020-10-03 19:26:57.079913 ted2zim-2.0.8/PKG-INFO
--rw-r--r--   0 reg        (501) staff       (20)     4036 2020-08-27 16:19:06.000000 ted2zim-2.0.8/README.md
--rwxr-xr-x   0 reg        (501) staff       (20)     2325 2020-09-11 16:04:31.000000 ted2zim-2.0.8/get_js_deps.sh
--rw-r--r--   0 reg        (501) staff       (20)      167 2020-09-11 16:04:31.000000 ted2zim-2.0.8/requirements.txt
--rw-r--r--   0 reg        (501) staff       (20)       38 2020-10-03 19:26:57.081406 ted2zim-2.0.8/setup.cfg
--rw-r--r--   0 reg        (501) staff       (20)     1514 2020-08-27 16:19:06.000000 ted2zim-2.0.8/setup.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.967558 ted2zim-2.0.8/ted2zim/
--rw-r--r--   0 reg        (501) staff       (20)        6 2020-10-03 19:25:52.000000 ted2zim-2.0.8/ted2zim/VERSION
--rwxr-xr-x   0 reg        (501) staff       (20)        0 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/__init__.py
--rw-r--r--   0 reg        (501) staff       (20)      360 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/__main__.py
--rw-r--r--   0 reg        (501) staff       (20)      890 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/constants.py
--rwxr-xr-x   0 reg        (501) staff       (20)     5657 2020-09-30 10:22:38.000000 ted2zim-2.0.8/ted2zim/entrypoint.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.970653 ted2zim-2.0.8/ted2zim/locale/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.960979 ted2zim-2.0.8/ted2zim/locale/hi/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.971338 ted2zim-2.0.8/ted2zim/locale/hi/LC_MESSAGES/
--rw-r--r--   0 reg        (501) staff       (20)      750 2020-09-25 09:34:49.000000 ted2zim-2.0.8/ted2zim/locale/hi/LC_MESSAGES/messages.mo
--rw-r--r--   0 reg        (501) staff       (20)     1124 2020-09-25 09:34:49.000000 ted2zim-2.0.8/ted2zim/locale/hi/LC_MESSAGES/messages.po
--rw-r--r--   0 reg        (501) staff       (20)      894 2020-09-25 09:34:49.000000 ted2zim-2.0.8/ted2zim/locale/messages.pot
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.972861 ted2zim-2.0.8/ted2zim/multi/
--rw-r--r--   0 reg        (501) staff       (20)        0 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/multi/__init__.py
--rw-r--r--   0 reg        (501) staff       (20)      373 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/multi/__main__.py
--rw-r--r--   0 reg        (501) staff       (20)     3403 2020-09-01 08:27:06.000000 ted2zim-2.0.8/ted2zim/multi/entrypoint.py
--rw-r--r--   0 reg        (501) staff       (20)    12353 2020-09-01 09:25:50.000000 ted2zim-2.0.8/ted2zim/multi/scraper.py
--rw-r--r--   0 reg        (501) staff       (20)     1365 2020-09-11 16:04:31.000000 ted2zim-2.0.8/ted2zim/processing.py
--rw-r--r--   0 reg        (501) staff       (20)    42945 2020-10-03 19:25:46.000000 ted2zim-2.0.8/ted2zim/scraper.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.974278 ted2zim-2.0.8/ted2zim/templates/
--rw-r--r--   0 reg        (501) staff       (20)     4079 2020-09-25 09:34:49.000000 ted2zim-2.0.8/ted2zim/templates/article.html
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.980294 ted2zim-2.0.8/ted2zim/templates/assets/
--rw-r--r--   0 reg        (501) staff       (20)     4139 2020-09-25 09:34:49.000000 ted2zim-2.0.8/ted2zim/templates/assets/app.js
--rw-r--r--   0 reg        (501) staff       (20)     2062 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/article.css
--rw-r--r--   0 reg        (501) staff       (20)      617 2020-09-22 10:03:21.000000 ted2zim-2.0.8/ted2zim/templates/assets/article.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.982903 ted2zim-2.0.8/ted2zim/templates/assets/chosen/
--rw-r--r--   0 reg        (501) staff       (20)      538 2018-06-08 14:43:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen-sprite.png
--rw-r--r--   0 reg        (501) staff       (20)      738 2018-06-08 14:43:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen-sprite@2x.png
--rw-r--r--   0 reg        (501) staff       (20)    12188 2018-06-08 14:43:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.css
--rw-r--r--   0 reg        (501) staff       (20)    47491 2018-06-08 14:43:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.jquery.js
--rw-r--r--   0 reg        (501) staff       (20)    29121 2018-06-08 14:43:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.jquery.min.js
--rw-r--r--   0 reg        (501) staff       (20)    10220 2018-06-08 14:43:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.min.css
--rw-r--r--   0 reg        (501) staff       (20)      819 2018-06-08 14:43:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/chosen/composer.json
--rw-r--r--   0 reg        (501) staff       (20)     2581 2020-09-25 09:29:01.000000 ted2zim-2.0.8/ted2zim/templates/assets/db.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.991929 ted2zim-2.0.8/ted2zim/templates/assets/font/
--rwxr-xr-x   0 reg        (501) staff       (20)   142472 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Black.ttf
--rwxr-xr-x   0 reg        (501) staff       (20)   135820 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Bold.ttf
--rwxr-xr-x   0 reg        (501) staff       (20)   140276 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Light.ttf
--rwxr-xr-x   0 reg        (501) staff       (20)   145932 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-LightItalic.ttf
--rwxr-xr-x   0 reg        (501) staff       (20)   145348 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Regular.ttf
--rw-r--r--   0 reg        (501) staff       (20)     5203 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/home.css
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.994596 ted2zim-2.0.8/ted2zim/templates/assets/img/
--rw-r--r--   0 reg        (501) staff       (20)    16277 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/img/TED.png
--rw-r--r--   0 reg        (501) staff       (20)     1713 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/assets/img/TED_small.png
--rw-r--r--   0 reg        (501) staff       (20)    89476 2020-10-03 19:26:47.000000 ted2zim-2.0.8/ted2zim/templates/assets/jquery.min.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:57.037318 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/
--rw-r--r--   0 reg        (501) staff       (20)     1116 2019-03-12 21:12:44.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING
--rw-r--r--   0 reg        (501) staff       (20)     1317 2019-03-12 21:13:31.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-dav1d.txt
--rw-r--r--   0 reg        (501) staff       (20)     1466 2019-03-12 21:13:31.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-ogg.txt
--rw-r--r--   0 reg        (501) staff       (20)     1928 2019-03-12 21:13:32.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-opus.txt
--rw-r--r--   0 reg        (501) staff       (20)     1470 2019-03-12 21:13:32.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-theora.txt
--rw-r--r--   0 reg        (501) staff       (20)     1470 2019-03-12 21:13:32.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-vorbis.txt
--rw-r--r--   0 reg        (501) staff       (20)      732 2019-03-12 21:13:31.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/LICENSE-nestegg.txt
--rw-r--r--   0 reg        (501) staff       (20)     1537 2019-03-12 21:13:32.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/LICENSE-vpx.txt
--rw-r--r--   0 reg        (501) staff       (20)     1436 2019-03-12 21:13:32.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/PATENTS-vpx.txt
--rw-r--r--   0 reg        (501) staff       (20)    18635 2019-06-18 15:00:08.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/README.md
--rw-r--r--   0 reg        (501) staff       (20)     3327 2019-06-18 15:01:30.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/dynamicaudio.swf
--rw-r--r--   0 reg        (501) staff       (20)    10882 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   133919 2019-06-18 15:06:14.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   235857 2019-06-18 15:06:12.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus.js
--rw-r--r--   0 reg        (501) staff       (20)    10800 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   136930 2019-06-18 15:05:05.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   244171 2019-06-18 15:05:03.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis.js
--rw-r--r--   0 reg        (501) staff       (20)    66341 2019-06-18 15:09:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   120118 2019-06-18 15:09:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem
--rw-r--r--   0 reg        (501) staff       (20)   337274 2019-06-18 15:09:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js
--rw-r--r--   0 reg        (501) staff       (20)    12697 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   435089 2019-06-18 15:09:02.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   934028 2019-06-18 15:08:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1.js
--rw-r--r--   0 reg        (501) staff       (20)    11685 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    62814 2019-06-18 15:07:01.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   128000 2019-06-18 15:06:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora.js
--rw-r--r--   0 reg        (501) staff       (20)    67131 2019-06-18 15:09:44.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)     7758 2019-06-18 15:09:42.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem
--rw-r--r--   0 reg        (501) staff       (20)   143573 2019-06-18 15:09:44.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:42.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js
--rw-r--r--   0 reg        (501) staff       (20)    13113 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   123379 2019-06-18 15:08:12.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   260845 2019-06-18 15:08:10.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8.js
--rw-r--r--   0 reg        (501) staff       (20)    64871 2019-06-18 15:09:48.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    32370 2019-06-18 15:09:46.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem
--rw-r--r--   0 reg        (501) staff       (20)   223005 2019-06-18 15:09:48.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:46.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js
--rw-r--r--   0 reg        (501) staff       (20)    13118 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   238580 2019-06-18 15:08:36.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   465673 2019-06-18 15:08:34.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9.js
--rw-r--r--   0 reg        (501) staff       (20)    14111 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    59932 2019-06-18 15:03:33.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   171551 2019-06-18 15:03:30.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg.js
--rw-r--r--   0 reg        (501) staff       (20)    14304 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    48118 2019-06-18 15:04:13.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   122752 2019-06-18 15:04:11.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm.js
--rw-r--r--   0 reg        (501) staff       (20)   140564 2019-06-18 15:01:30.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-es2017.js
--rw-r--r--   0 reg        (501) staff       (20)     4142 2019-06-18 15:01:30.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-support.js
--rw-r--r--   0 reg        (501) staff       (20)     2235 2019-06-18 15:01:27.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-version.js
--rw-r--r--   0 reg        (501) staff       (20)     9543 2019-06-18 15:01:28.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-worker-audio.js
--rw-r--r--   0 reg        (501) staff       (20)     9591 2019-06-18 15:01:28.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-worker-video.js
--rw-r--r--   0 reg        (501) staff       (20)   148482 2019-06-18 15:01:30.000000 ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv.js
--rw-r--r--   0 reg        (501) staff       (20)     7287 2020-10-03 19:26:55.000000 ted2zim-2.0.8/ted2zim/templates/assets/polyfills.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:57.048363 ted2zim-2.0.8/ted2zim/templates/assets/videojs/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:57.050583 ted2zim-2.0.8/ted2zim/templates/assets/videojs/font/
--rwxr-xr-x   0 reg        (501) staff       (20)    28407 2020-04-16 15:49:19.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/font/VideoJS.svg
--rwxr-xr-x   0 reg        (501) staff       (20)     7080 2020-04-16 15:49:19.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/font/VideoJS.ttf
--rwxr-xr-x   0 reg        (501) staff       (20)     4324 2020-04-16 15:49:19.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/font/VideoJS.woff
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:57.079017 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/
--rw-r--r--   0 reg        (501) staff       (20)     5054 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ar.js
--rw-r--r--   0 reg        (501) staff       (20)     5027 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ar.json
--rw-r--r--   0 reg        (501) staff       (20)     1356 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ba.js
--rw-r--r--   0 reg        (501) staff       (20)     1329 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ba.json
--rw-r--r--   0 reg        (501) staff       (20)     1946 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/bg.js
--rw-r--r--   0 reg        (501) staff       (20)     1919 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/bg.json
--rw-r--r--   0 reg        (501) staff       (20)     1494 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ca.js
--rw-r--r--   0 reg        (501) staff       (20)     1467 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ca.json
--rw-r--r--   0 reg        (501) staff       (20)     3869 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cs.js
--rw-r--r--   0 reg        (501) staff       (20)     3842 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cs.json
--rw-r--r--   0 reg        (501) staff       (20)     3848 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cy.js
--rw-r--r--   0 reg        (501) staff       (20)     3739 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cy.json
--rw-r--r--   0 reg        (501) staff       (20)     1425 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/da.js
--rw-r--r--   0 reg        (501) staff       (20)     1398 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/da.json
--rw-r--r--   0 reg        (501) staff       (20)     4413 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/de.js
--rw-r--r--   0 reg        (501) staff       (20)     4387 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/de.json
--rw-r--r--   0 reg        (501) staff       (20)     3616 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/el.js
--rw-r--r--   0 reg        (501) staff       (20)     3589 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/el.json
--rw-r--r--   0 reg        (501) staff       (20)     4093 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/en.js
--rw-r--r--   0 reg        (501) staff       (20)     4066 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/en.json
--rw-r--r--   0 reg        (501) staff       (20)     4542 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/es.js
--rw-r--r--   0 reg        (501) staff       (20)     4514 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/es.json
--rw-r--r--   0 reg        (501) staff       (20)     5013 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fa.js
--rw-r--r--   0 reg        (501) staff       (20)     4986 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fa.json
--rw-r--r--   0 reg        (501) staff       (20)     1376 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fi.js
--rw-r--r--   0 reg        (501) staff       (20)     1349 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fi.json
--rw-r--r--   0 reg        (501) staff       (20)     4447 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fr.js
--rw-r--r--   0 reg        (501) staff       (20)     4420 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fr.json
--rw-r--r--   0 reg        (501) staff       (20)     4438 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gd.js
--rwxr-xr-x   0 reg        (501) staff       (20)     4411 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gd.json
--rw-r--r--   0 reg        (501) staff       (20)     4432 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gl.js
--rw-r--r--   0 reg        (501) staff       (20)     4405 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gl.json
--rw-r--r--   0 reg        (501) staff       (20)     4632 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/he.js
--rw-r--r--   0 reg        (501) staff       (20)     4523 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/he.json
--rw-r--r--   0 reg        (501) staff       (20)     1356 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hr.js
--rw-r--r--   0 reg        (501) staff       (20)     1329 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hr.json
--rw-r--r--   0 reg        (501) staff       (20)     1430 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hu.js
--rw-r--r--   0 reg        (501) staff       (20)     1403 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hu.json
--rw-r--r--   0 reg        (501) staff       (20)     1474 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/it.js
--rw-r--r--   0 reg        (501) staff       (20)     1447 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/it.json
--rw-r--r--   0 reg        (501) staff       (20)     1663 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ja.js
--rw-r--r--   0 reg        (501) staff       (20)     1636 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ja.json
--rw-r--r--   0 reg        (501) staff       (20)     1537 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ko.js
--rw-r--r--   0 reg        (501) staff       (20)     1510 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ko.json
--rw-r--r--   0 reg        (501) staff       (20)     4227 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nb.js
--rw-r--r--   0 reg        (501) staff       (20)     4200 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nb.json
--rw-r--r--   0 reg        (501) staff       (20)     4130 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nl.js
--rw-r--r--   0 reg        (501) staff       (20)     4102 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nl.json
--rw-r--r--   0 reg        (501) staff       (20)     4216 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nn.js
--rw-r--r--   0 reg        (501) staff       (20)     4189 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nn.json
--rw-r--r--   0 reg        (501) staff       (20)     4331 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/oc.js
--rw-r--r--   0 reg        (501) staff       (20)     4304 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/oc.json
--rw-r--r--   0 reg        (501) staff       (20)     2028 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pl.js
--rw-r--r--   0 reg        (501) staff       (20)     2001 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pl.json
--rw-r--r--   0 reg        (501) staff       (20)     4104 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-BR.js
--rw-r--r--   0 reg        (501) staff       (20)     4178 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-BR.json
--rw-r--r--   0 reg        (501) staff       (20)     2382 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-PT.js
--rw-r--r--   0 reg        (501) staff       (20)     2351 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-PT.json
--rw-r--r--   0 reg        (501) staff       (20)     5418 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ru.js
--rw-r--r--   0 reg        (501) staff       (20)     5391 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ru.json
--rw-r--r--   0 reg        (501) staff       (20)     4097 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sk.js
--rw-r--r--   0 reg        (501) staff       (20)     4069 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sk.json
--rw-r--r--   0 reg        (501) staff       (20)     1348 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sr.js
--rw-r--r--   0 reg        (501) staff       (20)     1321 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sr.json
--rw-r--r--   0 reg        (501) staff       (20)     4158 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sv.js
--rw-r--r--   0 reg        (501) staff       (20)     4131 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sv.json
--rw-r--r--   0 reg        (501) staff       (20)     3443 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/tr.js
--rw-r--r--   0 reg        (501) staff       (20)     3416 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/tr.json
--rw-r--r--   0 reg        (501) staff       (20)     5448 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/uk.js
--rw-r--r--   0 reg        (501) staff       (20)     5431 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/uk.json
--rw-r--r--   0 reg        (501) staff       (20)     4139 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/vi.js
--rw-r--r--   0 reg        (501) staff       (20)     4112 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/vi.json
--rw-r--r--   0 reg        (501) staff       (20)     3737 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-CN.js
--rw-r--r--   0 reg        (501) staff       (20)     3707 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-CN.json
--rw-r--r--   0 reg        (501) staff       (20)     3739 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hans.js
--rw-r--r--   0 reg        (501) staff       (20)     3707 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hans.json
--rw-r--r--   0 reg        (501) staff       (20)     3746 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hant.js
--rw-r--r--   0 reg        (501) staff       (20)     3714 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hant.json
--rw-r--r--   0 reg        (501) staff       (20)     3744 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-TW.js
--rw-r--r--   0 reg        (501) staff       (20)     3714 2020-04-16 15:48:59.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-TW.json
--rw-r--r--   0 reg        (501) staff       (20)    45293 2020-04-16 15:48:58.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/video-js.css
--rw-r--r--   0 reg        (501) staff       (20)    40028 2020-04-16 15:49:18.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/video-js.min.css
--rw-r--r--   0 reg        (501) staff       (20)  1383342 2020-04-16 15:48:30.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.cjs.js
--rw-r--r--   0 reg        (501) staff       (20)  1382824 2020-04-16 15:48:30.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.es.js
--rw-r--r--   0 reg        (501) staff       (20)  1863694 2020-04-16 15:48:27.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.js
--rw-r--r--   0 reg        (501) staff       (20)   497845 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.min.js
--rw-r--r--   0 reg        (501) staff       (20)    17645 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/videojs-ogvjs.js
--rw-r--r--   0 reg        (501) staff       (20)   988813 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim/templates/assets/webp-hero.bundle.js
--rw-r--r--   0 reg        (501) staff       (20)     1828 2020-09-22 10:03:21.000000 ted2zim-2.0.8/ted2zim/templates/assets/zim_prefix.js
--rw-r--r--   0 reg        (501) staff       (20)      701 2020-08-27 16:19:06.000000 ted2zim-2.0.8/ted2zim/templates/favicon.png
--rw-r--r--   0 reg        (501) staff       (20)     2287 2020-09-25 09:34:49.000000 ted2zim-2.0.8/ted2zim/templates/home.html
--rw-r--r--   0 reg        (501) staff       (20)     3120 2020-09-01 08:27:06.000000 ted2zim-2.0.8/ted2zim/utils.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2020-10-03 19:26:56.970383 ted2zim-2.0.8/ted2zim.egg-info/
--rw-r--r--   0 reg        (501) staff       (20)     5268 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim.egg-info/PKG-INFO
--rw-r--r--   0 reg        (501) staff       (20)     8891 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim.egg-info/SOURCES.txt
--rw-r--r--   0 reg        (501) staff       (20)        1 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim.egg-info/dependency_links.txt
--rw-r--r--   0 reg        (501) staff       (20)       95 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim.egg-info/entry_points.txt
--rw-r--r--   0 reg        (501) staff       (20)        1 2020-08-28 07:39:15.000000 ted2zim-2.0.8/ted2zim.egg-info/not-zip-safe
--rw-r--r--   0 reg        (501) staff       (20)      167 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim.egg-info/requires.txt
--rw-r--r--   0 reg        (501) staff       (20)        8 2020-10-03 19:26:56.000000 ted2zim-2.0.8/ted2zim.egg-info/top_level.txt
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.616699 ted2zim-2.0.9/
+-rw-r--r--   0 reg        (501) staff       (20)     2080 2021-06-10 13:35:31.000000 ted2zim-2.0.9/CHANGELOG.md
+-rw-r--r--   0 reg        (501) staff       (20)       89 2020-08-27 16:19:06.000000 ted2zim-2.0.9/MANIFEST.in
+-rw-r--r--   0 reg        (501) staff       (20)     5268 2021-06-10 13:36:50.616438 ted2zim-2.0.9/PKG-INFO
+-rw-r--r--   0 reg        (501) staff       (20)     4036 2020-08-27 16:19:06.000000 ted2zim-2.0.9/README.md
+-rwxr-xr-x   0 reg        (501) staff       (20)     2325 2020-09-11 16:04:31.000000 ted2zim-2.0.9/get_js_deps.sh
+-rw-r--r--   0 reg        (501) staff       (20)      167 2021-06-10 13:35:33.000000 ted2zim-2.0.9/requirements.txt
+-rw-r--r--   0 reg        (501) staff       (20)       38 2021-06-10 13:36:50.616770 ted2zim-2.0.9/setup.cfg
+-rw-r--r--   0 reg        (501) staff       (20)     1514 2020-08-27 16:19:06.000000 ted2zim-2.0.9/setup.py
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.535258 ted2zim-2.0.9/ted2zim/
+-rw-r--r--   0 reg        (501) staff       (20)        6 2021-06-10 13:35:42.000000 ted2zim-2.0.9/ted2zim/VERSION
+-rwxr-xr-x   0 reg        (501) staff       (20)        0 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/__init__.py
+-rw-r--r--   0 reg        (501) staff       (20)      360 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/__main__.py
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.539599 ted2zim-2.0.9/ted2zim/__pycache__/
+-rw-r--r--   0 reg        (501) staff       (20)      129 2021-06-07 08:50:54.000000 ted2zim-2.0.9/ted2zim/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 reg        (501) staff       (20)     1187 2021-06-07 08:50:54.000000 ted2zim-2.0.9/ted2zim/__pycache__/constants.cpython-38.pyc
+-rw-r--r--   0 reg        (501) staff       (20)     3343 2021-06-07 08:51:49.000000 ted2zim-2.0.9/ted2zim/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 reg        (501) staff       (20)      890 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/constants.py
+-rwxr-xr-x   0 reg        (501) staff       (20)     5657 2020-09-30 10:22:38.000000 ted2zim-2.0.9/ted2zim/entrypoint.py
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.540682 ted2zim-2.0.9/ted2zim/locale/
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.530251 ted2zim-2.0.9/ted2zim/locale/hi/
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.542143 ted2zim-2.0.9/ted2zim/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 reg        (501) staff       (20)      750 2020-09-25 09:34:49.000000 ted2zim-2.0.9/ted2zim/locale/hi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 reg        (501) staff       (20)     1124 2020-09-25 09:34:49.000000 ted2zim-2.0.9/ted2zim/locale/hi/LC_MESSAGES/messages.po
+-rw-r--r--   0 reg        (501) staff       (20)      894 2020-09-25 09:34:49.000000 ted2zim-2.0.9/ted2zim/locale/messages.pot
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.543778 ted2zim-2.0.9/ted2zim/multi/
+-rw-r--r--   0 reg        (501) staff       (20)        0 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/multi/__init__.py
+-rw-r--r--   0 reg        (501) staff       (20)      373 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/multi/__main__.py
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.545130 ted2zim-2.0.9/ted2zim/multi/__pycache__/
+-rw-r--r--   0 reg        (501) staff       (20)      135 2021-06-07 08:50:54.000000 ted2zim-2.0.9/ted2zim/multi/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 reg        (501) staff       (20)      441 2021-06-07 08:50:54.000000 ted2zim-2.0.9/ted2zim/multi/__pycache__/__main__.cpython-38.pyc
+-rw-r--r--   0 reg        (501) staff       (20)     2844 2021-06-07 08:50:54.000000 ted2zim-2.0.9/ted2zim/multi/__pycache__/entrypoint.cpython-38.pyc
+-rw-r--r--   0 reg        (501) staff       (20)     3403 2020-09-01 08:27:06.000000 ted2zim-2.0.9/ted2zim/multi/entrypoint.py
+-rw-r--r--   0 reg        (501) staff       (20)    12353 2020-09-01 09:25:50.000000 ted2zim-2.0.9/ted2zim/multi/scraper.py
+-rw-r--r--   0 reg        (501) staff       (20)     1365 2020-09-11 16:04:31.000000 ted2zim-2.0.9/ted2zim/processing.py
+-rw-r--r--   0 reg        (501) staff       (20)    42945 2020-10-03 19:25:46.000000 ted2zim-2.0.9/ted2zim/scraper.py
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.546733 ted2zim-2.0.9/ted2zim/templates/
+-rw-r--r--   0 reg        (501) staff       (20)     4079 2020-09-25 09:34:49.000000 ted2zim-2.0.9/ted2zim/templates/article.html
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.551753 ted2zim-2.0.9/ted2zim/templates/assets/
+-rw-r--r--   0 reg        (501) staff       (20)     4139 2020-09-25 09:34:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/app.js
+-rw-r--r--   0 reg        (501) staff       (20)     2062 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/article.css
+-rw-r--r--   0 reg        (501) staff       (20)      617 2020-09-22 10:03:21.000000 ted2zim-2.0.9/ted2zim/templates/assets/article.js
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.553734 ted2zim-2.0.9/ted2zim/templates/assets/chosen/
+-rw-r--r--   0 reg        (501) staff       (20)      538 2018-06-08 14:43:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen-sprite.png
+-rw-r--r--   0 reg        (501) staff       (20)      738 2018-06-08 14:43:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen-sprite@2x.png
+-rw-r--r--   0 reg        (501) staff       (20)    12188 2018-06-08 14:43:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.css
+-rw-r--r--   0 reg        (501) staff       (20)    47491 2018-06-08 14:43:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.jquery.js
+-rw-r--r--   0 reg        (501) staff       (20)    29121 2018-06-08 14:43:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.jquery.min.js
+-rw-r--r--   0 reg        (501) staff       (20)    10220 2018-06-08 14:43:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.min.css
+-rw-r--r--   0 reg        (501) staff       (20)      819 2018-06-08 14:43:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/chosen/composer.json
+-rw-r--r--   0 reg        (501) staff       (20)     2581 2020-09-25 09:29:01.000000 ted2zim-2.0.9/ted2zim/templates/assets/db.js
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.560032 ted2zim-2.0.9/ted2zim/templates/assets/font/
+-rwxr-xr-x   0 reg        (501) staff       (20)   142472 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Black.ttf
+-rwxr-xr-x   0 reg        (501) staff       (20)   135820 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Bold.ttf
+-rwxr-xr-x   0 reg        (501) staff       (20)   140276 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Light.ttf
+-rwxr-xr-x   0 reg        (501) staff       (20)   145932 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-LightItalic.ttf
+-rwxr-xr-x   0 reg        (501) staff       (20)   145348 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Regular.ttf
+-rw-r--r--   0 reg        (501) staff       (20)     5203 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/home.css
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.561983 ted2zim-2.0.9/ted2zim/templates/assets/img/
+-rw-r--r--   0 reg        (501) staff       (20)    16277 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/img/TED.png
+-rw-r--r--   0 reg        (501) staff       (20)     1713 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/assets/img/TED_small.png
+-rw-r--r--   0 reg        (501) staff       (20)    89476 2021-06-10 13:36:45.000000 ted2zim-2.0.9/ted2zim/templates/assets/jquery.min.js
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.582107 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/
+-rw-r--r--   0 reg        (501) staff       (20)     1116 2019-03-12 21:12:44.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING
+-rw-r--r--   0 reg        (501) staff       (20)     1317 2019-03-12 21:13:31.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-dav1d.txt
+-rw-r--r--   0 reg        (501) staff       (20)     1466 2019-03-12 21:13:31.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-ogg.txt
+-rw-r--r--   0 reg        (501) staff       (20)     1928 2019-03-12 21:13:32.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-opus.txt
+-rw-r--r--   0 reg        (501) staff       (20)     1470 2019-03-12 21:13:32.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-theora.txt
+-rw-r--r--   0 reg        (501) staff       (20)     1470 2019-03-12 21:13:32.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-vorbis.txt
+-rw-r--r--   0 reg        (501) staff       (20)      732 2019-03-12 21:13:31.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/LICENSE-nestegg.txt
+-rw-r--r--   0 reg        (501) staff       (20)     1537 2019-03-12 21:13:32.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/LICENSE-vpx.txt
+-rw-r--r--   0 reg        (501) staff       (20)     1436 2019-03-12 21:13:32.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/PATENTS-vpx.txt
+-rw-r--r--   0 reg        (501) staff       (20)    18635 2019-06-18 15:00:08.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/README.md
+-rw-r--r--   0 reg        (501) staff       (20)     3327 2019-06-18 15:01:30.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/dynamicaudio.swf
+-rw-r--r--   0 reg        (501) staff       (20)    10882 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)   133919 2019-06-18 15:06:14.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   235857 2019-06-18 15:06:12.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus.js
+-rw-r--r--   0 reg        (501) staff       (20)    10800 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)   136930 2019-06-18 15:05:05.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   244171 2019-06-18 15:05:03.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis.js
+-rw-r--r--   0 reg        (501) staff       (20)    66341 2019-06-18 15:09:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)   120118 2019-06-18 15:09:56.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem
+-rw-r--r--   0 reg        (501) staff       (20)   337274 2019-06-18 15:09:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:56.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js
+-rw-r--r--   0 reg        (501) staff       (20)    12697 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)   435089 2019-06-18 15:09:02.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   934028 2019-06-18 15:08:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1.js
+-rw-r--r--   0 reg        (501) staff       (20)    11685 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)    62814 2019-06-18 15:07:01.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   128000 2019-06-18 15:06:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora.js
+-rw-r--r--   0 reg        (501) staff       (20)    67131 2019-06-18 15:09:44.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)     7758 2019-06-18 15:09:42.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem
+-rw-r--r--   0 reg        (501) staff       (20)   143573 2019-06-18 15:09:44.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:42.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js
+-rw-r--r--   0 reg        (501) staff       (20)    13113 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)   123379 2019-06-18 15:08:12.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   260845 2019-06-18 15:08:10.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8.js
+-rw-r--r--   0 reg        (501) staff       (20)    64871 2019-06-18 15:09:48.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)    32370 2019-06-18 15:09:46.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem
+-rw-r--r--   0 reg        (501) staff       (20)   223005 2019-06-18 15:09:48.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:46.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js
+-rw-r--r--   0 reg        (501) staff       (20)    13118 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)   238580 2019-06-18 15:08:36.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   465673 2019-06-18 15:08:34.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9.js
+-rw-r--r--   0 reg        (501) staff       (20)    14111 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)    59932 2019-06-18 15:03:33.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   171551 2019-06-18 15:03:30.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg.js
+-rw-r--r--   0 reg        (501) staff       (20)    14304 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.js
+-rw-r--r--   0 reg        (501) staff       (20)    48118 2019-06-18 15:04:13.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.wasm
+-rw-r--r--   0 reg        (501) staff       (20)   122752 2019-06-18 15:04:11.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm.js
+-rw-r--r--   0 reg        (501) staff       (20)   140564 2019-06-18 15:01:30.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-es2017.js
+-rw-r--r--   0 reg        (501) staff       (20)     4142 2019-06-18 15:01:30.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-support.js
+-rw-r--r--   0 reg        (501) staff       (20)     2235 2019-06-18 15:01:27.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-version.js
+-rw-r--r--   0 reg        (501) staff       (20)     9543 2019-06-18 15:01:28.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-worker-audio.js
+-rw-r--r--   0 reg        (501) staff       (20)     9591 2019-06-18 15:01:28.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-worker-video.js
+-rw-r--r--   0 reg        (501) staff       (20)   148482 2019-06-18 15:01:30.000000 ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv.js
+-rw-r--r--   0 reg        (501) staff       (20)     7287 2021-06-10 13:36:48.000000 ted2zim-2.0.9/ted2zim/templates/assets/polyfills.js
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.590583 ted2zim-2.0.9/ted2zim/templates/assets/videojs/
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.592600 ted2zim-2.0.9/ted2zim/templates/assets/videojs/font/
+-rwxr-xr-x   0 reg        (501) staff       (20)    28407 2020-04-16 15:49:19.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/font/VideoJS.svg
+-rwxr-xr-x   0 reg        (501) staff       (20)     7080 2020-04-16 15:49:19.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/font/VideoJS.ttf
+-rwxr-xr-x   0 reg        (501) staff       (20)     4324 2020-04-16 15:49:19.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/font/VideoJS.woff
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.615978 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/
+-rw-r--r--   0 reg        (501) staff       (20)     5054 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ar.js
+-rw-r--r--   0 reg        (501) staff       (20)     5027 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ar.json
+-rw-r--r--   0 reg        (501) staff       (20)     1356 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ba.js
+-rw-r--r--   0 reg        (501) staff       (20)     1329 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ba.json
+-rw-r--r--   0 reg        (501) staff       (20)     1946 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/bg.js
+-rw-r--r--   0 reg        (501) staff       (20)     1919 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/bg.json
+-rw-r--r--   0 reg        (501) staff       (20)     1494 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ca.js
+-rw-r--r--   0 reg        (501) staff       (20)     1467 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ca.json
+-rw-r--r--   0 reg        (501) staff       (20)     3869 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cs.js
+-rw-r--r--   0 reg        (501) staff       (20)     3842 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cs.json
+-rw-r--r--   0 reg        (501) staff       (20)     3848 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cy.js
+-rw-r--r--   0 reg        (501) staff       (20)     3739 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cy.json
+-rw-r--r--   0 reg        (501) staff       (20)     1425 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/da.js
+-rw-r--r--   0 reg        (501) staff       (20)     1398 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/da.json
+-rw-r--r--   0 reg        (501) staff       (20)     4413 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/de.js
+-rw-r--r--   0 reg        (501) staff       (20)     4387 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/de.json
+-rw-r--r--   0 reg        (501) staff       (20)     3616 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/el.js
+-rw-r--r--   0 reg        (501) staff       (20)     3589 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/el.json
+-rw-r--r--   0 reg        (501) staff       (20)     4093 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/en.js
+-rw-r--r--   0 reg        (501) staff       (20)     4066 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/en.json
+-rw-r--r--   0 reg        (501) staff       (20)     4542 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/es.js
+-rw-r--r--   0 reg        (501) staff       (20)     4514 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/es.json
+-rw-r--r--   0 reg        (501) staff       (20)     5013 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fa.js
+-rw-r--r--   0 reg        (501) staff       (20)     4986 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fa.json
+-rw-r--r--   0 reg        (501) staff       (20)     1376 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fi.js
+-rw-r--r--   0 reg        (501) staff       (20)     1349 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fi.json
+-rw-r--r--   0 reg        (501) staff       (20)     4447 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fr.js
+-rw-r--r--   0 reg        (501) staff       (20)     4420 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fr.json
+-rw-r--r--   0 reg        (501) staff       (20)     4438 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gd.js
+-rwxr-xr-x   0 reg        (501) staff       (20)     4411 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gd.json
+-rw-r--r--   0 reg        (501) staff       (20)     4432 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gl.js
+-rw-r--r--   0 reg        (501) staff       (20)     4405 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gl.json
+-rw-r--r--   0 reg        (501) staff       (20)     4632 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/he.js
+-rw-r--r--   0 reg        (501) staff       (20)     4523 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/he.json
+-rw-r--r--   0 reg        (501) staff       (20)     1356 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hr.js
+-rw-r--r--   0 reg        (501) staff       (20)     1329 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hr.json
+-rw-r--r--   0 reg        (501) staff       (20)     1430 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hu.js
+-rw-r--r--   0 reg        (501) staff       (20)     1403 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hu.json
+-rw-r--r--   0 reg        (501) staff       (20)     1474 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/it.js
+-rw-r--r--   0 reg        (501) staff       (20)     1447 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/it.json
+-rw-r--r--   0 reg        (501) staff       (20)     1663 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ja.js
+-rw-r--r--   0 reg        (501) staff       (20)     1636 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ja.json
+-rw-r--r--   0 reg        (501) staff       (20)     1537 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ko.js
+-rw-r--r--   0 reg        (501) staff       (20)     1510 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ko.json
+-rw-r--r--   0 reg        (501) staff       (20)     4227 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nb.js
+-rw-r--r--   0 reg        (501) staff       (20)     4200 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nb.json
+-rw-r--r--   0 reg        (501) staff       (20)     4130 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nl.js
+-rw-r--r--   0 reg        (501) staff       (20)     4102 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nl.json
+-rw-r--r--   0 reg        (501) staff       (20)     4216 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nn.js
+-rw-r--r--   0 reg        (501) staff       (20)     4189 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nn.json
+-rw-r--r--   0 reg        (501) staff       (20)     4331 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/oc.js
+-rw-r--r--   0 reg        (501) staff       (20)     4304 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/oc.json
+-rw-r--r--   0 reg        (501) staff       (20)     2028 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pl.js
+-rw-r--r--   0 reg        (501) staff       (20)     2001 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pl.json
+-rw-r--r--   0 reg        (501) staff       (20)     4104 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-BR.js
+-rw-r--r--   0 reg        (501) staff       (20)     4178 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-BR.json
+-rw-r--r--   0 reg        (501) staff       (20)     2382 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-PT.js
+-rw-r--r--   0 reg        (501) staff       (20)     2351 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-PT.json
+-rw-r--r--   0 reg        (501) staff       (20)     5418 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ru.js
+-rw-r--r--   0 reg        (501) staff       (20)     5391 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ru.json
+-rw-r--r--   0 reg        (501) staff       (20)     4097 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sk.js
+-rw-r--r--   0 reg        (501) staff       (20)     4069 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sk.json
+-rw-r--r--   0 reg        (501) staff       (20)     1348 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sr.js
+-rw-r--r--   0 reg        (501) staff       (20)     1321 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sr.json
+-rw-r--r--   0 reg        (501) staff       (20)     4158 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sv.js
+-rw-r--r--   0 reg        (501) staff       (20)     4131 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sv.json
+-rw-r--r--   0 reg        (501) staff       (20)     3443 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/tr.js
+-rw-r--r--   0 reg        (501) staff       (20)     3416 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/tr.json
+-rw-r--r--   0 reg        (501) staff       (20)     5448 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/uk.js
+-rw-r--r--   0 reg        (501) staff       (20)     5431 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/uk.json
+-rw-r--r--   0 reg        (501) staff       (20)     4139 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/vi.js
+-rw-r--r--   0 reg        (501) staff       (20)     4112 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/vi.json
+-rw-r--r--   0 reg        (501) staff       (20)     3737 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-CN.js
+-rw-r--r--   0 reg        (501) staff       (20)     3707 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-CN.json
+-rw-r--r--   0 reg        (501) staff       (20)     3739 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hans.js
+-rw-r--r--   0 reg        (501) staff       (20)     3707 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hans.json
+-rw-r--r--   0 reg        (501) staff       (20)     3746 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hant.js
+-rw-r--r--   0 reg        (501) staff       (20)     3714 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hant.json
+-rw-r--r--   0 reg        (501) staff       (20)     3744 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-TW.js
+-rw-r--r--   0 reg        (501) staff       (20)     3714 2020-04-16 15:48:59.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-TW.json
+-rw-r--r--   0 reg        (501) staff       (20)    45293 2020-04-16 15:48:58.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/video-js.css
+-rw-r--r--   0 reg        (501) staff       (20)    40028 2020-04-16 15:49:18.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/video-js.min.css
+-rw-r--r--   0 reg        (501) staff       (20)  1383342 2020-04-16 15:48:30.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.cjs.js
+-rw-r--r--   0 reg        (501) staff       (20)  1382824 2020-04-16 15:48:30.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.es.js
+-rw-r--r--   0 reg        (501) staff       (20)  1863694 2020-04-16 15:48:27.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.js
+-rw-r--r--   0 reg        (501) staff       (20)   497845 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.min.js
+-rw-r--r--   0 reg        (501) staff       (20)    17645 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/videojs-ogvjs.js
+-rw-r--r--   0 reg        (501) staff       (20)   988813 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim/templates/assets/webp-hero.bundle.js
+-rw-r--r--   0 reg        (501) staff       (20)     1828 2020-09-22 10:03:21.000000 ted2zim-2.0.9/ted2zim/templates/assets/zim_prefix.js
+-rw-r--r--   0 reg        (501) staff       (20)      701 2020-08-27 16:19:06.000000 ted2zim-2.0.9/ted2zim/templates/favicon.png
+-rw-r--r--   0 reg        (501) staff       (20)     2287 2020-09-25 09:34:49.000000 ted2zim-2.0.9/ted2zim/templates/home.html
+-rw-r--r--   0 reg        (501) staff       (20)     3120 2020-09-01 08:27:06.000000 ted2zim-2.0.9/ted2zim/utils.py
+drwxr-xr-x   0 reg        (501) staff       (20)        0 2021-06-10 13:36:50.537814 ted2zim-2.0.9/ted2zim.egg-info/
+-rw-r--r--   0 reg        (501) staff       (20)     5268 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim.egg-info/PKG-INFO
+-rw-r--r--   0 reg        (501) staff       (20)     9173 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim.egg-info/SOURCES.txt
+-rw-r--r--   0 reg        (501) staff       (20)        1 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim.egg-info/dependency_links.txt
+-rw-r--r--   0 reg        (501) staff       (20)       95 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim.egg-info/entry_points.txt
+-rw-r--r--   0 reg        (501) staff       (20)        1 2020-08-28 07:39:15.000000 ted2zim-2.0.9/ted2zim.egg-info/not-zip-safe
+-rw-r--r--   0 reg        (501) staff       (20)      167 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim.egg-info/requires.txt
+-rw-r--r--   0 reg        (501) staff       (20)        8 2021-06-10 13:36:49.000000 ted2zim-2.0.9/ted2zim.egg-info/top_level.txt
```

### Comparing `ted2zim-2.0.8/CHANGELOG.md` & `ted2zim-2.0.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.0.9
+
+- updated scraperlib
+
 # 2.0.8
 
 - fixed bug in video URL finding if ted json as an h264 entry with None value
 
 # 2.0.7
 
 - use `eng` as default locale
```

### Comparing `ted2zim-2.0.8/PKG-INFO` & `ted2zim-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ted2zim
-Version: 2.0.8
+Version: 2.0.9
 Summary: Make ZIM file from TED Talks
 Home-page: https://github.com/openzim/ted
 Author: dattaz
 Author-email: taz@dattaz.fr
 License: GPLv3+
 Description: # ted2zim
```

### Comparing `ted2zim-2.0.8/README.md` & `ted2zim-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/get_js_deps.sh` & `ted2zim-2.0.9/get_js_deps.sh`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/setup.py` & `ted2zim-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/constants.py` & `ted2zim-2.0.9/ted2zim/constants.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/entrypoint.py` & `ted2zim-2.0.9/ted2zim/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/locale/hi/LC_MESSAGES/messages.mo` & `ted2zim-2.0.9/ted2zim/locale/hi/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/locale/hi/LC_MESSAGES/messages.po` & `ted2zim-2.0.9/ted2zim/locale/hi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/locale/messages.pot` & `ted2zim-2.0.9/ted2zim/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/multi/entrypoint.py` & `ted2zim-2.0.9/ted2zim/multi/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/multi/scraper.py` & `ted2zim-2.0.9/ted2zim/multi/scraper.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/processing.py` & `ted2zim-2.0.9/ted2zim/processing.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/scraper.py` & `ted2zim-2.0.9/ted2zim/scraper.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/article.html` & `ted2zim-2.0.9/ted2zim/templates/article.html`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/app.js` & `ted2zim-2.0.9/ted2zim/templates/assets/app.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/article.css` & `ted2zim-2.0.9/ted2zim/templates/assets/article.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/article.js` & `ted2zim-2.0.9/ted2zim/templates/assets/article.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen-sprite.png` & `ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen-sprite@2x.png` & `ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.css` & `ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.jquery.js` & `ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.jquery.min.js` & `ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/chosen/chosen.min.css` & `ted2zim-2.0.9/ted2zim/templates/assets/chosen/chosen.min.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/chosen/composer.json` & `ted2zim-2.0.9/ted2zim/templates/assets/chosen/composer.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/db.js` & `ted2zim-2.0.9/ted2zim/templates/assets/db.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Black.ttf` & `ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Bold.ttf` & `ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Light.ttf` & `ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-LightItalic.ttf` & `ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/font/Roboto-Regular.ttf` & `ted2zim-2.0.9/ted2zim/templates/assets/font/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/home.css` & `ted2zim-2.0.9/ted2zim/templates/assets/home.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/img/TED.png` & `ted2zim-2.0.9/ted2zim/templates/assets/img/TED.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/img/TED_small.png` & `ted2zim-2.0.9/ted2zim/templates/assets/img/TED_small.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/jquery.min.js` & `ted2zim-2.0.9/ted2zim/templates/assets/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-dav1d.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-dav1d.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-ogg.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-ogg.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-opus.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-opus.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-theora.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-theora.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/COPYING-vorbis.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/COPYING-vorbis.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/LICENSE-nestegg.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/LICENSE-nestegg.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/LICENSE-vpx.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/LICENSE-vpx.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/PATENTS-vpx.txt` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/PATENTS-vpx.txt`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/README.md` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/README.md`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/dynamicaudio.swf` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/dynamicaudio.swf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-opus.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-audio-vorbis.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-av1.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-theora.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp8.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-decoder-video-vp9.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-ogg.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.wasm` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm-wasm.wasm`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-demuxer-webm.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-es2017.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-es2017.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-support.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-support.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-version.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-version.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-worker-audio.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-worker-audio.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv-worker-video.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv-worker-video.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/ogvjs/ogv.js` & `ted2zim-2.0.9/ted2zim/templates/assets/ogvjs/ogv.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/polyfills.js` & `ted2zim-2.0.9/ted2zim/templates/assets/polyfills.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/font/VideoJS.svg` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/font/VideoJS.svg`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/font/VideoJS.ttf` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/font/VideoJS.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/font/VideoJS.woff` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/font/VideoJS.woff`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ar.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ar.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ar.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ba.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ba.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ba.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ba.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/bg.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/bg.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/bg.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ca.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ca.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ca.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cs.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cs.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cs.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cy.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/cy.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/cy.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/da.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/da.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/da.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/da.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/de.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/de.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/de.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/de.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/el.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/el.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/el.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/el.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/en.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/en.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/en.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/en.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/es.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/es.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/es.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/es.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fa.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fa.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fa.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fi.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fi.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fi.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fr.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/fr.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/fr.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gd.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gd.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gd.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gd.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gl.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/gl.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/gl.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/he.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/he.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/he.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/he.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hr.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hr.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hr.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hu.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/hu.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/hu.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/it.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/it.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/it.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/it.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ja.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ja.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ja.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ko.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ko.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ko.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nb.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nb.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nb.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nl.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nl.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nl.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nn.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nn.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/nn.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/nn.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/oc.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/oc.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/oc.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pl.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pl.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pl.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-BR.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-BR.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-BR.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-BR.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-PT.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-PT.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/pt-PT.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/pt-PT.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ru.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/ru.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/ru.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sk.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sk.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sk.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sr.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sr.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sr.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sv.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/sv.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/sv.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/tr.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/tr.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/tr.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/uk.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/uk.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/uk.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/vi.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/vi.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/vi.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-CN.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-CN.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-CN.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-CN.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hans.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hans.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hans.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hans.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hant.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hant.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-Hant.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-Hant.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-TW.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-TW.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/lang/zh-TW.json` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/lang/zh-TW.json`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/video-js.css` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/video-js.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/video-js.min.css` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/video-js.min.css`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.cjs.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.cjs.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.es.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.es.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs/video.min.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs/video.min.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/videojs-ogvjs.js` & `ted2zim-2.0.9/ted2zim/templates/assets/videojs-ogvjs.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/webp-hero.bundle.js` & `ted2zim-2.0.9/ted2zim/templates/assets/webp-hero.bundle.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/assets/zim_prefix.js` & `ted2zim-2.0.9/ted2zim/templates/assets/zim_prefix.js`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/favicon.png` & `ted2zim-2.0.9/ted2zim/templates/favicon.png`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/templates/home.html` & `ted2zim-2.0.9/ted2zim/templates/home.html`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim/utils.py` & `ted2zim-2.0.9/ted2zim/utils.py`

 * *Files identical despite different names*

### Comparing `ted2zim-2.0.8/ted2zim.egg-info/PKG-INFO` & `ted2zim-2.0.9/ted2zim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ted2zim
-Version: 2.0.8
+Version: 2.0.9
 Summary: Make ZIM file from TED Talks
 Home-page: https://github.com/openzim/ted
 Author: dattaz
 Author-email: taz@dattaz.fr
 License: GPLv3+
 Description: # ted2zim
```

### Comparing `ted2zim-2.0.8/ted2zim.egg-info/SOURCES.txt` & `ted2zim-2.0.9/ted2zim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,27 @@
 ted2zim.egg-info/PKG-INFO
 ted2zim.egg-info/SOURCES.txt
 ted2zim.egg-info/dependency_links.txt
 ted2zim.egg-info/entry_points.txt
 ted2zim.egg-info/not-zip-safe
 ted2zim.egg-info/requires.txt
 ted2zim.egg-info/top_level.txt
+ted2zim/__pycache__/__init__.cpython-38.pyc
+ted2zim/__pycache__/constants.cpython-38.pyc
+ted2zim/__pycache__/utils.cpython-38.pyc
 ted2zim/locale/messages.pot
 ted2zim/locale/hi/LC_MESSAGES/messages.mo
 ted2zim/locale/hi/LC_MESSAGES/messages.po
 ted2zim/multi/__init__.py
 ted2zim/multi/__main__.py
 ted2zim/multi/entrypoint.py
 ted2zim/multi/scraper.py
+ted2zim/multi/__pycache__/__init__.cpython-38.pyc
+ted2zim/multi/__pycache__/__main__.cpython-38.pyc
+ted2zim/multi/__pycache__/entrypoint.cpython-38.pyc
 ted2zim/templates/article.html
 ted2zim/templates/favicon.png
 ted2zim/templates/home.html
 ted2zim/templates/assets/app.js
 ted2zim/templates/assets/article.css
 ted2zim/templates/assets/article.js
 ted2zim/templates/assets/db.js
```

