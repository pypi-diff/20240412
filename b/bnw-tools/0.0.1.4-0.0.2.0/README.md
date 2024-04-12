# Comparing `tmp/bnw_tools-0.0.1.4.tar.gz` & `tmp/bnw_tools-0.0.2.0.tar.gz`

## Comparing `bnw_tools-0.0.1.4.tar` & `bnw_tools-0.0.2.0.tar`

### file list

```diff
@@ -1,86 +1,88 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/ORKG/__init__.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/ORKG/bibtex_to_csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/core/__init__.py
--rw-r--r--   0        0        0    19567 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/core/helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/__init__.py
--rw-r--r--   0        0        0    29781 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/extract_from_html.py
--rw-r--r--   0        0        0    14100 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/util_pdf.py
--rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/util_pytube.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/util_whisper.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/util_zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/nlp/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/nlp/my_stop_words.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/nlp/nlp.py
--rw-r--r--   0        0        0    50294 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/nlp/util_nlp.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/extract/nlp/util_stanza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/createVTT.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/graphvizify.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/util_networkx.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/util_wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/LaTeX/__init__.py
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/LaTeX/texify.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/__init__.py
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/mediaWiki.py
--rw-r--r--   0        0        0    12173 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/playlist2wiki-converter.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/wiki_bot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/wiki/__init__.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/wiki/barlow.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/wiki/main.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/__init__.py
--rw-r--r--   0        0        0    14902 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/bibtex_to_notes.py
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/nlped_whispered_folder.py
--rw-r--r--   0        0        0    13441 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/obsidize.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/transitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/__init__.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/k_score.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/similarity.py
--rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/spellcheck.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/util_wordfreq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/library/__init__.py
--rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/library/barlow.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/review/library/main.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/data/README.md
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/data/sample/de/BMZ_1_LegendariesundArtefakte.mp3.vtt
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/data/sample/en/Therapist_Reacts_to_Everything_Everywhere_All_at_Once.mp3.vtt
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/__init__.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/whispered_folder.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/README.md
--rw-r--r--   0        0        0    24292 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/SWARM-SLR_Stage_I.ipynb
--rw-r--r--   0        0        0    29215 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/SWARM-SLR_Stage_II.ipynb
--rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/SWARM-SLR_Stage_III.ipynb
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/SWARM-SLR_Stage_IV.ipynb
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/data/analysis555283.md
--rw-r--r--   0        0        0    39495 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/data/analysis628237.md
--rw-r--r--   0        0        0  1139782 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/data/evaluation.ipynb
--rw-r--r--   0        0        0   269307 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 1.jpg
--rw-r--r--   0        0        0   514898 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 2.jpg
--rw-r--r--   0        0        0   404234 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 3.jpg
--rw-r--r--   0        0        0   910897 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 4 - Details.jpg
--rw-r--r--   0        0        0   535633 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 4.jpg
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/bibtex_to_ORKG/Bibtex_to_ORKG.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/bibtex_to_ORKG/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/bibtex_to_ORKG/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/bibtex_to_ORKG/config sample.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/config/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/config/config.cfg
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/k_score/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/k_score/config sample.yml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/scripts/k_score/k_score_Zotero.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/tests/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/tests/test.ipynb
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/tests/test.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/tests/test_nlp.py
--rw-r--r--   0        0        0    32050 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/ORKG/RF_Map.json
--rw-r--r--   0        0        0   487111 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/bnw_tools/ORKG/ResearchFields.json
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/LICENSE
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/README.md
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 bnw_tools-0.0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/ORKG/__init__.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/ORKG/bibtex_to_csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/core/__init__.py
+-rw-r--r--   0        0        0    19567 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/core/helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/__init__.py
+-rw-r--r--   0        0        0    29781 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/extract_from_html.py
+-rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/util_pdf.py
+-rw-r--r--   0        0        0    11616 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/util_pytube.py
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/util_whisper.py
+-rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/util_zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/nlp/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/nlp/my_stop_words.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/nlp/nlp.py
+-rw-r--r--   0        0        0    74257 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/nlp/util_nlp.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/extract/nlp/util_stanza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/createVTT.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/graphvizify.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/util_networkx.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/util_pyplot.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/util_wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/LaTeX/__init__.py
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/LaTeX/texify.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/__init__.py
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/mediaWiki.py
+-rw-r--r--   0        0        0    12173 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/playlist2wiki-converter.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/wiki_bot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/wiki/__init__.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/wiki/barlow.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/wiki/main.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/__init__.py
+-rw-r--r--   0        0        0    14902 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/bibtex_to_notes.py
+-rw-r--r--   0        0        0    22917 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/nlped_whispered_folder.py
+-rw-r--r--   0        0        0    13441 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/obsidize.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/transitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/__init__.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/k_score.py
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/similarity.py
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/spellcheck.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/util_wordfreq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/library/__init__.py
+-rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/library/barlow.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/review/library/main.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/data/README.md
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/data/sample/de/BMZ_1_LegendariesundArtefakte.mp3.vtt
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/data/sample/en/Therapist_Reacts_to_Everything_Everywhere_All_at_Once.mp3.vtt
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/__init__.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/whispered_folder.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/README.md
+-rw-r--r--   0        0        0    24292 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/SWARM-SLR_Stage_I.ipynb
+-rw-r--r--   0        0        0    29775 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/SWARM-SLR_Stage_II.ipynb
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/SWARM-SLR_Stage_III.ipynb
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/SWARM-SLR_Stage_IV.ipynb
+-rw-r--r--   0        0        0    11723 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/data/analysis555283.md
+-rw-r--r--   0        0        0    41799 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/data/analysis628237.md
+-rw-r--r--   0        0        0  5031063 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/data/evaluation.ipynb
+-rw-r--r--   0        0        0   269307 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 1.jpg
+-rw-r--r--   0        0        0   514898 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 2.jpg
+-rw-r--r--   0        0        0   404234 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 3.jpg
+-rw-r--r--   0        0        0   910897 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 4 - Details.jpg
+-rw-r--r--   0        0        0   535633 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 4.jpg
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/bibtex_to_ORKG/Bibtex_to_ORKG.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/bibtex_to_ORKG/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/bibtex_to_ORKG/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/bibtex_to_ORKG/config sample.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/config/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/config/config.cfg
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/k_score/README.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/k_score/config sample.yml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/scripts/k_score/k_score_Zotero.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/tests/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/tests/test.ipynb
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/tests/test.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/tests/test_nlp.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/tests/test_viz.py
+-rw-r--r--   0        0        0    32050 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/ORKG/RF_Map.json
+-rw-r--r--   0        0        0   487111 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/bnw_tools/ORKG/ResearchFields.json
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/LICENSE
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/README.md
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 bnw_tools-0.0.2.0/PKG-INFO
```

### Comparing `bnw_tools-0.0.1.4/bnw_tools/ORKG/bibtex_to_csv.py` & `bnw_tools-0.0.2.0/bnw_tools/ORKG/bibtex_to_csv.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/core/helper.py` & `bnw_tools-0.0.2.0/bnw_tools/core/helper.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/extract/extract_from_html.py` & `bnw_tools-0.0.2.0/bnw_tools/extract/extract_from_html.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/extract/util_pdf.py` & `bnw_tools-0.0.2.0/bnw_tools/extract/util_pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,21 +122,30 @@
             return None
 
     def get_dict(self):
         return {
             'text': self.text,
         }
 
-    def get(self, attr: str):
+    def get(self, attr: str, None_if_not_found=False):
         if attr == "dict":
             return self.get_dict()
         elif attr == "title":
             return os.path.splitext(os.path.basename(self.path))[0]
         elif hasattr(self, attr):
             return getattr(self, attr)
+        elif self.metadata and attr in self.metadata:
+            return self.metadata[attr]
+        None_if_not_found = ["year", "month", "day", "author"]
+        if attr in None_if_not_found:
+            return None
+        if None_if_not_found:
+            return None
+        else:
+            raise ValueError(f"Invalid parameter '{attr}'")
 
     def save(self, force=False):
         if self.text:
             if force or not os.path.exists(self.text_path):
                 with open(self.get_text_path(), "w", encoding="utf-8") as f:
                     f.write(self.text)
```

### Comparing `bnw_tools-0.0.1.4/bnw_tools/extract/util_pytube.py` & `bnw_tools-0.0.2.0/bnw_tools/extract/util_pytube.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/extract/util_whisper.py` & `bnw_tools-0.0.2.0/bnw_tools/extract/util_whisper.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/extract/nlp/nlp.py` & `bnw_tools-0.0.2.0/bnw_tools/extract/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/extract/nlp/util_nlp.py` & `bnw_tools-0.0.2.0/bnw_tools/extract/nlp/util_nlp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import argparse
 import os
 import json
 import spacy
 from spacy.cli.download import download
 from flair.data import Sentence, Token
 from flair.models import SequenceTagger
@@ -12,37 +13,42 @@
 import numpy as np
 import math
 import re
 import urllib.request
 from mutagen.easyid3 import EasyID3
 import importlib
 from termcolor import colored
+from pathlib import Path
+import warnings
+import shutil
+
 
 from ...review import similarity
 from ...core import helper
 from ...publish import util_wordcloud
+from ...publish import util_pyplot
 from ...publish.Obsidian import nlped_whispered_folder
 from ...extract import util_pdf
 from ...extract import util_zotero
 from ...extract import util_pytube
 from ...extract.nlp.my_stop_words import MY_STOP_WORDS
 
 
 def get_json_data(path):
     if os.path.exists(path) and os.path.splitext(path)[1] == ".json":
         try:
-            with open(path, 'r', encoding='utf8') as f:
+            with open(path, "r", encoding="utf8") as f:
                 return json.load(f)
         except Exception as e:
             print(f"Could not load {path}: {str(e)}")
             return None
 
 
 def dump_json(path, output_dict):
-    with open(path, 'w', encoding='utf-8') as output_file:
+    with open(path, "w", encoding="utf-8") as output_file:
         json.dump(output_dict, output_file, indent=4, ensure_ascii=False)
 
 
 def data_to_attributes(instance, data, do_named_entities=True):
     if not isinstance(data, dict):
         return None
     words = None
@@ -64,42 +70,51 @@
                 setattr(instance, key, value)
     if words or stops:
         setattr(instance, "bag_of_words", BagOfWords(words=words, stops=stops))
 
 
 class NLPTools:
     naming_conventions = {
-        "en": {"spacy": "en_core_web_sm", "SequenceTagger": "ner", "WordEmbeddings": "glove"},
-        "de": {"spacy": "de_core_news_sm", "SequenceTagger": "flair/ner-german", "WordEmbeddings": "de"},
+        "en": {
+            "spacy": "en_core_web_sm",
+            "SequenceTagger": "ner",
+            "WordEmbeddings": "glove",
+        },
+        "de": {
+            "spacy": "de_core_news_sm",
+            "SequenceTagger": "flair/ner-german",
+            "WordEmbeddings": "de",
+        },
         # add more languages and their naming conventions as needed
     }
 
     def __init__(self):
         self.STOP_WORDS = {}
         self.spacy = {}
         self.WordEmbeddings = {}
         self.DocumentPoolEmbeddings = {}
         self.SequenceTagger = {}
 
     def get_STOP_WORDS(self, language):
         if language in self.STOP_WORDS:
             return self.STOP_WORDS[language]
-        stop_words_module = importlib.import_module(
-            f"spacy.lang.{language}.stop_words")
+        stop_words_module = importlib.import_module(f"spacy.lang.{language}.stop_words")
         self.STOP_WORDS[language] = MY_STOP_WORDS[language].union(
-            stop_words_module.STOP_WORDS)
+            stop_words_module.STOP_WORDS
+        )
         # TODO: Idea to allways include the english stop-words, since sometimes other languages use english as well
         return self.STOP_WORDS[language]
 
     def get_spacy(self, language):
         if language in self.spacy:
             return self.spacy[language]
         try:
-            nlp_model = self.naming_conventions.get(
-                language, {}).get("spacy", f"{language}_core_news_sm")
+            nlp_model = self.naming_conventions.get(language, {}).get(
+                "spacy", f"{language}_core_news_sm"
+            )
             try:
                 self.spacy[language] = spacy.load(nlp_model)
             except OSError:
                 download(model=nlp_model)
                 self.spacy[language] = spacy.load(nlp_model)
 
             stop_words = self.get_STOP_WORDS(language)
@@ -116,51 +131,60 @@
             print(f"Error loading spacy: {str(e)}")
             return None
 
     def get_WordEmbeddings(self, language):
         if language in self.WordEmbeddings:
             return self.WordEmbeddings[language]
         try:
-            word_embeddings_model = self.naming_conventions.get(
-                language, {}).get("WordEmbeddings", language)
-            self.WordEmbeddings[language] = WordEmbeddings(
-                word_embeddings_model)
+            word_embeddings_model = self.naming_conventions.get(language, {}).get(
+                "WordEmbeddings", language
+            )
+            self.WordEmbeddings[language] = WordEmbeddings(word_embeddings_model)
             return self.WordEmbeddings[language]
         except Exception as e:
             print(f"Error loading WordEmbeddings for {language}: {str(e)}")
             return None
 
     def get_DocumentPoolEmbeddings(self, language):
         if language in self.DocumentPoolEmbeddings:
             return self.DocumentPoolEmbeddings[language]
         try:
             self.DocumentPoolEmbeddings[language] = DocumentPoolEmbeddings(
-                [self.get_WordEmbeddings(language)])
+                [self.get_WordEmbeddings(language)]
+            )
             return self.DocumentPoolEmbeddings[language]
         except Exception as e:
-            print(
-                f"Error loading DocumentPoolEmbeddings for {language}: {str(e)}")
+            print(f"Error loading DocumentPoolEmbeddings for {language}: {str(e)}")
             return None
 
     def get_SequenceTagger(self, language):
         if language in self.SequenceTagger:
             return self.SequenceTagger[language]
         try:
-            sequence_tagger_model = self.naming_conventions.get(
-                language, {}).get("SequenceTagger", f"flair/ner-{language.lower()}")
-            self.SequenceTagger[language] = SequenceTagger.load(
-                sequence_tagger_model)
+            sequence_tagger_model = self.naming_conventions.get(language, {}).get(
+                "SequenceTagger", f"flair/ner-{language.lower()}"
+            )
+            self.SequenceTagger[language] = SequenceTagger.load(sequence_tagger_model)
             return self.SequenceTagger[language]
         except Exception as e:
             print(f"Error loading SequenceTagger for {language}: {str(e)}")
             return None
 
 
 class BagOfWords:
-    def __init__(self, words: Dict[str, int] = None, stops: Dict[str, int] = None, tf: Dict[str, float] = None, tf_idf: Dict[str, float] = None, text=None, nlptools=None, language=None):
+    def __init__(
+        self,
+        words: Dict[str, int] = None,
+        stops: Dict[str, int] = None,
+        tf: Dict[str, float] = None,
+        tf_idf: Dict[str, float] = None,
+        text=None,
+        nlptools=None,
+        language=None,
+    ):
         self.words = words or defaultdict(int)
         self.stops = stops or defaultdict(int)
         self.tf = tf or {}
         self.tf_idf = tf_idf or {}
 
         if self.words and language:
             self.update_stops(language, nlptools)
@@ -174,16 +198,17 @@
     def calc_tf(self):
         total = sum(self.words.values())
         self.tf = {word: count / total for word, count in self.words.items()}
         self.sort(do_words=False, do_tf=True)
         return self.tf
 
     def calc_tf_idf(self, idf: Dict[str, float]):
-        self.tf_idf = {word: frequency * idf[word]
-                       for word, frequency in self.get_tf().items()}
+        self.tf_idf = {
+            word: frequency * idf[word] for word, frequency in self.get_tf().items()
+        }
         self.sort(do_words=False, do_tf_idf=True)
         return self.tf_idf
 
     def get_tf(self):
         if not self.tf:
             return self.calc_tf()
         return self.tf
@@ -195,29 +220,31 @@
 
     def sort(self, do_words=True, do_tf=False, do_tf_idf=False):
         if do_words:
             if len(self.words):
                 # self.words = {k: v for k, v in sorted(self.words.items(),
                 #   key=lambda x: x[1], reverse=True)}
                 self.words = dict(
-                    sorted(self.words.items(), key=lambda x: (-x[1], x[0])))
+                    sorted(self.words.items(), key=lambda x: (-x[1], x[0]))
+                )
 
             if len(self.stops):
                 # self.stops = {k: v for k, v in sorted(self.stops.items(),
                 #   key=lambda x: x[1], reverse=True)}
                 self.stops = dict(
-                    sorted(self.stops.items(), key=lambda x: (-x[1], x[0])))
+                    sorted(self.stops.items(), key=lambda x: (-x[1], x[0]))
+                )
         if do_tf:
             if len(self.tf):
-                self.tf = dict(
-                    sorted(self.tf.items(), key=lambda x: (-x[1], x[0])))
+                self.tf = dict(sorted(self.tf.items(), key=lambda x: (-x[1], x[0])))
         if do_tf_idf:
             if len(self.tf_idf):
                 self.tf_idf = dict(
-                    sorted(self.tf_idf.items(), key=lambda x: (-x[1], x[0])))
+                    sorted(self.tf_idf.items(), key=lambda x: (-x[1], x[0]))
+                )
 
     def get(self):
         return self.words
 
     def add(self, other):
         for word, count in other.words.items():
             if word in self.words:
@@ -237,15 +264,15 @@
         self.sort()
 
     def update_stops(self, language, nlptools: NLPTools = None):
         def special_stop_rules(key, vocab):
             if len(key) < 2:
                 return True
             if not key.isalpha() and key not in vocab:
-                if len(re.findall('[a-zA-Z\d]', key)) < 2:
+                if len(re.findall("[a-zA-Z\d]", key)) < 2:
                     return True
             # way to harsh, not every word is in (that language's) vocab
             # if key not in vocab:
             #     return True
             return False
 
         nlptools = nlptools or NLPTools()
@@ -267,33 +294,45 @@
         self.sort()
         return len(to_bag) + len(to_stop)
 
     # bag_of_words = {k: v for k, v in sorted(bag_of_words.items(), key=lambda item: item[1], reverse=True)}
 
 
 class NamedEntities:
-    def __init__(self, entities: Dict[str, List[str]] = None, text=None,):
+    def __init__(
+        self,
+        entities: Dict[str, List[str]] = None,
+        text=None,
+    ):
         self.entities = entities or {}
 
         if text:
             self.from_nlp_text(text)
 
     def __len__(self):
         return len(self.entities)
 
     def sort(self):
         if not self.entities:
             return
         val = list(self.entities.values())[0]
         if isinstance(val, list):
-            self.entities = {k: v for k, v in sorted(
-                self.entities.items(), key=lambda item: len(item[1]), reverse=True)}
+            self.entities = {
+                k: v
+                for k, v in sorted(
+                    self.entities.items(), key=lambda item: len(item[1]), reverse=True
+                )
+            }
         if isinstance(val, int):
-            self.entities = {k: v for k, v in sorted(
-                self.entities.items(), key=lambda item: item[1], reverse=True)}
+            self.entities = {
+                k: v
+                for k, v in sorted(
+                    self.entities.items(), key=lambda item: item[1], reverse=True
+                )
+            }
 
     def add(self, other, path=None):
         for key, value in other.entities.items():
             if path:
                 path = os.path.basename(path)
                 value = [f"{path}: {x}" for x in value]
             if key in self.entities:
@@ -319,22 +358,23 @@
     def get(self):
         return self.entities
 
     def get_frequencies(self):
         return {k: len(v) for k, v in self.entities.items()}
 
     def from_nlp_text(self, sentence):
-        for entity in sentence.get_spans('ner'):
+        for entity in sentence.get_spans("ner"):
             rep = f"Span[{entity.start_position}:{entity.end_position}]: {entity.tag} ({round(entity.score, 2)})"
             if entity.text in self.entities:
                 self.entities[entity.text].append(rep)
             else:
                 self.entities[entity.text] = [rep]
         self.sort()
 
+
 # File classes
 
 
 class Transcript:
     def __init__(self, path=None, text=None, segments=None, language=None):
         """
         A class representing a transcript.
@@ -368,15 +408,15 @@
             candidates = ["\n\n", "\n", ".", "!", "?", ",", " "]
 
             begin = 0
             end = jump
             while end < len(text):
                 next_stop = 0
                 for fi in candidates:
-                    pos = text[begin + jump:end + jump].find(fi)
+                    pos = text[begin + jump : end + jump].find(fi)
                     if pos >= 0 and pos <= jump * 2:
                         next_stop = pos
                         break
                 end = begin + jump + next_stop + 1
                 pieces.append(text[begin:end])
                 begin = end
             pieces.append(text[begin:])
@@ -408,19 +448,15 @@
         if not self.iscomplete() and path:
             self.from_file(path)
         else:
             print("missing path to load transcript")
         return self.iscomplete()
 
     def get_dict(self):
-        return {
-            'text': self.text,
-            'segments': self.segments,
-            'language': self.language
-        }
+        return {"text": self.text, "segments": self.segments, "language": self.language}
 
     def get(self, attr: str):
         if attr == "dict":
             return self.get_dict()
         elif hasattr(self, attr):
             return getattr(self, attr)
 
@@ -480,15 +516,23 @@
             return self.metadata
 
     def get_dict(self):
         return self.metadata.items()
 
 
 class NLPFeatureAnalysis:
-    def __init__(self, path=None, bag_of_words=None, named_entities=None, nlptools: NLPTools = None, transcript: Transcript = None, do_named_entities=True):
+    def __init__(
+        self,
+        path=None,
+        bag_of_words=None,
+        named_entities=None,
+        nlptools: NLPTools = None,
+        transcript: Transcript = None,
+        do_named_entities=True,
+    ):
         """
         A class representing NLP feature analysis.
 
         Args:
             bag_of_words (dict): A dictionary representing bag of words.
             named_entities (list): A list of named entities.
             tf_idf (dict): A dictionary representing tf-idf values.
@@ -500,18 +544,17 @@
         """
         self.path: str = path
         self.bag_of_words: BagOfWords = bag_of_words or BagOfWords()
         self.named_entities: NamedEntities = named_entities or NamedEntities()
         if path:
             self.from_file(path, do_named_entities=do_named_entities)
         if transcript and transcript.text:
-            self.complete(transcript, nlptools,
-                          do_named_entities=do_named_entities)
+            self.complete(transcript, nlptools, do_named_entities=do_named_entities)
 
-    def from_file(self, path: str = None, do_named_entities: bool=True) -> None:
+    def from_file(self, path: str = None, do_named_entities: bool = True) -> None:
         """
         Load transcript from the given path.
 
         Args:
             path (str): Path to the transcript file.
         """
         if path is None:
@@ -522,15 +565,20 @@
         data_to_attributes(self, data, do_named_entities)
 
     def iscomplete(self) -> bool:
         if self.bag_of_words.get() and self.named_entities.get():
             return True
         return False
 
-    def complete(self, transcript: Transcript, nlptools: NLPTools = None, do_named_entities: bool = True) -> bool:
+    def complete(
+        self,
+        transcript: Transcript,
+        nlptools: NLPTools = None,
+        do_named_entities: bool = True,
+    ) -> bool:
         """Processes a JSON file containing text and returns a Document object.
 
         Args:
             json_path (str): The path to the input JSON file.
 
         Returns:
             Document: The Document object representing the input text.
@@ -547,75 +595,82 @@
         if do_named_entities:
             self.fill_named_entities(transcript, nlptools)
         self.fill_bag_of_words(transcript, nlptools)
 
         # create a Document object and return it
         entity_change = self.named_entities.update()
         BagOfWords_change = self.bag_of_words.update_stops(
-            transcript.language, nlptools)
+            transcript.language, nlptools
+        )
         if changes or BagOfWords_change or entity_change:
             self.save(should_have_nen=do_named_entities)
         return self.iscomplete()
 
-    def fill_bag_of_words(self, transcript: Transcript, nlptools: NLPTools = None) -> Union[BagOfWords, bool]:
+    def fill_bag_of_words(
+        self, transcript: Transcript, nlptools: NLPTools = None
+    ) -> Union[BagOfWords, bool]:
         if not self.bag_of_words.get():
             nlptools = nlptools or NLPTools()
             if not transcript.iscomplete():
                 print("You need a text in a known language to complete " + self.path)
                 return False
             # create a Sentence object from the text
 
             bow = BagOfWords()
 
             for text in transcript.get_manageable_text_sizes():
                 doc = nlptools.get_spacy(transcript.language)(text)
 
-                bow.add(BagOfWords(
-                    text=doc, nlptools=nlptools, language=transcript.language))
+                bow.add(
+                    BagOfWords(
+                        text=doc, nlptools=nlptools, language=transcript.language
+                    )
+                )
 
             # get the bag of words and non-stop-words
             self.bag_of_words = bow
             return self.bag_of_words
         else:
             self.bag_of_words.update_stops(
-                language=transcript.language, nlptools=nlptools)
+                language=transcript.language, nlptools=nlptools
+            )
             return False
 
-    def fill_named_entities(self, transcript: Transcript, nlptools: NLPTools = None) -> Union[NamedEntities, bool]:
+    def fill_named_entities(
+        self, transcript: Transcript, nlptools: NLPTools = None
+    ) -> Union[NamedEntities, bool]:
         if not self.named_entities.get():
             nlptools = nlptools or NLPTools()
             if not transcript.iscomplete():
                 print("You need a text in a known language to complete " + self.path)
                 return False
 
             nen = NamedEntities()
 
             for text in transcript.get_manageable_text_sizes():
                 sentence = Sentence(text)
 
-                nlptools.get_DocumentPoolEmbeddings(
-                    transcript.language).embed(sentence)
+                nlptools.get_DocumentPoolEmbeddings(transcript.language).embed(sentence)
 
                 # get the named entities
                 # todo: Worked
-                nlptools.get_SequenceTagger(
-                    transcript.language).predict(sentence)
+                nlptools.get_SequenceTagger(transcript.language).predict(sentence)
                 nen.add(NamedEntities(text=sentence))
             self.named_entities = nen
             return self.named_entities
         else:
             return False
 
     def get_dict(self) -> dict:
         # Todo: consider writing 'tf' to file as well.
         return {
-            'bag_of_words': self.bag_of_words.words,
-            'tf_idf': self.bag_of_words.get_tf_idf(),
-            'named_entities': self.named_entities.get(),
-            'stop_words': self.bag_of_words.stops
+            "bag_of_words": self.bag_of_words.words,
+            "tf_idf": self.bag_of_words.get_tf_idf(),
+            "named_entities": self.named_entities.get(),
+            "stop_words": self.bag_of_words.stops,
         }
 
     def save(self, path: Optional[str] = None, should_have_nen: bool = True) -> None:
         if path is None:
             path = self.path
         output_dict = self.get_dict()
 
@@ -623,15 +678,21 @@
             print(f"No {colored('words', 'red')} in file: " + path)
         elif len(self.named_entities) == 0 and should_have_nen:
             print(f"No {colored('named entities', 'red')} in file: " + path)
         dump_json(path, output_dict)
 
 
 class ResearchQuestion:
-    def __init__(self, title: str = None, path: str = None, keywords: dict[str, int] = None, queries: dict[str, str] = None):
+    def __init__(
+        self,
+        title: str = None,
+        path: str = None,
+        keywords: dict[str, int] = None,
+        queries: dict[str, str] = None,
+    ):
         self.path: str = None
         self.title: str = title
         self.keywords: dict[str, int] = keywords
         self.queries: dict[str, str] = queries
         self.tag: str = None
 
     def from_file(self, path: str = None):
@@ -645,16 +706,20 @@
                 return None
         while "\n" in lines:
             lines.remove("\n")
         while "```\n" in lines:
             lines.remove("```\n")
         self.title = lines.pop(0).strip().split("::")[1].strip()
 
-        self.tag = helper.get_clean_title(
-            self.title, obsidian=True).replace(" ", "_")
+        # self.tag = helper.get_clean_title(
+        #     self.title, obsidian=True).replace(" ", "_")
+        self.tag = Path(path).stem
+        for char in [" ", ":", ",", ";", "."]:
+            self.tag = self.tag.replace(char, "_")
+
         tag_found = False
 
         self.keywords = {}
         self.queries = {}
         in_keywords = False
         in_queries = False
         current_name = ""
@@ -684,57 +749,67 @@
             elif in_keywords:
                 if line.startswith("### "):
 
                     if current_name:
                         self.keywords[current_name] = current_group
                         current_name = ""
                         current_group = {}
-                    current_name = line.strip().split(
-                        "::")[0].split("### ")[1].lower()
+                    current_name = line.strip().split("::")[0].split("### ")[1].lower()
                 else:
                     keyword, weight = line.strip().split("::")
-                    current_group[keyword.lower().strip()] = int(
-                        weight.strip())
+                    current_group[keyword.lower().strip()] = int(weight.strip())
             elif in_queries:
                 if line.startswith("### "):
                     if current_name:
                         self.queries[current_name] = current_query
                         current_name = ""
                         current_query = ""
                     current_name = line.strip().split("::")[0].split("### ")[1]
                 else:
                     current_query += line.strip()
 
         if not tag_found:
             with open(path, "a", encoding="utf-8") as f:
