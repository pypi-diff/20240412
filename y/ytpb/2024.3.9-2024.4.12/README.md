# Comparing `tmp/ytpb-2024.3.9.tar.gz` & `tmp/ytpb-2024.4.12.tar.gz`

## Comparing `ytpb-2024.3.9.tar` & `ytpb-2024.4.12.tar`

### file list

```diff
@@ -1,121 +1,141 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.3.9/.gitattributes
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.3.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.3.9/.readthedocs.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ytpb-2024.3.9/CHANGELOG.rst
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.3.9/CONTRIBUTING.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ytpb-2024.3.9/Makefile
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/changelog.rst
--rw-r--r--   0        0        0    19028 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/cli.rst
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/contributing.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/index.rst
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/quick.rst
--rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/reference.rst
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.3.9/docs/why.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/notebooks/shared/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/__main__.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cache.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/conditional.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/config.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/download.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/exceptions.py
--rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/fetchers.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/ffmpeg.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/info.py
--rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/locate.py
--rw-r--r--   0        0        0    10240 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/merge.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/mpd.py
--rw-r--r--   0        0        0    14255 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/playback.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/segment.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/streams.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/types.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/actions/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/actions/capture.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/actions/compose.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/actions/download.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/__init__.py
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/common.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/options.py
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/commands/__init__.py
--rw-r--r--   0        0        0    17612 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/commands/capture.py
--rw-r--r--   0        0        0    12911 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/commands/download.py
--rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/cli/commands/mpd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/utils/__init__.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/utils/date.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/utils/other.py
--rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/utils/path.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/utils/remote.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 ytpb-2024.3.9/src/ytpb/utils/url.py
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/conftest.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/helpers.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_cache.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_download.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_fetchers.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_info.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_locate.py
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_merge.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_mpd.py
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_playback.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_playback_session.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_segment.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_streams.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/actions/__init__.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/actions/test_compose.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/actions/test_download.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/conftest.py
--rw-r--r--   0        0        0    31979 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/test_download_command.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/test_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/capture/__init__.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/capture/test_frame_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/mpd/__init__.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/mpd/test_compose_command.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/cli/mpd/test_refresh_command.py
--rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/info-1695928670.json
--rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/manifest-1695928670.mpd
--rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/webpage-1695928670.html
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_compose_mpd_with_no_streams.out
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_dry_run_option.out
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_no_cut_option.out
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_no_merge_option.out
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/expected/test_refresh_mpd.out
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/gap-cases/gap-case-1-fixture.csv
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/gap-cases/gap-case-2-fixture.csv
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/gap-cases/gap-case-3-fixture.csv
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959120.i140.mp4
--rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959120.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959121.i140.mp4
--rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959121.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959122.i140.mp4
--rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959122.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959123.i140.mp4
--rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959123.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959203.i140.mp4
--rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/data/segments/7959203.i244.webm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/utils/__init__.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/utils/test_date.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/utils/test_path.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/utils/test_remote.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 ytpb-2024.3.9/tests/utils/test_url.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.3.9/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.3.9/LICENSE
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ytpb-2024.3.9/README.rst
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 ytpb-2024.3.9/pyproject.toml
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 ytpb-2024.3.9/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.gitattributes
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.readthedocs.yaml
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 ytpb-2024.4.12/CHANGELOG.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.4.12/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.4.12/Makefile
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 ytpb-2024.4.12/config.toml.example
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/changelog.rst
+-rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/cli.rst
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/contributing.rst
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/cookbook.rst
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/index.rst
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/quick.rst
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/reference.rst
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/why.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/index.rst
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/usage.rst
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/index.rst
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.actions.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.cache.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.download.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.errors.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.fetchers.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.info.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.locate.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.merge.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.playback.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.representations.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.segment.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.streams.rst
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 ytpb-2024.4.12/etc/Containerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/notebooks/shared/.gitkeep
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/__main__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/api.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cache.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/conditional.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/config.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/download.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/errors.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/fetchers.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/ffmpeg.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/info.py
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/locate.py
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/merge.py
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/playback.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/representations.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/segment.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/streams.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/types.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/__init__.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/capture.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/compose.py
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/download.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/__init__.py
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/common.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/options.py
+-rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/__init__.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/capture.py
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/download.py
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/mpd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/__init__.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/date.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/other.py
+-rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/remote.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/url.py
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/conftest.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/helpers.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_cache.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_download.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_fetchers.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_info.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_locate.py
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_merge.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_playback.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_playback_session.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_representations.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_segment.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_streams.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/actions/__init__.py
+-rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/actions/test_compose.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/actions/test_download.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/conftest.py
+-rw-r--r--   0        0        0    39866 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/test_download_command.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/test_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/capture/__init__.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/capture/test_frame_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/mpd/__init__.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/mpd/test_compose_command.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/mpd/test_refresh_command.py
+-rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/info-1695928670.json
+-rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/manifest-1695928670.mpd
+-rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/webpage-1695928670.html
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd_with_no_streams.out
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_dry_run_option.out
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_no_cut_option.out
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_no_merge_option.out
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_refresh_mpd.out
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/gap-cases/gap-case-1-fixture.csv
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/gap-cases/gap-case-2-fixture.csv
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/gap-cases/gap-case-3-fixture.csv
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959120.i140.mp4
+-rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959120.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959121.i140.mp4
+-rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959121.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959122.i140.mp4
+-rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959122.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959123.i140.mp4
+-rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959123.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959203.i140.mp4
+-rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959203.i244.webm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/__init__.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_date.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_path.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_remote.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_url.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.4.12/LICENSE
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 ytpb-2024.4.12/README.rst
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 ytpb-2024.4.12/pyproject.toml
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 ytpb-2024.4.12/PKG-INFO
```

### Comparing `ytpb-2024.3.9/CONTRIBUTING.rst` & `ytpb-2024.4.12/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/docs/cli.rst` & `ytpb-2024.4.12/docs/cli.rst`

 * *Files 5% similar despite different names*

```diff
@@ -174,14 +174,24 @@
   $ ytpb download -i 2023-12-31T01:20:00+00/2024-01-02T10:20:00+00 ...
 
 Note that the time part delimiter ("T") is necessary when only time components
 to change are supplied: ::
 
   $ ytpb download -i 2024-01-02T10:20:00+00/T25M30S ...
 
+*Unix timestamp*
+^^^^^^^^^^^^^^^^
+
+* ``--interval <timestamp>/<timestamp>``
+
+where ``<timestamp> = "@"<epoch-seconds>``:
+
+The date and time interval can also be specified with Unix timestamps as: ::
+
+   $ ytpb download -i @1704190800/@1704190830 ...
 
 *'Now' keyword*
 ^^^^^^^^^^^^^^^
 
 * ``-i/--interval <start>/now``
 
 To refer to the current moment, the end part accepts the ``now`` keyword: ::
@@ -263,29 +273,30 @@
   $ ytpb download -i 0/now ...
 
 Compatibility table
 -------------------
 
 .. table:: **Table:** Interval parts compatibility
 
-   +----------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   |                      | Date and time | Time | Duration | Replacing components | Sequence number | 'Now', '..' |
-   +======================+===============+======+==========+======================+=================+=============+
-   | Date and time        |       Y       |  Y   |    Y     |          Y           |        Y        |      Y      |
-   +----------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Time                 |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y      |
-   +----------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Duration             |       Y       |  Y   |   *N*    |         *N*          |        Y        |     *N*     |
-   +----------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Replacing components |       Y       | *N*  |   *N*    |         *N*          |       *N*       |     *N*     |
-   +----------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | Sequence number      |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y      |
-   +----------------------+---------------+------+----------+----------------------+-----------------+-------------+
-   | 'Now', '..'          |       Y       |  Y   |   *N*    |         *N*          |        Y        |     *N*     |
-   +----------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   |                           | Date and time | Time | Duration | Replacing components | Sequence number | 'Now', '..' |
+   |                           | / Timestamp   |      |          |                      |                 |             |
+   +===========================+===============+======+==========+======================+=================+=============+
+   | Date and time / Timestamp |       Y       |  Y   |    Y     |          Y           |        Y        |      Y      |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   | Time                      |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y      |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   | Duration                  |       Y       |  Y   |   *N*    |         *N*          |        Y        |     *N*     |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   | Replacing components      |       Y       | *N*  |   *N*    |         *N*          |       *N*       |     *N*     |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   | Sequence number           |       Y       |  Y   |    Y     |         *N*          |        Y        |      Y      |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
+   | 'Now', '..'               |       Y       |  Y   |   *N*    |         *N*          |        Y        |     *N*     |
+   +---------------------------+---------------+------+----------+----------------------+-----------------+-------------+
 
 Specifying formats
 ==================
 
 Now let's look at the ``-af/--audio-format(s)`` and ``-vf/--video-format(s)``
 options. It accepts *format spec* string, a query expression used to select the
 desired formats (MPEG-DASH `representations
@@ -351,20 +362,26 @@
 and (c) via ``-af/--audio-format(s)`` and ``-vf/--video-format(s)`` options.
 
 The default option values are as follows:
 
 .. code:: TOML
 
 	  [options.download]
-	  audio_format = "itag eq 140"
-	  video_format = "best(@mp4 and @1080p30)"
+	  audio_format = "@140"
+	  video_format = "best(@mp4 and <=1080p and @30fps)"
+
+          [options.capture.frame]
+	  video_format = "best(@mp4 and @30fps)"
+
+          [options.capture.timelapse]
+	  video_format = "best(@mp4 and @30fps)"
 
 	  [options.mpd.compose]
-	  audio_formats = "itag eq 140"
-	  video_formats = "best(@webm and @1080p)"
+	  audio_formats = "@140"
+	  video_formats = "@webm and [@720p or @1080p] and @30fps"
 
 See `Configuring`_ for more information on configuring.
 
 Specifying output name
 ======================
 
 There are two options to change the default output naming: (a) specify a full output
@@ -490,21 +507,22 @@
 
 The configuration provides the way to set up default values of the command
 options and change other settings via configuration files. It's optional, and
 the default, built-in settings are used.
 
 By default, the ``config.toml`` file is looked up under the ``~/.config/ytpb``
 directory (or in ``$XDG_CONFIG_HOME`` if set). Also, the ``--config`` option can
-be used to override the default file. The priority of applying the settings is
-following: default settings < the ``config.toml`` file under the default
-directory < a file provided via the ``--config`` option < commands options.
+be used to override the default file location. The priority of applying the
+settings is following: default settings < the ``config.toml`` file under the
+default directory < a file provided via the ``--config`` option < commands
+options.
 
-See the ``config.toml.example`` configuration file for the available fields and
-descriptions.
+See `config.toml.example`_ for the available fields and their descriptions.
 
+.. _config.toml.example: https://github.com/xymaxim/ytpb/blob/main/config.toml.example
 
 Advanced usage
 **************
 
 Merging without cutting
 =======================
```

### Comparing `ytpb-2024.3.9/docs/quick.rst` & `ytpb-2024.4.12/docs/quick.rst`

 * *Files 9% similar despite different names*

```diff
@@ -25,40 +25,43 @@
 :ref:`cli:Specifying rewind interval`). For example, it would be handy to locate
 the desired moments first by previewing them and only after download a full
 excerpt. To run downloading in the :ref:`preview mode <Preview mode>`, use the
 ``-p/--preview`` option: ::
 
   $ ytpb download -i 2024-01-02T10:20:00+00/.. -p <STREAM>
 
+Check also out how to `download
+<https://ytpb.readthedocs.io/en/latest/cookbook.html#download-segments-with-curl>`__
+media segments with an external downloader.
+
 Compose and play
 ****************
 
-  Note: Requires a custom FFmpeg build (or <= 5.1.4). See issue `#4
-  <https://github.com/xymaxim/ytpb/issues/4>`__.
-
 If you want to play an excerpt without downloading it, you can compose a static
-MPEG-DASH manifest (MPD) file and then play it in a player that supports DASH
-streams: ::
+MPEG-DASH manifest (MPD) file: ::
 
-  $ ytpb mpd compose -i 2024-01-02T10:20:00+00/PT30S <STREAM>
-  $ mpv Stream-Title_20240102T102000+00.mpd
+  $ ytpb mpd compose -i 2024-01-02T10:20:00+00/PT30S <STREAM> && ls
+  $ Stream-Title_20240102T102000+00.mpd
 
 By default, a manifest will contain a 128k AAC audio track and 720p (or better)
 30 fps VP9 video channels.
 
-Fetch and demux
-===============
+Next, you can play a composed manifest in a player that supports MPEG-DASH (for
+example, with `mpv <https://mpv.io/>`__):
 
-Once you have a composed MPD, you can not only play it, but also convert
-selected streams to a video file. First, list all available streams and then
-select the desired streams to convert with the ``-map`` option (use ``-c copy``
-to avoid transcoding actual audio and video): ::
+  *Note:* Requires a custom mpv build. See `#4
+  <https://github.com/xymaxim/ytpb/issues/4>`__ for details.
+
+::
+
+  $ mpv Stream-Title_20240102T102000+00.mpd
 
-  $ ffprobe <MPD>
-  $ ffmpeg -i <MPD> -map 0:0 -map 0:1 -c copy out.mp4
+Check also out how to `convert
+<https://ytpb.readthedocs.io/en/latest/cookbook.html#fetch-and-demux-segments-with-ffmpeg>`__
+a manifest to a media file with FFmpeg.
 
 Play
 ****
 
 Playing and rewinding live streams are possible without downloading or
 composing. Take a look at `mpv-ytpb <https://github.com/xymaxim/mpv-ytpb>`__. It
 provides interactive experience with no need to leave the mpv player.
```

### Comparing `ytpb-2024.3.9/docs/reference.rst` & `ytpb-2024.4.12/docs/reference.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Reference
 #########
 
-This section explains some general aspects and terms.
+This document explains some general aspects and terms.
+
+*For the API reference, see* :doc:`this <package/api/index>` *document.*
 
 .. contents:: Contents
    :depth: 2
    :backlinks: top
    :local:
 
+.. _format-spec:
+
 Format spec
 ***********
 
 The desired MPEG-DASH representations, referred to media segments of specific
 format, could be selected by conditional expressions (or *format spec*). One
 format spec could refer to one or more representations.
 
@@ -60,23 +64,27 @@
 for use in conditions are listed below.
 
 Common
 ------
 
 .. table::
 
-   +---------------+--------+----------------+------------+
-   | Attribute     | Type   | Description    | Example    |
-   +===============+========+================+============+
-   | ``itag``      | Number | Value of itag  | 244        |
-   +---------------+--------+----------------+------------+
-   | ``mime_type`` | String | MIME type      | video/webm |
-   +---------------+--------+----------------+------------+
-   | ``codecs``    | String | Codec name     | vp9        |
-   +---------------+--------+----------------+------------+
+   +---------------+--------+--------------------+------------+
+   | Attribute     | Type   | Description        | Example    |
+   +===============+========+====================+============+
+   | ``itag``      | Number | Value of itag      | 244        |
+   +---------------+--------+--------------------+------------+
+   | ``mime_type`` | String | MIME type          | video/webm |
+   +---------------+--------+--------------------+------------+
+   | ``type``      | String | Discrete MIME type | video      |
+   +---------------+--------+--------------------+------------+
+   | ``format``    | String | MIME subtype       | webm       |
+   +---------------+--------+--------------------+------------+
+   | ``codecs``    | String | Codec name         | vp9        |
+   +---------------+--------+--------------------+------------+
 
 Audio only
 ----------
 
 .. table::
 
    +-------------------------+------------+-----------------------+---------+
@@ -102,19 +110,29 @@
    | ``quality``    | String | Quality string (resolution and FPS) | 720p, 1080p60 |
    +----------------+--------+-------------------------------------+---------------+
 
 Aliases
 =======
 
 The expressions can be simplified with aliases (``@alias``). There are built-in
-aliases as well as custom, user-defined ones.
+aliases as well as custom, user-defined ones. The built-in aliases, in turn, can
+be divided into static (explicitly defined) and dynamic (defined by a regex
+pattern) ones.
+
 
 Built-in aliases
 ----------------
 
+*itags*
+^^^^^^^
+
+- ``(\d+)`` — ``itag eq \1``
+
+For example, ``@140`` expands to ``itag eq 140``.
+
 *Formats*
 ^^^^^^^^^
 
 - ``mp4`` — ``format eq mp4``
 - ``webm`` — ``format eq webm``
 
 *Qualities*