-                f.write(f"""
+                f.write(
+                    f"""
+# Results
+```dataview
+Table
+notes_for_{self.tag} as "Notes for {self.tag}"
+from "03_notes"
+where notes_for_{self.tag}
+SORT notes_for_{self.tag} DESC
+LIMIT 100
+```
+    
 # Files
 ```dataview
 Table
 {self.tag} as "Fit"
 from "03_notes"
 SORT {self.tag} DESC
 LIMIT 100
 ```
-""")
+"""
+                )
         if current_name:
             self.queries[current_name] = current_query
             current_name = ""
             current_query = ""
         # creation successful
         return True
 
     def get_total_note(research_questions):
         pieces = []
         tags = []
         for i, key in enumerate(research_questions):
             tags.append(key.tag)
             pieces.append(f"{key.tag} as RQ{i+1}")
         rq_sum = " + ".join(tags)
-        pieces.append(f"round({rq_sum},3) as \"Sum\"")
+        pieces.append(f'round({rq_sum},3) as "Sum"')
         total_cols = ", ".join(pieces)
         total_sort = f"SORT {rq_sum} desc"
 
         note = f"""## Research Questions
 ```dataview
 Table
 RQ as "RQ"
@@ -764,15 +839,15 @@
 
 ## Best Candidates
 ```dataview
 Table
 {total_cols}
 From "03_notes"
 {total_sort}
-WHERE contains(file.tasks.completed,false)
+WHERE !contains(file.tasks.completed,true)
 LIMIT 100
 ```
 """
         return note
 
 
 class MediaResource:
@@ -803,14 +878,37 @@
         self.nlp_analysis: NLPFeatureAnalysis = None
 
         self.obsidian_note: nlped_whispered_folder.ObsidianNote = None
 
         self.basename: str = None
         self.original_name: str = None
 
+        self.keyword_scores: Dict[str, float] = {}
+
+        self.visualizations: List[str] = []
+
+    def is_duplicate(self, mr: MediaResource):
+        common_fields = ["basename", "original_name"]
+        pdf_fields = ["title", "author", "year"]
+
+        common_equals = sum(mr.get(field) == self.get(field) for field in common_fields)
+        pdf_equals = sum(
+            mr.pdf.get(field, None_if_not_found=True)
+            == self.pdf.get(field, None_if_not_found=True)
+            for field in pdf_fields
+        )
+
+        if common_equals >= 2:
+            return True
+        elif pdf_equals >= 3:
+            return True
+        elif common_equals >= 1 + pdf_equals >= 2:
+            return True
+        return False
+
     def add_audio(self, path: str = None, file: Audio = None):
         if file:
             self.audio_file = file
         elif path:
             self.audio_file = Audio(path)
         self.search_original_name()
 
@@ -829,41 +927,62 @@
     def add_pdf(self, path: str = None, file: util_pdf.PDFDocument = None):
         if file:
             self.pdf = file
         elif path:
             self.pdf = util_pdf.PDFDocument(path)
         self.search_original_name()
 
-    def add_NLPFeatureAnalysis(self, path: str = None, file: NLPFeatureAnalysis = None, nlptools: NLPTools = None, do_named_entities=True):
+    def add_NLPFeatureAnalysis(
+        self,
+        path: str = None,
+        file: NLPFeatureAnalysis = None,
+        nlptools: NLPTools = None,
+        do_named_entities=True,
+    ):
         if file:
             self.nlp_analysis = file
         elif path:
             if self.pdf:
                 text_container = self.pdf
             elif self.transcript:
                 text_container = self.transcript
             else:
                 print(
-                    f"Lacking text basis, can't add NLPFeatureAnalysis for file {self.basename}")
+                    f"Lacking text basis, can't add NLPFeatureAnalysis for file {self.basename}"
+                )
                 return None
             self.nlp_analysis = NLPFeatureAnalysis(
-                path, nlptools=nlptools, transcript=text_container, do_named_entities=do_named_entities)
+                path,
+                nlptools=nlptools,
+                transcript=text_container,
+                do_named_entities=do_named_entities,
+            )
 
     def add_image(self, path: str = None):
         if path:
             self.image = path
 
-    def add_obsidian_note(self, path: str = None, file: nlped_whispered_folder.ObsidianNote = None):
+    def add_obsidian_note(
+        self, path: str = None, file: nlped_whispered_folder.ObsidianNote = None
+    ):
         if file:
             self.obsidian_note = file
         elif path:
             self.obsidian_note = nlped_whispered_folder.ObsidianNote(path)
         else:
             self.obsidian_note = nlped_whispered_folder.ObsidianNote()
 
+    def add_visualizations(self, path: str = None, files: List[str] = None):
+        if files:
+            for file in files:
+                if file not in self.visualizations:
+                    self.visualizations.append(file)
+        elif path:
+            self.visualizations = os.listdir(path)
+
     def search_original_name(self, force=False):
         if self.original_name and not force:
             return self.original_name
         candidates = []
         if self.pdf:
             candidates.append(self.pdf.get("title"))
         if self.audio_file:
@@ -883,62 +1002,68 @@
 
         Returns:
             Document: The Document object representing the input text.
         """
         nlptools = nlptools or NLPTools()
 
         self.transcript.complete()
-        self.nlp_analysis.complete(
-            nlptools, do_named_entities=do_named_entities)
+        self.nlp_analysis.complete(nlptools, do_named_entities=do_named_entities)
 
     def get_dict(self):
         # TODO: check if this throws errors, else revert
         # return dict(self.audio_file.get_dict()) | self.transcript.get_dict() | self.nlp_analysis.get_dict()
         result_dict = {}
         for key in self.__dict__:
             attr = getattr(self, key)
             try:
                 # todo: remove all get_dicts
-                if hasattr(attr, 'get_dict'):
+                if hasattr(attr, "get_dict"):
                     result_dict |= attr.get_dict()
-                elif hasattr(attr, 'get') and callable(attr.get):
-                    result_dict |= attr.get('dict')
+                elif hasattr(attr, "get") and callable(attr.get):
+                    result_dict |= attr.get("dict")
             except:
                 continue
         return result_dict
 
     def get(self, parameter):
-        if parameter == 'text':
+        if parameter == "text":
             if self.pdf is not None:
                 return self.pdf.get("text")
             elif self.transcript is not None:
                 return self.transcript.get("text")
             else:
                 return None
-        elif parameter == 'url':
+        elif parameter == "url":
             return self.url
-        elif parameter == 'dict':
+        elif parameter == "dict":
             return self.get_dict()
-        elif parameter == 'basename':
+        elif parameter == "basename":
             if self.basename:
                 return self.basename
             else:
                 path = None
                 if self.nlp_analysis:
                     path = self.nlp_analysis.path
                 elif self.pdf:
-                    path = self.info.pdf
+                    path = self.pdf.path
                 elif self.audio_file:
-                    path = self.info.audio_file
+                    # todo: check if this was ment to be called "self.audio_file.path"
+                    path = self.audio_file.path
                 elif self.info:
                     path = self.info.path
-                self.basename = os.path.splitext(os.path.basename(path))[0]
-                return self.basename
-        elif parameter == 'type':
+                if path:
+                    self.basename = os.path.splitext(os.path.basename(path))[0]
+                    return self.basename
+                else:
+                    warnings.warn("Could not build basename")
+                    return None
+        elif parameter == "type":
             return self.__class__.__name__
+        elif hasattr(self, parameter):
+            return getattr(self, parameter)
         else:
             raise ValueError(f"Invalid parameter '{parameter}'")
 
 
 class Subfolder:
     folder_formats = {
         "blank": [],
@@ -951,59 +1076,80 @@
         # 01 Extract
         "01_whisper": [".json"],  # todo: vtt
         # 02 Analyse
         # todo: renaming from _processed
         "02_nlp": [".json", "_processed.json"],
         # 03 Publish
         "03_notes": [".md"],
+        "03_visualizations": [".png"],
+        "03_visualizations": [".png"],
     }
 
-    def __init__(self, folder_path, type="blank"):
+    def __init__(self, folder_path, type="blank", zotero=False):
         self.path = os.path.join(folder_path, type)
         os.makedirs(self.path, exist_ok=True)
         self.type = type
-        self.endings = self.folder_formats[type]
-        if type == "00_PDFs":
+        if type in self.folder_formats:
+            self.endings = self.folder_formats[type]
+        # TODO: Need to put the util_zotero call in its own function to not clog the init
+        if type == "00_PDFs" and zotero:
             self.BibResources = util_zotero.BibResources(folder_path)
         if type == "00_RQs":
             self.research_questions: list[ResearchQuestion] = None
             self.get("research_questions")
-            
-    def lookfor(self, filename):
+
+    def lookfor(self, filename, allow_list=False):
         path_found = []
         path_suggested = []
         basename = os.path.basename(filename)
         stem = os.path.splitext(basename)[0]
         for ending in self.endings:
             path = os.path.join(self.path, stem + ending)
             if os.path.exists(path):
                 path_found.append(path)
             else:
                 path_suggested.append(path)
-        best_fit = path_found[0] if path_found else path_suggested[0] if path_suggested else None
+        if allow_list:
+            best_fit = (
+                path_found if path_found else path_suggested if path_suggested else None
+            )
+        else:
+            best_fit = (
+                path_found[0]
+                if path_found
+                else path_suggested[0] if path_suggested else None
+            )
         return best_fit
         # return found, not_found
 
     def get(self, arg: str = None):
         if arg.lower() == "rqs" or arg.lower() == "research_questions":
             if self.research_questions:
                 return self.research_questions
             files = self.get("files")
             if not files:
                 return None
             else:
+                non_RQ = []
                 if not self.research_questions:
                     self.research_questions: list[ResearchQuestion] = []
                 for file in self.get("files"):
                     rq = ResearchQuestion()
                     if rq.from_file(os.path.join(self.path, file)):
                         self.research_questions.append(rq)
-                with open(os.path.join(self.path, file), "w", encoding="utf8") as f:
-                    f.write(ResearchQuestion.get_total_note(
-                        self.research_questions))
+                    else:
+                        non_RQ.append(file)
+                for file in non_RQ:
+                    if file.startswith("Total"):
+                        with open(
+                            os.path.join(self.path, file), "w", encoding="utf8"
+                        ) as f:
+                            f.write(
+                                ResearchQuestion.get_total_note(self.research_questions)
+                            )
                 return self.research_questions
         elif arg == "files":
             return os.listdir(self.path)
 
 
 class Folder:
     """A class to represent a folder containing multiple Document instances.
@@ -1023,39 +1169,155 @@
         populate() -> None: Populates the stop_words, bag_of_words and named_entities attributes by aggregating
             the counts and occurrences of the respective attributes in all documents.
         save(output_path: str) -> None: Saves the Folder instance to a JSON file at the specified output path.
     """
 
     # Define paths as a class-level property
 
-    def __init__(self, folder_path, nlptools=None, language=None, media_resources: List[MediaResource] = None):
+    def __init__(
+        self,
+        folder_path,
+        nlptools=None,
+        language=None,
+        media_resources: List[MediaResource] = None,
+        publish=False,
+        config=None,
+        select=False,
+        zotero=None,
+    ):
         self.path = folder_path
-
+        if not zotero:
+            if nlptools:
+                zotero = True
+            elif select:
+                zotero = False
+            else:
+                zotero = True
         self.audio = Subfolder(folder_path, "00_audios")
-        self.pdf = Subfolder(folder_path, "00_PDFs")
+        self.pdf = Subfolder(folder_path, "00_PDFs", zotero=zotero)
         self.image = Subfolder(folder_path, "00_images")
         self.infos = Subfolder(folder_path, "00_infos")
         self.rq = Subfolder(folder_path, "00_RQs")
         self.whisper = Subfolder(folder_path, "01_whisper")
         self.analyse = Subfolder(folder_path, "02_nlp")
         self.notes = Subfolder(folder_path, "03_notes")
+        self.visualizations = Subfolder(folder_path, "03_visualizations")
+        self.selected = Subfolder(folder_path, "04_selected")
 
         self.media_resources: List[MediaResource] = media_resources or []
         self.added_docs = set()
         # todo: if media_resources, maybe fill set?
 
         self.bag_of_words = BagOfWords()
         self.named_entities = NamedEntities()
 
         self.df = defaultdict(int)
         self.idf = defaultdict(int)
         self.sim_matrix = None
-        
+        self.statdict = {}
+
+        self.config = config
+
         if nlptools:
             self.process(nlptools)
+        if publish:
+            self.publish()
+        if select:
+            self.select()
+
+    def select(self):
+        files = self.notes.get("files")
+        if not files:
+            return None
+        relevant = {}
+        copy = {}
+        scores = {}
+        for file in files:
+            if file.endswith(".md"):
+                with open(
+                    os.path.join(self.notes.path, file), "r", encoding="utf8"
+                ) as f:
+                    lines = f.readlines()
+                if "review_score:: \n" in lines:
+                    continue
+                else:
+                    rq_zone = False
+                    for line in lines:
+                        if "review_score::" in line:
+                            line = line.replace("review_score::", "")
+                            score = line.strip()
+                            if score not in relevant:
+                                relevant[score] = []
+                            relevant[score].append(file)
+                        if "![[" in line:
+                            filepath = line.split("![[")[1].split("]]")[0]
+                            if file not in copy:
+                                copy[file] = []
+                            copy[file].append(os.path.join(self.path, filepath))
+                        if "%%RQ Scores" in line:
+                            rq_zone = True
+                        elif rq_zone and line.startswith("RQ"):
+                            if file not in scores:
+                                scores[file] = {}
+                            rq, score = line.split("::")
+                            scores[file][rq] = float(score)
+                        elif rq_zone and line.startswith("%%"):
+                            rq_zone = False
+
+        if "select" in self.config:
+            to_be_selected = self.config["select"]
+            if to_be_selected:
+                for i in range(len(to_be_selected)):
+                    to_be_selected.append(str(to_be_selected[i]))
+                to_be_deleted = []
+                for score in relevant:
+                    if score not in to_be_selected:
+                        to_be_deleted.append(score)
+                for deletion in to_be_deleted:
+                    del relevant[deletion]
+
+        # sort the relevant dict by float value of score
+        relevant = dict(
+            sorted(relevant.items(), key=lambda item: float(item[0]), reverse=True)
+        )
+
+        for score, files in relevant.items():
+            score_path = os.path.join(self.selected.path, score)
+            if not os.path.exists(score_path):
+                os.makedirs(score_path)
+            for file in files:
+                for c in copy[file]:
+                    # copy every c into the selected folder
+                    src = c
+                    # Catch pdf and visualizations
+                    filename = file.replace(".md", "")
+                    pieces = c.split(filename)
+                    if len(pieces) < 2:
+                        continue
+                    dst = os.path.join(score_path, filename + pieces[1])
+                    if not os.path.exists(dst):
+                        shutil.copy(src, dst)
+
+        # create a csv in the selected folder with the selected files and their scores
+        with open(
+            os.path.join(self.selected.path, "selected.csv"), "w", encoding="utf8"
+        ) as f:
+            header = "file;score"
+            if scores:
+                header += ";"
+                header += ";".join(list(scores[list(scores.keys())[0]].keys()))
+            f.write(header + "\n")
+            for score, files in relevant.items():
+                for file in files:
+                    filename = file.replace(".md", "")
+                    f.write(f"{filename};{score}")
+                    if scores:
+                        for rq, score in scores[file].items():
+                            f.write(f";{score}")
+                    f.write("\n")
 
     def get_image(self):
         candidates = []
         if self.image and self.image.path:
             candidates = os.listdir(self.image.path)
         if candidates:
             return os.path.join(self.image.path, candidates[0])
@@ -1064,158 +1326,258 @@
             if mr.image:
                 if os.path.exists(mr.image):
                     return mr.image
             if mr.info:
                 if mr.info.thumbnail_urls:
                     # handle "if not mr.image"
                     file_path = mr.image
-                    urllib.request.urlretrieve(
-                        mr.info.thumbnail_urls[-1], file_path)
+                    urllib.request.urlretrieve(mr.info.thumbnail_urls[-1], file_path)
 
                     return file_path
 
     def calc_sim_matrix(self):
         # bag_sim_mat = similarity.compute_similarity_matrix(
         #     [doc.bag_of_words.get() for doc in self.documents], self.bag_of_words.get())
 
         bag_sim_mat = similarity.compute_similarity_matrix(
-            [mr.nlp_analysis.bag_of_words.tf_idf for mr in self.media_resources], self.bag_of_words.get())
+            [mr.nlp_analysis.bag_of_words.tf_idf for mr in self.media_resources],
+            self.bag_of_words.get(),
+        )
 
         # todo: option to eventually weigh named entities differently
         # nam_sim_mat = similarity.create_word_vectors(
         #     [doc.named_entities.get() for doc in self.documents], self.named_entities)
         self.sim_matrix = bag_sim_mat
         similarity.print_sim_matrix(self.sim_matrix, self.path)
         for mr in self.media_resources:
             should_have_nen = True
             if not mr.transcript:
                 should_have_nen = False
             mr.nlp_analysis.save(should_have_nen=should_have_nen)
 
     def calc_rq_sim(self):
+        """
+        The highest similarity to a research question belongs to the document that uses the most relevant keywords the most.
+        """
         if not self.rq.research_questions:
             return None
 
         def get_min_match(words: list[str], match_dict: dict[str, float]):
             found = []
             for word in words:
                 if "-" in word:
                     value = 0
                     if word in mr.nlp_analysis.bag_of_words.tf:
                         value += mr.nlp_analysis.bag_of_words.tf[word]
-                    synonyms = [
-                        word.replace("-", " "),
-                        word.replace("-", "")
-                    ]
+                    synonyms = [word.replace("-", " "), word.replace("-", "")]
                     for syn in synonyms:
                         if syn in mr.nlp_analysis.bag_of_words.tf:
                             value += mr.nlp_analysis.bag_of_words.tf[syn]
                     splits = word.split("-")
                     value += get_min_match(splits, match_dict)
                     if value:
                         found.append(value)
                     else:
                         found = None
                         break
                 else:
                     if word in mr.nlp_analysis.bag_of_words.tf:
-                        found.append(
-                            mr.nlp_analysis.bag_of_words.tf[word])
+                        found.append(mr.nlp_analysis.bag_of_words.tf[word])
                     else:
                         found = None
                         break
             if found:
                 return min(found)
             else:
                 return 0
 
+        ## Which words are actually relevant?
         relevant_keys = set()
         for rq in self.rq.get("rqs"):
             for group in rq.keywords.values():
                 # todo: see
                 relevant_keys.update(group)
                 # for keyword in group:
                 # relevant_keys.update(keyword.split(" "))
-        reduced_research_questions = []
-        for rq in self.rq.get("rqs"):
-            res = {}
-            ungrouped = {}
-            for group in rq.keywords.values():
-                ungrouped.update(group)
-            for key in relevant_keys:
-                value = 0
-                if key in ungrouped:
-                    # todo: utilize weight
-                    value = ungrouped[key]
-                    # value = 1
-                res[key] = value
-            reduced_research_questions.append(res)
 
+        ## Reduce the media resources to the relevant words
         reduced_media_resources = []
+
+        # to set the order and get indices
+        relevant_keys = list(relevant_keys)
         for mr in self.media_resources:
             res = {}
             for key in relevant_keys:
                 # Todo: synonyms / related words
                 key = key.lower()
                 if key in mr.nlp_analysis.bag_of_words.tf:
                     res[key] = mr.nlp_analysis.bag_of_words.tf[key]
                 else:
                     if " " in key:
                         subwords = key.split(" ")
                     else:
                         subwords = [key]
-                    res[key] = get_min_match(
-                        subwords, mr.nlp_analysis.bag_of_words.tf)
+                    res[key] = get_min_match(subwords, mr.nlp_analysis.bag_of_words.tf)
             reduced_media_resources.append(res)
+
+        normalised_media_resources = similarity.normalize(
+            reduced_media_resources, config=self.config
+        )
+
+        for idx, mr in enumerate(self.media_resources):
+            mr.keyword_scores = dict(
+                zip(relevant_keys, normalised_media_resources[idx])
+            )
+
+        rq_scores = []
+        for rq in self.rq.get("rqs"):
+            all_group_scores = []
+            # TODO: allow other weights for groups
+            group_weights = []
+            for group in rq.keywords.values():
+                group_weights.append(1)
+            group_weights = similarity.normalize(
+                group_weights, log_level=False, sqrt_level=False
+            )
+
+            for idx, group in enumerate(rq.keywords.values()):
+                group_weight = group_weights[idx]
+                keyword_indices = []
+                weights = []
+                for keyword, weight in group.items():
+                    keyword_indices.append(relevant_keys.index(keyword))
+                    weights.append(weight)
+
+                # reduce normalised_media_resources to only the keywords existing in this group
+                # media_resource_group_frequencies
+                current_group_media_resources = normalised_media_resources[
+                    :, keyword_indices
+                ]
+                # media_resource_group_frequencies_weighed
+                current_group_media_resources = np.array(
+                    current_group_media_resources
+                ) * np.array(weights)
+
+                # media_resource_group_scores
+                current_group_scores = current_group_media_resources.sum(axis=1)
+
+                # media_resource_group_scores_normalized
+                current_group_scores = similarity.normalize(
+                    current_group_scores, log_level=False, sqrt_level=False
+                )
+
+                current_group_scores = current_group_scores * group_weight
+                all_group_scores.append(current_group_scores)
+            all_group_scores = np.array(all_group_scores)
+
+            # TODO: see if there are other approaches.
+
+            # group_prodct this penalizes the those scoring 0 in any group by making the whole score 0
+            group_prodct = False
+
+            # group_sum does not reward a good spread of groups if one group scored very high
+            group_sum = False
+
+            # group_sum_average
+            group_average = True
+
+            if self.config:
+                group_prodct = self.config.get("group_prodct", group_prodct)
+                group_sum = self.config.get("group_sum", group_sum)
+                group_average = self.config.get("group_average", group_average)
+
+            if group_prodct:
+                all_group_scores = np.prod(all_group_scores, axis=0)
+            if group_sum:
+                all_group_scores = np.sum(all_group_scores, axis=0)
+            if group_average:
+                all_group_scores = np.mean(all_group_scores, axis=0)
+
+            all_group_scores = similarity.normalize(
+                all_group_scores, log_level=False, sqrt_level=False
+            )
+
+            rq_scores.append(all_group_scores)
+        rq_scores = np.array(rq_scores).transpose()
+        self.rq_sim_mat = rq_scores
+
+        # for keyword, weight in group.items():
+        #     relevant_keys.add(keyword)
+
+        #     res = {}
+        #     ungrouped = {}
+        #     groups.append(list(rq.keywords.values()))
+        #     for group in rq.keywords.values():
+        #         ungrouped.update(group)
+        #     for key in relevant_keys:
+        #         value = 0
+        #         if key in ungrouped:
+        #             # todo: utilize weight
+        #             value = ungrouped[key]
+        #             # value = 1
+        #         res[key] = value
+        #     reduced_research_questions.append(res)
+
         # TODO: calculate once per group, then again over all groups
-        self.rq_sim_mat = similarity.compute_weighed_similarity(
-            reduced_media_resources, reduced_research_questions)
 
-        similarity.print_rq([mr.get("basename") for mr in self.media_resources], self.rq_sim_mat,
-                            self.path, filename="RQ", additional_info=self.rq.research_questions)
+        # self.rq_sim_mat = similarity.compute_weighed_similarity(
+        #     reduced_media_resources, reduced_research_questions, config=self.config)
+
+        similarity.print_rq(
+            [mr.get("basename") for mr in self.media_resources],
+            self.rq_sim_mat,
+            self.path,
+            filename="RQ",
+            additional_info=self.rq.research_questions,
+        )
 
     def add_media_resource(self, media_resource: MediaResource):
         if media_resource:
             self.media_resources.append(media_resource)
 
     def calc_idf(self):
-        self.idf = {word: math.log(len(self.media_resources) / (frequency))
-                    for word, frequency in self.df.items()}
+        self.idf = {
+            word: math.log(len(self.media_resources) / (frequency))
+            for word, frequency in self.df.items()
+        }
         return self.idf
 
     def get_idf(self):
         if self.idf:
             return self.idf
         return self.calc_idf()
 
     def populate(self):
         for mr in self.media_resources:
             if mr.nlp_analysis.path not in self.added_docs:
                 self.bag_of_words.add(mr.nlp_analysis.bag_of_words)
                 self.named_entities.add(
-                    mr.nlp_analysis.named_entities, mr.nlp_analysis.path)
+                    mr.nlp_analysis.named_entities, mr.nlp_analysis.path
+                )
                 self.added_docs.add(mr.nlp_analysis.path)
                 # document frequency
                 for word in mr.nlp_analysis.bag_of_words.get().keys():
                     self.df[word] += 1
 
         for mr in self.media_resources:
             mr.nlp_analysis.bag_of_words.calc_tf_idf(self.get_idf())
         # self.bag_of_words.update_stops()
         self.named_entities.update()
         self.bag_of_words.sort()
         self.named_entities.sort()
 
     def get_dict(self):
         return {
-            'bag_of_words': self.bag_of_words.words,
-            'idf': self.idf,
-            'named_entities': self.named_entities.get(),
-            'stop_words': self.bag_of_words.stops,
-            'documents': [os.path.basename(mr.nlp_analysis.path) for mr in self.media_resources]
+            "bag_of_words": self.bag_of_words.words,
+            "idf": self.idf,
+            "named_entities": self.named_entities.get(),
+            "stop_words": self.bag_of_words.stops,
+            "documents": [
+                os.path.basename(mr.nlp_analysis.path) for mr in self.media_resources
+            ],
         }
 
     def save(self, output_path=None, do_named_entities=True):
         if output_path is None:
             output_path = os.path.join(self.path, "rep_Folder")
         output_dict = self.get_dict()
 
@@ -1227,108 +1589,397 @@
             print("Error on Folder: " + output_path)
         dump_json(output_path, output_dict)
 
     def save_summary(self, output_path, do_named_entities=True):
         if not len(self.media_resources):
             print(f"No Documents found in folder: {output_path}")
             return None
-        threshold = min(
-            int(list(self.bag_of_words.get().values())[0] / 100), 10)
+        threshold = min(int(list(self.bag_of_words.get().values())[0] / 100), 10)
         threshold = max(threshold, 3)
         output_dict = {
-            'bag_of_words': {k: v for k, v in list(self.bag_of_words.words.items())[:1000] if v >= threshold},
-            'stop_words': {k: v for k, v in list(self.bag_of_words.stops.items())[:1000] if v >= threshold},
-            'named_entities': {k: len(v) for k, v in list(self.named_entities.get().items())[:1000] if len(v) >= threshold},
-            'documents': [os.path.basename(doc.nlp_analysis.path) for doc in self.media_resources]
+            "bag_of_words": {
+                k: v
+                for k, v in list(self.bag_of_words.words.items())[:1000]
+                if v >= threshold
+            },
+            "stop_words": {
+                k: v
+                for k, v in list(self.bag_of_words.stops.items())[:1000]
+                if v >= threshold
+            },
+            "named_entities": {
+                k: len(v)
+                for k, v in list(self.named_entities.get().items())[:1000]
+                if len(v) >= threshold
+            },
+            "documents": [
+                os.path.basename(doc.nlp_analysis.path) for doc in self.media_resources
+            ],
         }
 
         relevant = [len(self.media_resources), len(self.bag_of_words)]
         if do_named_entities:
             relevant.append(len(self.named_entities))
 
         if any(count == 0 for count in relevant):
             print("Error on Folder: " + output_path)
         dump_json(output_path, output_dict)
 
     def process(self, nlptools=None):
         if nlptools is None:
             nlptools = NLPTools()
-        audios = [os.path.join(self.audio.path, f)
-                  for f in os.listdir(self.audio.path)]
+        audios = [os.path.join(self.audio.path, f) for f in os.listdir(self.audio.path)]
         pdfs = self.pdf.BibResources.pdfs
         do_named_entities = False
         if audios:
             do_named_entities = True
             for idx, path in enumerate(audios):
                 mr = MediaResource()
                 mr.add_audio(path=path)
                 mr.add_transcript(path=self.whisper.lookfor(path))
                 mr.add_info(path=self.infos.lookfor(path))
                 if not mr.transcript.text:
-                    mr.transcript.text, mr.transcript.language = mr.info.get_transcript()
+                    mr.transcript.text, mr.transcript.language = (
+                        mr.info.get_transcript()
+                    )
                 mr.add_image(path=self.image.lookfor(path))
                 # todo: eventually load thumbnails here
                 mr.add_NLPFeatureAnalysis(
-                    path=self.analyse.lookfor(path), nlptools=nlptools)
+                    path=self.analyse.lookfor(path), nlptools=nlptools
+                )
 
                 mr.add_obsidian_note(path=self.notes.lookfor(path))
+                mr.add_visualizations(path=self.notes.lookfor(path))
                 self.add_media_resource(mr)
         if pdfs:
             for idx, path in enumerate(pdfs):
                 mr = MediaResource()
                 mr.add_pdf(path=path)
-                mr.pdf.add_metadata(self.pdf.BibResources.get_metadata(path))
-                mr.add_NLPFeatureAnalysis(path=self.analyse.lookfor(
-                    path), nlptools=nlptools, do_named_entities=False)
+                metadata = self.pdf.BibResources.get_metadata(path)
+                if metadata == -1:
+                    # There was an error with the file
+                    # continue
+                    # TODO: Decide what is required here. For now, adding it without metadata.
+                    mr.pdf.add_metadata(None)
+                else:
+                    mr.pdf.add_metadata(metadata)
+                # # check if the file has already been added
+                # checking here is to intensive
+                mr.add_NLPFeatureAnalysis(
+                    path=self.analyse.lookfor(path),
+                    nlptools=nlptools,
+                    do_named_entities=False,
+                )
                 mr.add_obsidian_note(path=self.notes.lookfor(path))
                 self.add_media_resource(mr)
                 if idx % 100 == 99:
                     print(f"{idx+1} out of {len(pdfs)} added.")
             print(f"All {len(pdfs)} PDFs added.")
 
+        # check if the file has already been added
+        duplicates = set()
+        for x, mir in enumerate(self.media_resources):
+            if x in duplicates:
+                continue
+            for y in range(x + 1, len(self.media_resources)):
+                if y in duplicates:
+                    continue
+                if mir.is_duplicate(self.media_resources[y]):
+                    print(
+                        f"Duplicates: {mir.basename}\n{mir.pdf.path}\n{self.media_resources[y].pdf.path}"
+                    )
+                    duplicates.add(y)
+        # sort duplicates from highest to lowest
+        duplicates = sorted(duplicates, reverse=True)
+        for idx in duplicates:
+            self.media_resources.pop(idx)
+        print(f"Removed {len(duplicates)} duplicates.")
+
         if self.media_resources:
             self.populate()
             self.calc_sim_matrix()
             self.calc_rq_sim()
-            self.save(os.path.join(self.path, "00_Folder.json"),
-                      do_named_entities=do_named_entities)
-            self.save_summary(os.path.join(
-                self.path, "00_Folder_summary.json"), do_named_entities=do_named_entities)
+            self.save(
+                os.path.join(self.path, "00_Folder.json"),
+                do_named_entities=do_named_entities,
+            )
+            self.save_summary(
+                os.path.join(self.path, "00_Folder_summary.json"),
+                do_named_entities=do_named_entities,
+            )
+            self.analyse_metadata()
+
+    def analyse_metadata(self):
+
+        class Stats:
+            # Reward many high score media resources
+            # Factor of 1 just adds the scores, 2 squares them, 3 cubes them, etc.
+            # A higher factor rewards high scores more
+            RANK_FACTOR = 2
+
+            # Skip these in printing
+            skip = ["rq_scores", "rq_score_list", "RANK_FACTOR", "skip"]
+
+            def __init__(self, folder: Folder = None, mr_id: int = None):
+                self.media_names = {}
+                # create np array for rq scores with no length
+                # create np array for rq scores with no length
+                self.rq_score_list = []
+                self.rq_scores = np.array([[]])
+                self.rq_rank = 0
+                self.media_num = 0
+                if folder and mr_id:
+                    self.update(folder, mr_id)
+
+            # TypeError: Object of type Stats is not JSON serializable
+            def to_dict(self):
+                res_dict = {}
+                for attr in dir(self):
+                    if not attr.startswith("__") and not callable(getattr(self, attr)):
+                        # TypeError: Object of type ndarray is not JSON serializable
+                        if attr in Stats.skip:
+                            continue
+                        value = getattr(self, attr)
+                        if isinstance(value, np.ndarray):
+                            res_dict[attr] = value.tolist()
+                        else:
+                            res_dict[attr] = value
+                return res_dict
+
+            def to_csv(self, separator=";"):
+                sub_separtor = ","
+                if separator == ",":
+                    sub_separtor = ";"
+                res_list = []
+                for attr in dir(self):
+                    if not attr.startswith("__") and not callable(getattr(self, attr)):
+                        if attr in Stats.skip:
+                            continue
+                        value = getattr(self, attr)
+                        if isinstance(value, np.ndarray):
+                            value = value.tolist()
+                        if isinstance(value, list):
+                            # res_list.append("'" + f"' {sub_separtor} '".join(value) + "'")
+                            res_list.append(
+                                "'"
+                                + f"' {sub_separtor} '".join(str(v) for v in value)
+                                + "'"
+                            )
+                            # res_list.append(str(value))
+                        elif isinstance(value, dict):
+                            if attr == "media_names":
+                                res_list.append(
+                                    "'"
+                                    + f"' {sub_separtor} '".join(
+                                        [str(v) for v in value.values()]
+                                    )
+                                    + "'"
+                                )
+                            else:
+                                res_list.append(json.dumps(value))
+                        else:
+                            res_list.append(str(value))
+                # convert to string and join with separator
+                return separator.join(res_list)
+
+            def __str__(self):
+                return str(self.to_dict())
+
+            def update(self, folder: Folder, mr_id: int):
+                self.media_names[mr_id] = folder.media_resources[mr_id].basename
+                # update the self.rq_scores np array with the new rq scores
+                self.media_num += 1
+                # update the self.rq_scores np array with the new rq scores
+
+                self.rq_score_list.append(folder.rq_sim_mat[mr_id])
+
+                ## Reward many high score media resources
+                new_mean = np.mean(folder.rq_sim_mat[mr_id])
+                self.rq_rank += new_mean**Stats.RANK_FACTOR
+
+            def calc(self):
+                # calculate the self.rq_averages over all rq_scores columns
+                self.rq_scores = np.array(self.rq_score_list)
+
+                # calculate the self.rq_averages over all rq_scores columns
+                self.rq_averages = np.mean(self.rq_scores, axis=0)
+                self.rq_sums = np.sum(self.rq_scores, axis=0)
+                self.rq_maxs = np.max(self.rq_scores, axis=0)
+                self.rq_mins = np.min(self.rq_scores, axis=0)
+                self.rq_stds = np.std(self.rq_scores, axis=0)
+                self.rq_medians = np.median(self.rq_scores, axis=0)
+                self.rq_variances = np.var(self.rq_scores, axis=0)
+
+                # calculate the single values for averages, sumes, etc.
+                self.rq_average = np.mean(self.rq_averages)
+                self.rq_sum = np.sum(self.rq_sums)
+                self.rq_max = np.max(self.rq_maxs)
+                self.rq_min = np.min(self.rq_mins)
+                # # Those don't make sense:
+                # self.rq_std = np.std(self.rq_stds)
+                # self.rq_median = np.median(self.rq_medians)
+                # self.rq_variance = np.var(self.rq_variances)
+
+                # calculate a "rank" score that rewards high averages and quantities of media resources
+
+        # # TODO: Why does this not work?
+        # statdict:Dict[str,Dict[str,Stats]] = {
+        statdict = {
+            "year": defaultdict(Stats),
+            "author": defaultdict(Stats),
+            "journal": defaultdict(Stats),
+            # "language" : defaultdict(Stats),
+            "ENTRYTYPE": defaultdict(Stats),
+        }
+        synoyms = {
+            "author": ["authors"],
+            "journal": ["journaltitle", "venue", "booktitle"],
+        }
+        not_found = {}
+        for key in statdict.keys():
+            not_found[key] = set()
+        for mr_id, mr in enumerate(self.media_resources):
+            # Create a list of all authors / venues / years and their statistics
+            if mr.pdf and mr.pdf.metadata:
+                for key, stats in statdict.items():
+                    stat_key = mr.pdf.metadata.get(key)
+                    if not stat_key:
+                        for syn in synoyms.get(key, []):
+                            stat_key = mr.pdf.metadata.get(syn)
+                            if stat_key:
+                                break
+                    if stat_key:
+                        if key == "author":
+                            authors = stat_key.split(" and ")
+                            for author in authors:
+                                stats[author].update(self, mr_id)
+                        else:
+                            stats[stat_key].update(self, mr_id)
+                    else:
+                        not_found[key].update(list(mr.pdf.metadata.keys()))
+
+        for key, stats in statdict.items():
+            for name, stat in stats.items():
+                stat.calc()
+
+        for key, values in not_found.items():
+            ignore = list(statdict.keys())
+            ignore = ignore + ["file", "url", "urldate", "ID", "title"]
+            for ignore_key in ignore:
+                if ignore_key in values:
+                    values.remove(ignore_key)
+            print(f"No {colored(key, 'red')} in metadata, but found:\n{values}")
+
+        for key, stats in statdict.items():
+            # sort stats by rq_rank
+            statdict[key] = dict(
+                sorted(stats.items(), key=lambda x: x[1].rq_rank, reverse=True)
+            )
+
+        # print statdict to json and csv
+        for category, entry_dict in statdict.items():
+            res_dict = {}
+            for name, stat in entry_dict.items():
+                res_dict[name] = stat.to_dict()
+            dump_json(
+                os.path.join(self.path, f"metadata_stats_{category}.json"), res_dict
+            )
+            for key in res_dict.keys():
+                res_dict[key] = res_dict[key]["rq_rank"]
+            # TODO: add a more readable barchart feature here
+            # ylabel = "RQ rank"
+            # title = f"{category} ranked by RQ rank"
+            # util_pyplot.dict_to_barchart(res_dict, os.path.join(self.path, f"metadata_stats_{category}.png"), ylabel=ylabel, title=title)
+
+        for category, entry_dict in statdict.items():
+            first_stat = list(entry_dict.values())[0]
+            headers = [
+                attr
+                for attr in dir(first_stat)
+                if not attr.startswith("__") and not callable(getattr(first_stat, attr))
+            ]
+            for header in Stats.skip:
+                if header in headers:
+                    headers.remove(header)
+            headers = ["name"] + headers
+
+            with open(
+                os.path.join(self.path, f"metadata_stats_{category}.csv"),
+                "w",
+                encoding="utf8",
+            ) as f:
+                # Write headers to file
+                f.write(";".join(headers) + "\n")
+
+                for name, stat in entry_dict.items():
+                    # Write data to file
+                    f.write(f"{name};{stat.to_csv()}\n")
+
+        # print the top 10 of each category to console, along with their rank, number of media resources and average rq score
+        for key, stats in statdict.items():
+            print(f"{key}:\t name,\t rq_rank,\t # of media_resources,\t rq_average")
+            for i, (name, stat) in enumerate(list(stats.items())[:10]):
+                print(
+                    f"{i+1}. {name}:\t {round(stat.rq_rank, 3)} \t- {len(stat.media_names)} \t- {round(stat.rq_average,3)}"
+                )
+
+        self.statdict = statdict
+
+    def publish(self):
+        if self.media_resources:
+            try:
+                self.wordcloud()
+            except:
+                print("Publish to Wordcloud failed")
+            # Obsidian
+            try:
+                nlped_whispered_folder.folder(self, force=True)
+            except:
+                raise
+                print("Publish to Obsidian failed")
 
     # Wordcloud
     def wordcloud(self):
         util_wordcloud.generate_wordcloud(
-            self.bag_of_words.get(), os.path.join(self.path, "00_bag_of_words"))
+            self.bag_of_words.get(), os.path.join(self.path, "00_bag_of_words")
+        )
         util_wordcloud.generate_wordcloud(
-            self.named_entities.get_frequencies(), os.path.join(self.path, "00_named_entities"))
-        found, not_found = self.image.lookfor("Folder")
-        if found:
-            mask = found[0]
-            not_found = not_found[0]
-        mask = util_wordcloud.generate_mask()
-        util_wordcloud.generate_wordcloud_mask(
-            self.bag_of_words.get(), mask, os.path.join(self.path, "00_bag_of_words_mask"))
-        util_wordcloud.generate_wordcloud_mask(
-            self.named_entities.get_frequencies(), mask, os.path.join(self.path, "00_named_entities"))
+            self.named_entities.get_frequencies(),
+            os.path.join(self.path, "00_named_entities"),
+        )
+        ## TODO: Rework masks at a later point
+        # if self.image:
+        #     found, not_found = self.image.lookfor("Folder")
+        #     if found:
+        #         mask = found[0]
+        #         not_found = not_found[0]
+        #         mask = util_wordcloud.generate_mask()
+        #         util_wordcloud.generate_wordcloud_mask(
+        #             self.bag_of_words.get(), mask, os.path.join(self.path, "00_bag_of_words_mask"))
+        #         util_wordcloud.generate_wordcloud_mask(
+        #             self.named_entities.get_frequencies(), mask, os.path.join(self.path, "00_named_entities"))
 
 
 def main(input_path, output_path=None):
     if os.path.isfile(input_path):
         # process single file
         return MediaResource(paths={"transcript_file_path": input_path})
     elif os.path.isdir(input_path):
         # process all files in directory
         return Folder(input_path)
     else:
-        print('Invalid input path.')
+        print("Invalid input path.")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     parser = argparse.ArgumentParser(
-        description='Process JSON files and extract document features.')
-    parser.add_argument(
-        'input', help='path to JSON file or folder of JSON files')
+        description="Process JSON files and extract document features."
+    )
+    parser.add_argument("input", help="path to JSON file or folder of JSON files")
     parser.add_argument(
-        '-o', '--output', help='path to output file or folder (default: derived from input path)')
+        "-o",
+        "--output",
+        help="path to output file or folder (default: derived from input path)",
+    )
     args = parser.parse_args()
 
     main(args.input, args.output)
```

### Comparing `bnw_tools-0.0.1.4/bnw_tools/extract/nlp/util_stanza.py` & `bnw_tools-0.0.2.0/bnw_tools/extract/nlp/util_stanza.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/createVTT.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/createVTT.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/graphvizify.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/graphvizify.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/util_networkx.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/util_networkx.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/util_wordcloud.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/util_wordcloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,40 +13,50 @@
 import cv2
 
 
 if TYPE_CHECKING:
     from ..extract.nlp.util_nlp import Folder
 
 
-def generate_wordcloud(dict_word_count, output_file_path='wordcloud.png', width=1920, height=1080):
+def generate_wordcloud(dict_word_count, output_file_path='wordcloud.png', width=1920, height=1080, colormap=None, square=False, force=False):
     """
     Generates a wordcloud as a PNG image from a dictionary containing word count information.
 
     Args:
         dict_word_count: A dictionary containing word count information.
         output_file_path: The path and file name to save the generated image. Default is 'wordcloud.png'.
         width: The width of the generated image. Default is 1920.
         height: The height of the generated image. Default is 1080.
 
     Returns:
         None.
     """
     if not dict_word_count:
         return None
-
+    
     if not output_file_path.endswith(".png"):
         output_file_path += ".png"
-    wc = WordCloud(width=width, height=height)
+
+    if output_file_path and not force:
+        if os.path.exists(output_file_path):
+            # print(f"File already exists: {output_file_path}")
+            return
+    
+    colormap = 'rainbow' if colormap is None else colormap
+    # https://matplotlib.org/stable/users/explain/colors/colormaps.html
+
+    wc = WordCloud(width=width, height=height, colormap=colormap)
     wc.generate_from_frequencies(dict_word_count)
     wc.to_file(output_file_path)
 
-    new = min(height, width)
-    wc2 = WordCloud(width=new, height=new)
-    wc2.generate_from_frequencies(dict_word_count)
-    wc2.to_file(output_file_path.replace(".png", "_square.png"))
+    if square:
+        new = min(height, width)
+        wc2 = WordCloud(width=new, height=new, colormap=colormap)
+        wc2.generate_from_frequencies(dict_word_count)
+        wc2.to_file(output_file_path.replace(".png", "_square.png"))
 
 
 def generate_wordcloud_mask(dict_word_count, mask_path, output_file_path='wordcloud_mask.png', width=1920, height=1080):
     """
     Generates a wordcloud as a PNG image from a dictionary containing word count information and a mask image.
 
     Args:
```

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/LaTeX/texify.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/LaTeX/texify.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/mediaWiki.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/mediaWiki.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/playlist2wiki-converter.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/playlist2wiki-converter.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/wiki_bot.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/wiki_bot.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/MediaWiki/wiki/barlow.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/MediaWiki/wiki/barlow.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/bibtex_to_notes.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/bibtex_to_notes.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/obsidize.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/obsidize.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/publish/Obsidian/transitions.py` & `bnw_tools-0.0.2.0/bnw_tools/publish/Obsidian/transitions.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/review/k_score.py` & `bnw_tools-0.0.2.0/bnw_tools/review/k_score.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/review/similarity.py` & `bnw_tools-0.0.2.0/bnw_tools/review/similarity.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     for i, d in enumerate(dictionaries):
         for word, count in d.items():
             index = word_indices[word]
             vectors[i][index] = count
     return vectors
 
 
-def normalize(vectors, log_level=False, sqrt_level=2):
+def normalize(vectors, log_level=False, sqrt_level=2, config=None):
     """
     Normalize a list of vectors and reward higher word counts logarithmically.
 
     Parameters:
     ----------
     vectors : numpy.ndarray
         A 2D numpy array of shape (n_samples, n_features) containing the vectors to normalize.
@@ -87,46 +87,61 @@
 285        [0.613,  0.017,  0.023], 
            [1.0,    1.0,    1.0]])
     >>> normalize(vectors, log_level=5)
     array([[0,908,  0.855, 0.564],
            [0,947,  0.555, 0.591],
            [1.0,    1.0,    1.0]])
     """
+    # check if vectors is List[Dict[str, int]]
+    if isinstance(vectors[0], dict):
+        vectors = create_word_vectors(vectors)
+
+    if config:
+        log_level = config.get("log_level", log_level)
+        sqrt_level = config.get("sqrt_level", sqrt_level)
+
+
+
     max_values = np.max(vectors, axis=0)
-    indices_zero = max_values == 0
-    max_values[indices_zero] = 1  # replacing 0s with 1s
+        
+    if not np.isscalar(max_values):
+        # max_values is a vector.
+        indices_zero = max_values == 0
+        max_values[indices_zero] = 1  # replacing 0s with 1s
     vectors /= max_values
 
     if log_level:
         # Recommended: False, not fully tested.
         # If used: ~5, between 2 and 10
         vectors *= 10 ** (log_level - 1)
         vectors += 1
         vectors = np.log10(vectors) / (log_level - 1)
     if sqrt_level:
         vectors = np.sqrt(vectors)
+
+    # TODO: Reduce the reward of long documents
     return vectors
 
 # def compute_similarity_matrix(vectors):
 #     # todo: Include weighed cosine similarity
 #     return cosine_similarity(vectors)
 
-
-def compute_similarity_from_vectors(vector_a: List[Dict[str, int]], vector_b: List[Dict[str, int]]):
+# # TODO: does not seem to be used anymore
+def compute_similarity_from_vectors(vector_a: List[Dict[str, int]], vector_b: List[Dict[str, int]], config=None):
     np_vectors_a = create_word_vectors(vector_a)
-    np_vectors_a = normalize(np_vectors_a)
+    np_vectors_a = normalize(np_vectors_a, config=config)
 
     np_vectors_b = create_word_vectors(vector_b)
     sim_matrix = cosine_similarity(np_vectors_a, np_vectors_b)
     return sim_matrix
 
 
-def compute_weighed_similarity(vector_a: List[Dict[str, int]], vector_b: List[Dict[str, int]]):
+def compute_weighed_similarity(vector_a: List[Dict[str, int]], vector_b: List[Dict[str, int]], config=None):
     np_vectors_a = create_word_vectors(vector_a)
-    np_vectors_a = normalize(np_vectors_a)
+    np_vectors_a = normalize(np_vectors_a, config=config)
 
     np_vectors_b = create_word_vectors(vector_b)
     sim_matrix = np.zeros((len(np_vectors_a), len(np_vectors_b)))
     target = np.ones(len(np_vectors_b[0]))
     for c_a, vector_a in enumerate(np_vectors_a):
         for c_b, weight in enumerate(np_vectors_b):
             if sum(vector_a * weight) == 0:
@@ -173,14 +188,15 @@
     csv_file = os.path.join(path, filename) + '.csv'
     pd.DataFrame(sim_matrix).to_csv(csv_file, index=False,
                                     header=False, sep=";", decimal=",")
 
     # ax.legend()
 
     print(f"Similarity matrix saved as {png_file} and {csv_file}.")
+    plt.close()
 
 
 def print_sim_matrix(sim_matrix, path, prefix="", filename="", suffix="_similarity_matrix", xlabel='Documents', ylabel='Documents', dpi=300, vmin=None, vmax=None, cmap=None, additional_info: ResearchQuestion = None):
     # If i want to see the figure:
     # fig, ax = plt.subplots()
     fig, ax = plt.subplots()
     # plt.show()
@@ -220,7 +236,8 @@
 
     # Save similarity matrix as CSV
     csv_file = os.path.join(path, filename) + '.csv'
     pd.DataFrame(sim_matrix).to_csv(csv_file, index=False,
                                     header=False, sep=";", decimal=",")
 
     print(f"Similarity matrix saved as {png_file} and {csv_file}.")
+    plt.close()
```

### Comparing `bnw_tools-0.0.1.4/bnw_tools/review/spellcheck.py` & `bnw_tools-0.0.2.0/bnw_tools/review/spellcheck.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/review/library/barlow.py` & `bnw_tools-0.0.2.0/bnw_tools/review/library/barlow.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/data/sample/de/BMZ_1_LegendariesundArtefakte.mp3.vtt` & `bnw_tools-0.0.2.0/data/sample/de/BMZ_1_LegendariesundArtefakte.mp3.vtt`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/data/sample/en/Therapist_Reacts_to_Everything_Everywhere_All_at_Once.mp3.vtt` & `bnw_tools-0.0.2.0/data/sample/en/Therapist_Reacts_to_Everything_Everywhere_All_at_Once.mp3.vtt`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/whispered_folder.py` & `bnw_tools-0.0.2.0/scripts/whispered_folder.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/README.md` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/README.md`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/SWARM-SLR_Stage_I.ipynb` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/SWARM-SLR_Stage_I.ipynb`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/SWARM-SLR_Stage_III.ipynb` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/SWARM-SLR_Stage_III.ipynb`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 20% similar despite different names*