@@ -151,23 +169,23 @@
 
 ``30fps``, ``60fps`` — ``frame_rate eq 30``, ``frame_rate eq 60``
 
 Custom aliases
 --------------
 
 The custom aliases could extend and update the built-in ones. The corresponding
-field in ``config.toml`` is ``format_spec.aliases``.
+field in ``config.toml`` is ``general.aliases``.
 
 Here is an example of how to define (and reuse) aliases:
 
 .. code:: TOML
 
-	  [format_spec.aliases]
-	  preferred-video = "best(@<=1080p and @30fps)"
-          video-for-mpd = "[@720p or @1080p] and @webm"
+	  [general.aliases]
+	  preferred-videos = "@<=1080p and @30fps"
+          video-for-mpd = "best(@preferred-videos and @webm)"
 
 Locating moment in a stream
 ***************************
 
 A moment in a stream is associated with a date it occurred (captured). We rely
 on the ingestion dates of media segments for dates. (A MPEG-DASH stream consists
 of a chain of sequential media segments with a fixed duration.) Thus, to locate a
```

### Comparing `ytpb-2024.3.9/docs/why.rst` & `ytpb-2024.4.12/docs/why.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/src/ytpb/cache.py` & `ytpb-2024.4.12/src/ytpb/cache.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-"""A naive disk-based caching solution via JSON. Invalidation is based on the
-filenaming."""
+"""Naive disk-based caching via JSON files.
+
+The cache invalidation is based on the filenaming: ``<expires-at>~<key>``.
+
+In the playback context, ``key`` is a video ID and ``expires-at`` is a
+timestamp referred to the expiration time of segment base URL.
+"""
 
 import json
 import time
 from pathlib import Path
 from typing import Iterable
 
 import structlog
@@ -12,20 +17,29 @@
 
 
 def _find_cached_item_paths(key: str, cache_directory: Path) -> Iterable[Path]:
     return cache_directory.glob(f"*~{key}")
 
 
 def _check_item_is_expired(item_name: str) -> bool:
-    """Check if an item has expired or not based on the item filename."""
+    """Checks if an item has expired based on the item filename."""
     expires_at = int(item_name.split("~")[0])
     return time.time() >= expires_at
 
 
 def read_from_cache(key: str, cache_directory: Path) -> dict | None:
+    """Reads a cached item.
+
+    Args:
+        key: A cached item key.
+        cache_directory: A cached items location.
+
+    Returns:
+        A dictionary of a cached item.
+    """
     try:
         found_item_paths = _find_cached_item_paths(key, cache_directory)
         *earlier_item_paths, latest_item_path = sorted(found_item_paths)
     except ValueError:
         item = None
     else:
         for path in earlier_item_paths:
@@ -42,25 +56,34 @@
 
     return item
 
 
 def write_to_cache(
     key: str, expires_at: str, item: dict, cache_directory: Path
 ) -> None:
-    """Write an item to the cache file. The previous cached items with the key
-    will be removed before."""
+    """Writes a cache item to a file.
+
+    The existing cached items with ``key`` (both expired and unexpired) will be
+    removed before writing.
+
+    Args:
+        key: A cache item key.
+        expires_at: When a cache item will be expired.
+        cache_directory: A cached items location.
+    """
     cache_directory.mkdir(parents=True, exist_ok=True)
     if old_item_paths := _find_cached_item_paths(key, cache_directory):
         for path in old_item_paths:
             path.unlink()
     new_item_path = cache_directory / f"{expires_at}~{key}"
     with open(new_item_path, "w") as f:
         json.dump(item, f)
     logger.debug("New cache item has been created: %s", new_item_path)
 
 
 def remove_expired_cache_items(cache_directory: Path) -> None:
+    """Removes expired cache items."""
     for path in sorted(cache_directory.glob("*~*")):
         if _check_item_is_expired(path.name):
             path.unlink()
         else:
             break
```

### Comparing `ytpb-2024.3.9/src/ytpb/conditional.py` & `ytpb-2024.4.12/src/ytpb/conditional.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import re
 from typing import Any, Callable
 
 import pycond as pc
 
 import structlog
 
-from ytpb.config import BUILT_IN_ALIASES
-from ytpb.exceptions import QueryError
+from ytpb.config import ALIAS_EXPAND_FUNCTIONS, ALL_ALIASES
+from ytpb.errors import QueryError
 from ytpb.types import AudioOrVideoStream
 
 logger = structlog.get_logger(__name__)
 
 ALIAS_RE = re.compile(r"@([\w<>=-]+)(?!\s)?")
 FORMAT_SPEC_RE = re.compile(
     r"^(?:(?P<function>[\w\-]+)\((?P<expr>[^\(\)]+)\)|(?P<just_expr>[^\(\)]+))$"
 )
 
 
 def _expand_aliases(expression: str, aliases: dict[str, str]) -> str:
-    all_aliases = BUILT_IN_ALIASES | aliases
+    for f in ALIAS_EXPAND_FUNCTIONS:
+        expression = f(expression)
+
+    all_aliases = ALL_ALIASES | aliases
     for matched in ALIAS_RE.finditer(expression):
         alias_with_symbol = matched.group()
         alias = matched.group(1)
         try:
             aliased_value = all_aliases[alias]
             expression = expression.replace(alias_with_symbol, aliased_value)
         except KeyError:
```

### Comparing `ytpb-2024.3.9/src/ytpb/config.py` & `ytpb-2024.4.12/src/ytpb/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 import operator
 import os
+import re
 import tomllib
 from collections import ChainMap
 from functools import reduce
 from itertools import product
 from pathlib import Path
-from typing import Any
+from typing import Any, Callable
 
 import structlog
 from platformdirs import user_config_path
 
 
 class AddressableMixin:
     def traverse(self, address: str, default: Any = None, delimiter: str = ".") -> Any:
@@ -28,14 +29,24 @@
 
 class AddressableChainMap(ChainMap, AddressableMixin):
     """ChainMap that allows to use an address to access a nested value."""
 
 
 USER_AGENT = "Mozilla/5.0 (Android 14; Mobile; rv:68.0) Gecko/68.0 Firefox/120.0"
 
+
+# Dynamic aliases (such aliases that are expanded by functions).
+def expand_itag_aliases(format_spec: str) -> str:
+    """@<itag> = itag eq <itag>"""
+    return re.sub(r"@(\d+)\b", r"itag eq \1", format_spec)
+
+
+ALIAS_EXPAND_FUNCTIONS: tuple[Callable[[str], str]] = (expand_itag_aliases,)
+
+# Static aliases (such aliases that are explicitly defined).
 FORMAT_ALIASES = {"mp4": "format eq mp4", "webm": "format eq webm"}
 
 VIDEO_QUALITY_HEIGHTS = (144, 240, 360, 480, 720, 1080, 1440, 2160)
 
 VIDEO_QUALITY_30FPS_ALIASES = {
     f"{height}p": f"height eq {height} and frame_rate eq 30"
     for height in VIDEO_QUALITY_HEIGHTS
@@ -75,14 +86,16 @@
     **VIDEO_QUALITY_30FPS_ALIASES,
     **VIDEO_QUALITY_60FPS_ALIASES,
     **VIDEO_QUALITY_WITH_OPERATOR_ALIASES,
     **NAME_QUALITY_ALIASES,
     **FRAME_PER_SECOND_ALIASES,
 }
 