```diff
@@ -1,690 +1,701 @@
-00000000: 7b0a 2022 6365 6c6c 7322 3a20 5b0a 2020  {. "cells": [.  
-00000010: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
-00000020: 3a20 226d 6172 6b64 6f77 6e22 2c0a 2020  : "markdown",.  
-00000030: 2022 6d65 7461 6461 7461 223a 207b 7d2c   "metadata": {},
-00000040: 0a20 2020 2273 6f75 7263 6522 3a20 5b0a  .   "source": [.
-00000050: 2020 2020 2223 2053 7461 6765 2049 4949      "# Stage III
-00000060: 5c6e 222c 0a20 2020 2022 5468 6973 2073  \n",.    "This s
-00000070: 7461 6765 2069 7320 6174 2074 6865 2068  tage is at the h
-00000080: 6561 7274 206f 6620 6120 6c69 7465 7261  eart of a litera
-00000090: 7475 7265 2072 6576 6965 772e 2049 7420  ture review. It 
-000000a0: 6973 2077 6865 7265 206e 6577 2069 6e66  is where new inf
-000000b0: 6f72 6d61 7469 6f6e 2069 7320 6465 7269  ormation is deri
-000000c0: 7665 6420 616e 6420 7379 6e74 6865 7369  ved and synthesi
-000000d0: 7a65 642e 2057 6869 6c65 2074 6f6f 6c73  zed. While tools
-000000e0: 2063 616e 2061 7373 6973 7420 696e 2069   can assist in i
-000000f0: 6e66 6f72 6d61 7469 6f6e 2065 7874 7261  nformation extra
-00000100: 6374 696f 6e20 616e 6420 2073 7472 7563  ction and  struc
-00000110: 7475 7269 6e67 2074 6869 7320 696e 666f  turing this info
-00000120: 726d 6174 696f 6e2c 2074 6865 2072 6573  rmation, the res
-00000130: 6561 7263 6865 7273 2069 6e73 6967 6874  earchers insight
-00000140: 2069 7320 6465 6669 6e69 6e67 2074 6869   is defining thi
-00000150: 7320 7374 6167 652e 5c6e 222c 0a20 2020  s stage.\n",.   
-00000160: 2022 5c6e 222c 0a20 2020 2022 2a2a 576f   "\n",.    "**Wo
-00000170: 726b 6c6f 6164 2064 6973 7472 6962 7574  rkload distribut
-00000180: 696f 6e2a 2a5c 6e22 2c0a 2020 2020 225c  ion**\n",.    "\
-00000190: 6e22 2c0a 2020 2020 227c 4163 746f 727c  n",.    "|Actor|
-000001a0: 5469 6d65 7c5c 6e22 2c0a 2020 2020 227c  Time|\n",.    "|
-000001b0: 3a2d 2d2d 2d7c 3a2d 2d2d 2d7c 5c6e 222c  :----|:----|\n",
-000001c0: 0a20 2020 2022 7c52 6573 6561 7263 6865  .    "|Researche
-000001d0: 727c 3f20 6d69 6e7c 5c6e 222c 0a20 2020  r|? min|\n",.   
-000001e0: 2022 5c6e 222c 0a20 2020 2022 2a2a 546f   "\n",.    "**To
-000001f0: 6f6c 732a 2a5c 6e22 2c0a 2020 2020 222a  ols**\n",.    "*
-00000200: 2052 6573 6561 7263 6820 416e 6e6f 7461   Research Annota
-00000210: 7469 6f6e 2044 6174 6162 6173 6520 2865  tion Database (e
-00000220: 2e67 2e20 5b4f 524b 475d 2868 7474 7073  .g. [ORKG](https
-00000230: 3a2f 2f6f 726b 672e 6f72 672f 2929 5c6e  ://orkg.org/))\n
-00000240: 222c 0a20 2020 2022 2a20 4d61 726b 646f  ",.    "* Markdo
-00000250: 776e 2066 696c 6520 7669 6577 6572 2028  wn file viewer (
-00000260: 652e 672e 205b 4f62 7369 6469 616e 5d28  e.g. [Obsidian](
-00000270: 6874 7470 733a 2f2f 6f62 7369 6469 616e  https://obsidian
-00000280: 2e6d 642f 2920 7769 7468 205b 4461 7461  .md/) with [Data
-00000290: 7669 6577 5d28 6874 7470 733a 2f2f 6769  view](https://gi
-000002a0: 7468 7562 2e63 6f6d 2f62 6c61 636b 736d  thub.com/blacksm
-000002b0: 6974 6867 752f 6f62 7369 6469 616e 2d64  ithgu/obsidian-d
-000002c0: 6174 6176 6965 7729 2070 6c75 6769 6e29  ataview) plugin)
-000002d0: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
-000002e0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-000002f0: 226d 6172 6b64 6f77 6e22 2c0a 2020 2022  "markdown",.   "
-00000300: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
-00000310: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
-00000320: 2020 2223 2320 5461 736b 2036 3a20 416e    "## Task 6: An
-00000330: 616c 7973 6973 5c6e 222c 0a20 2020 2022  alysis\n",.    "
-00000340: 5c6e 222c 0a20 2020 2022 7c53 7465 707c  \n",.    "|Step|
-00000350: 5265 7375 6c74 7c52 6571 7569 7265 6d65  Result|Requireme
-00000360: 6e74 7c5c 6e22 2c0a 2020 2020 227c 3a2d  nt|\n",.    "|:-
-00000370: 2d2d 2d7c 3a2d 2d2d 2d7c 3a2d 2d2d 2d7c  ---|:----|:----|
-00000380: 5c6e 222c 0a20 2020 2022 7c52 6573 6f75  \n",.    "|Resou
-00000390: 7263 6520 616e 6e6f 7461 7469 6f6e 7c63  rce annotation|c
-000003a0: 6f6e 7472 6962 7574 696f 6e20 7265 7072  ontribution repr
-000003b0: 6573 656e 7461 7469 6f6e 7c34 392e 2061  esentation|49. a
-000003c0: 6e6e 6f74 6174 6520 7468 6520 646f 6375  nnotate the docu
-000003d0: 6d65 6e74 3c62 723e 3530 2e20 7265 7072  ment<br>50. repr
-000003e0: 6573 656e 7420 7468 6520 616e 6e6f 7461  esent the annota
-000003f0: 7469 6f6e 206d 6163 6869 6e65 2d72 6561  tion machine-rea
-00000400: 6461 626c 653c 6272 3e35 312e 2061 6e6e  dable<br>51. ann
-00000410: 6f74 6174 6520 636f 6c6c 6162 6f72 6174  otate collaborat
-00000420: 6976 656c 797c 5c6e 220a 2020 205d 0a20  ively|\n".   ]. 
-00000430: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
-00000440: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
-00000450: 6e22 2c0a 2020 2022 6d65 7461 6461 7461  n",.   "metadata
-00000460: 223a 207b 7d2c 0a20 2020 2273 6f75 7263  ": {},.   "sourc
-00000470: 6522 3a20 5b0a 2020 2020 2223 2323 2053  e": [.    "### S
-00000480: 7465 7020 362e 3120 5265 736f 7572 6365  tep 6.1 Resource
-00000490: 2061 6e6e 6f74 6174 696f 6e5c 6e22 2c0a   annotation\n",.
-000004a0: 2020 2020 222a 2a52 6571 7569 7265 6d65      "**Requireme
-000004b0: 6e74 733a 2a2a 5c6e 222c 0a20 2020 2022  nts:**\n",.    "
-000004c0: 2a20 616e 6e6f 7461 7465 2074 6865 2064  * annotate the d
-000004d0: 6f63 756d 656e 745c 6e22 2c0a 2020 2020  ocument\n",.    
-000004e0: 222a 2072 6570 7265 7365 6e74 2074 6865  "* represent the
-000004f0: 2061 6e6e 6f74 6174 696f 6e20 6d61 6368   annotation mach
-00000500: 696e 652d 7265 6164 6162 6c65 5c6e 222c  ine-readable\n",
-00000510: 0a20 2020 2022 2a20 616e 6e6f 7461 7465  .    "* annotate
-00000520: 2063 6f6c 6c61 626f 7261 7469 7665 6c79   collaboratively
-00000530: 5c6e 222c 0a20 2020 2022 5c6e 222c 0a20  \n",.    "\n",. 
-00000540: 2020 2022 5768 696c 6520 7468 6973 2073     "While this s
-00000550: 7465 7020 7075 7473 2065 6d70 6861 7369  tep puts emphasi
-00000560: 7320 6f6e 2073 7472 7563 7475 7265 6420  s on structured 
-00000570: 616e 6e6f 7461 7469 6f6e 2c20 6974 2069  annotation, it i
-00000580: 7320 6164 7669 7365 6420 746f 2073 7461  s advised to sta
-00000590: 7274 2061 2073 6967 6e69 6669 6361 6e74  rt a significant
-000005a0: 2070 6f72 7469 6f6e 206f 6620 7468 6520   portion of the 
-000005b0: 776f 726b 2069 6e20 6120 666c 6578 6962  work in a flexib
-000005c0: 6c65 2065 6e76 6972 6f6e 6d65 6e74 2e20  le environment. 
-000005d0: 4475 7269 6e67 2074 6865 2063 6f75 7273  During the cours
-000005e0: 6520 6f66 2065 7874 7261 6374 696e 6720  e of extracting 
-000005f0: 696e 666f 726d 6174 696f 6e2c 2074 6865  information, the
-00000600: 2073 7472 7563 7475 7265 2072 6571 7569   structure requi
-00000610: 7265 6420 746f 2062 6573 7420 7265 7072  red to best repr
-00000620: 6573 656e 7420 7468 6973 2069 6e66 6f72  esent this infor
-00000630: 6d61 7469 6f6e 2069 7320 6c69 6b65 6c79  mation is likely
-00000640: 2074 6f20 6368 616e 6765 2069 7465 7261   to change itera
-00000650: 7469 7665 6c79 2e20 5c6e 222c 0a20 2020  tively. \n",.   
-00000660: 2022 5c6e 222c 0a20 2020 2022 7c53 7465   "\n",.    "|Ste
-00000670: 707c 5044 4620 7265 6164 6572 3c62 723e  p|PDF reader<br>
-00000680: 652e 672e 205b 4163 726f 6261 7420 5265  e.g. [Acrobat Re
-00000690: 6164 6572 5d28 6874 7470 733a 2f2f 7777  ader](https://ww
-000006a0: 772e 6164 6f62 652e 636f 6d2f 6465 2f61  w.adobe.com/de/a
-000006b0: 6372 6f62 6174 2f70 6466 2d72 6561 6465  crobat/pdf-reade
-000006c0: 722e 6874 6d6c 297c 4d61 726b 646f 776e  r.html)|Markdown
-000006d0: 2065 6469 746f 723c 6272 3e65 2e67 2e20   editor<br>e.g. 
-000006e0: 5b4f 6273 6964 6961 6e5d 2868 7474 7073  [Obsidian](https
-000006f0: 3a2f 2f6f 6273 6964 6961 6e2e 6d64 2f29  ://obsidian.md/)
-00000700: 7c53 7072 6561 6473 6865 6574 2065 6469  |Spreadsheet edi
-00000710: 746f 723c 6272 3e65 2e67 2e20 5b45 7863  tor<br>e.g. [Exc
-00000720: 656c 5d28 6874 7470 733a 2f2f 7777 772e  el](https://www.
-00000730: 6d69 6372 6f73 6f66 742e 636f 6d2f 6465  microsoft.com/de
-00000740: 2d64 652f 6d69 6372 6f73 6f66 742d 3336  -de/microsoft-36
-00000750: 352f 6578 6365 6c29 2c20 5b47 6f6f 676c  5/excel), [Googl
-00000760: 6520 5368 6565 7473 5d28 6874 7470 733a  e Sheets](https:
-00000770: 2f2f 646f 6373 2e67 6f6f 676c 652e 636f  //docs.google.co
-00000780: 6d2f 7370 7265 6164 7368 6565 7473 297c  m/spreadsheets)|
-00000790: 4b6f 6e77 6c65 6467 6520 6772 6170 6820  Konwledge graph 
-000007a0: 6564 6974 6f72 3c62 723e 652e 672e 205b  editor<br>e.g. [
-000007b0: 4f52 4b47 5d28 6874 7470 733a 2f2f 6f72  ORKG](https://or
-000007c0: 6b67 2e6f 7267 2f29 7c5c 6e22 2c0a 2020  kg.org/)|\n",.  
-000007d0: 2020 227c 3a2d 2d2d 2d7c 3a2d 2d2d 2d7c    "|:----|:----|
-000007e0: 3a2d 2d2d 2d7c 3a2d 2d2d 2d7c 3a2d 2d2d  :----|:----|:---
-000007f0: 2d7c 5c6e 222c 0a20 2020 2022 7c65 6173  -|\n",.    "|eas
-00000800: 6520 6f66 2075 7365 7c2b 2b7c 2b7c 2b2b  e of use|++|+|++
-00000810: 7c2b 2d7c 5c6e 222c 0a20 2020 2022 7c66  |+-|\n",.    "|f
-00000820: 6c65 7869 626c 6520 666f 726d 6174 7c2d  lexible format|-
-00000830: 7c2b 2b7c 2b7c 2b2d 7c5c 6e22 2c0a 2020  |++|+|+-|\n",.  
-00000840: 2020 227c 7374 7275 6374 7572 6564 2064    "|structured d
-00000850: 6174 617c 2d7c 2b2d 7c2b 7c2b 2b7c 5c6e  ata|-|+-|+|++|\n
-00000860: 222c 0a20 2020 2022 7c69 6e74 6572 6f70  ",.    "|interop
-00000870: 6572 6162 6c65 2064 6174 617c 2d2d 7c2d  erable data|--|-
-00000880: 2d7c 2b2b 7c2b 2b7c 5c6e 222c 0a20 2020  -|++|++|\n",.   
-00000890: 2022 7c63 6f6c 6c61 626f 7261 7469 7665   "|collaborative
-000008a0: 2061 6e6e 6f74 6174 696f 6e7c 2d2d 7c2d   annotation|--|-
-000008b0: 2d7c 2b2d 7c2b 2b7c 5c6e 222c 0a20 2020  -|+-|++|\n",.   
-000008c0: 2022 5c6e 222c 0a20 2020 2022 5357 4152   "\n",.    "SWAR
-000008d0: 4d2d 534c 5220 6164 7669 7365 7320 746f  M-SLR advises to
-000008e0: 2077 6f72 6b20 7573 6520 6120 7661 7269   work use a vari
-000008f0: 6574 7920 6f66 2074 6f6f 6c73 2061 6e64  ety of tools and
-00000900: 2077 6f72 6b20 746f 7761 7264 7320 6d6f   work towards mo
-00000910: 7265 2073 7472 7563 7475 7265 6420 6461  re structured da
-00000920: 7461 2c20 7768 696c 6520 6d61 6b69 6e67  ta, while making
-00000930: 2075 7365 206f 6620 6561 7365 206f 6620   use of ease of 
-00000940: 7573 6520 616e 6420 666c 6578 6962 696c  use and flexibil
-00000950: 6974 793a 5c6e 222c 0a20 2020 2022 5c6e  ity:\n",.    "\n
-00000960: 222c 0a20 2020 2022 3c64 6976 2061 6c69  ",.    "<div ali
-00000970: 676e 3d5c 2263 656e 7465 725c 223e 5c6e  gn=\"center\">\n
-00000980: 222c 0a20 2020 2022 3c69 6d67 2073 7263  ",.    "<img src
-00000990: 3d5c 2269 6d61 6765 732f 5461 736b 2036  =\"images/Task 6
-000009a0: 202d 2030 3120 4f62 7369 6469 616e 2052   - 01 Obsidian R
-000009b0: 512e 706e 675c 2220 7769 6474 683d 5c22  Q.png\" width=\"
-000009c0: 3935 255c 2220 2f3e 5c6e 222c 0a20 2020  95%\" />\n",.   
-000009d0: 2022 3c66 6967 6361 7074 696f 6e3e 4f62   "<figcaption>Ob
-000009e0: 7369 6469 616e 206f 7665 7276 6965 7720  sidian overview 
-000009f0: 6f66 2074 6865 2061 6e61 6c79 7a65 6420  of the analyzed 
-00000a00: 6c69 6272 6172 792e 2054 6865 2072 6967  library. The rig
-00000a10: 6874 2073 6964 6520 6465 7069 6374 7320  ht side depicts 
-00000a20: 7468 6520 646f 6375 6d65 6e74 7320 286e  the documents (n
-00000a30: 6f64 6573 2920 616e 6420 7468 6569 7220  odes) and their 
-00000a40: 7369 6d69 6c61 7269 7479 2074 6f20 6f74  similarity to ot
-00000a50: 6865 7220 646f 6375 6d65 6e74 7320 2865  her documents (e
-00000a60: 6467 6573 292e 2054 6865 206e 6f64 6573  dges). The nodes
-00000a70: 2061 7265 2063 6f6c 6f72 6564 2062 6173   are colored bas
-00000a80: 6564 206f 6e20 7468 6569 7220 7265 6c65  ed on their rele
-00000a90: 7661 6e63 6520 6f6e 2061 7665 7261 6765  vance on average
-00000aa0: 2028 6772 6565 6e29 2c20 6f72 2074 6f20   (green), or to 
-00000ab0: 6120 7265 7365 6172 6368 2071 7565 7374  a research quest
-00000ac0: 696f 6e20 2852 5129 2028 6865 7265 3a20  ion (RQ) (here: 
-00000ad0: 5251 3120 7265 642c 2052 5132 2062 6c75  RQ1 red, RQ2 blu
-00000ae0: 6529 2e20 5468 6520 6c65 6674 2073 6964  e). The left sid
-00000af0: 6520 7368 6f77 7320 7468 6520 5251 312d  e shows the RQ1-
-00000b00: 6669 6c65 2e20 4561 6368 2052 5120 7265  file. Each RQ re
-00000b10: 7072 6573 656e 7461 7469 6f6e 2064 6973  presentation dis
-00000b20: 706c 6179 7320 7468 6520 646f 6375 6d65  plays the docume
-00000b30: 6e74 7320 7468 6174 2073 636f 7265 6420  nts that scored 
-00000b40: 6869 6768 6573 7420 666f 7220 7468 6520  highest for the 
-00000b50: 5251 2773 2072 6573 7065 6374 6976 6520  RQ's respective 
-00000b60: 7765 6967 6865 6420 6b65 7977 6f72 6473  weighed keywords
-00000b70: 2e3c 2f66 6967 6361 7074 696f 6e3e 5c6e  .</figcaption>\n
-00000b80: 222c 0a20 2020 2022 3c2f 6469 763e 5c6e  ",.    "</div>\n
-00000b90: 222c 0a20 2020 2022 5c6e 222c 0a20 2020  ",.    "\n",.   
-00000ba0: 2022 3c62 723e 5c6e 222c 0a20 2020 2022   "<br>\n",.    "
-00000bb0: 5c6e 222c 0a20 2020 2022 3c64 6976 2061  \n",.    "<div a
-00000bc0: 6c69 676e 3d5c 2263 656e 7465 725c 223e  lign=\"center\">
-00000bd0: 5c6e 222c 0a20 2020 2022 3c69 6d67 2073  \n",.    "<img s
-00000be0: 7263 3d5c 2269 6d61 6765 732f 5461 736b  rc=\"images/Task
-00000bf0: 2036 202d 2030 3220 4f62 7369 6469 616e   6 - 02 Obsidian
-00000c00: 2044 6f63 756d 656e 742e 706e 675c 2220   Document.png\" 
-00000c10: 7769 6474 683d 5c22 3935 255c 2220 2f3e  width=\"95%\" />
-00000c20: 5c6e 222c 0a20 2020 2022 3c66 6967 6361  \n",.    "<figca
-00000c30: 7074 696f 6e3e 4f62 7369 6469 616e 2064  ption>Obsidian d
-00000c40: 6f63 756d 656e 7420 7669 6577 2e20 5468  ocument view. Th
-00000c50: 6520 6c65 6674 2073 6964 6520 6469 7370  e left side disp
-00000c60: 6c61 7973 2061 2064 6f63 756d 656e 742d  lays a document-
-00000c70: 7265 7072 6573 656e 7461 7469 6f6e 2c20  representation, 
-00000c80: 636f 6e74 6169 6e69 6e67 206d 6574 6164  containing metad
-00000c90: 6174 612c 2065 7874 7261 6374 6564 2069  ata, extracted i
-00000ca0: 6e66 6f72 6d61 7469 6f6e 2061 6e64 2061  nformation and a
-00000cb0: 6e20 656d 6265 6464 6564 2066 696c 6520  n embedded file 
-00000cc0: 7669 6577 6572 2e20 5468 6973 2064 6f63  viewer. This doc
-00000cd0: 756d 656e 7420 6361 6e20 6265 2075 7365  ument can be use
-00000ce0: 6420 746f 2061 6e6e 6f74 6174 652c 2063  d to annotate, c
-00000cf0: 7265 6174 6520 616e 6420 6c69 6e6b 2061  reate and link a
-00000d00: 6e79 2066 6f72 6d20 6f66 2064 6967 6974  ny form of digit
-00000d10: 616c 2061 6e6e 6f74 6174 696f 6e2c 2073  al annotation, s
-00000d20: 7563 6820 6173 2073 6372 6565 6e73 686f  uch as screensho
-00000d30: 7473 2c20 6772 6170 6869 6373 2c20 6361  ts, graphics, ca
-00000d40: 6c63 756c 6174 696f 6e73 2c20 6c69 6e6b  lculations, link
-00000d50: 732c 2065 7463 2e3c 2f66 6967 6361 7074  s, etc.</figcapt
-00000d60: 696f 6e3e 5c6e 222c 0a20 2020 2022 3c2f  ion>\n",.    "</
-00000d70: 6469 763e 5c6e 222c 0a20 2020 2022 5c6e  div>\n",.    "\n
-00000d80: 222c 0a20 2020 2022 3c62 723e 5c6e 222c  ",.    "<br>\n",
-00000d90: 0a20 2020 2022 5c6e 222c 0a20 2020 2022  .    "\n",.    "
-00000da0: 3c64 6976 2061 6c69 676e 3d5c 2263 656e  <div align=\"cen
-00000db0: 7465 725c 223e 5c6e 222c 0a20 2020 2022  ter\">\n",.    "
-00000dc0: 3c69 6d67 2073 7263 3d5c 2269 6d61 6765  <img src=\"image
-00000dd0: 732f 5461 736b 2036 202d 2030 3320 4f62  s/Task 6 - 03 Ob
-00000de0: 7369 6469 616e 2054 6f74 616c 2e70 6e67  sidian Total.png
-00000df0: 5c22 2077 6964 7468 3d5c 2239 3525 5c22  \" width=\"95%\"
-00000e00: 202f 3e5c 6e22 2c0a 2020 2020 223c 6669   />\n",.    "<fi
-00000e10: 6763 6170 7469 6f6e 3e4f 6273 6964 6961  gcaption>Obsidia
-00000e20: 6e20 7072 6f67 7265 7373 2074 7261 636b  n progress track
-00000e30: 696e 672e 2054 6865 206c 6566 7420 7369  ing. The left si
-00000e40: 6465 2073 686f 7773 206d 6f72 6520 6f66  de shows more of
-00000e50: 2074 6865 2061 2064 6f63 756d 656e 742d   the a document-
-00000e60: 7265 7072 6573 656e 7461 7469 6f6e 2c20  representation, 
-00000e70: 7768 6963 6820 616c 736f 206c 6973 7473  which also lists
-00000e80: 2074 6865 206d 6f73 7420 7369 6d69 6c61   the most simila
-00000e90: 7220 646f 6375 6d65 6e74 7320 616e 6420  r documents and 
-00000ea0: 7468 6569 7220 7265 7370 6563 7469 7665  their respective
-00000eb0: 2073 636f 7265 732e 2054 6865 2072 6967   scores. The rig
-00000ec0: 6874 2073 6964 6520 6465 7069 6374 7320  ht side depicts 
-00000ed0: 7468 6520 5c22 546f 7461 6c5c 2220 7461  the \"Total\" ta
-00000ee0: 622c 2070 726f 7669 6469 6e67 2061 6e20  b, providing an 
-00000ef0: 6f76 6572 7669 6577 206f 7665 7220 616c  overview over al
-00000f00: 6c20 7265 7365 6172 6368 2071 7565 7374  l research quest
-00000f10: 696f 6e73 2061 6e64 2061 2070 726f 6772  ions and a progr
-00000f20: 6573 7320 7472 6163 6b69 6e67 2066 6f72  ess tracking for
-00000f30: 2074 6865 2065 6e74 6972 6520 5357 4152   the entire SWAR
-00000f40: 4d2d 534c 522e 2057 6974 6820 6561 6368  M-SLR. With each
-00000f50: 2061 6e6e 6f74 6174 6564 2064 6f63 756d   annotated docum
-00000f60: 656e 742c 2074 6865 2072 6573 6561 7263  ent, the researc
-00000f70: 6865 7220 7072 6f67 7265 7373 6573 2074  her progresses t
-00000f80: 6872 6f75 6768 2074 6865 205c 2242 6573  hrough the \"Bes
-00000f90: 7420 4361 6e64 6964 6174 6573 5c22 2073  t Candidates\" s
-00000fa0: 7461 636b 2e3c 2f66 6967 6361 7074 696f  tack.</figcaptio
-00000fb0: 6e3e 5c6e 222c 0a20 2020 2022 3c2f 6469  n>\n",.    "</di
-00000fc0: 763e 5c6e 222c 0a20 2020 2022 5c6e 222c  v>\n",.    "\n",
-00000fd0: 0a20 2020 2022 3c62 723e 5c6e 222c 0a20  .    "<br>\n",. 
-00000fe0: 2020 2022 5c6e 222c 0a20 2020 2022 3c64     "\n",.    "<d
-00000ff0: 6976 2061 6c69 676e 3d5c 2263 656e 7465  iv align=\"cente
-00001000: 725c 223e 5c6e 222c 0a20 2020 2022 3c69  r\">\n",.    "<i
-00001010: 6d67 2073 7263 3d5c 2269 6d61 6765 732f  mg src=\"images/
-00001020: 5461 736b 2036 202d 2030 3420 4f62 7369  Task 6 - 04 Obsi
-00001030: 6469 616e 2041 6e6e 6f74 6174 696f 6e2e  dian Annotation.
-00001040: 706e 675c 2220 7769 6474 683d 5c22 3935  png\" width=\"95
-00001050: 255c 2220 2f3e 5c6e 222c 0a20 2020 2022  %\" />\n",.    "
-00001060: 3c66 6967 6361 7074 696f 6e3e 4f62 7369  <figcaption>Obsi
-00001070: 6469 616e 2064 6f63 756d 656e 7420 616e  dian document an
-00001080: 6e6f 7461 7469 6f6e 2e20 5468 6520 6c65  notation. The le
-00001090: 6674 2073 6964 6520 7368 6f77 7320 616e  ft side shows an
-000010a0: 2061 6e6e 6f74 6174 6564 2064 6f63 756d   annotated docum
-000010b0: 656e 7420 696e 636c 7564 696e 6720 7175  ent including qu
-000010c0: 6f74 6573 2061 6e64 2073 6372 6565 6e73  otes and screens
-000010d0: 686f 7473 2e20 4279 206d 6172 6b69 6e67  hots. By marking
-000010e0: 2069 7420 6173 205c 2257 6f72 6b20 696e   it as \"Work in
-000010f0: 2050 726f 6772 6573 735c 222c 2069 7420   Progress\", it 
-00001100: 6765 7473 206d 6f76 6564 2066 726f 6d20  gets moved from 
-00001110: 7468 6520 5c22 4265 7374 2043 616e 6469  the \"Best Candi
-00001120: 6461 7465 735c 2220 746f 205c 224d 6f64  dates\" to \"Mod
-00001130: 6966 6965 645c 222e 204f 6e63 6520 6974  ified\". Once it
-00001140: 2069 7320 6d61 726b 6564 2061 7320 5c22   is marked as \"
-00001150: 5061 7065 7220 7265 6164 2061 6e64 2043  Paper read and C
-00001160: 6f6e 7472 6962 7574 696f 6e20 636f 6d70  ontribution comp
-00001170: 6c65 7465 645c 222c 2069 7420 6973 206c  leted\", it is l
-00001180: 6973 7465 6420 756e 6465 7220 5c22 446f  isted under \"Do
-00001190: 6e65 5c22 2e3c 2f66 6967 6361 7074 696f  ne\".</figcaptio
-000011a0: 6e3e 5c6e 222c 0a20 2020 2022 3c2f 6469  n>\n",.    "</di
-000011b0: 763e 5c6e 222c 0a20 2020 2022 5c6e 222c  v>\n",.    "\n",
-000011c0: 0a20 2020 2022 3c62 723e 5c6e 222c 0a20  .    "<br>\n",. 
-000011d0: 2020 2022 5c6e 222c 0a20 2020 2022 3c64     "\n",.    "<d
-000011e0: 6976 3e5c 6e22 2c0a 2020 2020 223c 6469  iv>\n",.    "<di
-000011f0: 7620 7374 796c 653d 5c22 6469 7370 6c61  v style=\"displa
-00001200: 793a 2066 6c65 783b 206a 7573 7469 6679  y: flex; justify
-00001210: 2d63 6f6e 7465 6e74 3a20 6365 6e74 6572  -content: center
-00001220: 3b5c 223e 5c6e 222c 0a20 2020 2022 3c69  ;\">\n",.    "<i
-00001230: 6d67 2073 7263 3d5c 2269 6d61 6765 732f  mg src=\"images/
-00001240: 5461 736b 2036 202d 2030 3420 4f62 7369  Task 6 - 04 Obsi
-00001250: 6469 616e 2041 6e6e 6f74 6174 696f 6e2e  dian Annotation.
-00001260: 706e 675c 2220 7769 6474 683d 5c22 3435  png\" width=\"45
-00001270: 255c 2220 2f3e 5c6e 222c 0a20 2020 2022  %\" />\n",.    "
-00001280: 3c69 6d67 2073 7263 3d5c 2269 6d61 6765  <img src=\"image
-00001290: 732f 5461 736b 2036 202d 2030 3620 5370  s/Task 6 - 06 Sp
-000012a0: 7265 6164 7368 6565 742e 706e 675c 2220  readsheet.png\" 
-000012b0: 7769 6474 683d 5c22 3435 255c 2220 2f3e  width=\"45%\" />
-000012c0: 5c6e 222c 0a20 2020 2022 3c2f 6469 763e  \n",.    "</div>
-000012d0: 5c6e 222c 0a20 2020 2022 3c66 6967 6361  \n",.    "<figca
-000012e0: 7074 696f 6e3e 4279 2075 7369 6e67 204f  ption>By using O
-000012f0: 6273 6964 6961 6e20 616e 6420 7468 6520  bsidian and the 
-00001300: 656d 6265 6464 6564 2050 4446 2076 6965  embedded PDF vie
-00001310: 7765 722c 2074 6865 2072 6573 6561 7263  wer, the researc
-00001320: 6865 7220 6361 6e20 6765 7420 6120 6265  her can get a be
-00001330: 7474 6572 2066 6565 6c69 6e67 2066 6f72  tter feeling for
-00001340: 2074 6865 2072 6571 7569 7265 6420 6461   the required da
-00001350: 7461 2073 7472 7563 7475 7265 2e20 4974  ta structure. It
-00001360: 6572 6174 6976 656c 7920 616e 6420 7769  eratively and wi
-00001370: 7468 6f75 7420 6c6f 6f73 696e 6720 616e  thout loosing an
-00001380: 6e6f 7461 7469 6f6e 2066 726f 6d20 6561  notation from ea
-00001390: 726c 6965 7220 7374 6167 6573 2c20 7468  rlier stages, th
-000013a0: 6520 7265 7365 6172 6368 6572 2063 616e  e researcher can
-000013b0: 2070 726f 6772 6573 7320 746f 7761 7264   progress toward
-000013c0: 7320 6120 7374 7275 6374 7572 6564 203c  s a structured <
-000013d0: 6120 6872 6566 3d5c 2268 7474 7073 3a2f  a href=\"https:/
-000013e0: 2f64 6f63 732e 676f 6f67 6c65 2e63 6f6d  /docs.google.com
-000013f0: 2f73 7072 6561 6473 6865 6574 732f 642f  /spreadsheets/d/
-00001400: 314b 554d 5365 715f 507a 7034 4b76 655a  1KUMSeq_Pzp4KveZ
-00001410: 3770 6235 7264 6463 7373 6b31 5842 5469  7pb5rddcssk1XBTi
-00001420: 4c48 6e69 4430 6433 6e44 716f 2f65 6469  LHniD0d3nDqo/edi
-00001430: 7423 6769 643d 305c 223e 7370 7265 6164  t#gid=0\">spread
-00001440: 7368 6565 743c 2f61 3e2c 2077 6974 686f  sheet</a>, witho
-00001450: 7574 206d 6f64 656c 6c69 6e67 206f 7574  ut modelling out
-00001460: 2074 6865 2073 656d 616e 7469 6320 7374   the semantic st
-00001470: 7275 6374 7572 6520 6120 7072 696f 7269  ructure a priori
-00001480: 2e5c 6e22 2c0a 2020 2020 223c 2f64 6976  .\n",.    "</div
-00001490: 3e5c 6e22 0a20 2020 5d0a 2020 7d2c 0a20  >\n".   ].  },. 
-000014a0: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
-000014b0: 223a 2022 6d61 726b 646f 776e 222c 0a20  ": "markdown",. 
-000014c0: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
-000014d0: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
-000014e0: 0a20 2020 2022 2323 2054 6173 6b20 373a  .    "## Task 7:
-000014f0: 2053 796e 7468 6573 6973 5c6e 222c 0a20   Synthesis\n",. 
-00001500: 2020 2022 5c6e 222c 0a20 2020 2022 7c53     "\n",.    "|S
-00001510: 7465 707c 5265 7375 6c74 7c52 6571 7569  tep|Result|Requi
-00001520: 7265 6d65 6e74 7c5c 6e22 2c0a 2020 2020  rement|\n",.    
-00001530: 227c 3a2d 2d2d 2d7c 3a2d 2d2d 2d7c 3a2d  "|:----|:----|:-
-00001540: 2d2d 2d7c 5c6e 222c 0a20 2020 2022 7c43  ---|\n",.    "|C
-00001550: 6f6d 7061 7265 2063 6f6e 7472 6962 7574  ompare contribut
-00001560: 696f 6e73 7c63 6f6d 7061 7269 736f 6e7c  ions|comparison|
-00001570: 3532 2e20 6465 6669 6e65 2063 6f6d 7061  52. define compa
-00001580: 7269 736f 6e20 7072 6f70 6572 7469 6573  rison properties
-00001590: 3c62 723e 3533 2e20 696e 7365 7274 2063  <br>53. insert c
-000015a0: 6f6e 7472 6962 7574 696f 6e20 7661 6c75  ontribution valu
-000015b0: 6573 7c5c 6e22 2c0a 2020 2020 227c 4372  es|\n",.    "|Cr
-000015c0: 6166 7420 6172 6775 6d65 6e74 7320 6261  aft arguments ba
-000015d0: 7365 6420 6f6e 2066 696e 6469 6e67 737c  sed on findings|
-000015e0: 646f 6375 6d65 6e74 2063 6c61 696d 737c  document claims|
-000015f0: 3534 2e20 6964 656e 7469 6679 2065 7669  54. identify evi
-00001600: 6465 6e63 6520 2864 6174 6129 3c62 723e  dence (data)<br>
-00001610: 3535 2e20 6573 7461 626c 6973 6820 7761  55. establish wa
-00001620: 7272 616e 747c 5c6e 222c 0a20 2020 2022  rrant|\n",.    "
-00001630: 7c43 7269 7469 7175 6520 7468 6520 6c69  |Critique the li
-00001640: 7465 7261 7475 7265 7c74 6865 7369 7320  terature|thesis 
-00001650: 636c 6169 6d73 7c35 362e 2069 6465 6e74  claims|56. ident
-00001660: 6966 7920 6576 6964 656e 6365 2028 636c  ify evidence (cl
-00001670: 6169 6d73 293c 6272 3e35 372e 2069 6465  aims)<br>57. ide
-00001680: 6e74 6966 7920 7061 7474 6572 6e73 3c62  ntify patterns<b
-00001690: 723e 3538 2e20 6465 7465 6374 2066 616c  r>58. detect fal
-000016a0: 6c61 6369 6573 3c62 723e 3539 2e20 6964  lacies<br>59. id
-000016b0: 656e 7469 6679 2063 6f6e 666c 6963 7473  entify conflicts
-000016c0: 3c62 723e 3630 2e20 7265 736f 6c76 6520  <br>60. resolve 
-000016d0: 636f 6e66 6c69 6374 737c 220a 2020 205d  conflicts|".   ]
-000016e0: 0a20 207d 2c0a 2020 7b0a 2020 2022 6365  .  },.  {.   "ce
-000016f0: 6c6c 5f74 7970 6522 3a20 226d 6172 6b64  ll_type": "markd
-00001700: 6f77 6e22 2c0a 2020 2022 6d65 7461 6461  own",.   "metada
-00001710: 7461 223a 207b 7d2c 0a20 2020 2273 6f75  ta": {},.   "sou
-00001720: 7263 6522 3a20 5b0a 2020 2020 2223 2323  rce": [.    "###
-00001730: 2053 7465 7020 372e 3120 436f 6d70 6172   Step 7.1 Compar
-00001740: 6520 636f 6e74 7269 6275 7469 6f6e 735c  e contributions\
-00001750: 6e22 2c0a 2020 2020 222a 2a52 6571 7569  n",.    "**Requi
-00001760: 7265 6d65 6e74 733a 2a2a 5c6e 222c 0a20  rements:**\n",. 
-00001770: 2020 2022 2a20 6465 6669 6e65 2063 6f6d     "* define com
-00001780: 7061 7269 736f 6e20 7072 6f70 6572 7469  parison properti
-00001790: 6573 5c6e 222c 0a20 2020 2022 2a20 696e  es\n",.    "* in
-000017a0: 7365 7274 2063 6f6e 7472 6962 7574 696f  sert contributio
-000017b0: 6e20 7661 6c75 6573 5c6e 222c 0a20 2020  n values\n",.   
-000017c0: 2022 3c64 6976 3e5c 6e22 2c0a 2020 2020   "<div>\n",.    
-000017d0: 2220 2020 203c 6469 7620 7374 796c 653d  "    <div style=
-000017e0: 5c22 6469 7370 6c61 793a 2066 6c65 783b  \"display: flex;
-000017f0: 206a 7573 7469 6679 2d63 6f6e 7465 6e74   justify-content
-00001800: 3a20 6365 6e74 6572 3b5c 223e 5c6e 222c  : center;\">\n",
-00001810: 0a20 2020 2022 2020 2020 2020 2020 3c69  .    "        <i
-00001820: 6d67 2073 7263 3d5c 2269 6d61 6765 732f  mg src=\"images/
-00001830: 5461 736b 2036 202d 2030 3620 5370 7265  Task 6 - 06 Spre
-00001840: 6164 7368 6565 742e 706e 675c 2220 7769  adsheet.png\" wi
-00001850: 6474 683d 5c22 3435 255c 2220 2f3e 5c6e  dth=\"45%\" />\n
-00001860: 222c 0a20 2020 2022 2020 2020 2020 2020  ",.    "        
-00001870: 3c69 6d67 2073 7263 3d5c 2269 6d61 6765  <img src=\"image
-00001880: 732f 5461 736b 2037 202d 2030 3120 4b6e  s/Task 7 - 01 Kn
-00001890: 6f77 6c65 6467 6520 4772 6170 682e 706e  owledge Graph.pn
-000018a0: 675c 2220 7769 6474 683d 5c22 3435 255c  g\" width=\"45%\
-000018b0: 2220 2f3e 5c6e 222c 0a20 2020 2022 2020  " />\n",.    "  
-000018c0: 2020 3c2f 6469 763e 5c6e 222c 0a20 2020    </div>\n",.   
-000018d0: 2022 4174 2061 6e79 2070 6f69 6e74 2069   "At any point i
-000018e0: 6e20 7469 6d65 2c20 7468 6520 7265 7365  n time, the rese
-000018f0: 6172 6368 6572 2063 616e 2073 7461 7274  archer can start
-00001900: 2061 6e64 2069 7465 7261 7465 206f 6e20   and iterate on 
-00001910: 7468 6569 7220 6461 7461 206d 6f64 656c  their data model
-00001920: 2c20 616e 6420 6f6e 6365 2069 7465 7261  , and once itera
-00001930: 7469 6f6e 7320 7374 6167 6e61 7465 2061  tions stagnate a
-00001940: 6e64 203c 623e 636f 6d70 6172 6973 6f6e  nd <b>comparison
-00001950: 2070 726f 7065 7274 6965 7320 6172 6520   properties are 
-00001960: 6465 6669 6e65 643c 2f62 3e2c 2074 6865  defined</b>, the
-00001970: 7920 6361 6e20 7072 6f67 7265 7373 2074  y can progress t
-00001980: 6f77 6172 6473 2074 6865 206e 6578 7420  owards the next 
-00001990: 7374 6167 652c 2066 726f 6d20 286c 6f63  stage, from (loc
-000019a0: 616c 2920 3c61 2068 7265 663d 5c22 6874  al) <a href=\"ht
-000019b0: 7470 733a 2f2f 646f 6373 2e67 6f6f 676c  tps://docs.googl
-000019c0: 652e 636f 6d2f 7370 7265 6164 7368 6565  e.com/spreadshee
-000019d0: 7473 2f64 2f31 4b55 4d53 6571 5f50 7a70  ts/d/1KUMSeq_Pzp
-000019e0: 344b 7665 5a37 7062 3572 6464 6373 736b  4KveZ7pb5rddcssk
-000019f0: 3158 4254 694c 486e 6944 3064 336e 4471  1XBTiLHniD0d3nDq
-00001a00: 6f2f 6564 6974 2367 6964 3d30 5c22 3e73  o/edit#gid=0\">s
-00001a10: 7072 6561 6473 6865 6574 3c2f 613e 2074  preadsheet</a> t
-00001a20: 6f20 6120 676c 6f62 616c 203c 6120 6872  o a global <a hr
-00001a30: 6566 3d5c 2268 7474 7073 3a2f 2f6f 726b  ef=\"https://ork
-00001a40: 672e 6f72 672f 636f 6d70 6172 6973 6f6e  g.org/comparison
-00001a50: 2f52 3635 3931 3334 2f5c 223e 6b6e 6f77  /R659134/\">know
-00001a60: 6c65 6467 6520 6772 6170 683c 2f61 3e2e  ledge graph</a>.
-00001a70: 5c6e 222c 0a20 2020 2022 3c2f 6469 763e  \n",.    "</div>
-00001a80: 5c6e 222c 0a20 2020 2022 5c6e 222c 0a20  \n",.    "\n",. 
-00001a90: 2020 2022 3c62 723e 5c6e 222c 0a20 2020     "<br>\n",.   
-00001aa0: 2022 5c6e 222c 0a20 2020 2022 3c69 6d67   "\n",.    "<img
-00001ab0: 2073 7479 6c65 3d5c 2266 6c6f 6174 3a20   style=\"float: 
-00001ac0: 7269 6768 743b 206d 6172 6769 6e3a 2032  right; margin: 2
-00001ad0: 3070 783b 5c22 2073 7263 3d5c 2269 6d61  0px;\" src=\"ima
-00001ae0: 6765 732f 5461 736b 2037 202d 2030 3220  ges/Task 7 - 02 
-00001af0: 4f52 4b47 2066 6561 7475 7265 732e 706e  ORKG features.pn
-00001b00: 675c 2220 7769 6474 683d 5c22 3535 255c  g\" width=\"55%\
-00001b10: 223e 5c6e 222c 0a20 2020 2022 5c6e 222c  ">\n",.    "\n",
-00001b20: 0a20 2020 2022 4279 2075 7369 6e67 2074  .    "By using t
-00001b30: 6865 205b 4f52 4b47 2069 6d70 6f72 7420  he [ORKG import 
-00001b40: 746f 6f6c 735d 2868 7474 7073 3a2f 2f6f  tools](https://o
-00001b50: 726b 672e 6f72 672f 746f 6f6c 7329 2c20  rkg.org/tools), 
-00001b60: 7468 6572 6520 6172 6520 6469 6666 6572  there are differ
-00001b70: 656e 7420 6571 7561 6c6c 7920 7669 6162  ent equally viab
-00001b80: 6c65 2077 6f72 6b66 6c6f 7773 3a5c 6e22  le workflows:\n"
-00001b90: 2c0a 2020 2020 222a 2049 6620 7468 6520  ,.    "* If the 
-00001ba0: 2a2a 7370 7265 6164 7368 6565 742a 2a20  **spreadsheet** 
-00001bb0: 636f 6e74 6169 6e73 2061 6c6c 2063 6f6c  contains all col
-00001bc0: 756d 6e73 2028 7072 6f70 6572 7469 6573  umns (properties
-00001bd0: 292c 2064 6f63 756d 656e 7473 2061 6e64  ), documents and
-00001be0: 2074 6865 6972 2072 6573 7065 6374 6976   their respectiv
-00001bf0: 6520 636f 6e74 7269 6275 7469 6f6e 7320  e contributions 
-00001c00: 2876 616c 7565 7329 2c20 7468 6520 5b63  (values), the [c
-00001c10: 7376 2d69 6d70 6f72 745d 2868 7474 7073  sv-import](https
-00001c20: 3a2f 2f6f 726b 672e 6f72 672f 6373 762d  ://orkg.org/csv-
-00001c30: 696d 706f 7274 2920 6973 2061 2076 6572  import) is a ver
-00001c40: 7920 7669 6162 6c65 2074 6f6f 6c2c 2063  y viable tool, c
-00001c50: 6f6e 7665 7274 696e 6720 6c61 7267 6520  onverting large 
-00001c60: 706f 7274 696f 6e73 206f 6620 7265 6c61  portions of rela
-00001c70: 7469 6f6e 616c 2064 6174 6120 746f 2067  tional data to g
-00001c80: 7261 7068 2073 7472 7563 7475 7265 2e5c  raph structure.\
-00001c90: 6e22 2c0a 2020 2020 222a 2049 6620 7468  n",.    "* If th
-00001ca0: 6520 2a2a 4f52 4b47 2066 6561 7475 7265  e **ORKG feature
-00001cb0: 732a 2a20 7375 6368 2061 7320 7374 7275  s** such as stru
-00001cc0: 6374 7572 6564 205b 6c69 7374 735d 2868  ctured [lists](h
-00001cd0: 7474 7073 3a2f 2f6f 726b 672e 6f72 672f  ttps://orkg.org/
-00001ce0: 6c69 7374 2f6e 6577 2920 616e 6420 5b50  list/new) and [P
-00001cf0: 4446 2074 6578 7420 616e 6e6f 7461 7469  DF text annotati
-00001d00: 6f6e 5d28 6874 7470 733a 2f2f 6f72 6b67  on](https://orkg
-00001d10: 2e6f 7267 2f70 6466 2d74 6578 742d 616e  .org/pdf-text-an
-00001d20: 6e6f 7461 7469 6f6e 2920 6172 6520 7072  notation) are pr
-00001d30: 6566 6572 6564 2c20 7468 6520 6b6e 6f77  efered, the know
-00001d40: 6c65 6467 6520 6772 6170 6820 6361 6e20  ledge graph can 
-00001d50: 616c 736f 2062 6520 7574 696c 697a 6564  also be utilized
-00001d60: 206f 6e63 6520 7468 6520 7370 7265 6164   once the spread
-00001d70: 7368 6565 7420 6d6f 6465 6c69 6e67 2073  sheet modeling s
-00001d80: 7461 676e 6174 6573 2e20 5468 6973 2061  tagnates. This a
-00001d90: 6c6c 6f77 7320 7468 6520 6372 6561 7469  llows the creati
-00001da0: 6f6e 206f 6620 6120 5b74 656d 706c 6174  on of a [templat
-00001db0: 655d 2868 7474 7073 3a2f 2f6f 726b 672e  e](https://orkg.
-00001dc0: 6f72 672f 7465 6d70 6c61 7465 2f29 2c20  org/template/), 
-00001dd0: 7374 7265 616d 6c69 6e69 6e67 2074 6865  streamlining the
-00001de0: 205b 6164 6469 6e67 5d28 6874 7470 733a   [adding](https:
-00001df0: 2f2f 6f72 6b67 2e6f 7267 2f61 6464 2d70  //orkg.org/add-p
-00001e00: 6170 6572 2920 616e 6420 5b65 6469 7469  aper) and [editi
-00001e10: 6e67 5d28 6874 7470 733a 2f2f 6f72 6b67  ng](https://orkg
-00001e20: 2e6f 7267 2f63 6f6e 7472 6962 7574 696f  .org/contributio
-00001e30: 6e2d 6564 6974 6f72 2920 6f66 2064 6f63  n-editor) of doc
-00001e40: 756d 656e 7473 2e22 0a20 2020 5d0a 2020  uments.".   ].  
-00001e50: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
-00001e60: 7479 7065 223a 2022 6d61 726b 646f 776e  type": "markdown
-00001e70: 222c 0a20 2020 226d 6574 6164 6174 6122  ",.   "metadata"
-00001e80: 3a20 7b7d 2c0a 2020 2022 736f 7572 6365  : {},.   "source
-00001e90: 223a 205b 0a20 2020 2022 2323 2320 5374  ": [.    "### St
-00001ea0: 6570 2037 2e32 2043 7261 6674 2061 7267  ep 7.2 Craft arg
-00001eb0: 756d 656e 7473 2062 6173 6564 206f 6e20  uments based on 
-00001ec0: 6669 6e64 696e 6773 5c6e 222c 0a20 2020  findings\n",.   
-00001ed0: 2022 2a2a 5265 7175 6972 656d 656e 7473   "**Requirements
-00001ee0: 3a2a 2a5c 6e22 2c0a 2020 2020 222a 2069  :**\n",.    "* i
-00001ef0: 6465 6e74 6966 7920 6576 6964 656e 6365  dentify evidence
-00001f00: 2028 6461 7461 295c 6e22 2c0a 2020 2020   (data)\n",.    
-00001f10: 222a 2065 7374 6162 6c69 7368 2077 6172  "* establish war
-00001f20: 7261 6e74 5c6e 222c 0a20 2020 2022 5c6e  rant\n",.    "\n
-00001f30: 222c 0a20 2020 2022 3c62 6c6f 636b 7175  ",.    "<blockqu
-00001f40: 6f74 653e 3c62 3e57 6172 7261 6e74 3c2f  ote><b>Warrant</
-00001f50: 623e 202d 2054 6865 2072 6561 736f 6e69  b> - The reasoni
-00001f60: 6e67 2075 7365 6420 696e 2061 6e20 6172  ng used in an ar
-00001f70: 6775 6d65 6e74 2074 6f20 616c 6c6f 7720  gument to allow 
-00001f80: 7468 6520 7265 7365 6172 6368 6572 2c20  the researcher, 
-00001f90: 616e 6420 616e 7920 7265 6164 6572 2c20  and any reader, 
-00001fa0: 746f 2061 6363 6570 7420 7468 6520 6576  to accept the ev
-00001fb0: 6964 656e 6365 2070 7265 7365 6e74 6564  idence presented
-00001fc0: 2061 7320 7265 6173 6f6e 6162 6c65 2070   as reasonable p
-00001fd0: 726f 6f66 2074 6861 7420 7468 6520 706f  roof that the po
-00001fe0: 7369 7469 6f6e 206f 6620 7468 6520 636c  sition of the cl
-00001ff0: 6169 6d20 6973 2063 6f72 7265 6374 2e3c  aim is correct.<
-00002000: 6272 3e5c 6e22 2c0a 2020 2020 222d 2d20  br>\n",.    "-- 
-00002010: 4272 656e 6461 2054 2e20 4d63 4576 6f79  Brenda T. McEvoy
-00002020: 2061 6e64 204c 6177 7265 6e63 6520 412e   and Lawrence A.
-00002030: 204d 6163 6869 3a20 3c69 3e54 6865 204c   Machi: <i>The L
-00002040: 6974 6572 6174 7572 6520 5265 7669 6577  iterature Review
-00002050: 3a20 5369 7820 5374 6570 7320 746f 2053  : Six Steps to S
-00002060: 7563 6365 7373 3c2f 693e 2c20 7061 6765  uccess</i>, page
-00002070: 2036 345c 6e22 2c0a 2020 2020 223c 2f62   64\n",.    "</b
-00002080: 6c6f 636b 7175 6f74 653e 5c6e 222c 0a20  lockquote>\n",. 
-00002090: 2020 2022 5c6e 222c 0a20 2020 2022 2a48     "\n",.    "*H
-000020a0: 696e 742a 3a20 5374 6570 2037 2e32 2061  int*: Step 7.2 a
-000020b0: 6e64 2037 2e33 2065 7370 6563 6961 6c6c  nd 7.3 especiall
-000020c0: 7920 6265 6e65 6669 7420 6672 6f6d 2061  y benefit from a
-000020d0: 6464 6974 696f 6e61 6c20 7265 6164 696e  dditional readin
-000020e0: 6720 6f66 206c 6974 6572 6174 7572 6520  g of literature 
-000020f0: 7265 7669 6577 2067 7569 6465 6c69 6e65  review guideline
-00002100: 732c 2070 726f 7669 6469 6e67 2063 6f6e  s, providing con
-00002110: 7465 7874 2066 6f72 2074 6865 2070 7265  text for the pre
-00002120: 7365 6e74 2074 6572 6d69 6e6f 6c6f 6779  sent terminology
-00002130: 2061 6e64 2072 6571 7569 7265 6d65 6e74   and requirement
-00002140: 732e 2054 6865 7265 2069 7320 6375 7272  s. There is curr
-00002150: 656e 746c 7920 6e6f 2074 6f6f 6c20 7375  ently no tool su
-00002160: 7070 6f72 7420 7072 6573 656e 7420 7769  pport present wi
-00002170: 7468 696e 2074 6865 2053 5741 524d 2d53  thin the SWARM-S
-00002180: 4c52 2c20 6d61 6b69 6e67 202a 6564 7563  LR, making *educ
-00002190: 6174 6520 7468 6520 7265 7365 6172 6368  ate the research
-000021a0: 6572 2a20 7468 6520 6265 7374 2070 7261  er* the best pra
-000021b0: 6374 6963 6520 6375 7272 656e 746c 7920  ctice currently 
-000021c0: 6176 6169 6c61 626c 652e 2052 6563 6f6d  available. Recom
-000021d0: 6d65 6e64 6174 696f 6e73 2069 6e63 6c75  mendations inclu
-000021e0: 6465 2c20 6275 7420 6172 6520 6e6f 7420  de, but are not 
-000021f0: 6c69 6d69 7465 6420 746f 3a5c 6e22 2c0a  limited to:\n",.
-00002200: 2020 2020 222a 2042 7265 6e64 6120 542e      "* Brenda T.
-00002210: 204d 6345 766f 7920 616e 6420 4c61 7772   McEvoy and Lawr
-00002220: 656e 6365 2041 2e20 4d61 6368 693a 203c  ence A. Machi: <
-00002230: 693e 5468 6520 4c69 7465 7261 7475 7265  i>The Literature
-00002240: 2052 6576 6965 773a 2053 6978 2053 7465   Review: Six Ste
-00002250: 7073 2074 6f20 5375 6363 6573 733c 2f69  ps to Success</i
-00002260: 3e2c 2070 6167 6520 3634 2074 6f20 3133  >, page 64 to 13
-00002270: 335c 6e22 2c0a 2020 2020 222a 2048 6967  3\n",.    "* Hig
-00002280: 6769 6e73 204a 5054 2c20 5468 6f6d 6173  gins JPT, Thomas
-00002290: 204a 2c20 4368 616e 646c 6572 204a 2c20   J, Chandler J, 
-000022a0: 4375 6d70 7374 6f6e 204d 2c20 4c69 2054  Cumpston M, Li T
-000022b0: 2c20 5061 6765 204d 4a2c 2057 656c 6368  , Page MJ, Welch
-000022c0: 2056 4120 2865 6469 746f 7273 292e 2043   VA (editors). C
-000022d0: 6f63 6872 616e 6520 4861 6e64 626f 6f6b  ochrane Handbook
-000022e0: 2066 6f72 2053 7973 7465 6d61 7469 6320   for Systematic 
-000022f0: 5265 7669 6577 7320 6f66 2049 6e74 6572  Reviews of Inter
-00002300: 7665 6e74 696f 6e73 2076 6572 7369 6f6e  ventions version
-00002310: 2036 2e34 2028 7570 6461 7465 6420 4175   6.4 (updated Au
-00002320: 6775 7374 2032 3032 3329 2e20 436f 6368  gust 2023). Coch
-00002330: 7261 6e65 2c20 3230 3233 2e20 4176 6169  rane, 2023. Avai
-00002340: 6c61 626c 6520 6672 6f6d 205b 7777 772e  lable from [www.
-00002350: 7472 6169 6e69 6e67 2e63 6f63 6872 616e  training.cochran
-00002360: 652e 6f72 672f 6861 6e64 626f 6f6b 5d28  e.org/handbook](
-00002370: 7777 772e 7472 6169 6e69 6e67 2e63 6f63  www.training.coc
-00002380: 6872 616e 652e 6f72 672f 6861 6e64 626f  hrane.org/handbo
-00002390: 6f6b 292e 5c6e 222c 0a20 2020 2022 5c6e  ok).\n",.    "\n
-000023a0: 222c 0a20 2020 2022 5c6e 222c 0a20 2020  ",.    "\n",.   
-000023b0: 2022 5769 7468 2061 6c6c 2072 6571 7569   "With all requi
-000023c0: 7265 6420 6461 7461 206e 6f77 2070 7265  red data now pre
-000023d0: 7365 6e74 2069 6e20 6d61 6368 696e 652d  sent in machine-
-000023e0: 7265 6164 6162 6c65 2066 6f72 6d2c 2061  readable form, a
-000023f0: 7267 756d 656e 7473 2063 616e 2062 6520  rguments can be 
-00002400: 6372 6166 7465 642e 2045 6163 6820 6172  crafted. Each ar
-00002410: 6775 6d65 6e74 2072 6571 7569 7265 7320  gument requires 
-00002420: 6461 7461 2c20 6176 6169 6c61 626c 6520  data, available 
-00002430: 7468 726f 7567 6820 7468 6520 636f 6e74  through the cont
-00002440: 7269 6275 7469 6f6e 732c 2061 6e64 2063  ributions, and c
-00002450: 616e 2062 6520 7761 7272 616e 7465 6420  an be warranted 
-00002460: 7468 726f 7567 6820 6c69 7374 732c 2063  through lists, c
-00002470: 6f6d 7061 7269 736f 6e73 2c20 7669 7375  omparisons, visu
-00002480: 616c 697a 6174 696f 6e73 2c20 7265 7669  alizations, revi
-00002490: 6577 7320 616e 6420 7369 6d69 6c61 7220  ews and similar 
-000024a0: 746f 6f6c 7320 6465 7369 676e 6564 2074  tools designed t
-000024b0: 6f20 7379 6e74 6865 7369 7a65 2064 6174  o synthesize dat
-000024c0: 612e 5c6e 222c 0a20 2020 2022 5c6e 222c  a.\n",.    "\n",
-000024d0: 0a20 2020 2022 2323 2323 2045 7861 6d70  .    "#### Examp
-000024e0: 6c65 5c6e 222c 0a20 2020 2022 2a20 2a43  le\n",.    "* *C
-000024f0: 6c61 696d 2a3a 2058 4d4c 2069 7320 6e6f  laim*: XML is no
-00002500: 7420 7265 7175 6972 6564 2074 6f20 7265  t required to re
-00002510: 7072 6573 656e 7420 616e 6420 6578 6368  present and exch
-00002520: 616e 6765 2061 6572 6f73 7061 6365 2065  ange aerospace e
-00002530: 6e67 696e 6565 7269 6e67 2073 7973 7465  ngineering syste
-00002540: 6d20 7374 7275 6374 7572 6573 2e5c 6e22  m structures.\n"
-00002550: 2c0a 2020 2020 222a 202a 4576 6964 656e  ,.    "* *Eviden
-00002560: 6365 2a3a 2038 3220 6469 6666 6572 656e  ce*: 82 differen
-00002570: 7420 646f 6375 6d65 6e74 7320 7265 706f  t documents repo
-00002580: 7274 696e 6720 6f6e 2061 6572 6f73 7061  rting on aerospa
-00002590: 6365 2065 6e67 696e 6565 7273 2065 7863  ce engineers exc
-000025a0: 6861 6e67 696e 6720 7379 7374 656d 2073  hanging system s
-000025b0: 7472 7563 7475 7265 732e 2031 3720 6f66  tructures. 17 of
-000025c0: 2074 6865 6d20 6469 6420 6e6f 7420 7573   them did not us
-000025d0: 6520 584d 4c2e 220a 2020 205d 0a20 207d  e XML.".   ].  }
-000025e0: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
-000025f0: 7970 6522 3a20 226d 6172 6b64 6f77 6e22  ype": "markdown"
-00002600: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
-00002610: 207b 7d2c 0a20 2020 2273 6f75 7263 6522   {},.   "source"
-00002620: 3a20 5b0a 2020 2020 2223 2323 2053 7465  : [.    "### Ste
-00002630: 7020 372e 3320 4372 6974 6971 7565 2074  p 7.3 Critique t
-00002640: 6865 206c 6974 6572 6174 7572 655c 6e22  he literature\n"
-00002650: 2c0a 2020 2020 222a 2a52 6571 7569 7265  ,.    "**Require
-00002660: 6d65 6e74 733a 2a2a 5c6e 222c 0a20 2020  ments:**\n",.   
-00002670: 2022 2a20 6964 656e 7469 6679 2065 7669   "* identify evi
-00002680: 6465 6e63 6520 2863 6c61 696d 7329 5c6e  dence (claims)\n
-00002690: 222c 0a20 2020 2022 2a20 6964 656e 7469  ",.    "* identi
-000026a0: 6679 2070 6174 7465 726e 735c 6e22 2c0a  fy patterns\n",.
-000026b0: 2020 2020 222a 2064 6574 6563 7420 6661      "* detect fa
-000026c0: 6c6c 6163 6965 735c 6e22 2c0a 2020 2020  llacies\n",.    
-000026d0: 222a 2069 6465 6e74 6966 7920 636f 6e66  "* identify conf
-000026e0: 6c69 6374 735c 6e22 2c0a 2020 2020 222a  licts\n",.    "*
-000026f0: 2072 6573 6f6c 7665 2063 6f6e 666c 6963   resolve conflic
-00002700: 7473 205c 6e22 2c0a 2020 2020 225c 6e22  ts \n",.    "\n"
-00002710: 2c0a 2020 2020 2245 6163 6820 636c 6169  ,.    "Each clai
-00002720: 6d20 6e6f 7720 6265 636f 6d65 7320 6576  m now becomes ev
-00002730: 6964 656e 6365 2069 6e20 6974 7365 6c66  idence in itself
-00002740: 2e20 4861 7669 6e67 2063 6f6c 6c65 6374  . Having collect
-00002750: 6564 2061 6e64 2073 7570 706f 7274 6564  ed and supported
-00002760: 206d 756c 7469 706c 6520 636c 6169 6d73   multiple claims
-00002770: 2c20 7468 6579 206d 6179 2073 686f 7720  , they may show 
-00002780: 7061 7474 6572 6e73 2c20 652e 672e 206f  patterns, e.g. o
-00002790: 6620 636f 7272 656c 6174 696f 6e20 6f72  f correlation or
-000027a0: 2063 6175 7361 7469 6f6e 2e20 5468 6973   causation. This
-000027b0: 2061 6c6c 6f77 7320 7468 6520 696e 6665   allows the infe
-000027c0: 7265 6e63 6520 6f66 206e 6577 202a 6d65  rence of new *me
-000027d0: 7461 2063 6c61 696d 732a 2c20 7573 696e  ta claims*, usin
-000027e0: 6720 7468 6573 6520 6e6f 7720 7375 7070  g these now supp
-000027f0: 6f72 7465 6420 636c 6169 6d73 2061 7320  orted claims as 
-00002800: 7468 6569 7220 6576 6964 656e 6365 2e20  their evidence. 
-00002810: 5468 6573 6520 636c 6169 6d73 2061 6e64  These claims and
-00002820: 206d 6574 612d 636c 6169 6d73 2073 686f   meta-claims sho
-00002830: 756c 6420 6265 2063 6865 636b 6564 2061  uld be checked a
-00002840: 6761 696e 2066 6f72 2066 616c 6c61 6369  gain for fallaci
-00002850: 6f75 7320 7265 6173 6f6e 696e 6720 616e  ous reasoning an
-00002860: 6420 636f 6e66 6c69 6374 7320 746f 2061  d conflicts to a
-00002870: 7373 7572 6520 696e 7465 726e 616c 2063  ssure internal c
-00002880: 6f6e 7369 7374 656e 6379 206f 6620 616c  onsistency of al
-00002890: 6c20 636c 6169 6d73 2061 6e64 2065 7669  l claims and evi
-000028a0: 6465 6e63 652e 5c6e 222c 0a20 2020 2022  dence.\n",.    "
-000028b0: 5c6e 222c 0a20 2020 2022 2323 2323 2045  \n",.    "#### E
-000028c0: 7861 6d70 6c65 5c6e 222c 0a20 2020 2022  xample\n",.    "
-000028d0: 2a20 2a43 6c61 696d 2a3a 2041 6572 6f73  * *Claim*: Aeros
-000028e0: 7061 6365 2065 6e67 696e 6565 7273 2063  pace engineers c
-000028f0: 616e 2075 7365 2076 6172 696f 7573 206b  an use various k
-00002900: 6e6f 776c 6564 6765 2072 6570 7265 7365  nowledge represe
-00002910: 6e74 6174 696f 6e73 2074 6f20 7265 7072  ntations to repr
-00002920: 6573 656e 7420 616e 6420 6578 6368 616e  esent and exchan
-00002930: 6765 2074 6865 6972 2073 7973 7465 6d20  ge their system 
-00002940: 7374 7275 6374 7572 6573 2074 6f20 7461  structures to ta
-00002950: 696c 6f72 2074 6f20 7468 6569 7220 7370  ilor to their sp
-00002960: 6563 6966 6963 2073 6974 7561 7469 6f6e  ecific situation
-00002970: 2e5c 6e22 2c0a 2020 2020 222a 202a 4576  .\n",.    "* *Ev
-00002980: 6964 656e 6365 2a3a 5c6e 222c 0a20 2020  idence*:\n",.   
-00002990: 2022 2020 2a20 584d 4c20 6973 206e 6f74   "  * XML is not
-000029a0: 2072 6571 7569 7265 6420 746f 2072 6570   required to rep
-000029b0: 7265 7365 6e74 2061 6e64 2065 7863 6861  resent and excha
-000029c0: 6e67 6520 6165 726f 7370 6163 6520 656e  nge aerospace en
-000029d0: 6769 6e65 6572 696e 6720 7379 7374 656d  gineering system
-000029e0: 2073 7472 7563 7475 7265 732e 5c6e 222c   structures.\n",
-000029f0: 0a20 2020 2022 2020 2a20 5379 734d 4c20  .    "  * SysML 
-00002a00: 6973 2075 7365 6420 6279 2061 6572 6f73  is used by aeros
-00002a10: 7061 6365 2065 6e67 696e 6565 7273 2074  pace engineers t
-00002a20: 6f20 7265 7072 6573 656e 7420 7379 7374  o represent syst
-00002a30: 656d 2073 7472 7563 7475 7265 732e 5c6e  em structures.\n
-00002a40: 222c 0a20 2020 2022 2020 2a20 5244 4620  ",.    "  * RDF 
-00002a50: 6361 6e20 7265 7072 6573 656e 7420 636f  can represent co
-00002a60: 6d70 6c65 7820 7379 7374 656d 732c 2073  mplex systems, s
-00002a70: 7570 706f 7274 696e 6720 6469 6666 6572  upporting differ
-00002a80: 656e 7420 7365 7269 616c 697a 6174 696f  ent serializatio
-00002a90: 6e20 666f 726d 6174 732e 5c6e 220a 2020  n formats.\n".  
-00002aa0: 205d 0a20 207d 0a20 5d2c 0a20 226d 6574   ].  }. ],. "met
-00002ab0: 6164 6174 6122 3a20 7b0a 2020 226c 616e  adata": {.  "lan
-00002ac0: 6775 6167 655f 696e 666f 223a 207b 0a20  guage_info": {. 
-00002ad0: 2020 226e 616d 6522 3a20 2270 7974 686f    "name": "pytho
-00002ae0: 6e22 0a20 207d 0a20 7d2c 0a20 226e 6266  n".  }. },. "nbf
-00002af0: 6f72 6d61 7422 3a20 342c 0a20 226e 6266  ormat": 4,. "nbf
-00002b00: 6f72 6d61 745f 6d69 6e6f 7222 3a20 320a  ormat_minor": 2.
-00002b10: 7d0a                                     }.
+00000000: 7b0d 0a20 2263 656c 6c73 223a 205b 0d0a  {.. "cells": [..
+00000010: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
+00000020: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
+00000030: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
+00000040: 207b 7d2c 0d0a 2020 2022 736f 7572 6365   {},..   "source
+00000050: 223a 205b 0d0a 2020 2020 2223 2053 7461  ": [..    "# Sta
+00000060: 6765 2049 4949 5c6e 222c 0d0a 2020 2020  ge III\n",..    
+00000070: 2254 6869 7320 7374 6167 6520 6973 2061  "This stage is a
+00000080: 7420 7468 6520 6865 6172 7420 6f66 2061  t the heart of a
+00000090: 206c 6974 6572 6174 7572 6520 7265 7669   literature revi
+000000a0: 6577 2e20 4974 2069 7320 7768 6572 6520  ew. It is where 
+000000b0: 6e65 7720 696e 666f 726d 6174 696f 6e20  new information 
+000000c0: 6973 2064 6572 6976 6564 2061 6e64 2073  is derived and s
+000000d0: 796e 7468 6573 697a 6564 2e20 5768 696c  ynthesized. Whil
+000000e0: 6520 746f 6f6c 7320 6361 6e20 6173 7369  e tools can assi
+000000f0: 7374 2069 6e20 696e 666f 726d 6174 696f  st in informatio
+00000100: 6e20 6578 7472 6163 7469 6f6e 2061 6e64  n extraction and
+00000110: 2020 7374 7275 6374 7572 696e 6720 7468    structuring th
+00000120: 6973 2069 6e66 6f72 6d61 7469 6f6e 2c20  is information, 
+00000130: 7468 6520 7265 7365 6172 6368 6572 7320  the researchers 
+00000140: 696e 7369 6768 7420 6973 2064 6566 696e  insight is defin
+00000150: 696e 6720 7468 6973 2073 7461 6765 2e5c  ing this stage.\
+00000160: 6e22 2c0d 0a20 2020 2022 5c6e 222c 0d0a  n",..    "\n",..
+00000170: 2020 2020 222a 2a57 6f72 6b6c 6f61 6420      "**Workload 
+00000180: 6469 7374 7269 6275 7469 6f6e 2a2a 5c6e  distribution**\n
+00000190: 222c 0d0a 2020 2020 225c 6e22 2c0d 0a20  ",..    "\n",.. 
+000001a0: 2020 2022 7c41 6374 6f72 7c54 696d 657c     "|Actor|Time|
+000001b0: 5c6e 222c 0d0a 2020 2020 227c 3a2d 2d2d  \n",..    "|:---
+000001c0: 2d7c 3a2d 2d2d 2d7c 5c6e 222c 0d0a 2020  -|:----|\n",..  
+000001d0: 2020 227c 5265 7365 6172 6368 6572 7c3f    "|Researcher|?
+000001e0: 206d 696e 7c5c 6e22 2c0d 0a20 2020 2022   min|\n",..    "
+000001f0: 5c6e 222c 0d0a 2020 2020 222a 2a54 6f6f  \n",..    "**Too
+00000200: 6c73 2a2a 5c6e 222c 0d0a 2020 2020 222a  ls**\n",..    "*
+00000210: 2052 6573 6561 7263 6820 416e 6e6f 7461   Research Annota
+00000220: 7469 6f6e 2044 6174 6162 6173 6520 2865  tion Database (e
+00000230: 2e67 2e20 5b4f 524b 475d 2868 7474 7073  .g. [ORKG](https
+00000240: 3a2f 2f6f 726b 672e 6f72 672f 2929 5c6e  ://orkg.org/))\n
+00000250: 222c 0d0a 2020 2020 222a 204d 6172 6b64  ",..    "* Markd
+00000260: 6f77 6e20 6669 6c65 2076 6965 7765 7220  own file viewer 
+00000270: 2865 2e67 2e20 5b4f 6273 6964 6961 6e5d  (e.g. [Obsidian]
+00000280: 2868 7474 7073 3a2f 2f6f 6273 6964 6961  (https://obsidia
+00000290: 6e2e 6d64 2f29 2077 6974 6820 5b44 6174  n.md/) with [Dat
+000002a0: 6176 6965 775d 2868 7474 7073 3a2f 2f67  aview](https://g
+000002b0: 6974 6875 622e 636f 6d2f 626c 6163 6b73  ithub.com/blacks
+000002c0: 6d69 7468 6775 2f6f 6273 6964 6961 6e2d  mithgu/obsidian-
+000002d0: 6461 7461 7669 6577 2920 706c 7567 696e  dataview) plugin
+000002e0: 2922 0d0a 2020 205d 0d0a 2020 7d2c 0d0a  )"..   ]..  },..
+000002f0: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
+00000300: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
+00000310: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
+00000320: 207b 7d2c 0d0a 2020 2022 736f 7572 6365   {},..   "source
+00000330: 223a 205b 0d0a 2020 2020 2223 2320 5461  ": [..    "## Ta
+00000340: 736b 2036 3a20 416e 616c 7973 6973 5c6e  sk 6: Analysis\n
+00000350: 222c 0d0a 2020 2020 225c 6e22 2c0d 0a20  ",..    "\n",.. 
+00000360: 2020 2022 7c53 7465 707c 5265 7375 6c74     "|Step|Result
+00000370: 7c52 6571 7569 7265 6d65 6e74 7c5c 6e22  |Requirement|\n"
+00000380: 2c0d 0a20 2020 2022 7c3a 2d2d 2d2d 7c3a  ,..    "|:----|:
+00000390: 2d2d 2d2d 7c3a 2d2d 2d2d 7c5c 6e22 2c0d  ----|:----|\n",.
+000003a0: 0a20 2020 2022 7c52 6573 6f75 7263 6520  .    "|Resource 
+000003b0: 616e 6e6f 7461 7469 6f6e 7c63 6f6e 7472  annotation|contr
+000003c0: 6962 7574 696f 6e20 7265 7072 6573 656e  ibution represen
+000003d0: 7461 7469 6f6e 7c34 392e 2061 6e6e 6f74  tation|49. annot
+000003e0: 6174 6520 7468 6520 646f 6375 6d65 6e74  ate the document
+000003f0: 3c62 723e 3530 2e20 7265 7072 6573 656e  <br>50. represen
+00000400: 7420 7468 6520 616e 6e6f 7461 7469 6f6e  t the annotation
+00000410: 206d 6163 6869 6e65 2d72 6561 6461 626c   machine-readabl
+00000420: 653c 6272 3e35 312e 2061 6e6e 6f74 6174  e<br>51. annotat
+00000430: 6520 636f 6c6c 6162 6f72 6174 6976 656c  e collaborativel
+00000440: 797c 5c6e 220d 0a20 2020 5d0d 0a20 207d  y|\n"..   ]..  }
+00000450: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
+00000460: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
+00000470: 6e22 2c0d 0a20 2020 226d 6574 6164 6174  n",..   "metadat
+00000480: 6122 3a20 7b7d 2c0d 0a20 2020 2273 6f75  a": {},..   "sou
+00000490: 7263 6522 3a20 5b0d 0a20 2020 2022 2323  rce": [..    "##
+000004a0: 2320 5374 6570 2036 2e31 2052 6573 6f75  # Step 6.1 Resou
+000004b0: 7263 6520 616e 6e6f 7461 7469 6f6e 5c6e  rce annotation\n
+000004c0: 222c 0d0a 2020 2020 222a 2a52 6571 7569  ",..    "**Requi
+000004d0: 7265 6d65 6e74 733a 2a2a 5c6e 222c 0d0a  rements:**\n",..
+000004e0: 2020 2020 222a 2061 6e6e 6f74 6174 6520      "* annotate 
+000004f0: 7468 6520 646f 6375 6d65 6e74 5c6e 222c  the document\n",
+00000500: 0d0a 2020 2020 222a 2072 6570 7265 7365  ..    "* represe
+00000510: 6e74 2074 6865 2061 6e6e 6f74 6174 696f  nt the annotatio
+00000520: 6e20 6d61 6368 696e 652d 7265 6164 6162  n machine-readab
+00000530: 6c65 5c6e 222c 0d0a 2020 2020 222a 2061  le\n",..    "* a
+00000540: 6e6e 6f74 6174 6520 636f 6c6c 6162 6f72  nnotate collabor
+00000550: 6174 6976 656c 795c 6e22 2c0d 0a20 2020  atively\n",..   
+00000560: 2022 5c6e 222c 0d0a 2020 2020 2257 6869   "\n",..    "Whi
+00000570: 6c65 2074 6869 7320 7374 6570 2070 7574  le this step put
+00000580: 7320 656d 7068 6173 6973 206f 6e20 7374  s emphasis on st
+00000590: 7275 6374 7572 6564 2061 6e6e 6f74 6174  ructured annotat
+000005a0: 696f 6e2c 2069 7420 6973 2061 6476 6973  ion, it is advis
+000005b0: 6564 2074 6f20 7374 6172 7420 6120 7369  ed to start a si
+000005c0: 676e 6966 6963 616e 7420 706f 7274 696f  gnificant portio
+000005d0: 6e20 6f66 2074 6865 2077 6f72 6b20 696e  n of the work in
+000005e0: 2061 2066 6c65 7869 626c 6520 656e 7669   a flexible envi
+000005f0: 726f 6e6d 656e 742e 2044 7572 696e 6720  ronment. During 
+00000600: 7468 6520 636f 7572 7365 206f 6620 6578  the course of ex
+00000610: 7472 6163 7469 6e67 2069 6e66 6f72 6d61  tracting informa
+00000620: 7469 6f6e 2c20 7468 6520 7374 7275 6374  tion, the struct
+00000630: 7572 6520 7265 7175 6972 6564 2074 6f20  ure required to 
+00000640: 6265 7374 2072 6570 7265 7365 6e74 2074  best represent t
+00000650: 6869 7320 696e 666f 726d 6174 696f 6e20  his information 
+00000660: 6973 206c 696b 656c 7920 746f 2063 6861  is likely to cha
+00000670: 6e67 6520 6974 6572 6174 6976 656c 792e  nge iteratively.
+00000680: 205c 6e22 2c0d 0a20 2020 2022 5c6e 222c   \n",..    "\n",
+00000690: 0d0a 2020 2020 227c 5374 6570 7c50 4446  ..    "|Step|PDF
+000006a0: 2072 6561 6465 723c 6272 3e65 2e67 2e20   reader<br>e.g. 
+000006b0: 5b41 6372 6f62 6174 2052 6561 6465 725d  [Acrobat Reader]
+000006c0: 2868 7474 7073 3a2f 2f77 7777 2e61 646f  (https://www.ado
+000006d0: 6265 2e63 6f6d 2f64 652f 6163 726f 6261  be.com/de/acroba
+000006e0: 742f 7064 662d 7265 6164 6572 2e68 746d  t/pdf-reader.htm
+000006f0: 6c29 7c4d 6172 6b64 6f77 6e20 6564 6974  l)|Markdown edit
+00000700: 6f72 3c62 723e 652e 672e 205b 4f62 7369  or<br>e.g. [Obsi
+00000710: 6469 616e 5d28 6874 7470 733a 2f2f 6f62  dian](https://ob
+00000720: 7369 6469 616e 2e6d 642f 297c 5370 7265  sidian.md/)|Spre
+00000730: 6164 7368 6565 7420 6564 6974 6f72 3c62  adsheet editor<b
+00000740: 723e 652e 672e 205b 4578 6365 6c5d 2868  r>e.g. [Excel](h
+00000750: 7474 7073 3a2f 2f77 7777 2e6d 6963 726f  ttps://www.micro
+00000760: 736f 6674 2e63 6f6d 2f64 652d 6465 2f6d  soft.com/de-de/m
+00000770: 6963 726f 736f 6674 2d33 3635 2f65 7863  icrosoft-365/exc
+00000780: 656c 292c 205b 476f 6f67 6c65 2053 6865  el), [Google She
+00000790: 6574 735d 2868 7474 7073 3a2f 2f64 6f63  ets](https://doc
+000007a0: 732e 676f 6f67 6c65 2e63 6f6d 2f73 7072  s.google.com/spr
+000007b0: 6561 6473 6865 6574 7329 7c4b 6f6e 776c  eadsheets)|Konwl
+000007c0: 6564 6765 2067 7261 7068 2065 6469 746f  edge graph edito
+000007d0: 723c 6272 3e65 2e67 2e20 5b4f 524b 475d  r<br>e.g. [ORKG]
+000007e0: 2868 7474 7073 3a2f 2f6f 726b 672e 6f72  (https://orkg.or
+000007f0: 672f 297c 5c6e 222c 0d0a 2020 2020 227c  g/)|\n",..    "|
+00000800: 3a2d 2d2d 2d7c 3a2d 2d2d 2d7c 3a2d 2d2d  :----|:----|:---
+00000810: 2d7c 3a2d 2d2d 2d7c 3a2d 2d2d 2d7c 5c6e  -|:----|:----|\n
+00000820: 222c 0d0a 2020 2020 227c 6561 7365 206f  ",..    "|ease o
+00000830: 6620 7573 657c 2b2b 7c2b 7c2b 2b7c 2b2d  f use|++|+|++|+-
+00000840: 7c5c 6e22 2c0d 0a20 2020 2022 7c66 6c65  |\n",..    "|fle
+00000850: 7869 626c 6520 666f 726d 6174 7c2d 7c2b  xible format|-|+
+00000860: 2b7c 2b7c 2b2d 7c5c 6e22 2c0d 0a20 2020  +|+|+-|\n",..   
+00000870: 2022 7c73 7472 7563 7475 7265 6420 6461   "|structured da
+00000880: 7461 7c2d 7c2b 2d7c 2b7c 2b2b 7c5c 6e22  ta|-|+-|+|++|\n"
+00000890: 2c0d 0a20 2020 2022 7c69 6e74 6572 6f70  ,..    "|interop
+000008a0: 6572 6162 6c65 2064 6174 617c 2d2d 7c2d  erable data|--|-
+000008b0: 2d7c 2b2b 7c2b 2b7c 5c6e 222c 0d0a 2020  -|++|++|\n",..  
+000008c0: 2020 227c 636f 6c6c 6162 6f72 6174 6976    "|collaborativ
+000008d0: 6520 616e 6e6f 7461 7469 6f6e 7c2d 2d7c  e annotation|--|
+000008e0: 2d2d 7c2b 2d7c 2b2b 7c5c 6e22 2c0d 0a20  --|+-|++|\n",.. 
+000008f0: 2020 2022 5c6e 222c 0d0a 2020 2020 2253     "\n",..    "S
+00000900: 5741 524d 2d53 4c52 2061 6476 6973 6573  WARM-SLR advises
+00000910: 2074 6f20 776f 726b 2075 7365 2061 2076   to work use a v
+00000920: 6172 6965 7479 206f 6620 746f 6f6c 7320  ariety of tools 
+00000930: 616e 6420 776f 726b 2074 6f77 6172 6473  and work towards
+00000940: 206d 6f72 6520 7374 7275 6374 7572 6564   more structured
+00000950: 2064 6174 612c 2077 6869 6c65 206d 616b   data, while mak
+00000960: 696e 6720 7573 6520 6f66 2065 6173 6520  ing use of ease 
+00000970: 6f66 2075 7365 2061 6e64 2066 6c65 7869  of use and flexi
+00000980: 6269 6c69 7479 3a5c 6e22 2c0d 0a20 2020  bility:\n",..   
+00000990: 2022 5c6e 222c 0d0a 2020 2020 223c 6469   "\n",..    "<di
+000009a0: 7620 616c 6967 6e3d 5c22 6365 6e74 6572  v align=\"center
+000009b0: 5c22 3e5c 6e22 2c0d 0a20 2020 2022 3c69  \">\n",..    "<i
+000009c0: 6d67 2073 7263 3d5c 2269 6d61 6765 732f  mg src=\"images/
+000009d0: 5461 736b 2036 202d 2030 3120 4f62 7369  Task 6 - 01 Obsi
+000009e0: 6469 616e 2052 512e 706e 675c 2220 7769  dian RQ.png\" wi
+000009f0: 6474 683d 5c22 3935 255c 2220 2f3e 5c6e  dth=\"95%\" />\n
+00000a00: 222c 0d0a 2020 2020 223c 6669 6763 6170  ",..    "<figcap
+00000a10: 7469 6f6e 3e4f 6273 6964 6961 6e20 6f76  tion>Obsidian ov
+00000a20: 6572 7669 6577 206f 6620 7468 6520 616e  erview of the an
+00000a30: 616c 797a 6564 206c 6962 7261 7279 2e20  alyzed library. 
+00000a40: 5468 6520 7269 6768 7420 7369 6465 2064  The right side d
+00000a50: 6570 6963 7473 2074 6865 2064 6f63 756d  epicts the docum
+00000a60: 656e 7473 2028 6e6f 6465 7329 2061 6e64  ents (nodes) and
+00000a70: 2074 6865 6972 2073 696d 696c 6172 6974   their similarit
+00000a80: 7920 746f 206f 7468 6572 2064 6f63 756d  y to other docum
+00000a90: 656e 7473 2028 6564 6765 7329 2e20 5468  ents (edges). Th
+00000aa0: 6520 6e6f 6465 7320 6172 6520 636f 6c6f  e nodes are colo
+00000ab0: 7265 6420 6261 7365 6420 6f6e 2074 6865  red based on the
+00000ac0: 6972 2072 656c 6576 616e 6365 206f 6e20  ir relevance on 
+00000ad0: 6176 6572 6167 6520 2867 7265 656e 292c  average (green),
+00000ae0: 206f 7220 746f 2061 2072 6573 6561 7263   or to a researc
+00000af0: 6820 7175 6573 7469 6f6e 2028 5251 2920  h question (RQ) 
+00000b00: 2868 6572 653a 2052 5131 2072 6564 2c20  (here: RQ1 red, 
+00000b10: 5251 3220 626c 7565 292e 2054 6865 206c  RQ2 blue). The l
+00000b20: 6566 7420 7369 6465 2073 686f 7773 2074  eft side shows t
+00000b30: 6865 2052 5131 2d66 696c 652e 2045 6163  he RQ1-file. Eac
+00000b40: 6820 5251 2072 6570 7265 7365 6e74 6174  h RQ representat
+00000b50: 696f 6e20 6469 7370 6c61 7973 2074 6865  ion displays the
+00000b60: 2064 6f63 756d 656e 7473 2074 6861 7420   documents that 
+00000b70: 7363 6f72 6564 2068 6967 6865 7374 2066  scored highest f
+00000b80: 6f72 2074 6865 2052 5127 7320 7265 7370  or the RQ's resp
+00000b90: 6563 7469 7665 2077 6569 6768 6564 206b  ective weighed k
+00000ba0: 6579 776f 7264 732e 3c2f 6669 6763 6170  eywords.</figcap
+00000bb0: 7469 6f6e 3e5c 6e22 2c0d 0a20 2020 2022  tion>\n",..    "
+00000bc0: 3c2f 6469 763e 5c6e 222c 0d0a 2020 2020  </div>\n",..    
+00000bd0: 225c 6e22 2c0d 0a20 2020 2022 3c62 723e  "\n",..    "<br>
+00000be0: 5c6e 222c 0d0a 2020 2020 225c 6e22 2c0d  \n",..    "\n",.
+00000bf0: 0a20 2020 2022 3c64 6976 2061 6c69 676e  .    "<div align
+00000c00: 3d5c 2263 656e 7465 725c 223e 5c6e 222c  =\"center\">\n",
+00000c10: 0d0a 2020 2020 223c 696d 6720 7372 633d  ..    "<img src=
+00000c20: 5c22 696d 6167 6573 2f54 6173 6b20 3620  \"images/Task 6 
+00000c30: 2d20 3032 204f 6273 6964 6961 6e20 446f  - 02 Obsidian Do
+00000c40: 6375 6d65 6e74 2e70 6e67 5c22 2077 6964  cument.png\" wid
+00000c50: 7468 3d5c 2239 3525 5c22 202f 3e5c 6e22  th=\"95%\" />\n"
+00000c60: 2c0d 0a20 2020 2022 3c66 6967 6361 7074  ,..    "<figcapt
+00000c70: 696f 6e3e 4f62 7369 6469 616e 2064 6f63  ion>Obsidian doc
+00000c80: 756d 656e 7420 7669 6577 2e20 5468 6520  ument view. The 
+00000c90: 6c65 6674 2073 6964 6520 6469 7370 6c61  left side displa
+00000ca0: 7973 2061 2064 6f63 756d 656e 742d 7265  ys a document-re
+00000cb0: 7072 6573 656e 7461 7469 6f6e 2c20 636f  presentation, co
+00000cc0: 6e74 6169 6e69 6e67 206d 6574 6164 6174  ntaining metadat
+00000cd0: 612c 2065 7874 7261 6374 6564 2069 6e66  a, extracted inf
+00000ce0: 6f72 6d61 7469 6f6e 2061 6e64 2061 6e20  ormation and an 
+00000cf0: 656d 6265 6464 6564 2066 696c 6520 7669  embedded file vi
+00000d00: 6577 6572 2e20 5468 6973 2064 6f63 756d  ewer. This docum
+00000d10: 656e 7420 6361 6e20 6265 2075 7365 6420  ent can be used 
+00000d20: 746f 2061 6e6e 6f74 6174 652c 2063 7265  to annotate, cre
+00000d30: 6174 6520 616e 6420 6c69 6e6b 2061 6e79  ate and link any
+00000d40: 2066 6f72 6d20 6f66 2064 6967 6974 616c   form of digital
+00000d50: 2061 6e6e 6f74 6174 696f 6e2c 2073 7563   annotation, suc
+00000d60: 6820 6173 2073 6372 6565 6e73 686f 7473  h as screenshots
+00000d70: 2c20 6772 6170 6869 6373 2c20 6361 6c63  , graphics, calc
+00000d80: 756c 6174 696f 6e73 2c20 6c69 6e6b 732c  ulations, links,
+00000d90: 2065 7463 2e3c 2f66 6967 6361 7074 696f   etc.</figcaptio
+00000da0: 6e3e 5c6e 222c 0d0a 2020 2020 223c 2f64  n>\n",..    "</d
+00000db0: 6976 3e5c 6e22 2c0d 0a20 2020 2022 5c6e  iv>\n",..    "\n
+00000dc0: 222c 0d0a 2020 2020 223c 6272 3e5c 6e22  ",..    "<br>\n"
+00000dd0: 2c0d 0a20 2020 2022 5c6e 222c 0d0a 2020  ,..    "\n",..  
+00000de0: 2020 223c 6469 7620 616c 6967 6e3d 5c22    "<div align=\"
+00000df0: 6365 6e74 6572 5c22 3e5c 6e22 2c0d 0a20  center\">\n",.. 
+00000e00: 2020 2022 3c69 6d67 2073 7263 3d5c 2269     "<img src=\"i
+00000e10: 6d61 6765 732f 5461 736b 2036 202d 2030  mages/Task 6 - 0
+00000e20: 3320 4f62 7369 6469 616e 2054 6f74 616c  3 Obsidian Total
+00000e30: 2e70 6e67 5c22 2077 6964 7468 3d5c 2239  .png\" width=\"9
+00000e40: 3525 5c22 202f 3e5c 6e22 2c0d 0a20 2020  5%\" />\n",..   
+00000e50: 2022 3c66 6967 6361 7074 696f 6e3e 4f62   "<figcaption>Ob
+00000e60: 7369 6469 616e 2070 726f 6772 6573 7320  sidian progress 
+00000e70: 7472 6163 6b69 6e67 2e20 5468 6520 6c65  tracking. The le
+00000e80: 6674 2073 6964 6520 7368 6f77 7320 6d6f  ft side shows mo
+00000e90: 7265 206f 6620 7468 6520 6120 646f 6375  re of the a docu
+00000ea0: 6d65 6e74 2d72 6570 7265 7365 6e74 6174  ment-representat
+00000eb0: 696f 6e2c 2077 6869 6368 2061 6c73 6f20  ion, which also 
+00000ec0: 6c69 7374 7320 7468 6520 6d6f 7374 2073  lists the most s
+00000ed0: 696d 696c 6172 2064 6f63 756d 656e 7473  imilar documents
+00000ee0: 2061 6e64 2074 6865 6972 2072 6573 7065   and their respe
+00000ef0: 6374 6976 6520 7363 6f72 6573 2e20 5468  ctive scores. Th
+00000f00: 6520 7269 6768 7420 7369 6465 2064 6570  e right side dep
+00000f10: 6963 7473 2074 6865 205c 2254 6f74 616c  icts the \"Total
+00000f20: 5c22 2074 6162 2c20 7072 6f76 6964 696e  \" tab, providin
+00000f30: 6720 616e 206f 7665 7276 6965 7720 6f76  g an overview ov
+00000f40: 6572 2061 6c6c 2072 6573 6561 7263 6820  er all research 
+00000f50: 7175 6573 7469 6f6e 7320 616e 6420 6120  questions and a 
+00000f60: 7072 6f67 7265 7373 2074 7261 636b 696e  progress trackin
+00000f70: 6720 666f 7220 7468 6520 656e 7469 7265  g for the entire
+00000f80: 2053 5741 524d 2d53 4c52 2e20 5769 7468   SWARM-SLR. With
+00000f90: 2065 6163 6820 616e 6e6f 7461 7465 6420   each annotated 
+00000fa0: 646f 6375 6d65 6e74 2c20 7468 6520 7265  document, the re
+00000fb0: 7365 6172 6368 6572 2070 726f 6772 6573  searcher progres
+00000fc0: 7365 7320 7468 726f 7567 6820 7468 6520  ses through the 
+00000fd0: 5c22 4265 7374 2043 616e 6469 6461 7465  \"Best Candidate
+00000fe0: 735c 2220 7374 6163 6b2e 3c2f 6669 6763  s\" stack.</figc
+00000ff0: 6170 7469 6f6e 3e5c 6e22 2c0d 0a20 2020  aption>\n",..   
+00001000: 2022 3c2f 6469 763e 5c6e 222c 0d0a 2020   "</div>\n",..  
+00001010: 2020 225c 6e22 2c0d 0a20 2020 2022 3c62    "\n",..    "<b
+00001020: 723e 5c6e 222c 0d0a 2020 2020 225c 6e22  r>\n",..    "\n"
+00001030: 2c0d 0a20 2020 2022 3c64 6976 2061 6c69  ,..    "<div ali
+00001040: 676e 3d5c 2263 656e 7465 725c 223e 5c6e  gn=\"center\">\n
+00001050: 222c 0d0a 2020 2020 223c 696d 6720 7372  ",..    "<img sr
+00001060: 633d 5c22 696d 6167 6573 2f54 6173 6b20  c=\"images/Task 
+00001070: 3620 2d20 3034 204f 6273 6964 6961 6e20  6 - 04 Obsidian 
+00001080: 416e 6e6f 7461 7469 6f6e 2e70 6e67 5c22  Annotation.png\"
+00001090: 2077 6964 7468 3d5c 2239 3525 5c22 202f   width=\"95%\" /
+000010a0: 3e5c 6e22 2c0d 0a20 2020 2022 3c66 6967  >\n",..    "<fig
+000010b0: 6361 7074 696f 6e3e 4f62 7369 6469 616e  caption>Obsidian
+000010c0: 2064 6f63 756d 656e 7420 616e 6e6f 7461   document annota
+000010d0: 7469 6f6e 2e20 5468 6520 6c65 6674 2073  tion. The left s
+000010e0: 6964 6520 7368 6f77 7320 616e 2061 6e6e  ide shows an ann
+000010f0: 6f74 6174 6564 2064 6f63 756d 656e 7420  otated document 
+00001100: 696e 636c 7564 696e 6720 7175 6f74 6573  including quotes
+00001110: 2061 6e64 2073 6372 6565 6e73 686f 7473   and screenshots
+00001120: 2e20 4279 206d 6172 6b69 6e67 2069 7420  . By marking it 
+00001130: 6173 205c 2257 6f72 6b20 696e 2050 726f  as \"Work in Pro
+00001140: 6772 6573 735c 222c 2069 7420 6765 7473  gress\", it gets
+00001150: 206d 6f76 6564 2066 726f 6d20 7468 6520   moved from the 
+00001160: 5c22 4265 7374 2043 616e 6469 6461 7465  \"Best Candidate
+00001170: 735c 2220 746f 205c 224d 6f64 6966 6965  s\" to \"Modifie
+00001180: 645c 222e 204f 6e63 6520 6974 2069 7320  d\". Once it is 
+00001190: 6d61 726b 6564 2061 7320 5c22 5061 7065  marked as \"Pape
+000011a0: 7220 7265 6164 2061 6e64 2043 6f6e 7472  r read and Contr
+000011b0: 6962 7574 696f 6e20 636f 6d70 6c65 7465  ibution complete
+000011c0: 645c 222c 2069 7420 6973 206c 6973 7465  d\", it is liste
+000011d0: 6420 756e 6465 7220 5c22 446f 6e65 5c22  d under \"Done\"
+000011e0: 2e3c 2f66 6967 6361 7074 696f 6e3e 5c6e  .</figcaption>\n
+000011f0: 222c 0d0a 2020 2020 223c 2f64 6976 3e5c  ",..    "</div>\
+00001200: 6e22 2c0d 0a20 2020 2022 5c6e 222c 0d0a  n",..    "\n",..
+00001210: 2020 2020 223c 6272 3e5c 6e22 2c0d 0a20      "<br>\n",.. 
+00001220: 2020 2022 5c6e 222c 0d0a 2020 2020 223c     "\n",..    "<
+00001230: 6469 763e 5c6e 222c 0d0a 2020 2020 223c  div>\n",..    "<
+00001240: 6469 7620 7374 796c 653d 5c22 6469 7370  div style=\"disp
+00001250: 6c61 793a 2066 6c65 783b 206a 7573 7469  lay: flex; justi
+00001260: 6679 2d63 6f6e 7465 6e74 3a20 6365 6e74  fy-content: cent
+00001270: 6572 3b5c 223e 5c6e 222c 0d0a 2020 2020  er;\">\n",..    
+00001280: 223c 696d 6720 7372 633d 5c22 696d 6167  "<img src=\"imag
+00001290: 6573 2f54 6173 6b20 3620 2d20 3034 204f  es/Task 6 - 04 O
+000012a0: 6273 6964 6961 6e20 416e 6e6f 7461 7469  bsidian Annotati
+000012b0: 6f6e 2e70 6e67 5c22 2077 6964 7468 3d5c  on.png\" width=\
+000012c0: 2234 3525 5c22 202f 3e5c 6e22 2c0d 0a20  "45%\" />\n",.. 
+000012d0: 2020 2022 3c69 6d67 2073 7263 3d5c 2269     "<img src=\"i
+000012e0: 6d61 6765 732f 5461 736b 2036 202d 2030  mages/Task 6 - 0
+000012f0: 3620 5370 7265 6164 7368 6565 742e 706e  6 Spreadsheet.pn
+00001300: 675c 2220 7769 6474 683d 5c22 3435 255c  g\" width=\"45%\
+00001310: 2220 2f3e 5c6e 222c 0d0a 2020 2020 223c  " />\n",..    "<
+00001320: 2f64 6976 3e5c 6e22 2c0d 0a20 2020 2022  /div>\n",..    "
+00001330: 3c66 6967 6361 7074 696f 6e3e 4279 2075  <figcaption>By u
+00001340: 7369 6e67 204f 6273 6964 6961 6e20 616e  sing Obsidian an
+00001350: 6420 7468 6520 656d 6265 6464 6564 2050  d the embedded P
+00001360: 4446 2076 6965 7765 722c 2074 6865 2072  DF viewer, the r
+00001370: 6573 6561 7263 6865 7220 6361 6e20 6765  esearcher can ge
+00001380: 7420 6120 6265 7474 6572 2066 6565 6c69  t a better feeli
+00001390: 6e67 2066 6f72 2074 6865 2072 6571 7569  ng for the requi
+000013a0: 7265 6420 6461 7461 2073 7472 7563 7475  red data structu
+000013b0: 7265 2e20 4974 6572 6174 6976 656c 7920  re. Iteratively 
+000013c0: 616e 6420 7769 7468 6f75 7420 6c6f 6f73  and without loos
+000013d0: 696e 6720 616e 6e6f 7461 7469 6f6e 2066  ing annotation f
+000013e0: 726f 6d20 6561 726c 6965 7220 7374 6167  rom earlier stag
+000013f0: 6573 2c20 7468 6520 7265 7365 6172 6368  es, the research
+00001400: 6572 2063 616e 2070 726f 6772 6573 7320  er can progress 
+00001410: 746f 7761 7264 7320 6120 7374 7275 6374  towards a struct
+00001420: 7572 6564 203c 6120 6872 6566 3d5c 2268  ured <a href=\"h
+00001430: 7474 7073 3a2f 2f64 6f63 732e 676f 6f67  ttps://docs.goog
+00001440: 6c65 2e63 6f6d 2f73 7072 6561 6473 6865  le.com/spreadshe
+00001450: 6574 732f 642f 314b 554d 5365 715f 507a  ets/d/1KUMSeq_Pz
+00001460: 7034 4b76 655a 3770 6235 7264 6463 7373  p4KveZ7pb5rddcss
+00001470: 6b31 5842 5469 4c48 6e69 4430 6433 6e44  k1XBTiLHniD0d3nD
+00001480: 716f 2f65 6469 7423 6769 643d 305c 223e  qo/edit#gid=0\">
+00001490: 7370 7265 6164 7368 6565 743c 2f61 3e2c  spreadsheet</a>,
+000014a0: 2077 6974 686f 7574 206d 6f64 656c 6c69   without modelli
+000014b0: 6e67 206f 7574 2074 6865 2073 656d 616e  ng out the seman
+000014c0: 7469 6320 7374 7275 6374 7572 6520 6120  tic structure a 
+000014d0: 7072 696f 7269 2e5c 6e22 2c0d 0a20 2020  priori.\n",..   
+000014e0: 2022 3c2f 6469 763e 5c6e 220d 0a20 2020   "</div>\n"..   
+000014f0: 5d0d 0a20 207d 2c0d 0a20 207b 0d0a 2020  ]..  },..  {..  
+00001500: 2022 6365 6c6c 5f74 7970 6522 3a20 226d   "cell_type": "m
+00001510: 6172 6b64 6f77 6e22 2c0d 0a20 2020 226d  arkdown",..   "m
+00001520: 6574 6164 6174 6122 3a20 7b7d 2c0d 0a20  etadata": {},.. 
+00001530: 2020 2273 6f75 7263 6522 3a20 5b0d 0a20    "source": [.. 
+00001540: 2020 2022 2323 2054 6173 6b20 373a 2053     "## Task 7: S
+00001550: 796e 7468 6573 6973 5c6e 222c 0d0a 2020  ynthesis\n",..  
+00001560: 2020 225c 6e22 2c0d 0a20 2020 2022 7c53    "\n",..    "|S
+00001570: 7465 707c 5265 7375 6c74 7c52 6571 7569  tep|Result|Requi
+00001580: 7265 6d65 6e74 7c5c 6e22 2c0d 0a20 2020  rement|\n",..   
+00001590: 2022 7c3a 2d2d 2d2d 7c3a 2d2d 2d2d 7c3a   "|:----|:----|:
+000015a0: 2d2d 2d2d 7c5c 6e22 2c0d 0a20 2020 2022  ----|\n",..    "
+000015b0: 7c43 6f6d 7061 7265 2063 6f6e 7472 6962  |Compare contrib
+000015c0: 7574 696f 6e73 7c63 6f6d 7061 7269 736f  utions|compariso
+000015d0: 6e7c 3532 2e20 6465 6669 6e65 2063 6f6d  n|52. define com
+000015e0: 7061 7269 736f 6e20 7072 6f70 6572 7469  parison properti
+000015f0: 6573 3c62 723e 3533 2e20 696e 7365 7274  es<br>53. insert
+00001600: 2063 6f6e 7472 6962 7574 696f 6e20 7661   contribution va
+00001610: 6c75 6573 7c5c 6e22 2c0d 0a20 2020 2022  lues|\n",..    "
+00001620: 7c43 7261 6674 2061 7267 756d 656e 7473  |Craft arguments
+00001630: 2062 6173 6564 206f 6e20 6669 6e64 696e   based on findin
+00001640: 6773 7c64 6f63 756d 656e 7420 636c 6169  gs|document clai
+00001650: 6d73 7c35 342e 2069 6465 6e74 6966 7920  ms|54. identify 
+00001660: 6576 6964 656e 6365 2028 6461 7461 293c  evidence (data)<
+00001670: 6272 3e35 352e 2065 7374 6162 6c69 7368  br>55. establish
+00001680: 2077 6172 7261 6e74 7c5c 6e22 2c0d 0a20   warrant|\n",.. 
+00001690: 2020 2022 7c43 7269 7469 7175 6520 7468     "|Critique th
+000016a0: 6520 6c69 7465 7261 7475 7265 7c74 6865  e literature|the
+000016b0: 7369 7320 636c 6169 6d73 7c35 362e 2069  sis claims|56. i
+000016c0: 6465 6e74 6966 7920 6576 6964 656e 6365  dentify evidence
+000016d0: 2028 636c 6169 6d73 293c 6272 3e35 372e   (claims)<br>57.
+000016e0: 2069 6465 6e74 6966 7920 7061 7474 6572   identify patter
+000016f0: 6e73 3c62 723e 3538 2e20 6465 7465 6374  ns<br>58. detect
+00001700: 2066 616c 6c61 6369 6573 3c62 723e 3539   fallacies<br>59
+00001710: 2e20 6964 656e 7469 6679 2063 6f6e 666c  . identify confl
+00001720: 6963 7473 3c62 723e 3630 2e20 7265 736f  icts<br>60. reso
+00001730: 6c76 6520 636f 6e66 6c69 6374 737c 220d  lve conflicts|".
+00001740: 0a20 2020 5d0d 0a20 207d 2c0d 0a20 207b  .   ]..  },..  {
+00001750: 0d0a 2020 2022 6365 6c6c 5f74 7970 6522  ..   "cell_type"
+00001760: 3a20 226d 6172 6b64 6f77 6e22 2c0d 0a20  : "markdown",.. 
+00001770: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
+00001780: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
+00001790: 5b0d 0a20 2020 2022 2323 2320 5374 6570  [..    "### Step
+000017a0: 2037 2e31 2043 6f6d 7061 7265 2063 6f6e   7.1 Compare con
+000017b0: 7472 6962 7574 696f 6e73 5c6e 222c 0d0a  tributions\n",..
+000017c0: 2020 2020 222a 2a52 6571 7569 7265 6d65      "**Requireme
+000017d0: 6e74 733a 2a2a 5c6e 222c 0d0a 2020 2020  nts:**\n",..    
+000017e0: 222a 2064 6566 696e 6520 636f 6d70 6172  "* define compar
+000017f0: 6973 6f6e 2070 726f 7065 7274 6965 735c  ison properties\
+00001800: 6e22 2c0d 0a20 2020 2022 2a20 696e 7365  n",..    "* inse
+00001810: 7274 2063 6f6e 7472 6962 7574 696f 6e20  rt contribution 
+00001820: 7661 6c75 6573 5c6e 222c 0d0a 2020 2020  values\n",..    
+00001830: 223c 6469 763e 5c6e 222c 0d0a 2020 2020  "<div>\n",..    
+00001840: 2220 2020 203c 6469 7620 7374 796c 653d  "    <div style=
+00001850: 5c22 6469 7370 6c61 793a 2066 6c65 783b  \"display: flex;
+00001860: 206a 7573 7469 6679 2d63 6f6e 7465 6e74   justify-content
+00001870: 3a20 6365 6e74 6572 3b5c 223e 5c6e 222c  : center;\">\n",
+00001880: 0d0a 2020 2020 2220 2020 2020 2020 203c  ..    "        <
+00001890: 696d 6720 7372 633d 5c22 696d 6167 6573  img src=\"images
+000018a0: 2f54 6173 6b20 3620 2d20 3036 2053 7072  /Task 6 - 06 Spr
+000018b0: 6561 6473 6865 6574 2e70 6e67 5c22 2077  eadsheet.png\" w
+000018c0: 6964 7468 3d5c 2234 3525 5c22 202f 3e5c  idth=\"45%\" />\
+000018d0: 6e22 2c0d 0a20 2020 2022 2020 2020 2020  n",..    "      
+000018e0: 2020 3c69 6d67 2073 7263 3d5c 2269 6d61    <img src=\"ima
+000018f0: 6765 732f 5461 736b 2037 202d 2030 3120  ges/Task 7 - 01 
+00001900: 4b6e 6f77 6c65 6467 6520 4772 6170 682e  Knowledge Graph.
+00001910: 706e 675c 2220 7769 6474 683d 5c22 3435  png\" width=\"45
+00001920: 255c 2220 2f3e 5c6e 222c 0d0a 2020 2020  %\" />\n",..    
+00001930: 2220 2020 203c 2f64 6976 3e5c 6e22 2c0d  "    </div>\n",.
+00001940: 0a20 2020 2022 4174 2061 6e79 2070 6f69  .    "At any poi
+00001950: 6e74 2069 6e20 7469 6d65 2c20 7468 6520  nt in time, the 
+00001960: 7265 7365 6172 6368 6572 2063 616e 2073  researcher can s
+00001970: 7461 7274 2061 6e64 2069 7465 7261 7465  tart and iterate
+00001980: 206f 6e20 7468 6569 7220 6461 7461 206d   on their data m
+00001990: 6f64 656c 2c20 616e 6420 6f6e 6365 2069  odel, and once i
+000019a0: 7465 7261 7469 6f6e 7320 7374 6167 6e61  terations stagna
+000019b0: 7465 2061 6e64 203c 623e 636f 6d70 6172  te and <b>compar
+000019c0: 6973 6f6e 2070 726f 7065 7274 6965 7320  ison properties 
+000019d0: 6172 6520 6465 6669 6e65 643c 2f62 3e2c  are defined</b>,
+000019e0: 2074 6865 7920 6361 6e20 7072 6f67 7265   they can progre
+000019f0: 7373 2074 6f77 6172 6473 2074 6865 206e  ss towards the n
+00001a00: 6578 7420 7374 6167 652c 2066 726f 6d20  ext stage, from 
+00001a10: 286c 6f63 616c 2920 3c61 2068 7265 663d  (local) <a href=
+00001a20: 5c22 6874 7470 733a 2f2f 646f 6373 2e67  \"https://docs.g
+00001a30: 6f6f 676c 652e 636f 6d2f 7370 7265 6164  oogle.com/spread
+00001a40: 7368 6565 7473 2f64 2f31 4b55 4d53 6571  sheets/d/1KUMSeq
+00001a50: 5f50 7a70 344b 7665 5a37 7062 3572 6464  _Pzp4KveZ7pb5rdd
+00001a60: 6373 736b 3158 4254 694c 486e 6944 3064  cssk1XBTiLHniD0d
+00001a70: 336e 4471 6f2f 6564 6974 2367 6964 3d30  3nDqo/edit#gid=0
+00001a80: 5c22 3e73 7072 6561 6473 6865 6574 3c2f  \">spreadsheet</
+00001a90: 613e 2074 6f20 6120 676c 6f62 616c 203c  a> to a global <
+00001aa0: 6120 6872 6566 3d5c 2268 7474 7073 3a2f  a href=\"https:/
+00001ab0: 2f6f 726b 672e 6f72 672f 636f 6d70 6172  /orkg.org/compar
+00001ac0: 6973 6f6e 2f52 3635 3931 3334 2f5c 223e  ison/R659134/\">
+00001ad0: 6b6e 6f77 6c65 6467 6520 6772 6170 683c  knowledge graph<
+00001ae0: 2f61 3e2e 5c6e 222c 0d0a 2020 2020 223c  /a>.\n",..    "<
+00001af0: 2f64 6976 3e5c 6e22 2c0d 0a20 2020 2022  /div>\n",..    "
+00001b00: 5c6e 222c 0d0a 2020 2020 223c 6272 3e5c  \n",..    "<br>\
+00001b10: 6e22 2c0d 0a20 2020 2022 5c6e 222c 0d0a  n",..    "\n",..
+00001b20: 2020 2020 223c 696d 6720 7374 796c 653d      "<img style=
+00001b30: 5c22 666c 6f61 743a 2072 6967 6874 3b20  \"float: right; 
+00001b40: 6d61 7267 696e 3a20 3230 7078 3b5c 2220  margin: 20px;\" 
+00001b50: 7372 633d 5c22 696d 6167 6573 2f54 6173  src=\"images/Tas
+00001b60: 6b20 3720 2d20 3032 204f 524b 4720 6665  k 7 - 02 ORKG fe
+00001b70: 6174 7572 6573 2e70 6e67 5c22 2077 6964  atures.png\" wid
+00001b80: 7468 3d5c 2235 3525 5c22 3e5c 6e22 2c0d  th=\"55%\">\n",.
+00001b90: 0a20 2020 2022 5c6e 222c 0d0a 2020 2020  .    "\n",..    
+00001ba0: 2242 7920 7573 696e 6720 7468 6520 5b4f  "By using the [O
+00001bb0: 524b 4720 696d 706f 7274 2074 6f6f 6c73  RKG import tools
+00001bc0: 5d28 6874 7470 733a 2f2f 6f72 6b67 2e6f  ](https://orkg.o
+00001bd0: 7267 2f74 6f6f 6c73 292c 2074 6865 7265  rg/tools), there
+00001be0: 2061 7265 2064 6966 6665 7265 6e74 2065   are different e
+00001bf0: 7175 616c 6c79 2076 6961 626c 6520 776f  qually viable wo
+00001c00: 726b 666c 6f77 733a 5c6e 222c 0d0a 2020  rkflows:\n",..  
+00001c10: 2020 222a 2049 6620 7468 6520 2a2a 7370    "* If the **sp
+00001c20: 7265 6164 7368 6565 742a 2a20 636f 6e74  readsheet** cont
+00001c30: 6169 6e73 2061 6c6c 2063 6f6c 756d 6e73  ains all columns
+00001c40: 2028 7072 6f70 6572 7469 6573 292c 2064   (properties), d
+00001c50: 6f63 756d 656e 7473 2061 6e64 2074 6865  ocuments and the
+00001c60: 6972 2072 6573 7065 6374 6976 6520 636f  ir respective co
+00001c70: 6e74 7269 6275 7469 6f6e 7320 2876 616c  ntributions (val
+00001c80: 7565 7329 2c20 7468 6520 5b63 7376 2d69  ues), the [csv-i
+00001c90: 6d70 6f72 745d 2868 7474 7073 3a2f 2f6f  mport](https://o
+00001ca0: 726b 672e 6f72 672f 6373 762d 696d 706f  rkg.org/csv-impo
+00001cb0: 7274 2920 6973 2061 2076 6572 7920 7669  rt) is a very vi
+00001cc0: 6162 6c65 2074 6f6f 6c2c 2063 6f6e 7665  able tool, conve
+00001cd0: 7274 696e 6720 6c61 7267 6520 706f 7274  rting large port
+00001ce0: 696f 6e73 206f 6620 7265 6c61 7469 6f6e  ions of relation
+00001cf0: 616c 2064 6174 6120 746f 2067 7261 7068  al data to graph
+00001d00: 2073 7472 7563 7475 7265 2e5c 6e22 2c0d   structure.\n",.
+00001d10: 0a20 2020 2022 2a20 4966 2074 6865 202a  .    "* If the *
+00001d20: 2a4f 524b 4720 6665 6174 7572 6573 2a2a  *ORKG features**
+00001d30: 2073 7563 6820 6173 2073 7472 7563 7475   such as structu
+00001d40: 7265 6420 5b6c 6973 7473 5d28 6874 7470  red [lists](http
+00001d50: 733a 2f2f 6f72 6b67 2e6f 7267 2f6c 6973  s://orkg.org/lis
+00001d60: 742f 6e65 7729 2061 6e64 205b 5044 4620  t/new) and [PDF 
+00001d70: 7465 7874 2061 6e6e 6f74 6174 696f 6e5d  text annotation]
+00001d80: 2868 7474 7073 3a2f 2f6f 726b 672e 6f72  (https://orkg.or
+00001d90: 672f 7064 662d 7465 7874 2d61 6e6e 6f74  g/pdf-text-annot
+00001da0: 6174 696f 6e29 2061 7265 2070 7265 6665  ation) are prefe
+00001db0: 7265 642c 2074 6865 206b 6e6f 776c 6564  red, the knowled
+00001dc0: 6765 2067 7261 7068 2063 616e 2061 6c73  ge graph can als
+00001dd0: 6f20 6265 2075 7469 6c69 7a65 6420 6f6e  o be utilized on
+00001de0: 6365 2074 6865 2073 7072 6561 6473 6865  ce the spreadshe
+00001df0: 6574 206d 6f64 656c 696e 6720 7374 6167  et modeling stag
+00001e00: 6e61 7465 732e 2054 6869 7320 616c 6c6f  nates. This allo
+00001e10: 7773 2074 6865 2063 7265 6174 696f 6e20  ws the creation 
+00001e20: 6f66 2061 205b 7465 6d70 6c61 7465 5d28  of a [template](
+00001e30: 6874 7470 733a 2f2f 6f72 6b67 2e6f 7267  https://orkg.org
+00001e40: 2f74 656d 706c 6174 652f 292c 2073 7472  /template/), str
+00001e50: 6561 6d6c 696e 696e 6720 7468 6520 5b61  eamlining the [a
+00001e60: 6464 696e 675d 2868 7474 7073 3a2f 2f6f  dding](https://o
+00001e70: 726b 672e 6f72 672f 6164 642d 7061 7065  rkg.org/add-pape
+00001e80: 7229 2061 6e64 205b 6564 6974 696e 675d  r) and [editing]
+00001e90: 2868 7474 7073 3a2f 2f6f 726b 672e 6f72  (https://orkg.or
+00001ea0: 672f 636f 6e74 7269 6275 7469 6f6e 2d65  g/contribution-e
+00001eb0: 6469 746f 7229 206f 6620 646f 6375 6d65  ditor) of docume
+00001ec0: 6e74 732e 220d 0a20 2020 5d0d 0a20 207d  nts."..   ]..  }
+00001ed0: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
+00001ee0: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
+00001ef0: 6e22 2c0d 0a20 2020 226d 6574 6164 6174  n",..   "metadat
+00001f00: 6122 3a20 7b7d 2c0d 0a20 2020 2273 6f75  a": {},..   "sou
+00001f10: 7263 6522 3a20 5b0d 0a20 2020 2022 2323  rce": [..    "##
+00001f20: 2320 5374 6570 2037 2e32 2043 7261 6674  # Step 7.2 Craft
+00001f30: 2061 7267 756d 656e 7473 2062 6173 6564   arguments based
+00001f40: 206f 6e20 6669 6e64 696e 6773 5c6e 222c   on findings\n",
+00001f50: 0d0a 2020 2020 222a 2a52 6571 7569 7265  ..    "**Require
+00001f60: 6d65 6e74 733a 2a2a 5c6e 222c 0d0a 2020  ments:**\n",..  
+00001f70: 2020 222a 2069 6465 6e74 6966 7920 6576    "* identify ev
+00001f80: 6964 656e 6365 2028 6461 7461 295c 6e22  idence (data)\n"
+00001f90: 2c0d 0a20 2020 2022 2a20 6573 7461 626c  ,..    "* establ
+00001fa0: 6973 6820 7761 7272 616e 745c 6e22 2c0d  ish warrant\n",.
+00001fb0: 0a20 2020 2022 5c6e 222c 0d0a 2020 2020  .    "\n",..    
+00001fc0: 223c 626c 6f63 6b71 756f 7465 3e3c 623e  "<blockquote><b>
+00001fd0: 5761 7272 616e 743c 2f62 3e20 2d20 5468  Warrant</b> - Th
+00001fe0: 6520 7265 6173 6f6e 696e 6720 7573 6564  e reasoning used
+00001ff0: 2069 6e20 616e 2061 7267 756d 656e 7420   in an argument 
+00002000: 746f 2061 6c6c 6f77 2074 6865 2072 6573  to allow the res
+00002010: 6561 7263 6865 722c 2061 6e64 2061 6e79  earcher, and any
+00002020: 2072 6561 6465 722c 2074 6f20 6163 6365   reader, to acce
+00002030: 7074 2074 6865 2065 7669 6465 6e63 6520  pt the evidence 
+00002040: 7072 6573 656e 7465 6420 6173 2072 6561  presented as rea
+00002050: 736f 6e61 626c 6520 7072 6f6f 6620 7468  sonable proof th
+00002060: 6174 2074 6865 2070 6f73 6974 696f 6e20  at the position 
+00002070: 6f66 2074 6865 2063 6c61 696d 2069 7320  of the claim is 
+00002080: 636f 7272 6563 742e 3c62 723e 5c6e 222c  correct.<br>\n",
+00002090: 0d0a 2020 2020 222d 2d20 4272 656e 6461  ..    "-- Brenda
+000020a0: 2054 2e20 4d63 4576 6f79 2061 6e64 204c   T. McEvoy and L
+000020b0: 6177 7265 6e63 6520 412e 204d 6163 6869  awrence A. Machi
+000020c0: 3a20 3c69 3e54 6865 204c 6974 6572 6174  : <i>The Literat
+000020d0: 7572 6520 5265 7669 6577 3a20 5369 7820  ure Review: Six 
+000020e0: 5374 6570 7320 746f 2053 7563 6365 7373  Steps to Success
+000020f0: 3c2f 693e 2c20 7061 6765 2036 345c 6e22  </i>, page 64\n"
+00002100: 2c0d 0a20 2020 2022 3c2f 626c 6f63 6b71  ,..    "</blockq
+00002110: 756f 7465 3e5c 6e22 2c0d 0a20 2020 2022  uote>\n",..    "
+00002120: 5c6e 222c 0d0a 2020 2020 222a 4869 6e74  \n",..    "*Hint
+00002130: 2a3a 2053 7465 7020 372e 3220 616e 6420  *: Step 7.2 and 
+00002140: 372e 3320 6573 7065 6369 616c 6c79 2062  7.3 especially b
+00002150: 656e 6566 6974 2066 726f 6d20 6164 6469  enefit from addi
+00002160: 7469 6f6e 616c 2072 6561 6469 6e67 206f  tional reading o
+00002170: 6620 6c69 7465 7261 7475 7265 2072 6576  f literature rev
+00002180: 6965 7720 6775 6964 656c 696e 6573 2c20  iew guidelines, 
+00002190: 7072 6f76 6964 696e 6720 636f 6e74 6578  providing contex
+000021a0: 7420 666f 7220 7468 6520 7072 6573 656e  t for the presen
+000021b0: 7420 7465 726d 696e 6f6c 6f67 7920 616e  t terminology an
+000021c0: 6420 7265 7175 6972 656d 656e 7473 2e20  d requirements. 
+000021d0: 5468 6572 6520 6973 2063 7572 7265 6e74  There is current
+000021e0: 6c79 206e 6f20 746f 6f6c 2073 7570 706f  ly no tool suppo
+000021f0: 7274 2070 7265 7365 6e74 2077 6974 6869  rt present withi
+00002200: 6e20 7468 6520 5357 4152 4d2d 534c 522c  n the SWARM-SLR,
+00002210: 206d 616b 696e 6720 2a65 6475 6361 7465   making *educate
+00002220: 2074 6865 2072 6573 6561 7263 6865 722a   the researcher*
+00002230: 2074 6865 2062 6573 7420 7072 6163 7469   the best practi
+00002240: 6365 2063 7572 7265 6e74 6c79 2061 7661  ce currently ava
+00002250: 696c 6162 6c65 2e20 5265 636f 6d6d 656e  ilable. Recommen
+00002260: 6461 7469 6f6e 7320 696e 636c 7564 652c  dations include,
+00002270: 2062 7574 2061 7265 206e 6f74 206c 696d   but are not lim
+00002280: 6974 6564 2074 6f3a 5c6e 222c 0d0a 2020  ited to:\n",..  
+00002290: 2020 222a 2042 7265 6e64 6120 542e 204d    "* Brenda T. M
+000022a0: 6345 766f 7920 616e 6420 4c61 7772 656e  cEvoy and Lawren
+000022b0: 6365 2041 2e20 4d61 6368 693a 203c 693e  ce A. Machi: <i>
+000022c0: 5468 6520 4c69 7465 7261 7475 7265 2052  The Literature R
+000022d0: 6576 6965 773a 2053 6978 2053 7465 7073  eview: Six Steps
+000022e0: 2074 6f20 5375 6363 6573 733c 2f69 3e2c   to Success</i>,
+000022f0: 2070 6167 6520 3634 2074 6f20 3133 335c   page 64 to 133\
+00002300: 6e22 2c0d 0a20 2020 2022 2a20 4869 6767  n",..    "* Higg
+00002310: 696e 7320 4a50 542c 2054 686f 6d61 7320  ins JPT, Thomas 
+00002320: 4a2c 2043 6861 6e64 6c65 7220 4a2c 2043  J, Chandler J, C
+00002330: 756d 7073 746f 6e20 4d2c 204c 6920 542c  umpston M, Li T,
+00002340: 2050 6167 6520 4d4a 2c20 5765 6c63 6820   Page MJ, Welch 
+00002350: 5641 2028 6564 6974 6f72 7329 2e20 436f  VA (editors). Co
+00002360: 6368 7261 6e65 2048 616e 6462 6f6f 6b20  chrane Handbook 
+00002370: 666f 7220 5379 7374 656d 6174 6963 2052  for Systematic R
+00002380: 6576 6965 7773 206f 6620 496e 7465 7276  eviews of Interv
+00002390: 656e 7469 6f6e 7320 7665 7273 696f 6e20  entions version 
+000023a0: 362e 3420 2875 7064 6174 6564 2041 7567  6.4 (updated Aug
+000023b0: 7573 7420 3230 3233 292e 2043 6f63 6872  ust 2023). Cochr
+000023c0: 616e 652c 2032 3032 332e 2041 7661 696c  ane, 2023. Avail
+000023d0: 6162 6c65 2066 726f 6d20 5b77 7777 2e74  able from [www.t
+000023e0: 7261 696e 696e 672e 636f 6368 7261 6e65  raining.cochrane
+000023f0: 2e6f 7267 2f68 616e 6462 6f6f 6b5d 2877  .org/handbook](w
+00002400: 7777 2e74 7261 696e 696e 672e 636f 6368  ww.training.coch
+00002410: 7261 6e65 2e6f 7267 2f68 616e 6462 6f6f  rane.org/handboo
+00002420: 6b29 2e5c 6e22 2c0d 0a20 2020 2022 5c6e  k).\n",..    "\n
+00002430: 222c 0d0a 2020 2020 225c 6e22 2c0d 0a20  ",..    "\n",.. 
+00002440: 2020 2022 5769 7468 2061 6c6c 2072 6571     "With all req
+00002450: 7569 7265 6420 6461 7461 206e 6f77 2070  uired data now p
+00002460: 7265 7365 6e74 2069 6e20 6d61 6368 696e  resent in machin
+00002470: 652d 7265 6164 6162 6c65 2066 6f72 6d2c  e-readable form,
+00002480: 2061 7267 756d 656e 7473 2063 616e 2062   arguments can b
+00002490: 6520 6372 6166 7465 642e 2045 6163 6820  e crafted. Each 
+000024a0: 6172 6775 6d65 6e74 2072 6571 7569 7265  argument require
+000024b0: 7320 6461 7461 2c20 6176 6169 6c61 626c  s data, availabl
+000024c0: 6520 7468 726f 7567 6820 7468 6520 636f  e through the co
+000024d0: 6e74 7269 6275 7469 6f6e 732c 2061 6e64  ntributions, and
+000024e0: 2063 616e 2062 6520 7761 7272 616e 7465   can be warrante
+000024f0: 6420 7468 726f 7567 6820 6c69 7374 732c  d through lists,
+00002500: 2063 6f6d 7061 7269 736f 6e73 2c20 7669   comparisons, vi
+00002510: 7375 616c 697a 6174 696f 6e73 2c20 7265  sualizations, re
+00002520: 7669 6577 7320 616e 6420 7369 6d69 6c61  views and simila
+00002530: 7220 746f 6f6c 7320 6465 7369 676e 6564  r tools designed
+00002540: 2074 6f20 7379 6e74 6865 7369 7a65 2064   to synthesize d
+00002550: 6174 612e 5c6e 222c 0d0a 2020 2020 225c  ata.\n",..    "\
+00002560: 6e22 2c0d 0a20 2020 2022 2323 2323 2045  n",..    "#### E
+00002570: 7861 6d70 6c65 5c6e 222c 0d0a 2020 2020  xample\n",..    
+00002580: 222a 202a 436c 6169 6d2a 3a20 584d 4c20  "* *Claim*: XML 
+00002590: 6973 206e 6f74 2072 6571 7569 7265 6420  is not required 
+000025a0: 746f 2072 6570 7265 7365 6e74 2061 6e64  to represent and
+000025b0: 2065 7863 6861 6e67 6520 6165 726f 7370   exchange aerosp
+000025c0: 6163 6520 656e 6769 6e65 6572 696e 6720  ace engineering 
+000025d0: 7379 7374 656d 2073 7472 7563 7475 7265  system structure
+000025e0: 732e 5c6e 222c 0d0a 2020 2020 222a 202a  s.\n",..    "* *
+000025f0: 4576 6964 656e 6365 2a3a 2038 3220 6469  Evidence*: 82 di
+00002600: 6666 6572 656e 7420 646f 6375 6d65 6e74  fferent document
+00002610: 7320 7265 706f 7274 696e 6720 6f6e 2061  s reporting on a
+00002620: 6572 6f73 7061 6365 2065 6e67 696e 6565  erospace enginee
+00002630: 7273 2065 7863 6861 6e67 696e 6720 7379  rs exchanging sy
+00002640: 7374 656d 2073 7472 7563 7475 7265 732e  stem structures.
+00002650: 2031 3720 6f66 2074 6865 6d20 6469 6420   17 of them did 
+00002660: 6e6f 7420 7573 6520 584d 4c2e 220d 0a20  not use XML.".. 
+00002670: 2020 5d0d 0a20 207d 2c0d 0a20 207b 0d0a    ]..  },..  {..
+00002680: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+00002690: 226d 6172 6b64 6f77 6e22 2c0d 0a20 2020  "markdown",..   
+000026a0: 226d 6574 6164 6174 6122 3a20 7b7d 2c0d  "metadata": {},.
+000026b0: 0a20 2020 2273 6f75 7263 6522 3a20 5b0d  .   "source": [.
+000026c0: 0a20 2020 2022 2323 2320 5374 6570 2037  .    "### Step 7
+000026d0: 2e33 2043 7269 7469 7175 6520 7468 6520  .3 Critique the 
+000026e0: 6c69 7465 7261 7475 7265 5c6e 222c 0d0a  literature\n",..
+000026f0: 2020 2020 222a 2a52 6571 7569 7265 6d65      "**Requireme
+00002700: 6e74 733a 2a2a 5c6e 222c 0d0a 2020 2020  nts:**\n",..    
+00002710: 222a 2069 6465 6e74 6966 7920 6576 6964  "* identify evid
+00002720: 656e 6365 2028 636c 6169 6d73 295c 6e22  ence (claims)\n"
+00002730: 2c0d 0a20 2020 2022 2a20 6964 656e 7469  ,..    "* identi
+00002740: 6679 2070 6174 7465 726e 735c 6e22 2c0d  fy patterns\n",.
+00002750: 0a20 2020 2022 2a20 6465 7465 6374 2066  .    "* detect f
+00002760: 616c 6c61 6369 6573 5c6e 222c 0d0a 2020  allacies\n",..  
+00002770: 2020 222a 2069 6465 6e74 6966 7920 636f    "* identify co
+00002780: 6e66 6c69 6374 735c 6e22 2c0d 0a20 2020  nflicts\n",..   
+00002790: 2022 2a20 7265 736f 6c76 6520 636f 6e66   "* resolve conf
+000027a0: 6c69 6374 7320 5c6e 222c 0d0a 2020 2020  licts \n",..    
+000027b0: 225c 6e22 2c0d 0a20 2020 2022 4561 6368  "\n",..    "Each
+000027c0: 2063 6c61 696d 206e 6f77 2062 6563 6f6d   claim now becom
+000027d0: 6573 2065 7669 6465 6e63 6520 696e 2069  es evidence in i
+000027e0: 7473 656c 662e 2048 6176 696e 6720 636f  tself. Having co
+000027f0: 6c6c 6563 7465 6420 616e 6420 7375 7070  llected and supp
+00002800: 6f72 7465 6420 6d75 6c74 6970 6c65 2063  orted multiple c
+00002810: 6c61 696d 732c 2074 6865 7920 6d61 7920  laims, they may 
+00002820: 7368 6f77 2070 6174 7465 726e 732c 2065  show patterns, e
+00002830: 2e67 2e20 6f66 2063 6f72 7265 6c61 7469  .g. of correlati
+00002840: 6f6e 206f 7220 6361 7573 6174 696f 6e2e  on or causation.
+00002850: 2054 6869 7320 616c 6c6f 7773 2074 6865   This allows the
+00002860: 2069 6e66 6572 656e 6365 206f 6620 6e65   inference of ne
+00002870: 7720 2a6d 6574 6120 636c 6169 6d73 2a2c  w *meta claims*,
+00002880: 2075 7369 6e67 2074 6865 7365 206e 6f77   using these now
+00002890: 2073 7570 706f 7274 6564 2063 6c61 696d   supported claim
+000028a0: 7320 6173 2074 6865 6972 2065 7669 6465  s as their evide
+000028b0: 6e63 652e 2054 6865 7365 2063 6c61 696d  nce. These claim
+000028c0: 7320 616e 6420 6d65 7461 2d63 6c61 696d  s and meta-claim
+000028d0: 7320 7368 6f75 6c64 2062 6520 6368 6563  s should be chec
+000028e0: 6b65 6420 6167 6169 6e20 666f 7220 6661  ked again for fa
+000028f0: 6c6c 6163 696f 7573 2072 6561 736f 6e69  llacious reasoni
+00002900: 6e67 2061 6e64 2063 6f6e 666c 6963 7473  ng and conflicts
+00002910: 2074 6f20 6173 7375 7265 2069 6e74 6572   to assure inter
+00002920: 6e61 6c20 636f 6e73 6973 7465 6e63 7920  nal consistency 
+00002930: 6f66 2061 6c6c 2063 6c61 696d 7320 616e  of all claims an
+00002940: 6420 6576 6964 656e 6365 2e5c 6e22 2c0d  d evidence.\n",.
+00002950: 0a20 2020 2022 5c6e 222c 0d0a 2020 2020  .    "\n",..    
+00002960: 2223 2323 2320 4578 616d 706c 655c 6e22  "#### Example\n"
+00002970: 2c0d 0a20 2020 2022 2a20 2a43 6c61 696d  ,..    "* *Claim
+00002980: 2a3a 2041 6572 6f73 7061 6365 2065 6e67  *: Aerospace eng
+00002990: 696e 6565 7273 2063 616e 2075 7365 2076  ineers can use v
+000029a0: 6172 696f 7573 206b 6e6f 776c 6564 6765  arious knowledge
+000029b0: 2072 6570 7265 7365 6e74 6174 696f 6e73   representations
+000029c0: 2074 6f20 7265 7072 6573 656e 7420 616e   to represent an
+000029d0: 6420 6578 6368 616e 6765 2074 6865 6972  d exchange their
+000029e0: 2073 7973 7465 6d20 7374 7275 6374 7572   system structur
+000029f0: 6573 2074 6f20 7461 696c 6f72 2074 6f20  es to tailor to 
+00002a00: 7468 6569 7220 7370 6563 6966 6963 2073  their specific s
+00002a10: 6974 7561 7469 6f6e 2e5c 6e22 2c0d 0a20  ituation.\n",.. 
+00002a20: 2020 2022 2a20 2a45 7669 6465 6e63 652a     "* *Evidence*
+00002a30: 3a5c 6e22 2c0d 0a20 2020 2022 2020 2a20  :\n",..    "  * 
+00002a40: 584d 4c20 6973 206e 6f74 2072 6571 7569  XML is not requi
+00002a50: 7265 6420 746f 2072 6570 7265 7365 6e74  red to represent
+00002a60: 2061 6e64 2065 7863 6861 6e67 6520 6165   and exchange ae
+00002a70: 726f 7370 6163 6520 656e 6769 6e65 6572  rospace engineer
+00002a80: 696e 6720 7379 7374 656d 2073 7472 7563  ing system struc
+00002a90: 7475 7265 732e 5c6e 222c 0d0a 2020 2020  tures.\n",..    
+00002aa0: 2220 202a 2053 7973 4d4c 2069 7320 7573  "  * SysML is us
+00002ab0: 6564 2062 7920 6165 726f 7370 6163 6520  ed by aerospace 
+00002ac0: 656e 6769 6e65 6572 7320 746f 2072 6570  engineers to rep
+00002ad0: 7265 7365 6e74 2073 7973 7465 6d20 7374  resent system st
+00002ae0: 7275 6374 7572 6573 2e5c 6e22 2c0d 0a20  ructures.\n",.. 
+00002af0: 2020 2022 2020 2a20 5244 4620 6361 6e20     "  * RDF can 
+00002b00: 7265 7072 6573 656e 7420 636f 6d70 6c65  represent comple
+00002b10: 7820 7379 7374 656d 732c 2073 7570 706f  x systems, suppo
+00002b20: 7274 696e 6720 6469 6666 6572 656e 7420  rting different 
+00002b30: 7365 7269 616c 697a 6174 696f 6e20 666f  serialization fo
+00002b40: 726d 6174 732e 5c6e 220d 0a20 2020 5d0d  rmats.\n"..   ].
+00002b50: 0a20 207d 0d0a 205d 2c0d 0a20 226d 6574  .  }.. ],.. "met
+00002b60: 6164 6174 6122 3a20 7b0d 0a20 2022 6c61  adata": {..  "la
+00002b70: 6e67 7561 6765 5f69 6e66 6f22 3a20 7b0d  nguage_info": {.
+00002b80: 0a20 2020 226e 616d 6522 3a20 2270 7974  .   "name": "pyt
+00002b90: 686f 6e22 0d0a 2020 7d0d 0a20 7d2c 0d0a  hon"..  }.. },..
+00002ba0: 2022 6e62 666f 726d 6174 223a 2034 2c0d   "nbformat": 4,.
+00002bb0: 0a20 226e 6266 6f72 6d61 745f 6d69 6e6f  . "nbformat_mino
+00002bc0: 7222 3a20 320d 0a7d 0d0a                 r": 2..}..
```

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/data/analysis555283.md` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/data/analysis555283.md`

 * *Files 3% similar despite different names*

```diff
@@ -116,7 +116,19 @@
 #### Scores:
 ['A3', 'A1', 'A2', 'A2', 'A2', 'A2', 'A4', 'A2', 'A5', 'A4', 'A6', 'A4', 'A4', 'A6', 'A6', 'A1', 'A1', 'A1', 'A1', 'A1', 'A3', 'A1', 'A1', 'A1', 'A3', 'A5', 'A5', 'A5', 'A5', 'A5', 'A5', 'A5', 'A5', 'A3', 'A6', 'A6', 'A3', 'A3', '', 'A2', 'A1', 'A1', 'A3', 'A3', 'A1', 'A1', 'A1', 'A5', 'A3', 'A3', 'A3', 'A1', 'A5', 'A1', 'A5', 'A3', 'A3', 'A1', 'A1', 'A3', 'A3', 'A3', 'A3', 'A5', 'A5']
 #### Time total: 490 seconds (8.17 minutes)
 | Planning a review | Defining a scope | Search | Select | Evaluate | Analysis | Synthesis | Reporting | Demographic data | Conclusion |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | 26.62 | 79.48 | 31.14 | 161.16 | 49.15 | 17.77 | 62.95 | 47.05 | 11.24 | 3.47 |
 
+### Response ID: 35
+#### Metadata:
+| Date submitted | Last page | Start language | Date started | Date last action | Age | Education | Survey count | Experience |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 2024-02-11 22:33:45 | 10 | en | 2024-02-11 22:30:46 | 2024-02-11 22:33:45 | 26 | Bachelor's degree | 1 | Fair |
+#### Scores:
+['A3', '', 'A4', '', '', '', '', 'A4', '', 'A4', '', 'A4', '', '', '', 'A3', '', '', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', '', 'A7', '', 'A1', 'A3', 'A3', 'A3', '', 'A4', '', 'A4', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', '', 'A3', '', '', 'A3', 'A3', '', 'A3', '', 'A3', '', 'A3', '', 'A3', 'A3', 'A3', 'A7', 'A3']
+#### Time total: 183 seconds (3.06 minutes)
+| Planning a review | Defining a scope | Search | Select | Evaluate | Analysis | Synthesis | Reporting | Demographic data | Conclusion |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 27.91 | 37.05 | 13.43 | 37.22 | 14.86 | 7.07 | 11.16 | 9.2 | 20.55 | 4.97 |
+
```

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/data/analysis628237.md` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/data/analysis628237.md`

 * *Files 8% similar despite different names*