+ALL_ALIASES = {**BUILT_IN_ALIASES}
+
 DEFAULT_OUTPUT_PATH = "<title>_<input_start_date>"
 
 DEFAULT_CONFIG = AddressableDict(
     {
         "version": 1,
         "options": {
             "download": {
```

### Comparing `ytpb-2024.3.9/src/ytpb/exceptions.py` & `ytpb-2024.4.12/src/ytpb/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,53 +9,59 @@
 
 
 class YtpbError(Exception):
     """Base Ytpb exception."""
 
 
 class BroadcastStatusError(YtpbError):
+    """Raised because of :class:`ytpb.info.BroadcastStatus`."""
+
     def __init__(self, message: str, status: BroadcastStatus):
         self.status = status
         super().__init__(message)
 
 
 class InfoExtractError(YtpbError):
-    pass
+    """Failed to extract a YouTube video information."""
 
 
 class BaseUrlExpiredError(YtpbError):
     pass
 
 
 class CachedItemNotFoundError(YtpbError):
+    """Failed to find an unexpired cached item."""
+
     def __str__(self) -> str:
         return "Unexpired cached item doesn't exist for the video"
 
 
 class MaxRetryError(YtpbError):
     """Raised when retry limit has been exceeded."""
 
     def __init__(self, message, response):
         self.response = response
         super().__init__(message)
 
 
 class FFmpegRunError(YtpbError):
-    pass
+    """Raised during FFmpeg subprocess call."""
 
 
 class QueryError(YtpbError):
-    pass
+    """Failed to query streams with format spec."""
 
 
 class BadCommandArgument(YtpbError):
     pass
 
 
 class SequenceLocatingError(YtpbError):
-    pass
+    """Failed to locate a segment."""
 
 
 class SegmentDownloadError(YtpbError, requests.exceptions.HTTPError):
+    """Failed to download a segment."""
+
     def __init__(self, message: str, sequence: int):
         self.sequence = sequence
         super().__init__(message)
```

### Comparing `ytpb-2024.3.9/src/ytpb/fetchers.py` & `ytpb-2024.4.12/src/ytpb/fetchers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,127 @@
+"""Fetchers are used to gather essential information about videos.
+
+Such information includes the basic video information and streams.
+"""
+
 from abc import ABC, abstractmethod
 
 import requests
 import structlog
 from yt_dlp import DownloadError, YoutubeDL
 
-from ytpb.exceptions import BroadcastStatusError
+from ytpb.errors import BroadcastStatusError
 from ytpb.info import BroadcastStatus, extract_video_info, YouTubeVideoInfo
-from ytpb.mpd import extract_representations_info
+from ytpb.representations import extract_representations
 from ytpb.streams import Streams
-from ytpb.types import AudioOrVideoStream, AudioStream, VideoStream
+from ytpb.types import AudioOrVideoStream, AudioStream, SetOfStreams, VideoStream
 from ytpb.utils.url import extract_parameter_from_url
 
 logger = structlog.get_logger(__name__)
 
 
 class InfoFetcher(ABC):
-    def __init__(self, video_url: str, session: requests.Session | None = None):
+    """A base abstract class for fetchers.
+
+    Notes:
+        Keep in mind that fetchers serve to fetch information, not to
+        store.
+
+        A good practice would be to treat each fetch operation as atomic and
+        invoke it sequentially. This provides flexibility and will avoid
+        repeated calls triggered from outside.
+    """
+
+    def __init__(self, video_url: str, session: requests.Session | None = None) -> None:
+        """Constructs an object of this class.
+
+        Args:
+            video_url: A video URL.
+            base_url: A segment base URL.
+            session: A :class:`requests.Session` object.
+        """
         self.video_url = video_url
         self.session = session or requests.Session()
 
     @abstractmethod
     def fetch_video_info(self):
+        """Fetches basic information about a video."""
         raise NotImplementedError
 
     @abstractmethod
-    def fetch_streams(self, force_fetch: bool = True):
+    def fetch_streams(self):
+        """Fetches streams available for a video."""
         raise NotImplementedError
 
 
 class YtpbInfoFetcher(InfoFetcher):
-    def fetch_video_info(self):
-        logger.debug("Fetching index webpage and extracting video info")
+    """A native fetcher."""
+
+    def fetch_video_info(self) -> YouTubeVideoInfo:
+        logger.debug("Fetching index webpage and extracting info")
 
         response = self.session.get(self.video_url)
         response.raise_for_status()
 
         info = extract_video_info(self.video_url, response.text)
         if info.status != BroadcastStatus.ACTIVE:
             raise BroadcastStatusError("Stream is not live", info.status)
-        self.info = info
+        self._info = info
+
+        return info
 
-        return self.info
+    def fetch_streams(self) -> SetOfStreams:
+        assert self._info, "Video info is not set"
 
-    def fetch_streams(self, force_fetch: bool = True):
-        logger.debug("Fetching manifest file and extracting streams info")
+        logger.debug("Fetching manifest file and extracting streams")
 
-        dash_manifest_url = self.info.dash_manifest_url
+        dash_manifest_url = self._info.dash_manifest_url
         response = self.session.get(dash_manifest_url)
         response.raise_for_status()
 
-        streams_list = extract_representations_info(response.text)
+        streams_list = extract_representations(response.text)
         streams = Streams(streams_list)
 
         return streams
 
 
 class YoutubeDLInfoFetcher(InfoFetcher):
-    options = {
+    """A fetcher that uses :mod:`yt_dlp` to gather information.
+
+    All information is extracted from the :class:`~yt_dlp.YoutubeDL`'s
+    information dictionary.
+    """
+
+    #: The default options passed to :class:`yt_dlp.YoutubeDL`.
+    default_options = {
         "live_from_start": True,
         "quiet": True,
     }
 
-    def __init__(self, video_url: str, session: requests.Session | None = None):
+    def __init__(
+        self,
+        video_url: str,
+        session: requests.Session | None = None,
+        options: dict | None = None,
+    ) -> None:
+        """Constructs an object of this class.
+
+        Args:
+            video_url: A video URL.
+            base_url: A segment base URL.
+            session: A :class:`requests.Session` object.
+            options: Options passed to :class:`yt_dlp.YoutubeDL`.
+        """
         super().__init__(video_url, session)
-        self._ydl = YoutubeDL(self.options)
+        if options is not None:
+            options = self.default_options.update(options)
+        self._ydl = YoutubeDL(options)
         self._formats: list[dict] = []
 
-    def fetch_video_info(self):
+    def fetch_video_info(self) -> YouTubeVideoInfo:
         try:
             extracted = self._ydl.extract_info(self.video_url, download=False)
         except DownloadError as exc:
             raise AssertionError from exc
 
         try:
             self._formats = extracted["formats"]
@@ -125,20 +176,18 @@
                     "height": item["height"],
                     "frame_rate": item["fps"],
                 }
             )
             stream = VideoStream(**attributes)
         return stream
 
-    def fetch_streams(self, force_fetch: bool = True):
-        streams = Streams()
-
-        if not self._formats or force_fetch:
-            self.fetch_video_info()
+    def fetch_streams(self) -> SetOfStreams:
+        assert self._formats, "Formats are not set"
 
+        streams = Streams()
         for format_item in self._formats:
             try:
                 stream = self._parse_format_item(format_item)
                 streams.add(stream)
             except KeyError:
                 raise AssertionError
```

### Comparing `ytpb-2024.3.9/src/ytpb/ffmpeg.py` & `ytpb-2024.4.12/src/ytpb/ffmpeg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shlex
 import subprocess
 from pathlib import Path
 from typing import Any
 
 import structlog
 
-from ytpb.exceptions import FFmpegRunError
+from ytpb.errors import FFmpegRunError
 
 logger = structlog.get_logger(__name__)
 
 
 def run_ffmpeg(
     args: str | list[str], **subprocess_kwargs: Any
 ) -> subprocess.CompletedProcess:
```

### Comparing `ytpb-2024.3.9/src/ytpb/info.py` & `ytpb-2024.4.12/src/ytpb/info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,48 @@
+"""Basic information about videos."""
+
 import re
 from dataclasses import dataclass
 from enum import auto, StrEnum
 from typing import Any
 
 from lxml import etree
 
-from ytpb.exceptions import InfoExtractError
+from ytpb.errors import InfoExtractError
 
 
 class BroadcastStatus(StrEnum):
+    """Represents a live broadcast status."""
+
+    #: A broadcast is live.
     ACTIVE = auto()
+    #: A broadcast has been scheduled but started.
     UPCOMING = auto()
+    #: A broadcast has been completed.
     COMPLETED = auto()
+    #: A video is not a live broadcast.
     NONE = auto()
 
 
 @dataclass
 class YouTubeVideoInfo:
-    """Information about YouTube video."""
+    """Represents information about a video."""
 
     url: str
     title: str
     author: str
     status: BroadcastStatus
     dash_manifest_url: str | None = None
 
 
 class LeftNotFetched:
-    """Represents a value that is intentionally not fetched."""
+    pass
 
 
+#: A sentinel object for a value that is intentionally not fetched.
 LEFT_NOT_FETCHED = LeftNotFetched()
 
 
 def _find_one_or_raise(element: etree.Element, path: str, message: str = "") -> Any:
     """Find first subelement or value which matches the given XPath expression
     or raise an InfoExtractError error."""
     try:
@@ -47,14 +56,26 @@
     matched = re.search(r"(?<=dashManifestUrl\":\").*?(?=\")", index_page)
     if not matched:
         raise InfoExtractError("Could not find DASH manifest URL")
     return matched[0]
 
 
 def extract_video_info(url: str, index_page_text: str) -> YouTubeVideoInfo:
+    """Extracts an information about a video from an index page.
+
+    Args:
+        url: A video URL.
+        index_page_text: An index page string content.
+
+    Returns:
+        A :class:`YouTubeVideoInfo` filled with extracted attributes.
+
+    Raises:
+        InfoExtractError: If failed to extract an attribute.
+    """
     index_page_element = etree.HTML(index_page_text)
 
     # Extracting title and author:
     video_object_element = _find_one_or_raise(
         index_page_element,
         './/*[@itemtype="http://schema.org/VideoObject"]',
         "Could not find a http://schema.org/VideoObject element",
```

### Comparing `ytpb-2024.3.9/src/ytpb/locate.py` & `ytpb-2024.4.12/src/ytpb/locate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-"""Provides locating a segment with a desired time."""
+"""Locate segments by given times."""
 
 import math
 import tempfile
 from bisect import bisect_left
 from functools import partial
 from pathlib import Path
+from typing import NamedTuple, Self
 
 import requests
 import structlog
 
 from ytpb.download import compose_default_segment_filename, download_segment
-from ytpb.exceptions import SegmentDownloadError, SequenceLocatingError
+from ytpb.errors import SegmentDownloadError, SequenceLocatingError
 from ytpb.segment import Segment, SegmentMetadata
 from ytpb.types import SegmentSequence, Timestamp
 from ytpb.utils.remote import request_reference_sequence
 from ytpb.utils.url import extract_parameter_from_url
 
+__all__ = ("SegmentLocator", "LocateResult")
+
+
 logger = structlog.get_logger(__name__)
 
-# Number of bytes sufficient to cover the YouTube metadata in segment
-# files. Note that the minimum value varies for different media formats, so the
-# value was determined empirically for all available formats.
+#: Number of bytes sufficient to cover the YouTube metadata in segment
+#: files. Note that the minimum value varies for different media formats, so the
+#: value was determined empirically for all available MPEG-DASH formats.
 PARTIAL_SEGMENT_SIZE_BYTES = 2000
 
 # Absolute time difference tolerance (in seconds). See issue #5.
 TIME_DIFF_TOLERANCE = 3e-2
 
 
 class SequenceMetadataPair:
+    """Represents a pair of segment sequence number and :class:`SegmentMetadata`."""
+
     def __init__(self, sequence: SegmentSequence, locator: "SegmentLocator"):
         self.locator = locator
         self.sequence = sequence
 
     @property
     def sequence(self) -> SegmentSequence:
         return self._sequence
@@ -63,47 +69,73 @@
             force_download=False,
         )
         with open(downloaded_path, "rb") as f:
             metadata = Segment.parse_youtube_metadata(f.read())
         return metadata
 
 
+class LocateResult(NamedTuple):
+    """Represents a locate result."""
+
+    #: A segment sequence number.
+    sequence: SegmentSequence
+    #: A time difference between a target time and
+    #: :attr:`ytpb.segment.Segment.ingestion_start_date`.
+    time_difference: float
+    #: Wheter a target time falls in gap.
+    falls_in_gap: bool
+    #: Stores all locate steps as pairs of segment sequence nubmer and time
+    #: difference.
+    track: list[tuple[SegmentSequence, float]]
+
+
 class SegmentLocator:
-    """A locator which finds a segment with a desired time.
+    """A class that locates a segment with a desired time.
 
     A timeline may contain numerous gaps, which leads to under- or
     overestimation, and it needs to be taken into account.
 
     The locating consists of three steps: (1) a "look around", jump-based search
     to find a segment directly or outline a search domain (the jump length is
-    based on the time difference and constant duration of segments); (2) refine
-    an estimated sequence number using a binary search if a segment is not
-    found; (3) check whether a target time falls into gap or not.
+    based on the time difference and constant duration of segments); (2) search
+    for a segment in the outlined domain using a binary search if a segment is
+    not found in the previous step; (3) check whether a target time falls in gap
+    or not.
     """
 
     def __init__(
         self,
         base_url: str,
         reference_sequence: SegmentSequence | None = None,
         temp_directory: Path | None = None,
         session: requests.Session | None = None,
-    ) -> None:
+    ) -> Self:
+        """Constructs a segment locator.
+
+        Args:
+            base_url: A segment base URL.
+            reference_sequence: A segment sequence number used as a reference.
+            temp_directory: A temporary directory used to store downloaded
+              segments during locating.
+            session: A :class:`request.Session` object.
+        """
         self._temp_directory = temp_directory
         self.base_url = base_url
         self.session = session or requests.Session()
 
         if reference_sequence is None:
             reference_sequence = request_reference_sequence(base_url)
         self.reference = SequenceMetadataPair(reference_sequence, self)
         self.candidate: SequenceMetadataPair | None = None
 
         self.segment_duration = float(extract_parameter_from_url("dur", base_url))
         self.track: list[tuple[SegmentSequence, float]] = []
 
     def get_temp_directory(self):
+        """Gets (and creates if needed) a temporary directory."""
         if self._temp_directory is None:
             self._temp_directory = tempfile.mkdtemp()
         return self._temp_directory
 
     def _download_full_segment(self, sequence: SegmentSequence) -> Path:
         downloaded_path = download_segment(
             sequence,
@@ -134,59 +166,69 @@
 
     def _search_sequence(
         self,
         desired_time: Timestamp,
         start: SegmentSequence,
         end: SegmentSequence,
         is_end: bool,
-    ) -> tuple[SegmentSequence, bool]:
+    ) -> LocateResult:
         """Search for a segment with a desired time inside a search domain with
         the given start and end sequence numbers and perform a gap check."""
         search_domain = range(min((start, end)), max((start, end)) + 1)
         logger.debug("Start a binary search", domain=search_domain)
         bisect_key = partial(self._get_bisected_segment_timestamp, target=desired_time)
         found_index = bisect_left(search_domain, desired_time, key=bisect_key)
         self.candidate.sequence = search_domain[found_index - 1]
 
         # After the previous step the time difference is always positive.
-        candidate_diff_in_s = self._find_time_diff(self.candidate, desired_time)
-        if candidate_diff_in_s == 0:
-            return self.candidate.sequence, False
+        current_diff_in_s = self._find_time_diff(self.candidate, desired_time)
+        if current_diff_in_s == 0:
+            return LocateResult(self.candidate.sequence, 0, False, self.track)
 
         downloaded_path = self._download_full_segment(self.candidate.sequence)
         candidate_segment = Segment.from_file(downloaded_path)
         candidate_duration = candidate_segment.get_actual_duration()
 
         logger.debug(
             "Candidate time difference: %+f s, actual duration: %f s",
-            candidate_diff_in_s,
+            current_diff_in_s,
             candidate_duration,
         )
 
-        falls_into_gap = False
-        if candidate_duration < candidate_diff_in_s - TIME_DIFF_TOLERANCE:
-            falls_into_gap = True
-            logger.debug("Input target time falls into a gap")
+        falls_in_gap = False
+        if candidate_duration < current_diff_in_s - TIME_DIFF_TOLERANCE:
+            falls_in_gap = True
+            logger.debug("Input target time falls in a gap")
             if not is_end:
                 self.candidate.sequence += 1
                 current_diff_in_s = self._find_time_diff(self.candidate, desired_time)
                 self.track.append((self.candidate.sequence, current_diff_in_s))
                 logger.debug(
                     "Step to adjacent segment, time difference: %+f s",
                     current_diff_in_s,
                     seq=self.candidate.sequence,
                     time=self.candidate.metadata.ingestion_walltime,
                 )
 
-        return self.candidate.sequence, falls_into_gap
+        return LocateResult(
+            self.candidate.sequence, current_diff_in_s, falls_in_gap, self.track
+        )
 
     def find_sequence_by_time(
         self, desired_time: Timestamp, end: bool = False
-    ) -> tuple[SegmentSequence, bool]:
-        """Find sequence number of a segment by the given timestamp."""
+    ) -> LocateResult:
+        """Finds sequence number of a segment by the given timestamp.
+
+        Args:
+            desired_time: A target Unix timestamp.
+            end: Whether a segment belongs to the end of an interval.
+
+        Returns:
+            A :class:`LocateResult` object.
+        """
         logger.info(
             "Locating segment",
             end=end,
             target=desired_time,
             reference=self.reference.sequence,
         )
 
@@ -219,17 +261,18 @@
 
             jump_length_in_seq = int(current_diff_in_s // self.segment_duration)
             self.candidate = SequenceMetadataPair(
                 self.candidate.sequence + jump_length_in_seq, self
             )
             current_diff_in_s = self._find_time_diff(self.candidate, desired_time)
 
-        result: tuple[SegmentSequence, bool]
         if has_segment_found:
-            result = (self.candidate.sequence, False)
+            result = LocateResult(
+                self.candidate.sequence, current_diff_in_s, False, self.track
+            )
         else:
             try:
                 search_between = (self.track[-2][0], self.track[-1][0])
                 result = self._search_sequence(desired_time, *search_between, end)
             except SegmentDownloadError as exc:
                 raise SequenceLocatingError(exc) from exc
```

### Comparing `ytpb-2024.3.9/src/ytpb/merge.py` & `ytpb-2024.4.12/src/ytpb/merge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+"""Merge and cut media segments.
+
+Note:
+    The current implementation of segment merging is not optimal in terms of
+    disk space, as it requires triple the amount of the total size of
+    segments. Should be changed to use different techniques, without the need
+    for intermediate files.
+"""
+
+import functools
 import os
 import shlex
 from pathlib import Path
-from tempfile import NamedTemporaryFile
 from typing import Any
 
 from ytpb import ffmpeg
-from ytpb.utils.other import S_TO_MS
+
+__all__ = ("merge_segments", "mux_and_cut_boundary_segment")
+
 
 DEFAULT_VIDEO_ENCODING_SETTINGS = {
     "h264": "libx264 -crf 18",
     "vp9": "libvpx-vp9 -crf 31 -b:v 0",
     "av1": "libaom-av1 -crf 31",
 }
 
@@ -18,30 +29,32 @@
     if not iterable:
         return None
     return iterable[n]
 
 
 def mux_and_cut_boundary_segment(
     audio_segment_path: Path, video_segment_path: Path, output_path: Path, **cut_kwargs
-):
+) -> None:
+    """Muxes and cuts a boundary segment.
+
+    Args:
+        audio_segment_path: A path to an audio segment.
+        video_segment_path: A path to a video segment.
+        output_path: An output path of the muxed segment.
+        cut_kwargs: Cut keyword arguments: ``cut_at_start`` and ``cut_at_end``.
+    """
+
     def prepare_ffmpeg_input_options(
-        segment_path: Path, cut_at_start: int = 0, cut_at_end: int = 0
+        segment_path: Path, cut_at_start: float = 0, cut_at_end: float = 0
     ):
         assert cut_at_start or cut_at_end
         if cut_at_start > 0:
-            return ["-ss", f"{cut_at_start}ms", "-i", segment_path]
+            return ["-ss", f"{cut_at_start}s", "-i", segment_path]
         elif cut_at_end > 0:
-            with NamedTemporaryFile(suffix=segment_path.suffix) as f:
-                temp_path = Path(f.name)
-                ffmpeg.ffmpeg_stream_copy(segment_path, temp_path)
-                segment_duration_s = float(
-                    ffmpeg.ffprobe_show_entries(temp_path, "format=duration")
-                )
-            end_seek_pos: int = round(segment_duration_s * S_TO_MS) - cut_at_end
-            return ["-i", segment_path, "-to", f"{end_seek_pos}ms"]
+            return ["-i", segment_path, "-to", f"{cut_at_end}s"]
         else:
             return ["-i", segment_path]
 
     if not {"cut_at_start", "cut_at_end"} > cut_kwargs.keys():
         raise ValueError(
             "only cut_at_start or cut_at_end keyword argument is accepted in cut_kwargs"
         )
@@ -106,14 +119,15 @@
     with open(concat_file_path, "w") as f:
         f.writelines(concat_file_lines)
 
     return concat_file_path
 
 
 def ensure_cleanup_if_needed(f):
+    @functools.wraps(f)
     def g(*args, **kwargs):
         try:
             return f(*args, **kwargs)
         finally:
             if kwargs.get("cleanup", True):
                 assert getattr(g, "paths_to_cleanup", None) is not None
                 for path in g.paths_to_cleanup:
@@ -125,18 +139,37 @@
 @ensure_cleanup_if_needed
 def merge_segments(
     audio_segment_paths: list[Path] | None = None,
     video_segment_paths: list[Path] | None = None,
     output_directory: str | Path | None = None,
     output_stem: str | Path | None = None,
     temp_directory: str | Path | None = None,
-    cut_at_start: int = 0,
-    cut_at_end: int = 0,
+    cut_at_start: float = 0,
+    cut_at_end: float = 0,
     cleanup: bool = True,
 ) -> Path:
+    """Merges and cuts media segments.
+
+    The ``cut_at_start`` and ``cut_at_end`` arguments define the values to be
+    passed to FFmpeg: ``-ss <cut_at_start>s`` and ``-to <cut_at_end>s``,
+    respectively.
+
+    Args:
+        audio_segment_paths: Paths to audio segments.
+        video_segment_paths: Paths to video segments.
+        output_directory: Where to output the merged file.
+        output_stem: An output stem of the merged file.
+        temp_directory: Where to store intermediate files.
+        cut_at_start: An offset (in seconds) to cut at start.
+        cut_at_end: An offset (in seconds) to cut at end.
+        cleanup: Whether to cleanup intermediate files.
+
+    Returns:
+        A path of the merged file.
+    """
     merge_segments.paths_to_cleanup = []
 
     if audio_segment_paths is None and video_segment_paths is None:
         raise ValueError("Audio or/and video paths should be provided")
 
     audio_segment_paths = audio_segment_paths or []
     video_segment_paths = video_segment_paths or []
```

### Comparing `ytpb-2024.3.9/src/ytpb/mpd.py` & `ytpb-2024.4.12/src/ytpb/representations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import io
+"""Representations from MPEG-DASH MPD."""
+
 from dataclasses import dataclass
 from functools import total_ordering
 
 from lxml import etree
 
 
 NAMESPACES = {
@@ -10,19 +11,35 @@
     "yt": "http://youtube.com/yt/2012/10/10",
 }
 
 
 @total_ordering
 @dataclass(frozen=True)
 class VideoQuality:
+    """Represents a video quality (height and frame rate).
+
+    Examples:
+        The class supports comparison operations. For example: ::
+
+          >>> VideoQuality("720p") == VideoQuality("720p30")
+          True
+          >>> VideoQuality("720p") > VideoQuality("720p60")
+          True
+    """
+
     height: int
     frame_rate: float
 
     @classmethod
     def from_string(cls, value: str) -> "VideoQuality":
+        """Creates a :class:`VideoQuality` object from string.
+
+        Args:
+            value: A video quality string. For example: "720p", "1080p60".
+        """
         try:
             height, frame_rate = value.split("p")
             return cls(int(height), float(frame_rate or 30))
         except ValueError:
             raise ValueError("Value not formatted as video quality")
 
     def __str__(self) -> str:
@@ -43,56 +60,68 @@
             return True
         else:
             return False
 
 
 @dataclass(frozen=True, slots=True)
 class RepresentationInfo:
+    """Represents common attributes of audio and video representations."""
+
     itag: str
     mime_type: str
     codecs: str
     base_url: str
 
     @property
-    def format(self):
-        "An alias for a MIME subtype."
+    def type(self) -> str:
+        """An alias for a MIME type."""
+        return self.mime_type.split("/")[0]
+
+    @property
+    def format(self) -> str:
+        """An alias for a MIME subtype."""
         return self.mime_type.split("/")[1]
 
     def __repr__(self):
         return f"{type(self).__name__}(itag={self.itag})"
 
 
 @dataclass(frozen=True, repr=False)
 class AudioRepresentationInfo(RepresentationInfo):
+    """Represents attributes of audio representations."""
+
     audio_sampling_rate: int
 
 
 @dataclass(frozen=True, repr=False)
 class VideoRepresentationInfo(RepresentationInfo):
+    """Represents attributes of video representations."""
+
     width: int
     height: int
     frame_rate: int
 
     @property
     def quality(self) -> VideoQuality:
         return VideoQuality(self.height, self.frame_rate)
 
 
 def _eval_local_xpath(element: etree.Element, node: str) -> list[etree.Element]:
     return element.xpath(".//*[local-name() = $node]", node=node)
 
 
-def strip_manifest(manifest: etree.Element) -> bytes:
-    with io.BytesIO() as output_stream:
-        etree.strip_elements(manifest, f"{{{NAMESPACES['mpd']}}}SegmentList")
-        manifest.write(output_stream, pretty_print=True)
-        return output_stream.getvalue()
+def extract_representations(manifest_content: str) -> list[RepresentationInfo]:
+    """Extracts representations from a manifest.
 
+    Args:
+        manifest_content: An MPEG-DASH MPD string content.
 
-def extract_representations_info(manifest_content: str) -> list[RepresentationInfo]:
+    Returns:
+        A list of :class:`RepresentationInfo` objects.
+    """
     representations_info: list[RepresentationInfo] = []
 
     manifest = etree.fromstring(manifest_content.encode())
 
     adaptation_sets = manifest.xpath("//mpd:AdaptationSet", namespaces=NAMESPACES)
     for adaptation in adaptation_sets:
         mime_type = adaptation.get("mimeType")
```

### Comparing `ytpb-2024.3.9/src/ytpb/segment.py` & `ytpb-2024.4.12/src/ytpb/segment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,112 @@
+"""Media segments and their metadata."""
+
 import re
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 
 import av
 import structlog
 
-from ytpb.exceptions import YtpbError
+from ytpb.errors import YtpbError
 from ytpb.types import SegmentSequence, Timestamp
 from ytpb.utils.other import US_TO_S
 
 logger = structlog.get_logger(__name__)
 
 
 @dataclass
 class SegmentMetadata:
+    """Represents the YouTube segment metadata.
+
+    All timestamp and time-related values are in seconds.
+    """
+
     sequence_number: SegmentSequence
     ingestion_walltime: Timestamp
     ingestion_uncertainty: float
     stream_duration: float
     max_dvr_duration: float
     target_duration: float
     first_frame_time: Timestamp
     first_frame_uncertainty: float
     streamable: str | None = None
     encoding_alias: str | None = None
 
 
 @dataclass
 class Segment:
+    """A media segment."""
+
     def __init__(self) -> None:
         self.local_path: Path | None = None
         self.metadata: SegmentMetadata | None = None
         self.sequence: SegmentSequence | None = None
         self.is_partial: bool | None = None
 
     @classmethod
     def from_file(cls, path: Path) -> "Segment":
+        """Creates a :class:`Segment` object by reading file from path."""
         segment = cls()
 
         with open(path, "rb") as f:
             content = f.read()
             segment.local_path = path
 
         segment.metadata = Segment.parse_youtube_metadata(content)
         segment.sequence = segment.metadata.sequence_number
 
         return segment
 
     @classmethod
     def from_bytes(cls, content: bytes) -> "Segment":
+        """Creates a :class:`Segment` object from bytes."""
         segment = cls()
         segment.metadata = Segment.parse_youtube_metadata(content)
         segment.sequence = segment.metadata.sequence_number
         segment.is_partial = True
 
         return segment
 
     @property
-    def ingestion_start_date(self):
+    def ingestion_start_date(self) -> datetime:
+        """A segment ingestion start date.
+
+        Corresponds to the Ingestion-Walltime-Us value.
+        """
         timestamp = self.metadata.ingestion_walltime
         return datetime.fromtimestamp(timestamp, timezone.utc)
 
     @property
-    def ingestion_end_date(self):
+    def ingestion_end_date(self) -> datetime:
+        """A segment ingestion end date.
+
+        Corresponds to the actual segment duration started from the
+        Ingestion-Walltime-Us value.
+        """
         return self.ingestion_start_date + timedelta(seconds=self.get_actual_duration())
 
     @staticmethod
     def parse_youtube_metadata(content: bytes) -> SegmentMetadata:
+        """Parses the metadata from the full or partial content of a segment.
+
+        All timestamp and time-related values are converted to units of seconds.
+
+        Notes:
+            If partial content is provided, the amount of bytes should be enough
+            to cover the metadata header (see
+            :attr:`~ytpb.locate.PARTIAL_SEGMENT_SIZE_BYTES`).
+
+        Args:
+            content: Full or partial segment byte content.
+
+        Returns:
+            A parsed segment metadata.
+        """
         optional_fields = ("Streamable", "Encoding-Alias")
 
         def _search_for_metadata_field(
             name: str, content: bytes, optional: bool = False
         ) -> bytes | None:
             if matched := re.search(rf"{name}:\s(.+)\r\n".encode(), content):
                 value = matched.group(1)
@@ -109,14 +144,15 @@
                 value = cast_func(value_bytes)
                 name_as_key = name.removesuffix("-Us").lower().replace("-", "_")
                 parsed_metadata_fields[name_as_key] = value
 
         return SegmentMetadata(**parsed_metadata_fields)
 
     def get_actual_duration(self) -> float:
+        """Gets the actual segment duration in seconds."""
         with av.open(str(self.local_path)) as container:
             first_packet, *_, last_packet = list(container.demux())[:-1]
             end_timestamp = last_packet.pts + last_packet.duration
             duration = (end_timestamp - first_packet.pts) * float(
                 first_packet.time_base
             )
             return duration
```

### Comparing `ytpb-2024.3.9/src/ytpb/types.py` & `ytpb-2024.4.12/src/ytpb/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Any, Protocol, TypeAlias
 
 from ytpb.config import AddressableChainMap
-from ytpb.mpd import AudioRepresentationInfo, VideoRepresentationInfo
+from ytpb.representations import AudioRepresentationInfo, VideoRepresentationInfo
 
 
-Timestamp: TypeAlias = float
-
-SegmentSequence: TypeAlias = int
+class RelativeSegmentSequence(int): ...
 
 
-class RelativeSegmentSequence(int): ...
+Timestamp: TypeAlias = float
 
+SegmentSequence: TypeAlias = int
 
 AbsolutePointInStream: TypeAlias = datetime | SegmentSequence
 RelativePointInStream: TypeAlias = timedelta | RelativeSegmentSequence
 PointInStream: TypeAlias = AbsolutePointInStream | RelativePointInStream
 
 AudioStream: TypeAlias = AudioRepresentationInfo
 VideoStream: TypeAlias = VideoRepresentationInfo
 AudioOrVideoStream: TypeAlias = AudioStream | VideoStream
 SetOfStreams: TypeAlias = "Streams[AudioOrVideoStream]"
 
+ConfigMap: TypeAlias = AddressableChainMap
+
 
 class AddressableMappingProtocol(Protocol):
     def traverse(self, address: str, default: Any, delimiter: str) -> Any: ...
 
 
-ConfigMap: TypeAlias = AddressableChainMap
-
-
 @dataclass
 class DateInterval:
     """Represents a closed date interval."""
 
     start: datetime
     end: datetime
```

### Comparing `ytpb-2024.3.9/src/ytpb/actions/compose.py` & `ytpb-2024.4.12/src/ytpb/actions/compose.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""Actions to compose and refresh MPEG-DASH MPDs."""
+
 import copy
 from datetime import datetime, timezone
 
 from lxml import etree
 from lxml.builder import E
 
-from ytpb.exceptions import YtpbError
-from ytpb.mpd import NAMESPACES as NS
+from ytpb.errors import YtpbError
 from ytpb.playback import Playback, RewindInterval
+from ytpb.representations import NAMESPACES as NS
 from ytpb.segment import SegmentMetadata
 from ytpb.streams import SetOfStreams
 from ytpb.utils.other import S_TO_MS
 from ytpb.utils.url import extract_parameter_from_url
 
 
 def _build_top_level_comment_text(base_url: str) -> str:
@@ -94,14 +96,15 @@
 
     return mpd_element
 
 
 def compose_static_mpd(
     playback: Playback, rewind_interval: RewindInterval, streams: SetOfStreams
 ) -> str:
+    """Composes a static MPEG-DASH MPD."""
     mpd_element = _compose_mpd_skeleton(playback, streams)
 
     some_base_url = next(iter(streams)).base_url
 
     rewind_length = rewind_interval.end.sequence - rewind_interval.start.sequence + 1
     segment_duration_s = float(extract_parameter_from_url("dur", some_base_url))
     range_duration_s = rewind_length * int(segment_duration_s)
@@ -135,14 +138,15 @@
 
     return output.decode()
 
 
 def compose_dynamic_mpd(
     playback: Playback, rewind_metadata: SegmentMetadata, streams: SetOfStreams
 ) -> str:
+    """Composes a dynamic MPEG-DASH MPD."""
     mpd_element = _compose_mpd_skeleton(playback, streams)
     mpd_element.attrib["profiles"] = "urn:mpeg:dash:profile:isoff-live:2011"
 
     mpd_element.attrib.update(
         {
             "type": "dynamic",
             "availabilityStartTime": datetime.fromtimestamp(
@@ -178,14 +182,15 @@
         pretty_print=True,
     )
 
     return output.decode()
 
 
 def refresh_mpd(manifest_content: str, streams: SetOfStreams) -> str:
+    """Refreshes segment base URLs in a composed MPEG-DASH MPD."""
     manifest = etree.fromstring(manifest_content.encode())
 
     representation_elements = manifest.xpath("//mpd:Representation", namespaces=NS)
     for representation in representation_elements:
         base_url_element = representation.xpath(".//mpd:BaseURL", namespaces=NS)[0]
         if stream := streams.get_by_itag(itag := representation.get("id")):
             base_url_element.text = stream.base_url
```

### Comparing `ytpb-2024.3.9/src/ytpb/cli/__init__.py` & `ytpb-2024.4.12/src/ytpb/cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import atexit
 import logging
 import os
 import re
 import sys
 from copy import deepcopy
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime, timezone
 from fileinput import FileInput
 from pathlib import Path
 from typing import Any, cast, TextIO
 
 import click
 import cloup
 import structlog
 import toml
 
 from ytpb.cli.commands.capture import capture_group
 from ytpb.cli.commands.download import download_command
 from ytpb.cli.commands.mpd import mpd_group
+
+from ytpb.cli.common import suppress_output
 from ytpb.cli.options import config_options, logging_options
 from ytpb.config import (
+    ALL_ALIASES,
     DEFAULT_CONFIG,
     get_default_config_path,
     load_config_from_file,
     setup_logging,
     update_nested_dict,
 )
 from ytpb.types import ConfigMap
@@ -44,15 +47,16 @@
         return getattr(self.stream, attr)
 
 
 @dataclass
 class ContextObject:
     """This object is referenced as `ctx.obj`."""
 
-    config = ConfigMap(DEFAULT_CONFIG)
+    config: ConfigMap = field(default_factory=lambda: ConfigMap(DEFAULT_CONFIG))
+    original_stdout: TextIO = field(default_factory=lambda: sys.stdout)
 
 
 def load_config_into_context(ctx: click.Context, path: Path) -> dict:
     try:
         config_dict = load_config_from_file(path)
     except FileNotFoundError as e:
         raise click.FileError(
@@ -62,44 +66,68 @@
     except toml.TomlDecodeError as e:
         raise click.FileError(
             filename=path,
             hint=f"Could not load configuration file.\n{e}",
         )
 
     ctx.ensure_object(ContextObject)
-    ctx.obj.config.new_child(config_dict)
+    ctx.obj.config = ctx.obj.config.new_child(config_dict)
 
-    default_map_from_config = config_dict["options"]
+    default_map_from_config = ctx.obj.config["options"]
     ctx.default_map = update_nested_dict(ctx.default_map, default_map_from_config)
 
+    try:
+        ALL_ALIASES.update(ctx.obj.config["general"]["aliases"])
+    except KeyError:
+        pass
+
 
 @cloup.group(invoke_without_command=True)
 @cloup.option_group(
     "Global options",
     config_options,
     logging_options,
+    click.option(
+        "-q",
+        "--quiet",
+        help="Supress all normal output.",
+        default=False,
+        is_flag=True,
+        is_eager=True,
+    ),
 )
+@click.version_option(None, "-V", "--version", message="%(version)s")
 @click.pass_context
 def base_cli(
-    ctx: click.Context, config_path: Path, no_config: bool, debug: bool, report: bool
+    ctx: click.Context,
+    config_path: Path,
+    no_config: bool,
+    debug: bool,
+    report: bool,
+    quiet: bool,
 ) -> None:
     if ctx.invoked_subcommand is None:
         click.echo(ctx.get_help())
         ctx.exit()
 
     ctx.ensure_object(ContextObject)
     ctx.default_map = ctx.obj.config["options"]
 
+    if quiet:
+        suppress_output()
+
     if report:
         debug = True
         os.environ["NO_COLOR"] = "1"
 
         timestamp = datetime.now(tz=timezone.utc).strftime("%Y%m%d-%H%M%S")
         report_handle = open(Path.cwd() / f"ytpb-{timestamp}.log", "a")
-        sys.stdout = cast(TextIO, ReportStreamWrapper(sys.stdout, report_handle))
+        sys.stdout = cast(
+            TextIO, ReportStreamWrapper(ctx.obj.original_stdout, report_handle)
+        )
         sys.stderr = cast(TextIO, ReportStreamWrapper(sys.stderr, report_handle))
 
         @atexit.register
         def sanitize_report_file() -> None:
             report_handle.close()
             with FileInput(report_handle.name, inplace=True) as fi:
                 for line in fi:
```

### Comparing `ytpb-2024.3.9/src/ytpb/cli/common.py` & `ytpb-2024.4.12/src/ytpb/cli/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import email
+import os
 import sys
 import textwrap
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import click
 import cloup
 import structlog
 
 from ytpb.download import compose_default_segment_filename
-from ytpb.exceptions import (
+from ytpb.errors import (
     BadCommandArgument,
     BaseUrlExpiredError,
     BroadcastStatusError,
     CachedItemNotFoundError,
     QueryError,
 )
 from ytpb.fetchers import YoutubeDLInfoFetcher, YtpbInfoFetcher
@@ -203,15 +204,15 @@
         sys.exit(1)
 
 
 def query_streams_or_exit(
     streams: SetOfStreams,
     format_spec: str,
     param: str | None = None,
-    allow_empty: bool = True,
+    allow_empty: bool = False,
     allow_many: bool = True,
 ) -> SetOfStreams:
     try:
         queried_streams = streams.query(format_spec)
     except QueryError as exc:
         message = f"error: Invalid value for '{param}'. {exc}: '{format_spec}'"
         click.echo(message, err=True)
@@ -272,7 +273,11 @@
         raise click.BadParameter(message, ctx, param)
 
 
 def resolve_output_path(output_path: Path) -> Path:
     resolved_path = Path(output_path).expanduser().resolve()
     resolved_path.parent.mkdir(parents=True, exist_ok=True)
     return resolved_path
+
+
+def suppress_output() -> None:
+    sys.stdout = open(os.devnull, "w")
```

### Comparing `ytpb-2024.3.9/src/ytpb/cli/options.py` & `ytpb-2024.4.12/src/ytpb/cli/options.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/src/ytpb/cli/parameters.py` & `ytpb-2024.4.12/src/ytpb/cli/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, time, timedelta
+from datetime import datetime, time, timedelta, timezone
 from enum import auto, StrEnum
 from typing import Literal, NamedTuple
 
 import click
 import structlog
 from timedelta_isoformat import timedelta as isotimedelta
 
@@ -43,14 +43,20 @@
             # Seems like a date and time
             case value if value[:4].isdecimal():
                 try:
                     output = ensure_date_aware(datetime.fromisoformat(value))
                 except ValueError:
                     message = f"'{value}' does not match ISO 8601 date format."
                     self.fail(message, param, ctx)
+            # Unix timestamp
+            case value if value.startswith("@"):
+                timestamp = float(value.lstrip("@"))
+                output = ensure_date_aware(
+                    datetime.fromtimestamp(timestamp, timezone.utc)
+                )
             case _:
                 self.fail("Option doesn't allow '{}' value", param, ctx)
         return output
 
 
 class InputRewindInterval(NamedTuple):
     start: SegmentSequence | datetime | timedelta
@@ -102,14 +108,18 @@
                     second=parsed_time.second,
                     microsecond=parsed_time.microsecond,
                 )
                 output = output.astimezone(parsed_time.tzinfo)
             # Date and time
             case x if "T" in x:
                 output = datetime.fromisoformat(x)
+            # Unix timestamp
+            case x if x.startswith("@"):
+                timestamp = float(x.lstrip("@"))
+                output = datetime.fromtimestamp(timestamp, timezone.utc)
             case "now" | ".." as x:
                 output = x
             case _:
                 raise click.BadParameter(f"Incorrectly formatted part: {part}")
 
         return output
```

### Comparing `ytpb-2024.3.9/src/ytpb/cli/commands/capture.py` & `ytpb-2024.4.12/src/ytpb/cli/commands/capture.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,25 +41,25 @@
 )
 from ytpb.cli.parameters import (
     FormatSpecParamType,
     FormatSpecType,
     InputRewindInterval,
     PointInStreamParamType,
 )
-from ytpb.exceptions import QueryError, SegmentDownloadError, SequenceLocatingError
+from ytpb.errors import QueryError, SegmentDownloadError, SequenceLocatingError
 from ytpb.locate import SegmentLocator
 from ytpb.segment import Segment
 from ytpb.types import (
     AbsolutePointInStream,
     AddressableMappingProtocol,
     DateInterval,
     SegmentSequence,
 )
 from ytpb.utils.date import DurationFormatPattern, format_duration, ISO8601DateFormatter
-from ytpb.utils.other import resolve_relativity_in_interval, S_TO_MS
+from ytpb.utils.other import resolve_relativity_in_interval
 from ytpb.utils.path import (
     expand_template_output_path,
     IntervalOutputPathContext,
     MinimalOutputPathContext,
     OUTPUT_PATH_PLACEHOLDER_RE,
     OutputPathContextRenderer,
     render_minimal_output_path_context,
@@ -225,26 +225,26 @@
         case datetime() as date:
             try:
                 sl = SegmentLocator(
                     reference_base_url,
                     temp_directory=playback.get_temp_directory(),
                     session=playback.session,
                 )
-                moment_sequence, _ = sl.find_sequence_by_time(date.timestamp())
+                moment_sequence, *_ = sl.find_sequence_by_time(date.timestamp())
             except SequenceLocatingError:
                 message = "\nerror: An error occured during segment locating, exit."
                 click.echo(message, err=True)
                 sys.exit(1)
         case "now":
             moment_sequence = head_sequence
 
     click.echo("done.")
 
     try:
-        segment_path = playback.download_segment(moment_sequence, reference_base_url)
+        segment_path = playback.download_segment(moment_sequence, reference_stream)
         moment_segment = Segment.from_file(segment_path)
     except SegmentDownloadError as exc:
         click.echo()
         logger.error(exc, sequence=exc.sequence, exc_info=True)
         sys.exit(1)
 
     requested_moment_date: datetime
@@ -395,29 +395,27 @@
                 raise click.BadParameter(
                     "Open interval is only valid in the preview mode",
                     param=get_parameter_by_name("interval", ctx),
                 )
 
     try:
         rewind_interval = playback.locate_interval(
-            requested_start, requested_end, reference_stream.itag
+            requested_start, requested_end, reference_stream
         )
     except SequenceLocatingError:
         message = "\nerror: An error occured during segment locating, exit."
         click.echo(message, err=True)
         sys.exit(1)
 
     click.echo("done.")
 
-    start_segment = playback.get_downloaded_segment(
-        rewind_interval.start.sequence, reference_base_url
-    )
-    end_segment = playback.get_downloaded_segment(
-        rewind_interval.end.sequence, reference_base_url
+    start_segment = playback.get_segment(
+        rewind_interval.start.sequence, reference_stream
     )
+    end_segment = playback.get_segment(rewind_interval.end.sequence, reference_stream)
 
     requested_start_date: datetime
     match requested_start:
         case SegmentSequence():
             requested_start_date = start_segment.ingestion_start_date
         case datetime():
             requested_start_date = requested_start
@@ -435,29 +433,15 @@
 
     requested_date_interval = DateInterval(requested_start_date, requested_end_date)
     actual_date_interval = DateInterval(
         start_segment.ingestion_start_date,
         end_segment.ingestion_end_date,
     )
 
-    start_diff, end_diff = requested_date_interval - actual_date_interval
-
-    cut_at_start_s = start_diff if start_diff > 0 else 0
-    cut_at_end_s = abs(end_diff) if end_diff < 0 else 0
-    {
-        "cut_at_start": round(cut_at_start_s * int(S_TO_MS)),
-        "cut_at_end": round(cut_at_end_s * int(S_TO_MS)),
-    }
-    actual_date_interval = DateInterval(
-        start=actual_date_interval.start + timedelta(seconds=cut_at_start_s),
-        end=actual_date_interval.end - timedelta(seconds=cut_at_end_s),
-    )
-
-    s = requested_date_interval.start
-    e = requested_date_interval.end
+    s, e = requested_date_interval.start, requested_date_interval.end
     dates_to_capture = [s + every * i for i in range((e - s) // every + 1)]
 
     print_timelapse_summary_info(dates_to_capture, requested_date_interval.end, every)
 
     if preview:
         click.echo("info: Preview mode is enabled, only first 3 frames will be taken.")
         dates_to_capture = dates_to_capture[:3]
@@ -511,15 +495,15 @@
     with capturing_progress:
         # Save the first frame of a time-lapse -- the start segment was already located.
         first_frame_image = extract_frame_as_image(start_segment, requested_start_date)
         _save_ith_frame_as_image(first_frame_image, final_output_path, 0)
         capturing_progress.advance(capturing_task)
 
         captured = capture_frames(
-            playback, dates_to_capture[1:], reference_base_url, start_segment.sequence
+            playback, dates_to_capture[1:], reference_stream, start_segment.sequence
         )
         for i, (image, _) in enumerate(captured, 1):
             _save_ith_frame_as_image(image, final_output_path, i)
             capturing_progress.advance(capturing_task)
 
     try:
         saved_to_path_value = final_output_path.parent.relative_to(Path.cwd())
```

### Comparing `ytpb-2024.3.9/src/ytpb/cli/commands/download.py` & `ytpb-2024.4.12/src/ytpb/cli/commands/download.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,43 +15,44 @@
     get_parameter_by_name,
     print_summary_info,
     query_streams_or_exit,
     raise_for_sequence_ahead_of_current,
     raise_for_too_far_sequence,
     resolve_output_path,
     stream_argument,
+    suppress_output,
 )
 from ytpb.cli.options import (
     cache_options,
     interval_option,
     no_cleanup_option,
     preview_option,
     validate_output_path,
     yt_dlp_option,
 )
 from ytpb.cli.parameters import FormatSpecParamType, FormatSpecType, InputRewindInterval
-from ytpb.exceptions import SequenceLocatingError
+from ytpb.errors import SequenceLocatingError
 from ytpb.merge import merge_segments
 from ytpb.types import (
     AddressableMappingProtocol,
     DateInterval,
     RelativeSegmentSequence,
     SegmentSequence,
 )
-from ytpb.utils.other import resolve_relativity_in_interval, S_TO_MS
+from ytpb.utils.other import resolve_relativity_in_interval
 from ytpb.utils.path import (
     expand_template_output_path,
     IntervalOutputPathContext,
     MinimalOutputPathContext,
     OUTPUT_PATH_PLACEHOLDER_RE,
     render_interval_output_path_context,
     render_minimal_output_path_context,
 )
 from ytpb.utils.remote import request_reference_sequence
-from ytpb.utils.url import extract_parameter_from_url
+from ytpb.utils.url import build_segment_url, extract_parameter_from_url
 
 logger = structlog.get_logger(__name__)
 
 
 class DownloadOutputPathContext(
     MinimalOutputPathContext, IntervalOutputPathContext
 ): ...
@@ -83,14 +84,27 @@
         "--video-format",
         metavar="SPEC",
         type=FormatSpecParamType(FormatSpecType.VIDEO),
         help="Video format to download.",
     ),
     preview_option,
 )
+@cloup.option_group(
+    "Dump options",
+    cloup.option(
+        "--dump-base-urls",
+        is_flag=True,
+        help="Print base URLs and exit.",
+    ),
+    cloup.option(
+        "--dump-segment-urls",
+        is_flag=True,
+        help="Print segment URLs and exit.",
+    ),
+)
 @click.option(
     "-o",
     "--output",
     "output_path",
     type=click.Path(path_type=Path),
     help="Output path (without extension).",
     callback=validate_output_path(DownloadOutputPathContext),
@@ -102,45 +116,50 @@
     type=click.Path(path_type=Path),
     help="Path to a MPEG-DASH manifest.",
 )
 @click.option(
     "-X",
     "--dry-run",
     is_flag=True,
-    help=("Run without downloading."),
+    help="Run without downloading.",
 )
 @yt_dlp_option
 @click.option("--no-cut", is_flag=True, help="Do not perform excerpt cutting.")
 @click.option(
     "--no-merge",
     is_flag=True,
-    help=("Only download segments, without merging. This implies '--no-cleanup'."),
+    help="Only download segments, without merging. This implies '--no-cleanup'.",
 )
 @no_cleanup_option
 @cache_options
 @stream_argument
 @constraint(require_any, ["audio_format", "video_format"])
 @click.pass_context
 def download_command(
     ctx: click.Context,
     interval: InputRewindInterval,
     audio_format: str,
     video_format: str,
     preview: bool,
+    dump_base_urls: bool,
+    dump_segment_urls: bool,
     output_path: Path,
     from_manifest: Path,
     dry_run: bool,
     yt_dlp: bool,
     no_cut: bool,
     no_merge: bool,
     no_cleanup: bool,
     force_update_cache: bool,
     no_cache: bool,
     stream_url: str,
 ) -> int:
+    if dump_base_urls or dump_segment_urls:
+        suppress_output()
+
     if no_merge:
         no_cleanup = True
 
     playback = create_playback(ctx)
 
     queried_audio_streams = []
     if audio_format:
@@ -177,14 +196,21 @@
             f"   - Video: itag {video_stream.itag}, "
             f"{video_stream.format} ({video_stream.codecs}), "
             f"{video_stream.width}x{video_stream.height}, "
             f"{video_stream.frame_rate} fps"
         )
         logger.info("Queried video stream", base_url=video_stream.base_url)
 
+    if dump_base_urls:
+        if audio_format:
+            click.echo(audio_stream.base_url, ctx.obj.original_stdout)
+        if video_format:
+            click.echo(video_stream.base_url, ctx.obj.original_stdout)
+        sys.exit()
+
     click.echo()
     click.echo("(<<) Locating start and end in the stream... ", nl=False)
 
     reference_stream = video_stream or audio_stream
     reference_base_url = reference_stream.base_url
     head_sequence = request_reference_sequence(reference_base_url, playback.session)
 
@@ -216,32 +242,41 @@
         number_of_segments = round(preview_duration_value / segment_duration)
         requested_end = RelativeSegmentSequence(number_of_segments)
 
     try:
         rewind_interval = playback.locate_interval(
             requested_start,
             requested_end,
-            reference_stream.itag,
+            reference_stream,
         )
     except SequenceLocatingError:
         message = "\nerror: An error occured during segment locating, exit."
         click.echo(message, err=True)
         sys.exit(1)
 
     click.echo("done.")
 
+    if dump_segment_urls:
+        range_part = "[{start}-{end}]".format(
+            start=rewind_interval.start.sequence, end=rewind_interval.end.sequence
+        )
+        build_dump_url = lambda base_url: build_segment_url(base_url, range_part)
+        if audio_format:
+            click.echo(build_dump_url(audio_stream.base_url), ctx.obj.original_stdout)
+        if video_format:
+            click.echo(build_dump_url(video_stream.base_url), ctx.obj.original_stdout)
+        sys.exit()
+
     if preview and interval[1] != "..":
         click.echo("info: The preview mode is enabled, interval end is ignored.")
 
-    start_segment = playback.get_downloaded_segment(
-        rewind_interval.start.sequence, reference_base_url
-    )
-    end_segment = playback.get_downloaded_segment(
-        rewind_interval.end.sequence, reference_base_url
+    start_segment = playback.get_segment(
+        rewind_interval.start.sequence, reference_stream
     )
+    end_segment = playback.get_segment(rewind_interval.end.sequence, reference_stream)
 
     requested_start_date: datetime
     match requested_start:
         case SegmentSequence():
             requested_start_date = start_segment.ingestion_start_date
         case datetime():
             requested_start_date = requested_start
@@ -259,32 +294,30 @@
 
     requested_date_interval = DateInterval(requested_start_date, requested_end_date)
     actual_date_interval = DateInterval(
         start_segment.ingestion_start_date,
         end_segment.ingestion_end_date,
     )
 
-    if no_cut:
-        cut_kwargs = {}
-    else:
-        start_diff, end_diff = requested_date_interval - actual_date_interval
-        cut_at_start_s = start_diff if start_diff > 0 else 0
+    cut_kwargs: dict[str, float] = {}
+    if not no_cut:
+        cut_at_start = rewind_interval.start.cut_at
         if preview:
-            cut_at_end_s = 0
+            cut_at_end = 0
         else:
-            cut_at_end_s = abs(end_diff) if end_diff < 0 else 0
-        cut_kwargs = {
-            "cut_at_start": round(cut_at_start_s * int(S_TO_MS)),
-            "cut_at_end": round(cut_at_end_s * int(S_TO_MS)),
-        }
-        if not no_merge:
-            actual_date_interval = DateInterval(
-                actual_date_interval.start + timedelta(seconds=cut_at_start_s),
-                actual_date_interval.end - timedelta(seconds=cut_at_end_s),
-            )
+            cut_at_end = rewind_interval.end.cut_at
+        cut_kwargs.update(
+            {
+                "cut_at_start": cut_at_start,
+                "cut_at_end": cut_at_end,
+            }
+        )
+        actual_date_interval = DateInterval(
+            rewind_interval.start.date, rewind_interval.end.date
+        )
 
     print_summary_info(requested_date_interval, actual_date_interval, rewind_interval)
     click.echo()
 
     if dry_run:
         click.echo("notice: This is a dry run. Skip downloading and exit.")
     else:
@@ -310,59 +343,67 @@
                 render_download_output_path_context,
                 ctx.obj.config,
             )
         else:
             final_output_path = output_path
         final_output_path = resolve_output_path(final_output_path)
 
-        do_download_excerpt_segments = partial(
-            actions.download.download_excerpt,
+        total_segments = (
+            rewind_interval.end.sequence - rewind_interval.start.sequence + 1
+        )
+        progress_reporter = actions.download.RichProgressReporter()
+        if audio_stream:
+            progress_reporter.progress.add_task("   - Audio", total=total_segments)
+        if video_stream:
+            progress_reporter.progress.add_task("   - Video", total=total_segments)
+        do_download_segments = partial(
+            actions.download.download_segments,
             playback,
             rewind_interval,
-            audio_format,
-            video_format,
-            output_directory=final_output_path.parent,
-            output_stem=final_output_path.name,
-            no_merge=True,
+            [x for x in [audio_stream, video_stream] if x is not None],
+            progress_reporter=progress_reporter,
         )
 
         if no_merge:
             click.echo(
                 "(<<) Downloading segments {}-{} (no merge requested)...".format(
                     rewind_interval.start.sequence, rewind_interval.end.sequence
                 )
             )
-            download_result = do_download_excerpt_segments()
-            some_downloaded_paths = (
-                download_result.audio_segment_paths
-                or download_result.video_segment_paths
-            )
+            downloaded_segment_paths = do_download_segments()
+            some_downloaded_path = downloaded_segment_paths[0][0]
             click.echo(
-                "\nSuccess! Segments saved to {}/.".format(
-                    some_downloaded_paths[0].parent
-                )
+                "\nSuccess! Segments saved to {}/.".format(some_downloaded_path.parent)
             )
         else:
             click.echo("(<<) Preparing and saving the excerpt...")
             click.echo(
                 "1. Downloading segments {}-{}:".format(
                     rewind_interval.start.sequence, rewind_interval.end.sequence
                 )
             )
 
-            download_result = do_download_excerpt_segments()
+            downloaded_segment_paths = do_download_segments()
+            audio_and_video_segment_paths: list[list[Path]] = [[], []]
+            match audio_stream, video_stream:
+                case _, None:
+                    audio_and_video_segment_paths[0] = downloaded_segment_paths[0]
+                case None, _:
+                    audio_and_video_segment_paths[1] = downloaded_segment_paths[0]
+                case _:
+                    audio_and_video_segment_paths = downloaded_segment_paths
 
             if no_cut:
                 click.echo("2. Merging segments (no cut requested)... ", nl=False)
             else:
                 click.echo("2. Merging segments (may take a while)... ", nl=False)
 
             merged_path = merge_segments(
-                download_result.audio_segment_paths,
-                download_result.video_segment_paths,
+                audio_and_video_segment_paths[0],
+                audio_and_video_segment_paths[1],
                 output_directory=final_output_path.parent,
                 output_stem=final_output_path.name,
                 temp_directory=playback.get_temp_directory(),
                 **cut_kwargs,
             )
             click.echo("done.\n")
```

### Comparing `ytpb-2024.3.9/src/ytpb/cli/commands/mpd.py` & `ytpb-2024.4.12/src/ytpb/cli/commands/mpd.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 from ytpb.cli.options import (
     cache_options,
     interval_option,
     validate_output_path,
     yt_dlp_option,
 )
 from ytpb.cli.parameters import FormatSpecParamType, FormatSpecType
-from ytpb.exceptions import BroadcastStatusError
+from ytpb.errors import BroadcastStatusError
 from ytpb.fetchers import YoutubeDLInfoFetcher, YtpbInfoFetcher
 from ytpb.info import BroadcastStatus
-from ytpb.mpd import extract_representations_info
 from ytpb.playback import Playback
+from ytpb.representations import extract_representations
 from ytpb.streams import Streams
 from ytpb.types import DateInterval, SegmentSequence
 from ytpb.utils.date import express_timedelta_in_words
 from ytpb.utils.other import resolve_relativity_in_interval
 from ytpb.utils.path import expand_template_output_path, OUTPUT_PATH_PLACEHOLDER_RE
 from ytpb.utils.remote import request_reference_sequence
 from ytpb.utils.url import build_video_url_from_base_url, extract_parameter_from_url
@@ -187,24 +187,22 @@
             requested_end, head_sequence, ctx, "interval"
         )
     if requested_end == "now":
         requested_end = head_sequence - 1
 
     click.echo("(<<) Locating start and end in the stream... ", nl=False)
     rewind_interval = playback.locate_interval(
-        requested_start, requested_end, reference_stream.itag
+        requested_start, requested_end, reference_stream
     )
     click.echo("done.")
 
-    start_segment = playback.get_downloaded_segment(
-        rewind_interval.start.sequence, reference_base_url
-    )
-    end_segment = playback.get_downloaded_segment(
-        rewind_interval.end.sequence, reference_base_url
+    start_segment = playback.get_segment(
+        rewind_interval.start.sequence, reference_stream
     )
+    end_segment = playback.get_segment(rewind_interval.end.sequence, reference_stream)
 
     requested_start_date: datetime
     match requested_start:
         case SegmentSequence():
             requested_start_date = start_segment.ingestion_start_date
         case datetime():
             requested_start_date = requested_start
@@ -277,15 +275,15 @@
 def refresh_command(
     yt_dlp: bool,
     manifest: str,
 ) -> int:
     with open(manifest, "r", encoding="utf-8") as f:
         manifest_content = f.read()
 
-    list_of_streams = extract_representations_info(manifest_content)
+    list_of_streams = extract_representations(manifest_content)
     stream_url = build_video_url_from_base_url(list_of_streams[0].base_url)
 
     if yt_dlp:
         fetcher = YoutubeDLInfoFetcher(stream_url)
     else:
         fetcher = YtpbInfoFetcher(stream_url)
```

### Comparing `ytpb-2024.3.9/src/ytpb/utils/date.py` & `ytpb-2024.4.12/src/ytpb/utils/date.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/src/ytpb/utils/other.py` & `ytpb-2024.4.12/src/ytpb/utils/other.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/src/ytpb/utils/path.py` & `ytpb-2024.4.12/src/ytpb/utils/path.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/src/ytpb/utils/remote.py` & `ytpb-2024.4.12/src/ytpb/utils/remote.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from ytpb.exceptions import YtpbError
+from ytpb.errors import YtpbError
 from ytpb.types import AudioOrVideoStream, SegmentSequence, VideoStream
 
 
 def get_priority_reference_stream(streams: list[AudioOrVideoStream]) -> str:
     for stream in streams:
         if isinstance(stream, VideoStream):
             break
```

### Comparing `ytpb-2024.3.9/src/ytpb/utils/url.py` & `ytpb-2024.4.12/src/ytpb/utils/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import time
 from urllib.parse import parse_qs, urlparse
 
-from ytpb.exceptions import BadCommandArgument
+from ytpb.errors import BadCommandArgument
+from ytpb.types import SegmentSequence
 
 
 def normalize_video_url(video_url_or_id: str) -> str:
     video_id_re = r"(?P<video_id>[\w-]{11})"
     patterns = (
         rf"{video_id_re}$",
         rf"https://www\.(?:youtube\.com/watch\?v=|youtu\.be\/){video_id_re}(?![^&])",
@@ -59,10 +60,14 @@
 
 
 def build_video_url_from_base_url(base_url: str) -> str:
     video_id = extract_id_from_base_url(base_url)
     return build_video_url_with_id(video_id)
 
 
+def build_segment_url(base_url: str, sq: SegmentSequence | str) -> str:
+    return f"{base_url.rstrip('/')}/sq/{sq}"
+
+
 def check_base_url_is_expired(base_url: str) -> bool:
     expires_at = int(extract_parameter_from_url("expire", base_url))
     return time.time() >= expires_at
```

### Comparing `ytpb-2024.3.9/tests/conftest.py` & `ytpb-2024.4.12/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/helpers.py` & `ytpb-2024.4.12/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/test_cache.py` & `ytpb-2024.4.12/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/test_download.py` & `ytpb-2024.4.12/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/test_fetchers.py` & `ytpb-2024.4.12/tests/test_fetchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 from ytpb.fetchers import YoutubeDLInfoFetcher, YtpbInfoFetcher
 from ytpb.info import YouTubeVideoInfo
 from ytpb.playback import Playback
 from ytpb.streams import AudioOrVideoStream
 
 
 @patch("ytpb.fetchers.extract_video_info")
-@patch("ytpb.fetchers.extract_representations_info")
+@patch("ytpb.fetchers.extract_representations")
 def test_ytpb_info_fetcher(
-    mock_extract_representations_info: MagicMock,
+    mock_extract_representations: MagicMock,
     mock_extract_video_info: MagicMock,
     mocked_responses: responses.RequestsMock,
     stream_url: str,
     active_live_video_info: YouTubeVideoInfo,
     streams_in_list: list[AudioOrVideoStream],
     tmp_path: Path,
 ):
     mocked_responses.get(stream_url, status=200)
     mocked_responses.get(active_live_video_info.dash_manifest_url, status=200)
 
     mock_extract_video_info.return_value = active_live_video_info
-    mock_extract_representations_info.return_value = streams_in_list
+    mock_extract_representations.return_value = streams_in_list
 
     fetcher = YtpbInfoFetcher(stream_url)
     assert fetcher.fetch_video_info() == active_live_video_info
     assert len(fetcher.fetch_streams()) == len(streams_in_list)
 
 
 def test_youtube_dl_info_fetcher(
```

### Comparing `ytpb-2024.3.9/tests/test_merge.py` & `ytpb-2024.4.12/tests/test_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     output_stem = tmp_path / "merged"
 
     merge_segments(
         audio_segment_paths=[SEGMENT_BASE_PATH / "7959120.i140.mp4"],
         video_segment_paths=[SEGMENT_BASE_PATH / "7959120.i244.webm"],
         output_stem=output_stem,
         temp_directory=run_temp_directory,
-        cut_at_start=500,
+        cut_at_start=0.5,
     )
 
     expected_output_path = output_stem.with_suffix(".mkv")
     assert os.path.exists(expected_output_path)
 
     assert_number_of_streams(expected_output_path, 2)
     assert_approx_duration(expected_output_path, 1.5)
@@ -87,16 +87,16 @@
     output_stem = tmp_path / "merged"
 
     merge_segments(
         audio_segment_paths=[SEGMENT_BASE_PATH / "7959120.i140.mp4"],
         video_segment_paths=[SEGMENT_BASE_PATH / "7959120.i244.webm"],
         output_stem=output_stem,
         temp_directory=run_temp_directory,
-        cut_at_start=500,
-        cut_at_end=500,
+        cut_at_start=0.5,
+        cut_at_end=1.5,
     )
 
     expected_output_path = output_stem.with_suffix(".mkv")
     assert os.path.exists(expected_output_path)
 
     assert_number_of_streams(expected_output_path, 2)
     assert_approx_duration(expected_output_path, 1.5)
@@ -143,16 +143,16 @@
         ],
         video_segment_paths=[
             SEGMENT_BASE_PATH / "7959120.i244.webm",
             SEGMENT_BASE_PATH / "7959121.i244.webm",
         ],
         output_stem=output_stem,
         temp_directory=run_temp_directory,
-        cut_at_start=500,
-        cut_at_end=500,
+        cut_at_start=0.5,
+        cut_at_end=1.5,
     )
 
     expected_output_path = output_stem.with_suffix(".mkv")
     assert os.path.exists(expected_output_path)
 
     assert_number_of_streams(expected_output_path, 2)
     assert_approx_duration(expected_output_path, 3.0)
@@ -201,16 +201,16 @@
         video_segment_paths=[
             SEGMENT_BASE_PATH / "7959120.i244.webm",
             SEGMENT_BASE_PATH / "7959121.i244.webm",
             SEGMENT_BASE_PATH / "7959122.i244.webm",
         ],
         output_stem=output_stem,
         temp_directory=run_temp_directory,
-        cut_at_start=500,
-        cut_at_end=500,
+        cut_at_start=0.5,
+        cut_at_end=1.5,
     )
 
     expected_output_path = output_stem.with_suffix(".mkv")
     assert os.path.exists(expected_output_path)
 
     assert_number_of_streams(expected_output_path, 2)
     assert_approx_duration(expected_output_path, 5.0)
@@ -247,16 +247,16 @@
     merge_segments(
         audio_segment_paths=[
             SEGMENT_BASE_PATH / "7959120.i140.mp4",
             SEGMENT_BASE_PATH / "7959121.i140.mp4",
         ],
         output_stem=output_stem,
         temp_directory=run_temp_directory,
-        cut_at_start=500,
-        cut_at_end=500,
+        cut_at_start=0.5,
+        cut_at_end=1.5,
     )
 
     expected_output_path = output_stem.with_suffix(".mp4")
     assert os.path.exists(expected_output_path)
 
     assert_number_of_streams(expected_output_path, 1)
     assert_approx_duration(expected_output_path, 3.0)
@@ -293,16 +293,16 @@
     merge_segments(
         video_segment_paths=[
             SEGMENT_BASE_PATH / "7959120.i244.webm",
             SEGMENT_BASE_PATH / "7959121.i244.webm",
         ],
         output_stem=output_stem,
         temp_directory=run_temp_directory,
-        cut_at_start=500,
-        cut_at_end=500,
+        cut_at_start=0.5,
+        cut_at_end=1.5,
     )
 
     expected_output_path = output_stem.with_suffix(".webm")
     assert os.path.exists(expected_output_path)
 
     assert_number_of_streams(expected_output_path, 1)
     assert_approx_duration(expected_output_path, 3.0)
```

### Comparing `ytpb-2024.3.9/tests/test_playback.py` & `ytpb-2024.4.12/tests/test_playback.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,36 +7,50 @@
  2023-03-25T23:33:54.491Z  56.490Z  58.492Z
                   1679787234.491176
                            1679787236.489910
                                     1679787238.491916
 """
 
 import json
-from dataclasses import asdict
+from dataclasses import asdict, dataclass
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 from typing import Callable
 from urllib.parse import urljoin
 
 import pytest
 import responses
 
 from conftest import TEST_DATA_PATH
 from freezegun import freeze_time
 
-from ytpb.exceptions import (
+from ytpb.errors import (
     BaseUrlExpiredError,
     CachedItemNotFoundError,
     SequenceLocatingError,
 )
 from ytpb.fetchers import YtpbInfoFetcher
 from ytpb.info import YouTubeVideoInfo
-from ytpb.playback import Playback, RewindMoment
+from ytpb.playback import Playback, RewindInterval, RewindMoment
 from ytpb.streams import AudioOrVideoStream
-from ytpb.types import RelativeSegmentSequence
+from ytpb.types import (
+    AbsolutePointInStream,
+    RelativePointInStream,
+    RelativeSegmentSequence,
+    SegmentSequence,
+)
+
+
+@pytest.fixture
+def fake_stream(audio_base_url: str) -> "FakeStream":
+    @dataclass
+    class FakeStream:
+        base_url: str
+
+    return FakeStream(audio_base_url)
 
 
 class TestLocateMoment:
     @pytest.fixture(autouse=True)
     def setup_method(
         self,
         fake_info_fetcher: "FakeInfoFetcher",
@@ -47,37 +61,55 @@
         audio_base_url: str,
         tmp_path: Path,
     ):
         add_responses_callback_for_segment_urls(urljoin(audio_base_url, r"sq/\w+"))
         self.playback = Playback(stream_url, fetcher=fake_info_fetcher)
         self.playback.fetch_and_set_essential()
 
-    def test_start_sequence(self):
+    def test_start_sequence(self, fake_stream):
         sequence = 7959120
         date = datetime.fromtimestamp(1679787234.491176, tz=timezone.utc)
         expected = RewindMoment(date, sequence, 0, False)
-        assert expected == self.playback.locate_moment(sequence, "140")
+        assert expected == self.playback.locate_moment(sequence, fake_stream)
 
-    def test_end_sequence(self):
+    def test_end_sequence(self, fake_stream):
         sequence = 7959120
         date = datetime(2023, 3, 25, 23, 33, 56, 488092, tzinfo=timezone.utc)
         expected = RewindMoment(date, sequence, 0, True)
-        assert expected == self.playback.locate_moment(sequence, "140", True)
+        assert expected == self.playback.locate_moment(sequence, fake_stream, True)
 
-    def test_start_date(self, add_responses_callback_for_reference_base_url: Callable):
+    def test_start_date(
+        self, add_responses_callback_for_reference_base_url: Callable, fake_stream
+    ):
         add_responses_callback_for_reference_base_url()
         date = datetime.fromisoformat("2023-03-25T23:33:55Z")
-        expected = RewindMoment(date, 7959120, 0.508824, False)
-        assert expected == self.playback.locate_moment(date, "140")
+        expected = RewindMoment(date, 7959120, 0.508824, False, False)
+        actual = self.playback.locate_moment(date, fake_stream)
+        assert expected == RewindMoment(
+            actual.date,
+            actual.sequence,
+            pytest.approx(actual.cut_at, 1e-6),
+            actual.is_end,
+            actual.falls_in_gap,
+        )
 
-    def test_end_date(self, add_responses_callback_for_reference_base_url: Callable):
+    def test_end_date(
+        self, add_responses_callback_for_reference_base_url: Callable, fake_stream
+    ):
         add_responses_callback_for_reference_base_url()
         date = datetime.fromisoformat("2023-03-25T23:33:55Z")
-        expected = RewindMoment(date, 7959120, 0.508824, True)
-        assert expected == self.playback.locate_moment(date, "140", True)
+        expected = RewindMoment(date, 7959120, 0.508824, True, False)
+        actual = self.playback.locate_moment(date, fake_stream, True)
+        assert expected == RewindMoment(
+            actual.date,
+            actual.sequence,
+            pytest.approx(actual.cut_at, 1e-6),
+            actual.is_end,
+            actual.falls_in_gap,
+        )
 
 
 @pytest.mark.parametrize(
     "start,end",
     [
         (7959120, 7959121),
         (7959120, datetime.fromisoformat("2023-03-25T23:33:57Z")),
@@ -90,38 +122,39 @@
         ),
         (datetime.fromisoformat("2023-03-25T23:33:55Z"), timedelta(seconds=2)),
         (datetime.fromisoformat("2023-03-25T23:33:55Z"), RelativeSegmentSequence(1)),
         (timedelta(seconds=3), 7959121),  # segment duration (2 s) + 1 s
         (timedelta(seconds=2), datetime.fromisoformat("2023-03-25T23:33:57Z")),
         (RelativeSegmentSequence(1), 7959121),
         (RelativeSegmentSequence(1), datetime.fromisoformat("2023-03-25T23:33:57Z")),
-        (RelativeSegmentSequence(1), 7959121),
     ],
 )
 def test_locate_interval(
     start,
     end,
     fake_info_fetcher: "FakeInfoFetcher",
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     stream_url: str,
     active_live_video_info: YouTubeVideoInfo,
     audio_base_url: str,
+    fake_stream: "FakeStream",
     tmp_path: Path,
 ) -> None:
     # Given:
-    if not (isinstance(start, int) and isinstance(end, int)):
+    any_datetime = isinstance(start, datetime) or isinstance(end, datetime)
+    if type(start) is not SegmentSequence and any_datetime:
         add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(urljoin(audio_base_url, r"sq/\w+"))
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
-    interval = playback.locate_interval(start, end, "140")
+    interval = playback.locate_interval(start, end, fake_stream)
 
     # Then:
     assert interval.start.sequence == 7959120
     assert interval.end.sequence == 7959121
 
 
 @pytest.mark.parametrize(
@@ -134,20 +167,21 @@
     ],
 )
 def test_local_interval_with_relative_start_and_end(
     start: timedelta | RelativeSegmentSequence,
     end: timedelta | RelativeSegmentSequence,
     stream_url: str,
     fake_info_fetcher: "FakeInfoFetcher",
+    fake_stream: "FakeStream",
     tmp_path: Path,
 ):
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
     with pytest.raises(ValueError):
-        playback.locate_interval(start, end, "140")
+        playback.locate_interval(start, end, fake_stream)
 
 
 @pytest.mark.parametrize(
     "start,end",
     [
         (7959122, 7959121),
         (7959121, datetime.fromisoformat("2023-03-25T23:33:55Z")),
@@ -165,28 +199,53 @@
     fake_info_fetcher: "FakeInfoFetcher",
     add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     mocked_responses: responses.RequestsMock,
     stream_url: str,
     active_live_video_info: YouTubeVideoInfo,
     audio_base_url: str,
+    fake_stream: "FakeStream",
     tmp_path: Path,
 ) -> None:
     # Given:
-    if not (isinstance(start, int) and isinstance(end, int)):
+    if not isinstance(start, int):
         add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(urljoin(audio_base_url, r"sq/\w+"))
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
 
     # Then:
     with pytest.raises((ValueError, SequenceLocatingError)):
-        playback.locate_interval(start, end, "140")
+        playback.locate_interval(start, end, fake_stream)
+
+
+def test_insert_to_rewind_history(
+    fake_info_fetcher: "FakeInfoFetcher",
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    mocked_responses: responses.RequestsMock,
+    stream_url: str,
+    audio_base_url: str,
+    fake_stream: "FakeStream",
+    tmp_path: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_segment_urls(urljoin(audio_base_url, r"sq/\w+"))
+
+    # When:
+    playback = Playback(stream_url, fetcher=fake_info_fetcher)
+    playback.fetch_and_set_essential()
+    playback.locate_moment(7959120, fake_stream)
+    playback.locate_moment(7959122, fake_stream)
+
+    # Then:
+    assert playback.rewind_history.closest(1679787234.491176).value == 7959120
+    assert playback.rewind_history.closest(1679787238.491916).value == 7959122
 
 
 def test_create_playback_from_url(
     fake_info_fetcher: "FakeInfoFetcher",
     active_live_video_info: YouTubeVideoInfo,
     streams_in_list: list[AudioOrVideoStream],
     stream_url: str,
@@ -261,7 +320,16 @@
     with pytest.raises(CachedItemNotFoundError):
         Playback.from_cache(stream_url)
 
 
 def test_type_of_playback_default_fetcher(stream_url: str):
     playback = Playback(stream_url)
     assert isinstance(playback.fetcher, YtpbInfoFetcher)
+
+
+def test_rewind_interval_properties():
+    interval = RewindInterval(
+        RewindMoment(datetime(2024, 1, 2, 10, 20, 0), 0, 0),
+        RewindMoment(datetime(2024, 1, 2, 10, 20, 30), 1000, 0),
+    )
+    assert timedelta(seconds=30) == interval.duration
+    assert 1001 == len(interval.sequences)
```

### Comparing `ytpb-2024.3.9/tests/test_playback_session.py` & `ytpb-2024.4.12/tests/test_playback_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 from dataclasses import asdict
 from unittest.mock import patch
 from urllib.parse import urljoin
 
 import pytest
 import responses
-from ytpb.exceptions import MaxRetryError
+from ytpb.errors import MaxRetryError
 
 from ytpb.playback import Playback
 from ytpb.streams import AudioStream, Streams
 
 
 class SideEffectCycler:
     def __init__(self, side_effects):
```

### Comparing `ytpb-2024.3.9/tests/test_segment.py` & `ytpb-2024.4.12/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/test_streams.py` & `ytpb-2024.4.12/tests/test_streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ytpb.exceptions import QueryError
+from ytpb.errors import QueryError
 from ytpb.streams import AudioOrVideoStream, AudioStream, Streams
 
 
 def test_abstract_methods(streams_in_list: list[AudioOrVideoStream]):
     streams = Streams(streams_in_list)
 
     assert len(streams) == len(streams_in_list)
```

### Comparing `ytpb-2024.3.9/tests/test_types.py` & `ytpb-2024.4.12/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/actions/test_compose.py` & `ytpb-2024.4.12/tests/actions/test_compose.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import freezegun
 import pytest
 from freezegun import freeze_time
 
 from helpers import patched_freezgun_astimezone
 
 from ytpb.actions.compose import compose_dynamic_mpd, compose_static_mpd, refresh_mpd
-from ytpb.exceptions import YtpbError
+from ytpb.errors import YtpbError
 from ytpb.playback import Playback
 from ytpb.segment import SegmentMetadata
 from ytpb.streams import Streams
 from ytpb.types import AudioOrVideoStream, AudioStream, VideoStream
 
 freezegun.api.FakeDatetime.astimezone = patched_freezgun_astimezone
```

### Comparing `ytpb-2024.3.9/tests/actions/test_download.py` & `ytpb-2024.4.12/tests/actions/test_download.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,144 +3,177 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Callable
 from urllib.parse import urljoin
 
 import responses
 
+from helpers import assert_approx_duration
+
 from ytpb import actions
-from ytpb.playback import Playback
+from ytpb.playback import Playback, RewindInterval
 
 
 @dataclass
 class FakeRewindMoment:
     sequence: int
+    cut_at: float = 0
 
 
 @dataclass
 class FakeRewindInterval:
     start: FakeRewindMoment
     end: FakeRewindMoment
+    sequences = RewindInterval.sequences
+
+
+@dataclass
+class FakeStream:
+    base_url: str
 
 
-def test_download_excerpt_between_sequences_without_merging(
+def test_download_audio_segments(
+    fake_info_fetcher: "FakeInfoFetcher",
+    add_responses_callback_for_segment_urls: Callable,
+    stream_url: str,
+    audio_base_url: str,
+    run_temp_directory: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    playback = Playback(stream_url, fetcher=fake_info_fetcher)
+    playback.fetch_and_set_essential()
+    output_paths = actions.download.download_segments(
+        playback,
+        FakeRewindInterval(FakeRewindMoment(7959120), FakeRewindMoment(7959121)),
+        [FakeStream(audio_base_url)],
+    )
+
+    # Then:
+    assert output_paths == [
+        [
+            run_temp_directory / "segments/7959120.i140.mp4",
+            run_temp_directory / "segments/7959121.i140.mp4",
+        ]
+    ]
+
+
+def test_download_audio_and_video_segments(
     fake_info_fetcher: "FakeInfoFetcher",
     add_responses_callback_for_segment_urls: Callable,
     stream_url: str,
     audio_base_url: str,
     video_base_url: str,
     run_temp_directory: Path,
 ) -> None:
     # Given:
     add_responses_callback_for_segment_urls(
-        urljoin(audio_base_url, r"sq/\w+"), urljoin(video_base_url, r"sq/\w+")
+        urljoin(audio_base_url, r"sq/\w+"),
+        urljoin(video_base_url, r"sq/\w+"),
     )
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
-    _, *output_paths = actions.download.download_excerpt(
+    output_paths = actions.download.download_segments(
         playback,
         FakeRewindInterval(FakeRewindMoment(7959120), FakeRewindMoment(7959121)),
-        "itag eq 140",
-        "itag eq 244",
-        no_merge=True,
+        [FakeStream(audio_base_url), FakeStream(video_base_url)],
     )
 
     # Then:
     assert output_paths == [
-        None,
         [
             run_temp_directory / "segments/7959120.i140.mp4",
             run_temp_directory / "segments/7959121.i140.mp4",
         ],
         [
             run_temp_directory / "segments/7959120.i244.webm",
             run_temp_directory / "segments/7959121.i244.webm",
         ],
     ]
-    assert os.path.exists(run_temp_directory / "segments/7959120.i140.mp4")
-    assert os.path.exists(run_temp_directory / "segments/7959121.i140.mp4")
-    assert os.path.exists(run_temp_directory / "segments/7959120.i244.webm")
-    assert os.path.exists(run_temp_directory / "segments/7959121.i244.webm")
 
 
-def test_download_audio_excerpt_between_sequences_without_merging(
+def test_download_audio_excerpt_with_cutting(
     fake_info_fetcher: "FakeInfoFetcher",
     add_responses_callback_for_segment_urls: Callable,
     stream_url: str,
     audio_base_url: str,
     run_temp_directory: Path,
+    tmp_path: Path,
 ) -> None:
     # Given:
-    add_responses_callback_for_segment_urls(
-        urljoin(audio_base_url, r"sq/\w+"),
-    )
+    add_responses_callback_for_segment_urls(urljoin(audio_base_url, r"sq/\w+"))
 
     # When:
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
-    _, *output_paths = actions.download.download_excerpt(
+    output_result = actions.download.download_excerpt(
         playback,
-        FakeRewindInterval(FakeRewindMoment(7959120), FakeRewindMoment(7959121)),
-        "itag eq 140",
-        no_merge=True,
+        FakeRewindInterval(
+            FakeRewindMoment(7959120, cut_at=0.5),
+            FakeRewindMoment(7959121, cut_at=1.5),
+        ),
+        tmp_path / "output",
+        FakeStream(audio_base_url),
     )
 
     # Then:
-    assert output_paths == [
+    assert output_result == (
         None,
+        tmp_path / "output.mp4",
         [
             run_temp_directory / "segments/7959120.i140.mp4",
             run_temp_directory / "segments/7959121.i140.mp4",
         ],
         [],
-    ]
-    assert os.path.exists(run_temp_directory / "segments/7959120.i140.mp4")
-    assert os.path.exists(run_temp_directory / "segments/7959121.i140.mp4")
+    )
+    assert_approx_duration(output_result[1], 3)
 
 
-def test_download_excerpt_between_dates_without_merging(
+def test_download_audio_and_video_excerpt_without_cutting(
     fake_info_fetcher: "FakeInfoFetcher",
-    mocked_responses: responses.RequestsMock,
-    add_responses_callback_for_reference_base_url: Callable,
     add_responses_callback_for_segment_urls: Callable,
     stream_url: str,
     audio_base_url: str,
     video_base_url: str,
     run_temp_directory: Path,
+    tmp_path: Path,
 ) -> None:
     # Given:
-    add_responses_callback_for_reference_base_url()
     add_responses_callback_for_segment_urls(
         urljoin(audio_base_url, r"sq/\w+"), urljoin(video_base_url, r"sq/\w+")
     )
 
     # When:
-    start_date = datetime.fromisoformat("2023-03-25T23:33:55+00:00")
-    end_date = datetime.fromisoformat("2023-03-25T23:33:57+00:00")
-
     playback = Playback(stream_url, fetcher=fake_info_fetcher)
     playback.fetch_and_set_essential()
-
-    rewind_interval = playback.locate_interval(start_date, end_date, itag="140")
-    _, *output_paths = actions.download.download_excerpt(
-        playback, rewind_interval, "itag eq 140", "itag eq 244", no_merge=True
+    output_result = actions.download.download_excerpt(
+        playback,
+        FakeRewindInterval(
+            FakeRewindMoment(7959120, cut_at=0.5),
+            FakeRewindMoment(7959121, cut_at=1.5),
+        ),
+        tmp_path / "output",
+        FakeStream(audio_base_url),
+        FakeStream(video_base_url),
+        need_cut=False,
     )
 
     # Then:
-    assert output_paths == [
+    assert output_result == (
         None,
+        tmp_path / "output.mkv",
         [
             run_temp_directory / "segments/7959120.i140.mp4",
             run_temp_directory / "segments/7959121.i140.mp4",
         ],
         [
             run_temp_directory / "segments/7959120.i244.webm",
             run_temp_directory / "segments/7959121.i244.webm",
         ],
-    ]
-
-    assert os.path.exists(run_temp_directory / "segments/7959120.i140.mp4")
-    assert os.path.exists(run_temp_directory / "segments/7959121.i140.mp4")
-    assert os.path.exists(run_temp_directory / "segments/7959120.i244.webm")
-    assert os.path.exists(run_temp_directory / "segments/7959121.i244.webm")
+    )
+    assert_approx_duration(output_result[1], 4)
```

### Comparing `ytpb-2024.3.9/tests/cli/conftest.py` & `ytpb-2024.4.12/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/cli/test_download_command.py` & `ytpb-2024.4.12/tests/cli/test_download_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1088,7 +1088,294 @@
                 "-vf",
                 "none",
                 "INVALID",
             ],
             catch_exceptions=False,
             standalone_mode=False,
         )
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_custom_aliases(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    custom_config = {
+        "general": {
+            "aliases": {
+                "custom-alias": "itag eq 140",
+            }
+        }
+    }
+    config_path = Path(os.getenv("XDG_CONFIG_HOME")) / "ytpb/config.toml"
+    config_path.parent.mkdir(parents=True)
+    with config_path.open("w") as f:
+        toml.dump(custom_config, f)
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--config",
+                config_path,
+                "download",
+                "--dry-run",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-vf",
+                "none",
+                "-af",
+                "@custom-alias",
+                stream_url,
+            ],
+        )
+
+    # Then:
+    assert result.exit_code == 0
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_dynamic_aliases(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--dry-run",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-vf",
+                "none",
+                "-af",
+                "@140",
+                stream_url,
+            ],
+        )
+
+    # Then:
+    assert result.exit_code == 0
+
+
+@pytest.mark.parametrize(
+    "audio_format,video_format",
+    [
+        ("itag eq 140", "itag eq 0"),
+        ("itag eq 0", "itag eq 244"),
+    ],
+)
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_empty_representations(
+    audio_format: str,
+    video_format: str,
+    ytpb_cli_invoke: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--dry-run",
+                "--no-cut",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                audio_format,
+                "-vf",
+                video_format,
+                stream_url,
+            ],
+        )
+
+    assert result.exit_code == 1
+    assert "error: No streams found matching" in result.output
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_quiet_option(
+    add_responses_callback_for_reference_base_url,
+    add_responses_callback_for_segment_urls,
+    ytpb_cli_invoke: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "--quiet",
+                "download",
+                "--dry-run",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                stream_url,
+            ],
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert result.output == ""
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_report_option(
+    add_responses_callback_for_reference_base_url,
+    add_responses_callback_for_segment_urls,
+    ytpb_cli_invoke: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "--report",
+                "download",
+                "--dry-run",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                stream_url,
+            ],
+        )
+
+    # Then:
+    assert result.exit_code == 0
+    assert os.path.exists(tmp_path / "ytpb-20230326-000000.log")
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_dump_base_urls_option(
+    add_responses_callback_for_segment_urls,
+    ytpb_cli_invoke: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    video_base_url: str,
+    tmp_path: Path,
+) -> None:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "itag eq 244",
+                "--dump-base-urls",
+                stream_url,
+            ],
+        )
+
+    assert result.exit_code == 0
+    assert result.output == f"{audio_base_url}\n{video_base_url}\n"
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_dump_segment_urls_option(
+    add_responses_callback_for_reference_base_url,
+    add_responses_callback_for_segment_urls,
+    ytpb_cli_invoke: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    video_base_url: str,
+    tmp_path: Path,
+) -> None:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+        urljoin(video_base_url, r"sq/\w+"),
+    )
+
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--interval",
+                "7959120/7959121",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "itag eq 244",
+                "--dump-segment-urls",
+                stream_url,
+            ],
+        )
+
+    assert result.exit_code == 0
+    assert result.output == (
+        f"{audio_base_url.rstrip('/')}/sq/[7959120-7959121]\n"
+        f"{video_base_url.rstrip('/')}/sq/[7959120-7959121]\n"
+    )
```

### Comparing `ytpb-2024.3.9/tests/cli/test_parameters.py` & `ytpb-2024.4.12/tests/cli/test_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,21 @@
             (datetime(2024, 1, 2, 10, 20, tzinfo=timezone.utc), "now"),
         ),
         ("PT30S/now", (timedelta(seconds=30), "now")),
         (
             "20240102T102000+00/..",
             (datetime(2024, 1, 2, 10, 20, tzinfo=timezone.utc), ".."),
         ),
+        (
+            "@1704190800/@1704190830.123",
+            (
+                datetime(2024, 1, 2, 10, 20, 0, tzinfo=timezone.utc),
+                datetime(2024, 1, 2, 10, 20, 30, 123000, tzinfo=timezone.utc),
+            ),
+        ),
     ],
 )
 def test_rewind_interval(value: str, expected):
     assert expected == RewindIntervalParamType().convert(value, None, None)
 
 
 @pytest.mark.parametrize(
```

### Comparing `ytpb-2024.3.9/tests/cli/capture/test_frame_command.py` & `ytpb-2024.4.12/tests/cli/capture/test_frame_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/cli/mpd/test_compose_command.py` & `ytpb-2024.4.12/tests/cli/mpd/test_compose_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/cli/mpd/test_refresh_command.py` & `ytpb-2024.4.12/tests/cli/mpd/test_refresh_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/info-1695928670.json` & `ytpb-2024.4.12/tests/data/info-1695928670.json`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/manifest-1695928670.mpd` & `ytpb-2024.4.12/tests/data/manifest-1695928670.mpd`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/webpage-1695928670.html` & `ytpb-2024.4.12/tests/data/webpage-1695928670.html`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out` & `ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.4.12/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out` & `ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out` & `ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out` & `ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_no_cut_option.out` & `ytpb-2024.4.12/tests/data/expected/test_no_cut_option.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/expected/test_no_merge_option.out` & `ytpb-2024.4.12/tests/data/expected/test_no_merge_option.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/gap-cases/gap-case-1-fixture.csv` & `ytpb-2024.4.12/tests/data/gap-cases/gap-case-1-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/gap-cases/gap-case-2-fixture.csv` & `ytpb-2024.4.12/tests/data/gap-cases/gap-case-2-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/gap-cases/gap-case-3-fixture.csv` & `ytpb-2024.4.12/tests/data/gap-cases/gap-case-3-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959120.i140.mp4` & `ytpb-2024.4.12/tests/data/segments/7959120.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959120.i244.webm` & `ytpb-2024.4.12/tests/data/segments/7959120.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959121.i140.mp4` & `ytpb-2024.4.12/tests/data/segments/7959121.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959121.i244.webm` & `ytpb-2024.4.12/tests/data/segments/7959121.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959122.i140.mp4` & `ytpb-2024.4.12/tests/data/segments/7959122.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959122.i244.webm` & `ytpb-2024.4.12/tests/data/segments/7959122.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959123.i140.mp4` & `ytpb-2024.4.12/tests/data/segments/7959123.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959123.i244.webm` & `ytpb-2024.4.12/tests/data/segments/7959123.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959203.i140.mp4` & `ytpb-2024.4.12/tests/data/segments/7959203.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/data/segments/7959203.i244.webm` & `ytpb-2024.4.12/tests/data/segments/7959203.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/utils/test_date.py` & `ytpb-2024.4.12/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/utils/test_path.py` & `ytpb-2024.4.12/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/tests/utils/test_url.py` & `ytpb-2024.4.12/tests/utils/test_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ytpb.exceptions import BadCommandArgument
+from ytpb.errors import BadCommandArgument
 from ytpb.utils.url import (
     extract_media_type_from_url,
     extract_parameter_from_url,
     normalize_video_url,
 )
```

### Comparing `ytpb-2024.3.9/.gitignore` & `ytpb-2024.4.12/.gitignore`

 * *Files identical despite different names*

### Comparing `ytpb-2024.3.9/LICENSE` & `ytpb-2024.4.12/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Maxim Stolyarchuk
+Copyright (c) 2024 Maxim Stolyarchuk
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ytpb-2024.3.9/README.rst` & `ytpb-2024.4.12/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Ytpb
 ####
 
 A playback for YouTube live streams.
 
-.. image:: https://img.shields.io/pypi/v/ytpb
+|PyPI| |Tests|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/ytpb
    :target: https://pypi.org/project/ytpb
    :alt: PyPI - Version
 
-.. image:: https://github.com/xymaxim/ytpb/actions/workflows/ci.yml/badge.svg
+.. |Tests| image:: https://github.com/xymaxim/ytpb/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/xymaxim/ytpb/actions/workflows/ci.yml
    :alt: Tests
 
-.. |sep| unicode:: 0xA0 0xA0
-   :trim:
-
 `Project page`_ |sep| `Documentation`_ |sep| `Contributing`_
 
+.. |sep| unicode:: 0xA0
+   :trim:
+
 .. _Project page: https://github.com/xymaxim/ytpb
 .. _Documentation: https://ytpb.readthedocs.io/
 .. _Contributing: https://ytpb.readthedocs.io/en/latest/contributing.html
 
 *Rewind to past moments in live streams and download or play excerpts*
 
 Ytpb is a playback for YouTube live streams written in Python. It lets you go
 back to past moments beyond the limits of the web player. You can keep selected
 moments by downloading excerpts or play them instantly in your video player via
 MPEG-DASH.
 
+Check out also `mpv-ytpb <https://github.com/xymaxim/mpv-ytpb>`__ to play and
+rewind live streams interactively without leaving a player.
+
 Features
 ********
 
 - Command line interface (CLI) and Python library
 - Rewind live streams far beyond the limits of the web player
-- *Download audio and/or video excerpts*
+- Download audio and/or video excerpts
 
   - Save excerpts in different available audio and video formats
   - Precisely cut to exact moments without slow re-encoding
 
-- *Play and rewind instantly via MPEG-DASH*
+- Play and rewind instantly via MPEG-DASH
 
   - Compose DASH manifests to play it in your favorite player
   - Transcode/download excerpts into local files with FFmpeg
 
-- Play and rewind reactively and interactively (mpv + `mpv-ytpb
-  <https://github.com/xymaxim/mpv-ytpb>`__)
 - Capture a single frame or create time-lapse images
-- Makes use of yt-dlp to reliably extract information about videos
+- Makes use of yt-dlp to reliably extract information about videos (optionally)
 
 Demo
 ****
 
 .. image:: https://asciinema.org/a/645203.svg
    :target: https://asciinema.org/a/645203
    :alt: Asciinema
@@ -63,25 +66,35 @@
 <https://pypa.github.io/pipx/>`_: ::
 
   $ pipx install ytpb
 
 Further reading
 ***************
 
-After installing, check out the `documentation`_. The `Why Ytpb?`_ section
-explains why the project exists. For main usage scenarios, see `Quick
-start`_. The `Command line application`_ section goes deeper into the
-usage. `Reference`_ provides some general aspects and terms. Have any issues,
-suggestions, or want to contribute code?  `Contributing`_ tells how to
+After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
+why the project exists. For main usage scenarios, see `Quick start`_. The
+`Command line application`_ page goes deeper into the usage. `Reference`_
+provides some general aspects and terms. `Cookbook`_ contains some useful
+examples. See `Changelog`_ for the history of releases. Have any issues,
+suggestions, or want to contribute code? `Contributing`_ tells how to
 participate in the project.
 
 .. _Why Ytpb?: https://ytpb.readthedocs.io/en/latest/why.html
 .. _Quick start: https://ytpb.readthedocs.io/en/latest/quick.html
 .. _Command line application: https://ytpb.readthedocs.io/en/latest/cli.html
 .. _Reference: https://ytpb.readthedocs.io/en/latest/reference.html
+.. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html
+.. _Changelog: https://ytpb.readthedocs.io/en/latest/changelog.html
+
+Similar projects
+****************
+
+- `Kethsar/ytarchive <https://github.com/Kethsar/ytarchive>`__ — archive streams from the start
+- `rytsikau/ee.Yrewind <https://github.com/rytsikau/ee.Yrewind>`__ — rewind and save streams
+- `yt-dlp/yt-dlp#6498 <https://github.com/yt-dlp/yt-dlp/pull/6498>`__ — brings rewind range selection to yt-dlp
 
 License
 *******
 
 Ytpb is licensed under the MIT license. See `LICENSE`_ for details.
 
 .. _LICENSE: https://github.com/xymaxim/ytpb/blob/main/LICENSE
```

### Comparing `ytpb-2024.3.9/pyproject.toml` & `ytpb-2024.4.12/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "hatchling", "hatch-vcs" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ytpb"
 description = "A playback for YouTube live streams"
 readme = "README.rst"
-version = "2024.3.9"
+version = "2024.4.12"
 authors = [ { name = "Maxim Stolyarchuk" } ]
 keywords = [ "youtube" ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
@@ -37,15 +37,15 @@
     "yt_dlp>=2023.12.30",
 ]
 
 [project.optional-dependencies]
 test = [
     "freezegun>=1.4.0",
     "pytest>=7.4.4",
-    "pytest-matcher>=1.6.0",
+    "pytest-matcher==2.0.1",
     "pytest-socket>=0.6.0",
     "responses>=0.24.1"
 ]
 dev = [
     "ytpb[test]",
     "pre-commit",
 ]
@@ -71,7 +71,8 @@
 ]
 
 [tool.black]
 line-length = 88
 
 [tool.pytest.ini_options]
 pm-patterns-base-dir = "tests/data/expected/"
+pm-pattern-file-fmt = "{fn}{callspec}"
```

### Comparing `ytpb-2024.3.9/PKG-INFO` & `ytpb-2024.4.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ytpb
-Version: 2024.3.9
+Version: 2024.4.12
 Summary: A playback for YouTube live streams
 Project-URL: Source, https://github.com/xymaxim/ytpb
 Project-URL: Documentation, https://ytpb.readthedocs.io
 Author: Maxim Stolyarchuk
 License: MIT License
         
-        Copyright (c) 2023 Maxim Stolyarchuk
+        Copyright (c) 2024 Maxim Stolyarchuk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -54,68 +54,71 @@
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: ytpb[test]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx-toolbox==3.5.0; extra == 'docs'
 Requires-Dist: sphinx==7.2.6; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: freezegun>=1.4.0; extra == 'test'
-Requires-Dist: pytest-matcher>=1.6.0; extra == 'test'
+Requires-Dist: pytest-matcher==2.0.1; extra == 'test'
 Requires-Dist: pytest-socket>=0.6.0; extra == 'test'
 Requires-Dist: pytest>=7.4.4; extra == 'test'
 Requires-Dist: responses>=0.24.1; extra == 'test'
 Description-Content-Type: text/x-rst
 
 Ytpb
 ####
 
 A playback for YouTube live streams.
 
-.. image:: https://img.shields.io/pypi/v/ytpb
+|PyPI| |Tests|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/ytpb
    :target: https://pypi.org/project/ytpb
    :alt: PyPI - Version
 
-.. image:: https://github.com/xymaxim/ytpb/actions/workflows/ci.yml/badge.svg
+.. |Tests| image:: https://github.com/xymaxim/ytpb/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/xymaxim/ytpb/actions/workflows/ci.yml
    :alt: Tests
 
-.. |sep| unicode:: 0xA0 0xA0
-   :trim:
-
 `Project page`_ |sep| `Documentation`_ |sep| `Contributing`_
 
+.. |sep| unicode:: 0xA0
+   :trim:
+
 .. _Project page: https://github.com/xymaxim/ytpb
 .. _Documentation: https://ytpb.readthedocs.io/
 .. _Contributing: https://ytpb.readthedocs.io/en/latest/contributing.html
 
 *Rewind to past moments in live streams and download or play excerpts*
 
 Ytpb is a playback for YouTube live streams written in Python. It lets you go
 back to past moments beyond the limits of the web player. You can keep selected
 moments by downloading excerpts or play them instantly in your video player via
 MPEG-DASH.
 
+Check out also `mpv-ytpb <https://github.com/xymaxim/mpv-ytpb>`__ to play and
+rewind live streams interactively without leaving a player.
+
 Features
 ********
 
 - Command line interface (CLI) and Python library
 - Rewind live streams far beyond the limits of the web player
-- *Download audio and/or video excerpts*
+- Download audio and/or video excerpts
 
   - Save excerpts in different available audio and video formats
   - Precisely cut to exact moments without slow re-encoding
 
-- *Play and rewind instantly via MPEG-DASH*
+- Play and rewind instantly via MPEG-DASH
 
   - Compose DASH manifests to play it in your favorite player
   - Transcode/download excerpts into local files with FFmpeg
 
-- Play and rewind reactively and interactively (mpv + `mpv-ytpb
-  <https://github.com/xymaxim/mpv-ytpb>`__)
 - Capture a single frame or create time-lapse images
-- Makes use of yt-dlp to reliably extract information about videos
+- Makes use of yt-dlp to reliably extract information about videos (optionally)
 
 Demo
 ****
 
 .. image:: https://asciinema.org/a/645203.svg
    :target: https://asciinema.org/a/645203
    :alt: Asciinema
@@ -129,25 +132,35 @@
 <https://pypa.github.io/pipx/>`_: ::
 
   $ pipx install ytpb
 
 Further reading
 ***************
 
-After installing, check out the `documentation`_. The `Why Ytpb?`_ section
-explains why the project exists. For main usage scenarios, see `Quick
-start`_. The `Command line application`_ section goes deeper into the
-usage. `Reference`_ provides some general aspects and terms. Have any issues,
-suggestions, or want to contribute code?  `Contributing`_ tells how to
+After installing, check out the `documentation`_. The `Why Ytpb?`_ page explains
+why the project exists. For main usage scenarios, see `Quick start`_. The
+`Command line application`_ page goes deeper into the usage. `Reference`_
+provides some general aspects and terms. `Cookbook`_ contains some useful
+examples. See `Changelog`_ for the history of releases. Have any issues,
+suggestions, or want to contribute code? `Contributing`_ tells how to
 participate in the project.
 
 .. _Why Ytpb?: https://ytpb.readthedocs.io/en/latest/why.html
 .. _Quick start: https://ytpb.readthedocs.io/en/latest/quick.html
 .. _Command line application: https://ytpb.readthedocs.io/en/latest/cli.html
 .. _Reference: https://ytpb.readthedocs.io/en/latest/reference.html
+.. _Cookbook: https://ytpb.readthedocs.io/en/latest/cookbook.html
+.. _Changelog: https://ytpb.readthedocs.io/en/latest/changelog.html
+
+Similar projects
+****************
+
+- `Kethsar/ytarchive <https://github.com/Kethsar/ytarchive>`__ — archive streams from the start
+- `rytsikau/ee.Yrewind <https://github.com/rytsikau/ee.Yrewind>`__ — rewind and save streams
+- `yt-dlp/yt-dlp#6498 <https://github.com/yt-dlp/yt-dlp/pull/6498>`__ — brings rewind range selection to yt-dlp
 
 License
 *******
 
 Ytpb is licensed under the MIT license. See `LICENSE`_ for details.
 
 .. _LICENSE: https://github.com/xymaxim/ytpb/blob/main/LICENSE
```