```diff
@@ -451,7 +451,33 @@
 #### Scores:
 ['A2', 'A2', 'A3', 'A5', 'A3', 'A3', 'A3', 'A3', 'A4', 'A3', 'A5', 'A4', 'A4', 'A4', 'A4', 'A1', 'A1', 'A1', 'A1', 'A3', 'A3', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', '', 'A3', 'A3', 'A3', 'A3', '', 'A3', '', 'A3', 'A3', 'A3', 'A3', 'A3', 'A3', 'A2', 'A2', '', '']
 #### Time total: 3210 seconds (53.5 minutes)
 | Choose your Tool | Planning a review | Defining a scope | Search | Select | Evaluate | Analysis | Synthesis | Reporting | Demographic data | Conclusion |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | 50.35 | 17.02 | 110.08 | 65.7 | 2744.64 | 20.69 | 75 | 64.99 | 16.5 | 25.75 | 19.07 |
 
+### Response ID: 88
+#### Tool: Open Research Knowledge Graph (ORKG)
+#### Metadata:
+| Date submitted | Last page | Start language | Date started | Date last action | Age | Education | Survey count | Experience |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 2024-01-18 02:43:39 | 11 | en | 2024-01-18 02:37:52 | 2024-01-18 02:43:39 | 39 | Ph.D. or higher | 2-3 | Excellent |
+#### Scores:
+['A1', 'A1', 'A2', 'A2', 'A2', 'A2', 'A2', 'A2', 'A2', 'A2', 'A6', 'A8', 'A6', '', 'A8', 'A5', 'A1', 'A1', 'A5', 'A5', 'A5', 'A1', 'A1', 'A1', 'A1', 'A1', 'A9', 'A5', 'A5', 'A5', 'A9', 'A9', 'A9', 'A1', 'A10', 'A10', 'A2', 'A9', 'A9', 'A9', 'A1', 'A9', 'A9', 'A1', 'A1', 'A1', 'A9', 'A9', 'A1', 'A1', 'A1', 'A1', 'A1', 'A1', 'A1', 'A1', 'A1', 'A9', 'A9', 'A1', 'A1', 'A1', 'A1', 'A1', 'A1']
+#### Time total: 353 seconds (5.88 minutes)
+| Choose your Tool | Planning a review | Defining a scope | Search | Select | Evaluate | Analysis | Synthesis | Reporting | Demographic data | Conclusion |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 12.22 | 16.5 | 64.1 | 32.88 | 83.81 | 36.85 | 18.79 | 35.41 | 12.28 | 35.9 | 4.08 |
+
+### Response ID: 89
+#### Tool: LaTeX
+#### Metadata:
+| Date submitted | Last page | Start language | Date started | Date last action | Age | Education | Survey count | Experience |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 2024-01-18 02:48:23 | 11 | en | 2024-01-18 02:44:41 | 2024-01-18 02:48:23 | 39 | Ph.D. or higher | 2-3 | Excellent |
+#### Scores:
+['A9', 'A9', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A10', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A1', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A10', 'A10', 'A10', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A1', 'A1', 'A1', 'A1', 'A1', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A9', 'A1', 'A1', 'A1', 'A1', 'A1']
+#### Time total: 227 seconds (3.79 minutes)
+| Choose your Tool | Planning a review | Defining a scope | Search | Select | Evaluate | Analysis | Synthesis | Reporting | Demographic data | Conclusion |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 15.09 | 12.89 | 30.79 | 15.12 | 49.99 | 18.23 | 15.38 | 31.31 | 11.98 | 21.98 | 4.55 |
+
```

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 1.jpg` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 1.jpg`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 2.jpg` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 2.jpg`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 3.jpg` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 3.jpg`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 4 - Details.jpg` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 4 - Details.jpg`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/SWARM-SLR/images/Task 4.jpg` & `bnw_tools-0.0.2.0/scripts/SWARM-SLR/images/Task 4.jpg`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/bibtex_to_ORKG/Bibtex_to_ORKG.py` & `bnw_tools-0.0.2.0/scripts/bibtex_to_ORKG/Bibtex_to_ORKG.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/bibtex_to_ORKG/README.md` & `bnw_tools-0.0.2.0/scripts/bibtex_to_ORKG/README.md`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/k_score/README.md` & `bnw_tools-0.0.2.0/scripts/k_score/README.md`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/k_score/config sample.yml` & `bnw_tools-0.0.2.0/scripts/k_score/config sample.yml`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/scripts/k_score/k_score_Zotero.py` & `bnw_tools-0.0.2.0/scripts/k_score/k_score_Zotero.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/tests/README.md` & `bnw_tools-0.0.2.0/tests/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 
 #### Activate venv
 ```
 .venv/Scripts/activate
 ```
 *Hint*: Potentially, you need wrap it in an Set-ExecutionPolicy block, if you do not have the rights to execute scripts:
 ```
-Set-ExecutionPolicy RemoteSigned
+Set-ExecutionPolicy Unrestricted -Scope Process
 .venv/Scripts/activate
-Set-ExecutionPolicy Restricted
+Set-ExecutionPolicy Restricted -Scope Process
 ```
 *Hint*: this action is undone by typing ```deactivate```
 
 ### Everyday development
 #### Github: commit and push
 If you want, just use the Github Desktop version or the Visual Studio Code Github interface. Pressing buttons is simpler and often less dangerous.
 
@@ -93,15 +93,15 @@
 py -m pip install --upgrade build
 ```
 
 #### Package debugging
 ```
 pip uninstall -y bnw_tools
 py -m build
-pip install dist\bnw_tools-0.0.1.2.tar.gz
+pip install dist\bnw_tools-0.0.2.0.tar.gz
 ```
 
 *Note*: Change the version number
 
 #### Package publishing 
 ```
 twine upload dist/*
```

### Comparing `bnw_tools-0.0.1.4/tests/test_nlp.py` & `bnw_tools-0.0.2.0/tests/test_nlp.py`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/ORKG/RF_Map.json` & `bnw_tools-0.0.2.0/bnw_tools/ORKG/RF_Map.json`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/bnw_tools/ORKG/ResearchFields.json` & `bnw_tools-0.0.2.0/bnw_tools/ORKG/ResearchFields.json`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/.gitignore` & `bnw_tools-0.0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/LICENSE` & `bnw_tools-0.0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/README.md` & `bnw_tools-0.0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bnw_tools-0.0.1.4/pyproject.toml` & `bnw_tools-0.0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 # requires = ["hatchling<=1.18.0"]  
 build-backend = "hatchling.build"
 
 [project]
 name = "bnw_tools"
-version = "0.0.1.4"
+version = "0.0.2.0"
 authors = [
-  { name="BorgNetzWerk", email="info@borgnetzwerk.de" },
-  { name="Tim Wittenborg", email="tim.wittenborg@l3s.uni-hannover.de" },
+  { name = "BorgNetzWerk", email = "info@borgnetzwerk.de" },
+  { name = "Tim Wittenborg", email = "tim.wittenborg@l3s.uni-hannover.de" },
 ]
 description = "Tools developed in the BorgNetzWerk project for the extraction, analysis and publication of knowledge."
 keywords = ["BorgNetzWerk", "ORKG", "knowledge", "literature", "media"]
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.8, <3.12"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 dependencies = [
+  "scipy==1.10.1",
   "levenshtein",
   "pyyaml",
   "wordcloud",
   "opencv-python",
   "spacy>=3.0.0,<4.0.0",
   "flair",
   "pandas",
@@ -57,8 +58,8 @@
 
 [tool.hatch.build.targets.sdist.force-include]
 "bnw_tools/ORKG/ResearchFields.json" = "bnw_tools/ORKG/ResearchFields.json"
 "bnw_tools/ORKG/RF_Map.json" = "bnw_tools/ORKG/RF_Map.json"
 
 [tool.hatch.build.targets.wheel.force-include]
 "bnw_tools/ORKG/ResearchFields.json" = "bnw_tools/ORKG/ResearchFields.json"
-"bnw_tools/ORKG/RF_Map.json" = "bnw_tools/ORKG/RF_Map.json"
+"bnw_tools/ORKG/RF_Map.json" = "bnw_tools/ORKG/RF_Map.json"
```

### Comparing `bnw_tools-0.0.1.4/PKG-INFO` & `bnw_tools-0.0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bnw_tools
-Version: 0.0.1.4
+Version: 0.0.2.0
 Summary: Tools developed in the BorgNetzWerk project for the extraction, analysis and publication of knowledge.
 Project-URL: Homepage, https://borgnetzwerk.de/
 Project-URL: Repository, https://github.com/borgnetzwerk/tools
 Project-URL: Issues, https://github.com/borgnetzwerk/tools/issues
 Author-email: BorgNetzWerk <info@borgnetzwerk.de>, Tim Wittenborg <tim.wittenborg@l3s.uni-hannover.de>
 License-File: LICENSE
 Keywords: BorgNetzWerk,ORKG,knowledge,literature,media
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: <3.12,>=3.8
 Requires-Dist: bibtexparser
 Requires-Dist: flair
 Requires-Dist: jupyter
 Requires-Dist: levenshtein
 Requires-Dist: mutagen
 Requires-Dist: opencv-python
 Requires-Dist: pandas
@@ -23,14 +23,15 @@
 Requires-Dist: pdfminer
 Requires-Dist: pdfminer-six
 Requires-Dist: pdfquery
 Requires-Dist: pdfrw
 Requires-Dist: pymupdf
 Requires-Dist: pypdf2
 Requires-Dist: pyyaml
+Requires-Dist: scipy==1.10.1
 Requires-Dist: spacy<4.0.0,>=3.0.0
 Requires-Dist: termcolor
 Requires-Dist: wordcloud
 Requires-Dist: wordfreq
 Provides-Extra: whisper
 Requires-Dist: openai-whisper; extra == 'whisper'
 Provides-Extra: youtube
```

