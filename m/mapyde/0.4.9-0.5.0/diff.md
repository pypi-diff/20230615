# Comparing `tmp/mapyde-0.4.9.tar.gz` & `tmp/mapyde-0.5.0.tar.gz`

## Comparing `mapyde-0.4.9.tar` & `mapyde-0.5.0.tar`

### file list

```diff
@@ -1,132 +1,135 @@
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 mapyde-0.4.9/mkdocs.yml
--rw-r--r--   0        0        0    31329 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/FCChh.tcl
--rw-r--r--   0        0        0    30874 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/FCChh_PileUp.tcl
--rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS.tcl
--rw-r--r--   0        0        0    21543 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl
--rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl
--rw-r--r--   0        0        0    24350 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl
--rw-r--r--   0        0        0    53993 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/dzResolutionVsP.tcl
--rw-r--r--   0        0        0    61796 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/momentumResolutionVsP.tcl
--rw-r--r--   0        0        0    77748 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/muonMomentumResolutionVsP.tcl
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_c1c1_nodecays
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1_nodecays
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1_nojets_nodecays
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nodecays
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nojets_nodecays
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nodecays
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nojets_nodecays
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2n1_nodecays
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2n1_nojets_nodecays
--rw-r--r--   0        0        0    17921 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/GluinoBino.slha
--rw-r--r--   0        0        0    18960 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/Higgsino.slha
--rw-r--r--   0        0        0    48855 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/Higgsino_CMS_v4.slha
--rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/SleptonBino.slha
--rw-r--r--   0        0        0    20649 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/SleptonSneutrinoBino.slha
--rw-r--r--   0        0        0    22557 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/SleptonWinoBino.slha
--rw-r--r--   0        0        0    17927 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/StopBino.slha
--rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/WinoBino.slha
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/sm-full.slha
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/sm.slha
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/Hbb
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWK
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos_v4
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p_v4
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_v4
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p_v4
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_N2C1p
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VjjEWK
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VjjQCD
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/Zbb
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/Zmumu
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/charginos
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/gluons
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_c1c1
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_c1c1_nodecays
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1_nodecays
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1_nojets
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1_nojets_nodecays
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1m_nodecays
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1p_nodecays
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1_nodecays
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1_nojets
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1_nojets_nodecays
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_nodecays
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_nojets
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_nojets_nodecays
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isrinc
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isrinc2j
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isrslep
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/quarks
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/stops
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/stops_and_ttbar
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/ttbar
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/ttbar_and_gluino
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/pythia/pythia8_card.dat
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/pythia/pythia8_card_MLM.dat
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/pythia/pythia8_card_dipoleRecoil.dat
--rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/run/default_LO.dat
--rw-r--r--   0        0        0    17505 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/run/default_LO_oldformat.dat
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/run/default_NLO.dat
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/sherpa/tt
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/sherpa/ttbbjj
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/gen_ref_nav.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/index.md
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/install.md
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/intro.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/.overrides/main.html
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/assets/css/custom.css
--rw-r--r--   0        0        0    29259 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/assets/images/logo.svg
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/cli/about.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/cli/reference.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/meta/authors.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/meta/faq.md
--rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.4.9/likelihoods/Higgsino_2L_bkgonly.json
--rw-r--r--   0        0        0  1192502 2020-02-02 00:00:00.000000 mapyde-0.4.9/likelihoods/Slepton_bkgonly.json
--rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.4.9/likelihoods/WinoBino_noWeight_2L_bkgonly.json
--rwxr-xr-x   0        0        0     8087 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/Delphes2SA.py
--rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/FlatAna.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/FlatAna_uproot.py
--rw-r--r--   0        0        0    31519 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/HistCollections.py
--rwxr-xr-x   0        0        0     3750 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/SAtoJSON.py
--rwxr-xr-x   0        0        0     4109 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/SimpleAna.py
--rwxr-xr-x   0        0        0      793 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/formatSLHA.py
--rwxr-xr-x   0        0        0     1623 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/hepmcsplitter.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/likelihoodfitting.py
--rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/lowlevelAna.py
--rwxr-xr-x   0        0        0     4420 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/muscan.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/root2hdf5.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/root2hdf5_slepton.py
--rwxr-xr-x   0        0        0     2319 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/tthhAna.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/_version.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/_version.pyi
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/container.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/prefix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/py.typed
--rw-r--r--   0        0        0    17331 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/runner.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/typing.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/backends/__init__.py
--rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/backends/madgraph.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/cli/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/cli/config.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/cli/run.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 mapyde-0.4.9/templates/defaults.toml
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 mapyde-0.4.9/templates/ewkinos.toml
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 mapyde-0.4.9/templates/sleptons.toml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mapyde-0.4.9/tests/test_package.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mapyde-0.4.9/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mapyde-0.4.9/LICENSE
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 mapyde-0.4.9/README.md
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 mapyde-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 mapyde-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 mapyde-0.5.0/CITATION.cff
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 mapyde-0.5.0/mkdocs.yml
+-rw-r--r--   0        0        0    31329 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/FCChh.tcl
+-rw-r--r--   0        0        0    30874 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/FCChh_PileUp.tcl
+-rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/delphes_card_ATLAS.tcl
+-rw-r--r--   0        0        0    21543 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl
+-rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl
+-rw-r--r--   0        0        0    24350 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl
+-rw-r--r--   0        0        0    53993 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/dzResolutionVsP.tcl
+-rw-r--r--   0        0        0    61796 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/momentumResolutionVsP.tcl
+-rw-r--r--   0        0        0    77748 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/delphes/muonMomentumResolutionVsP.tcl
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_c1c1_nodecays
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2c1_nodecays
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2c1_nojets_nodecays
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2c1m_nodecays
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2c1m_nojets_nodecays
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2c1p_nodecays
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2c1p_nojets_nodecays
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2n1_nodecays
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/madspin/isr2L_n2n1_nojets_nodecays
+-rw-r--r--   0        0        0    17921 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/GluinoBino.slha
+-rw-r--r--   0        0        0    18960 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/Higgsino.slha
+-rw-r--r--   0        0        0    48855 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/Higgsino_CMS_v4.slha
+-rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/SleptonBino.slha
+-rw-r--r--   0        0        0    20649 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/SleptonSneutrinoBino.slha
+-rw-r--r--   0        0        0    22557 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/SleptonWinoBino.slha
+-rw-r--r--   0        0        0    17927 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/StopBino.slha
+-rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/WinoBino.slha
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/sm-full.slha
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/param/sm.slha
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/Hbb
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWK
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_charginos
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_charginos_v4
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_n2c1p
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_n2c1p_v4
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_v4
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWK_n2c1p
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_EWK_n2c1p_v4
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VBFSUSY_N2C1p
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VjjEWK
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/VjjQCD
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/Zbb
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/Zmumu
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/charginos
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/gluons
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_c1c1
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_c1c1_nodecays
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2c1
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2c1_nodecays
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2c1_nojets
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2c1_nojets_nodecays
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2c1m_nodecays
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2c1p_nodecays
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2n1
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2n1_nodecays
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2n1_nojets
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_n2n1_nojets_nodecays
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_nodecays
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_nojets
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isr2L_nojets_nodecays
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isrinc
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isrinc2j
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/isrslep
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/quarks
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/stops
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/stops_and_ttbar
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/ttbar
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/process/ttbar_and_gluino
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/pythia/pythia8_card.dat
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/pythia/pythia8_card_MLM.dat
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/pythia/pythia8_card_dipoleRecoil.dat
+-rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/run/default_LO.dat
+-rw-r--r--   0        0        0    17505 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/run/default_LO_oldformat.dat
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/run/default_NLO.dat
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/sherpa/tt
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 mapyde-0.5.0/cards/sherpa/ttbbjj
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/index.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/install.md
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/intro.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/.overrides/main.html
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    29259 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/cli/about.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/cli/reference.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/meta/authors.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mapyde-0.5.0/docs/meta/faq.md
+-rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.5.0/likelihoods/Higgsino_2L_bkgonly.json
+-rw-r--r--   0        0        0  1192502 2020-02-02 00:00:00.000000 mapyde-0.5.0/likelihoods/Slepton_bkgonly.json
+-rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.5.0/likelihoods/WinoBino_noWeight_2L_bkgonly.json
+-rwxr-xr-x   0        0        0     8087 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/Delphes2SA.py
+-rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/FlatAna.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/FlatAna_uproot.py
+-rw-r--r--   0        0        0    31527 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/HistCollections.py
+-rwxr-xr-x   0        0        0     3750 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/SAtoJSON.py
+-rwxr-xr-x   0        0        0     4109 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/SimpleAna.py
+-rwxr-xr-x   0        0        0      793 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/formatSLHA.py
+-rwxr-xr-x   0        0        0     1623 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/hepmcsplitter.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/likelihoodfitting.py
+-rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/lowlevelAna.py
+-rwxr-xr-x   0        0        0     4583 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/muscan.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/root2hdf5.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/root2hdf5_slepton.py
+-rwxr-xr-x   0        0        0     2319 2020-02-02 00:00:00.000000 mapyde-0.5.0/scripts/tthhAna.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/_version.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/_version.pyi
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/container.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/prefix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/py.typed
+-rw-r--r--   0        0        0    17353 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/runner.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/typing.py
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/backends/__init__.py
+-rw-r--r--   0        0        0    11516 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/backends/madgraph.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/cli/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/cli/config.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 mapyde-0.5.0/src/mapyde/cli/run.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 mapyde-0.5.0/templates/defaults.toml
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mapyde-0.5.0/templates/ewkinos.toml
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapyde-0.5.0/templates/sleptons.toml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 mapyde-0.5.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 mapyde-0.5.0/tests/test_config.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mapyde-0.5.0/tests/test_package.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mapyde-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mapyde-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 mapyde-0.5.0/README.md
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 mapyde-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 mapyde-0.5.0/PKG-INFO
```

### Comparing `mapyde-0.4.9/mkdocs.yml` & `mapyde-0.5.0/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         name: Switch to dark mode
   features:
     - navigation.sections
     - navigation.expand
     - navigation.tabs
     - navigation.tabs.sticky
     - navigation.instant
+    - content.code.copy
+    - content.code.annotate
 
 nav:
   - Home:
       - About: index.md
       - Installation: install.md
       - Introduction: intro.md
       - Code Reference: reference/
```

### Comparing `mapyde-0.4.9/cards/delphes/FCChh.tcl` & `mapyde-0.5.0/cards/delphes/FCChh.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/FCChh_PileUp.tcl` & `mapyde-0.5.0/cards/delphes/FCChh_PileUp.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS.tcl` & `mapyde-0.5.0/cards/delphes/delphes_card_ATLAS.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl` & `mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl` & `mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl` & `mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl` & `mapyde-0.5.0/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/dzResolutionVsP.tcl` & `mapyde-0.5.0/cards/delphes/dzResolutionVsP.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/momentumResolutionVsP.tcl` & `mapyde-0.5.0/cards/delphes/momentumResolutionVsP.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/delphes/muonMomentumResolutionVsP.tcl` & `mapyde-0.5.0/cards/delphes/muonMomentumResolutionVsP.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_c1c1_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_c1c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2c1_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2c1_nojets_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2c1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2c1m_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nojets_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2c1m_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2c1p_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nojets_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2c1p_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2n1_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2n1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/madspin/isr2L_n2n1_nojets_nodecays` & `mapyde-0.5.0/cards/madspin/isr2L_n2n1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/GluinoBino.slha` & `mapyde-0.5.0/cards/param/GluinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/Higgsino.slha` & `mapyde-0.5.0/cards/param/Higgsino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/Higgsino_CMS_v4.slha` & `mapyde-0.5.0/cards/param/Higgsino_CMS_v4.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/SleptonBino.slha` & `mapyde-0.5.0/cards/param/SleptonBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/SleptonSneutrinoBino.slha` & `mapyde-0.5.0/cards/param/SleptonSneutrinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/SleptonWinoBino.slha` & `mapyde-0.5.0/cards/param/SleptonWinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/StopBino.slha` & `mapyde-0.5.0/cards/param/StopBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/WinoBino.slha` & `mapyde-0.5.0/cards/param/WinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/sm-full.slha` & `mapyde-0.5.0/cards/param/sm-full.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/param/sm.slha` & `mapyde-0.5.0/cards/param/sm.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWK` & `mapyde-0.5.0/cards/process/VBFSUSY_EWK`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD` & `mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos` & `mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_charginos`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos_v4` & `mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_charginos_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p` & `mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_n2c1p`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p_v4` & `mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_n2c1p_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_v4` & `mapyde-0.5.0/cards/process/VBFSUSY_EWKQCD_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p` & `mapyde-0.5.0/cards/process/VBFSUSY_EWK_n2c1p`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p_v4` & `mapyde-0.5.0/cards/process/VBFSUSY_EWK_n2c1p_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/VBFSUSY_N2C1p` & `mapyde-0.5.0/cards/process/VBFSUSY_N2C1p`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/charginos` & `mapyde-0.5.0/cards/process/charginos`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L` & `mapyde-0.5.0/cards/process/isr2L`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_c1c1` & `mapyde-0.5.0/cards/process/isr2L_c1c1`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_c1c1_nodecays` & `mapyde-0.5.0/cards/process/isr2L_c1c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2c1` & `mapyde-0.5.0/cards/process/isr2L_n2c1`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2c1_nodecays` & `mapyde-0.5.0/cards/process/isr2L_n2c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2c1_nojets` & `mapyde-0.5.0/cards/process/isr2L_n2c1_nojets`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2c1_nojets_nodecays` & `mapyde-0.5.0/cards/process/isr2L_n2c1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2c1m_nodecays` & `mapyde-0.5.0/cards/process/isr2L_n2c1m_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2c1p_nodecays` & `mapyde-0.5.0/cards/process/isr2L_n2c1p_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2n1` & `mapyde-0.5.0/cards/process/isr2L_n2n1`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2n1_nodecays` & `mapyde-0.5.0/cards/process/isr2L_n2n1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2n1_nojets` & `mapyde-0.5.0/cards/process/isr2L_n2n1_nojets`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_n2n1_nojets_nodecays` & `mapyde-0.5.0/cards/process/isr2L_n2n1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_nodecays` & `mapyde-0.5.0/cards/process/isr2L_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_nojets` & `mapyde-0.5.0/cards/process/isr2L_nojets`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isr2L_nojets_nodecays` & `mapyde-0.5.0/cards/process/isr2L_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isrinc` & `mapyde-0.5.0/cards/process/isrinc`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isrinc2j` & `mapyde-0.5.0/cards/process/isrinc2j`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/isrslep` & `mapyde-0.5.0/cards/process/isrslep`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/stops` & `mapyde-0.5.0/cards/process/stops`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/stops_and_ttbar` & `mapyde-0.5.0/cards/process/stops_and_ttbar`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/process/ttbar_and_gluino` & `mapyde-0.5.0/cards/process/ttbar_and_gluino`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/pythia/pythia8_card.dat` & `mapyde-0.5.0/cards/pythia/pythia8_card.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/pythia/pythia8_card_MLM.dat` & `mapyde-0.5.0/cards/pythia/pythia8_card_MLM.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/pythia/pythia8_card_dipoleRecoil.dat` & `mapyde-0.5.0/cards/pythia/pythia8_card_dipoleRecoil.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/run/default_LO.dat` & `mapyde-0.5.0/cards/run/default_LO.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/run/default_LO_oldformat.dat` & `mapyde-0.5.0/cards/run/default_LO_oldformat.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/run/default_NLO.dat` & `mapyde-0.5.0/cards/run/default_NLO.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/sherpa/tt` & `mapyde-0.5.0/cards/sherpa/tt`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/cards/sherpa/ttbbjj` & `mapyde-0.5.0/cards/sherpa/ttbbjj`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/docs/gen_ref_nav.py` & `mapyde-0.5.0/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/docs/index.md` & `mapyde-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/docs/install.md` & `mapyde-0.5.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/docs/intro.md` & `mapyde-0.5.0/docs/intro.md`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/docs/assets/css/custom.css` & `mapyde-0.5.0/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/docs/assets/images/logo.svg` & `mapyde-0.5.0/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/likelihoods/Higgsino_2L_bkgonly.json` & `mapyde-0.5.0/likelihoods/Higgsino_2L_bkgonly.json`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/likelihoods/Slepton_bkgonly.json` & `mapyde-0.5.0/likelihoods/Slepton_bkgonly.json`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/likelihoods/WinoBino_noWeight_2L_bkgonly.json` & `mapyde-0.5.0/likelihoods/WinoBino_noWeight_2L_bkgonly.json`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/Delphes2SA.py` & `mapyde-0.5.0/scripts/Delphes2SA.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/FlatAna.py` & `mapyde-0.5.0/scripts/FlatAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/FlatAna_uproot.py` & `mapyde-0.5.0/scripts/FlatAna_uproot.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/HistCollections.py` & `mapyde-0.5.0/scripts/HistCollections.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,16 +654,16 @@
                         )
         self.branches["chi"][0] = min(chisq)
 
         # Leptons
         lepCount = 1
         for aLep in event.sortedleptons:
             self.branches["lepton%dpT" % lepCount][0] = aLep.PT
-            self.branches["lepton%dpT" % lepCount][0] = aLep.Eta
-            self.branches["lepton%dpT" % lepCount][0] = aLep.Phi
+            self.branches["lepton%deta" % lepCount][0] = aLep.Eta
+            self.branches["lepton%dphi" % lepCount][0] = aLep.Phi
             self.branches["mt%d" % lepCount][0] = ROOT.TMath.Sqrt(
                 2
                 * event.met.Pt()
                 * aLep.PT
                 * (1 - ROOT.TMath.Cos(aLep.P4().DeltaPhi(event.met)))
             )
             mindr = 999
@@ -672,16 +672,16 @@
             self.branches["dr%d" % lepCount][0] = mindr
             lepCount = lepCount + 1
             if lepCount >= self.maxleptons:
                 break
 
         for i in range(lepCount, self.maxleptons):
             self.branches["lepton%dpT" % i][0] = defaultfill
-            self.branches["lepton%dpT" % i][0] = defaultfill
-            self.branches["lepton%dpT" % i][0] = defaultfill
+            self.branches["lepton%deta" % i][0] = defaultfill
+            self.branches["lepton%dphi" % i][0] = defaultfill
             self.branches["mt%d" % i][0] = defaultfill
             self.branches["dr%d" % i][0] = defaultfill
 
         self.tree.Fill()
 
 
 # =====================================================================
@@ -781,16 +781,16 @@
             self.branches["jet%dphi" % i][0] = defaultfill
             self.branches["jet%db" % i][0] = defaultfill
 
         # Leptons
         lepCount = 1
         for aLep in event.sortedleptons:
             self.branches["lepton%dpT" % lepCount][0] = aLep.PT
-            self.branches["lepton%dpT" % lepCount][0] = aLep.Eta
-            self.branches["lepton%dpT" % lepCount][0] = aLep.Phi
+            self.branches["lepton%deta" % lepCount][0] = aLep.Eta
+            self.branches["lepton%dphi" % lepCount][0] = aLep.Phi
             self.branches["lepton%dmT" % lepCount][0] = ROOT.TMath.Sqrt(
                 2
                 * event.met.Pt()
                 * aLep.PT
                 * (1 - ROOT.TMath.Cos(aLep.P4().DeltaPhi(event.met)))
             )
             mindr = 999
@@ -799,16 +799,16 @@
             self.branches["lepton%dminjetdr" % lepCount][0] = mindr
             lepCount = lepCount + 1
             if lepCount >= self.maxleptons:
                 break
 
         for i in range(lepCount, self.maxleptons):
             self.branches["lepton%dpT" % i][0] = defaultfill
-            self.branches["lepton%dpT" % i][0] = defaultfill
-            self.branches["lepton%dpT" % i][0] = defaultfill
+            self.branches["lepton%deta" % i][0] = defaultfill
+            self.branches["lepton%dphi" % i][0] = defaultfill
             self.branches["lepton%dmT" % i][0] = defaultfill
             self.branches["lepton%dminjetdr" % i][0] = defaultfill
 
         self.tree.Fill()
 
 
 # =====================================================================
```

### Comparing `mapyde-0.4.9/scripts/SAtoJSON.py` & `mapyde-0.5.0/scripts/SAtoJSON.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/SimpleAna.py` & `mapyde-0.5.0/scripts/SimpleAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/formatSLHA.py` & `mapyde-0.5.0/scripts/formatSLHA.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/hepmcsplitter.py` & `mapyde-0.5.0/scripts/hepmcsplitter.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/likelihoodfitting.py` & `mapyde-0.5.0/scripts/likelihoodfitting.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/lowlevelAna.py` & `mapyde-0.5.0/scripts/lowlevelAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/muscan.py` & `mapyde-0.5.0/scripts/muscan.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 observations = ws.data(pdf)
 
 poi_values = np.linspace(0.1, 2, 10)
 
 init_pars = pdf.config.suggested_init()
 init_pars[pdf.config.poi_index] = 1.0
 
-obs_limit, exp_limits, (scan, results) = pyhf.infer.intervals.upperlimit(
+obs_limit, exp_limits, (scan, results) = pyhf.infer.intervals.upper_limits.upper_limit(
     observations, pdf, poi_values, level=0.05, return_results=True
 )
 
 print(f"Observed limit: {obs_limit}")
 print("Expected limit: %5.3f" % exp_limits[2])
 print("      -1 sigma: %5.3f" % exp_limits[1])
 print("      +1 sigma: %5.3f" % exp_limits[3])
@@ -143,14 +143,18 @@
         "observed": float(cls_results[0]),
         "expected": float(cls_results[1][2]),
         "p1sigma": float(cls_results[1][3]),
         "m1sigma": float(cls_results[1][1]),
         "p2sigma": float(cls_results[1][4]),
         "m2sigma": float(cls_results[1][0]),
     },
+    "scan": pyhf.tensorlib.tolist(scan),
+    "results": [
+        (pyhf.tensorlib.tolist(x[0]), pyhf.tensorlib.tolist(x[1])) for x in results
+    ],
 }
 
 # print(json.dumps(jsonoutput,indent=4))
 
 # make a json output file
 with open("muscan_results.json", "w") as jsonoutputfile:
     json.dump(jsonoutput, jsonoutputfile, indent=4)
```

### Comparing `mapyde-0.4.9/scripts/root2hdf5.py` & `mapyde-0.5.0/scripts/root2hdf5.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/root2hdf5_slepton.py` & `mapyde-0.5.0/scripts/root2hdf5_slepton.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/scripts/tthhAna.py` & `mapyde-0.5.0/scripts/tthhAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/src/mapyde/__init__.py` & `mapyde-0.5.0/src/mapyde/__init__.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/src/mapyde/container.py` & `mapyde-0.5.0/src/mapyde/container.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/src/mapyde/prefix.py` & `mapyde-0.5.0/src/mapyde/prefix.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,50 +12,51 @@
 from mapyde.typing import PathOrStr, Self
 
 
 class Prefix(sys.modules[__name__].__class__):  # type: ignore[misc]
     """
     A module-level wrapper around :mod:`mapyde` which will provide the prefixes
 
-    .. rubric:: Example (callable)
+    Examples:
 
-    .. code-block:: pycon
+    === "Callable"
 
+        ```pycon
         >>> import mapyde.prefix
         >>> import pathlib
         >>> curr_path = mapyde.prefix.data
         >>> curr_path  # doctest: +ELLIPSIS
         PosixPath('.../pyhf/schemas')
         >>> new_path = pathlib.Path("/home/root/my/new/path")
         >>> mapyde.prefix(new_path)  # doctest: +ELLIPSIS
         <module 'mapyde.prefix' from ...>
         >>> mapyde.prefix.data
         PosixPath('/home/root/my/new/path')
         >>> mapyde.prefix(curr_path)  # doctest: +ELLIPSIS
         <module 'mapyde.prefix' from ...>
         >>> mapyde.prefix.data  # doctest: +ELLIPSIS
         PosixPath('.../pyhf/schemas')
+        ```
 
-    .. rubric:: Example (context-manager)
-
-    .. code-block:: pycon
+    === "Context Manager"
 
+        ```pycon
         >>> import mapyde.prefix
         >>> import pathlib
         >>> curr_path = mapyde.prefix.data
         >>> curr_path  # doctest: +ELLIPSIS
         PosixPath('.../pyhf/schemas')
         >>> new_path = pathlib.Path("/home/root/my/new/path")
         >>> with mapyde.prefix(new_path):
         ...     print(repr(mapyde.prefix.data))
         ...
         PosixPath('/home/root/my/new/path')
         >>> mapyde.prefix.data  # doctest: +ELLIPSIS
         PosixPath('.../pyhf/schemas')
-
+        ```
     """
 
     suffix_cards: str = "cards"
     suffix_likelihoods: str = "likelihoods"
     suffix_scripts: str = "scripts"
     suffix_templates: str = "templates"
     _data: Path = Path()
```

### Comparing `mapyde-0.4.9/src/mapyde/runner.py` & `mapyde-0.5.0/src/mapyde/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         config["base"]["output"] = config["base"]["output"] + "_nodecays"
         config["pythia"]["skip"] = True
 
         madgraph.generate_mg5config(config)
 
         image = f"ghcr.io/scipp-atlas/mapyde/{config['madgraph']['version']}"
         command = bytes(
-            f"mg5_aMC /data/{config['madgraph']['generator']['output']} && rsync -a PROC_madgraph /data/madgraph\n",
+            f"mg5_aMC /data/{config['madgraph']['output']} && rsync -a PROC_madgraph /data/madgraph\n",
             "utf-8",
         )
 
         with Container(
             image=image,
             name=f"{config['base']['output']}__mgpy",
             engine=config["base"].get("engine", "docker"),
@@ -95,20 +95,20 @@
         config["base"]["output"] = origout
         config["pythia"]["skip"] = origpythia
 
     madgraph.generate_mg5config(config)
 
     image = f"ghcr.io/scipp-atlas/mapyde/{config['madgraph']['version']}"
     command = bytes(
-        f"mg5_aMC /data/{config['madgraph']['generator']['output']} && rsync -a PROC_madgraph /data/madgraph\n",
+        f"mg5_aMC /data/{config['madgraph']['output']} && rsync -a PROC_madgraph /data/madgraph\n",
         "utf-8",
     )
     if config["madgraph"].get("keep_output", False):
         command = bytes(
-            f"mg5_aMC /data/{config['madgraph']['generator']['output']} && \
+            f"mg5_aMC /data/{config['madgraph']['output']} && \
 mkdir -p /data/madgraph && \
 rsync -a PROC_madgraph/Events/run_01/unweighted_events.lhe.gz /data/madgraph/ && \
 rsync -a PROC_madgraph/Events/run_01/tag_1_pythia8_events.hepmc.gz /data/madgraph/ \n",
             "utf-8",
         )
 
     with Container(
@@ -367,40 +367,41 @@
 ) -> tuple[bytes, bytes, MutableConfig]:
     """
     Run statistical inference via pyhf.
     """
     assert config
 
     image = f"ghcr.io/scipp-atlas/mapyde/{config['pyhf']['image']}"
+    script = Path("/scripts", config["pyhf"]["script"])
     command = bytes(
-        f"""python3.8 /scripts/muscan.py -b /likelihoods/{config['pyhf']['likelihood']} -s {config['sa2json']['output']} -n {config['base']['output']} {config['pyhf']['gpu-options']} {config['pyhf']['other-options']}""",
+        f"""python3.8 {script} -b /likelihoods/{config['pyhf']['likelihood']} -s {config['sa2json']['output']} -n {config['base']['output']} {config['pyhf']['gpu-options']} {config['pyhf']['other-options']}""",
         "utf-8",
     )
 
     dumpconfig(config)
 
     addl_opts = None
     if "-c" not in config["pyhf"]["gpu-options"]:
         addl_opts = ["--gpus", "all"]
 
     with Container(
         image=image,
-        name=f"{config['base']['output']}__muscan",
+        name=f"{config['base']['output']}__{script.stem}",
         engine=config["base"].get("engine", "docker"),
         mounts=mounts(config),
         stdout=sys.stdout,
         output_path=utils.output_path(config),
         logs_path=config["base"]["logs"],
         cwd="/data",
         additional_options=addl_opts,
     ) as container:
         stdout, stderr = container.call(command)
 
     with Path(config["base"]["path"]).joinpath(
-        config["base"]["output"], "muscan_results.json"
+        config["base"]["output"], f"{script.stem}_results.json"
     ).open(encoding="utf-8") as fpointer:
         data = json.load(fpointer)
 
     return (
         stdout,
         stderr,
         data,
```

### Comparing `mapyde-0.4.9/src/mapyde/typing.py` & `mapyde-0.5.0/src/mapyde/typing.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/src/mapyde/utils.py` & `mapyde-0.5.0/src/mapyde/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 import os
 import re
 import sys
 import typing as T
 import unicodedata
 from pathlib import Path
 
-import toml
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
+
+import tomli_w
 from jinja2 import Environment, FileSystemLoader, Template
 
 from mapyde import prefix
 from mapyde.typing import ImmutableConfig, MutableConfig
 
 # importlib.resources.as_file wasn't added until Python 3.9
 # c.f. https://docs.python.org/3.9/library/importlib.html#importlib.resources.as_file
@@ -47,21 +52,21 @@
 def render_string(blob: str, variables: ImmutableConfig | None = None) -> str:
     """
     Render a string using various variables set by the mapyde package.
     """
     variables = variables or {}
     tpl = Template(blob)
     return tpl.render(
-        PWD=os.getenv("PWD"),
-        USER=os.getenv("USER"),
-        MAPYDE_DATA=prefix.data,  # type: ignore[attr-defined]
-        MAPYDE_CARDS=prefix.cards,  # type: ignore[attr-defined]  # pylint: disable=no-member
-        MAPYDE_LIKELIHOODS=prefix.likelihoods,  # type: ignore[attr-defined]  # pylint: disable=no-member
-        MAPYDE_SCRIPTS=prefix.scripts,  # type: ignore[attr-defined]  # pylint: disable=no-member
-        MAPYDE_TEMPLATES=prefix.templates,  # type: ignore[attr-defined]  # pylint: disable=no-member
+        PWD=Path(os.getenv("PWD", ".")).as_posix(),
+        USER=os.getenv("USER", "USER"),
+        MAPYDE_DATA=prefix.data.as_posix(),  # type: ignore[attr-defined]
+        MAPYDE_CARDS=prefix.cards.as_posix(),  # type: ignore[attr-defined]  # pylint: disable=no-member
+        MAPYDE_LIKELIHOODS=prefix.likelihoods.as_posix(),  # type: ignore[attr-defined]  # pylint: disable=no-member
+        MAPYDE_SCRIPTS=prefix.scripts.as_posix(),  # type: ignore[attr-defined]  # pylint: disable=no-member
+        MAPYDE_TEMPLATES=prefix.templates.as_posix(),  # type: ignore[attr-defined]  # pylint: disable=no-member
         **variables,
     )
 
 
 def env_override(value: T.Any, key: str) -> T.Any:
     """
     Helper function for jinja2 to override environment variables
@@ -74,53 +79,72 @@
     Helper function to load a local toml configuration by filename
     """
     env = Environment(loader=FileSystemLoader(cwd))
     env.filters["env_override"] = env_override
 
     tpl = env.get_template(filename)
     assert tpl.filename
-    with Path(tpl.filename).open(encoding="utf-8") as fpointer:
-        return toml.load(fpointer)
+    with Path(tpl.filename).open("rb") as fpointer:
+        return tomllib.load(fpointer)
 
 
-def build_config(user: MutableConfig) -> T.Any:
+def build_config(user: MutableConfig, depth: int = 0) -> T.Any:
     """
     Function to build a configuration from a user-provided toml configuration on top of the base/template one.
+
+    The templates can be further nested (this function is recursive) up to a maximum (non-configurable) depth of 10.
+
     """
 
-    template_path = Path(
-        render_string(
-            user["base"].get("template", "{{MAPYDE_TEMPLATES}}/defaults.toml")
-        )
+    template_str = user.get("base", {}).pop(
+        "template", str(prefix.templates / "defaults.toml")  # type: ignore[attr-defined]  # pylint: disable=no-member
     )
+    parent = {}
 
-    with resources.as_file(template_path) as template:
-        if not template.exists():
-            msg = f"{template_path} does not exist."
-            raise OSError(msg)
-        defaults = load_config(template.name, str(template.parent))
-
-    variables = merge(defaults, user)
-    return toml.loads(render_string(toml.dumps(variables), variables))
+    if template_str:
+        if depth >= 10:
+            msg = 'Maximum template depth (10) exceeded. This is likely due to your base template not having `"template" = false` set.'
+            raise RuntimeError(msg)
+
+        template_path = Path(render_string(template_str))
+
+        with resources.as_file(template_path) as template:
+            if not template.exists():
+                msg = f"{template_path} does not exist."
+                raise OSError(msg)
+            parent = build_config(
+                load_config(template.name, str(template.parent)), depth=depth + 1
+            )
+
+    variables = merge(parent, user)
+
+    # only render the entire merged configuration, not the intermediate ones
+    return (
+        variables
+        if depth
+        else tomllib.loads(render_string(tomli_w.dumps(variables), variables))
+    )
 
 
 def output_path(config: ImmutableConfig) -> Path:
     """
     Return the output path from the config.
     """
     return Path(config["base"]["path"]).joinpath(config["base"]["output"]).resolve()
 
 
 def slugify(value: str, allow_unicode: bool = False) -> str:
     """
-    Taken from https://github.com/django/django/blob/master/django/utils/text.py
-    Convert to ASCII if 'allow_unicode' is False. Convert spaces or repeated
-    dashes to single dashes. Remove characters that aren't alphanumerics,
-    underscores, or hyphens. Convert to lowercase. Also strip leading and
-    trailing whitespace, dashes, and underscores.
+    Taken from [django utils](https://github.com/django/django/blob/master/django/utils/text.py).
+
+    - Convert to ASCII if `allow_unicode` is False.
+    - Convert spaces or repeated dashes to single dashes.
+    - Remove characters that aren't alphanumerics, underscores, or hyphens.
+    - Convert to lowercase.
+    - Also strip leading and trailing whitespace, dashes, and underscores.
     """
     value = str(value)
     if allow_unicode:
         value = unicodedata.normalize("NFKC", value)
     else:
         value = (
             unicodedata.normalize("NFKD", value)
```

### Comparing `mapyde-0.4.9/src/mapyde/backends/madgraph.py` & `mapyde-0.5.0/src/mapyde/backends/madgraph.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,72 @@
 
 from mapyde.typing import ImmutableConfig
 
 logging.basicConfig()
 log = logging.getLogger()
 
 
+def generate_proc_card(config: ImmutableConfig, output_path: Path) -> Path:
+    """
+    Helper for creating the madgraph process card through two options:
+
+      - specifying the path inside process_path for the card to copy over
+      - specifying the contents as part of the config to use to make the process card
+
+    Examples:
+
+    ``` toml title="user_existing-card.toml"
+    [madgraph.proc]
+    name = "isrslep"
+    card = "{{madgraph['proc']['name']}}"
+    contents = false # (1)!
+    ```
+
+    1. specifying `false` (default) for the `contents` option while including the
+    path to the card is the way to copy the card `isrslep` from the process
+    card directory that is configured.
+
+    ``` toml title="user_on-the-fly.toml"
+    [madgraph.proc]
+    name = "isrslep"
+    card = false
+    contents = \"\"\"\\
+    import model MSSM_SLHA2
+    define lep = e- e+ mu- mu+ ta- ta+
+    generate p p > z, z > lep lep
+    output -f
+    \"\"\" # (1)!
+    ```
+
+    1. specifying the full process card contents to use for the process card will
+    generate a process card with the specified name instead of copying over
+    `isrslep` from the process card directory.
+    """
+
+    assert bool(config["madgraph"]["proc"]["card"]) ^ bool(
+        config["madgraph"]["proc"]["contents"]
+    ), "Must specify either the Madgraph process card to copy or the contents to use to generate a Madgraph process card."
+
+    if config["madgraph"]["proc"]["contents"]:
+        new_proc_card_path = output_path.joinpath(config["madgraph"]["proc"]["name"])
+        new_proc_card_path.write_text(config["madgraph"]["proc"]["contents"])
+    else:
+        # Copy the proc card
+        proc_card_path = (
+            Path(config["base"]["process_path"])
+            .joinpath(config["madgraph"]["proc"]["card"])
+            .resolve()
+        )
+        new_proc_card_path = output_path.joinpath(proc_card_path.name)
+        shutil.copyfile(proc_card_path, new_proc_card_path)
+
+    log.info("Process Card: %s", new_proc_card_path)
+    return new_proc_card_path
+
+
 def generate_mg5config(config: ImmutableConfig) -> None:
     """
     Helper for generating the madgraph configs. Replaces mg5creator.py.
     """
     old_versions = ["2.4.3", "2.3.3"]
     is_old_version = False
     if any(version in config["madgraph"]["version"] for version in old_versions):
@@ -80,17 +138,17 @@
                 new_pythia_card.write(config["pythia"]["additional_opts"])
 
         log.info("Pythia Card: %s", new_pythia_card_path)
         pythia_onoff = "Pythia8"
         pythia_config_path = f"/data/{new_pythia_card_path.name}"
 
     substitution = {
-        "ecms": float(config["madgraph"]["ecms"]) / 2,
-        "nevents": int(config["madgraph"]["nevents"]),
-        "iseed": int(config["madgraph"]["seed"]),
+        "ecms": float(config["madgraph"]["run"]["ecms"]) / 2,
+        "nevents": int(config["madgraph"]["run"]["nevents"]),
+        "iseed": int(config["madgraph"]["run"]["seed"]),
     }
 
     masses = config["madgraph"].get("masses", {})
     if any(key in masses for key in substitution):
         msg = "Particles cannot be named ecms, nevents, or iseed."
         raise ValueError(msg)
 
@@ -167,27 +225,18 @@
             fpointer.write(output)
 
     unused_keys = list(run_options.keys())
     if unused_keys:
         log.error("Unused keys supplied by you: %s", unused_keys)
         raise KeyError(unused_keys[0])
 
-    # Copy the proc card
-    proc_card_path = (
-        Path(config["base"]["process_path"])
-        .joinpath(config["madgraph"]["proc"]["card"])
-        .resolve()
-    )
-    new_proc_card_path = output_path.joinpath(proc_card_path.name)
-    log.info("Process Card: %s", new_proc_card_path)
-
-    shutil.copyfile(proc_card_path, new_proc_card_path)
+    new_proc_card_path = generate_proc_card(config, output_path)
 
     # Create the madgraph configuration card
-    mgconfig_card_path = output_path.joinpath(config["madgraph"]["generator"]["output"])
+    mgconfig_card_path = output_path.joinpath(config["madgraph"]["output"])
     log.info("MadGraph Config: %s", mgconfig_card_path)
 
     # Figure out the run_mode.  0=single core, 1=cluster, 2=multicore.
     if config["madgraph"]["batch"]:
         run_mode = "set run_mode 0"  # we don't have MadGraph launch cluster jobs for us, we handle that ourselves.
     elif int(config["madgraph"]["cores"]) > 0:
         run_mode = f"set run_mode 2\nset nb_core {config['madgraph']['cores']}"
@@ -231,15 +280,15 @@
 madspin={madspin_onoff}
 shower={pythia_onoff}
 reweight=OFF
 {madspin_config_path}
 /data/{new_param_card_path.name}
 /data/{new_run_card_path.name}
 {pythia_config_path}
-set iseed {config['madgraph']['seed']}
+set iseed {config['madgraph']['run']['seed']}
 done
 """
     if is_old_version:
         mg5config = f"""
 {run_mode}
 launch PROC_madgraph
 madspin={madspin_onoff}
@@ -248,15 +297,16 @@
 /data/{new_param_card_path.name}
 /data/{new_run_card_path.name}
 done
 """
 
     with mgconfig_card_path.open(mode="w", encoding="utf-8") as fpointer:
         # pylint: disable-next=consider-using-with
-        for proc_line in new_proc_card_path.open(encoding="utf-8"):
-            if not proc_line.strip():
-                continue
-            if proc_line.startswith("output"):
-                fpointer.write("output PROC_madgraph\n")
-            else:
-                fpointer.write(proc_line)
+        with new_proc_card_path.open(encoding="utf-8") as proc_lines:
+            for proc_line in proc_lines:
+                if not proc_line.strip():
+                    continue
+                if proc_line.startswith("output"):
+                    fpointer.write("output PROC_madgraph\n")
+                else:
+                    fpointer.write(proc_line)
         fpointer.write(mg5config)
```

### Comparing `mapyde-0.4.9/src/mapyde/cli/__init__.py` & `mapyde-0.5.0/src/mapyde/cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from __future__ import annotations
 
 from enum import Enum
 from typing import Optional
 
 import typer
+from trogon import Trogon
 
 import mapyde
 from mapyde.cli import config, run
 
 app = typer.Typer()
 app.add_typer(config.app, name="config")
 app.add_typer(run.app, name="run")
@@ -29,25 +30,30 @@
 
 
 PrefixOrNone = Optional[Prefix]
 
 
 @app.callback(invoke_without_command=True)
 def main(
+    ctx: typer.Context,
     version: bool = typer.Option(False, "--version", help="Print the current version."),
     prefix: PrefixOrNone = typer.Option(
         None, help="Print the path prefix for data files."
     ),
+    tui: bool = typer.Option(False, "--tui", help="Open Textual TUI."),
 ) -> None:
     """
     Manage top-level options
     """
     if version:
         typer.echo(f"mapyde v{mapyde.__version__}")
         raise typer.Exit()
     if prefix:
         typer.echo(getattr(mapyde.prefix, prefix.value).resolve())
         raise typer.Exit()
+    if tui:
+        Trogon(ctx.command, app_name=ctx.info_name, click_context=ctx).run()
+        ctx.exit()
 
 
 # for generating documentation using mkdocs-click
 typer_click_object = typer.main.get_command(app)
```

### Comparing `mapyde-0.4.9/src/mapyde/cli/config.py` & `mapyde-0.5.0/src/mapyde/cli/config.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/src/mapyde/cli/run.py` & `mapyde-0.5.0/src/mapyde/cli/run.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/templates/defaults.toml` & `mapyde-0.5.0/templates/sleptons.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [base]
-engine = "docker"
 path = "{{PWD}}"
 output = "output"
 logs = "logs"
 data_path = "{{MAPYDE_DATA}}"
 cards_path = "{{MAPYDE_CARDS}}"
 scripts_path = "{{MAPYDE_SCRIPTS}}"
 process_path = "{{MAPYDE_CARDS}}/process/"
@@ -12,87 +11,79 @@
 pythia_path = "{{MAPYDE_CARDS}}/pythia/"
 delphes_path = "{{MAPYDE_CARDS}}/delphes/"
 madspin_path = "{{MAPYDE_CARDS}}/madspin/"
 likelihoods_path = "{{MAPYDE_LIKELIHOODS}}"
 
 [madgraph]
 skip = false
-params = "Higgsino"
-ecms = 13000
-cores = 20
-nevents = 10000
-seed = 0
-version = "madgraph"
+params = "SleptonBino"
+cores = 1
+version = "madgraph:2.9.3"
 batch = false
 paramcard = "{{madgraph['params']}}.slha"
-
-[madgraph.generator]
 output = "run.mg5"
 
 [madgraph.masses]
-MN1 = 100
-MC1 = 150
+MSLEP = 250
+MN1 = 240
 
 [madgraph.run]
 card = "default_LO.dat"
+ecms = 13000
+nevents = 50000
+seed = 0
 
 [madgraph.run.options]
 mmjj = 0
 mmjjmax = -1
 deltaeta = 0
 ktdurham = -1
 xqcut = -1
 ptj = 20
-ptj1min = 0
+ptj1min = 50
 
 [madgraph.proc]
-name = "VBFSUSY_EWKQCD"
+name = "isrslep"
 card = "{{madgraph['proc']['name']}}"
 
 [madspin]
 skip = true
 card = ''
 
-[sherpa]
-proc="tt"
-nevents = 2
-cores = 1
-
 [pythia]
 skip = false
 card = "pythia8_card.dat"
 additional_opts = ""
 
 [delphes]
 skip = false
 additional_opts = ""
-card = "delphes_card_ATLAS.tcl"
+card = "delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl"
 version = "delphes"
 output = "delphes/delphes.root"
 
 [analysis]
 script = "Delphes2SA.py"
 XSoverride = -1
-kfactor = -1
+kfactor = 1.18
 output = "analysis/Delphes2SA.root"
-lumi = 1000
+lumi = 139000
 
 [simpleanalysis]
 skip = false
 additional_opts = ""
 name = "EwkCompressed2018"
+outputtag = ""
+input = ""
 
 [sa2json]
-inputs = "{{simpleanalysis['name']}}.root"
+inputs = "{{simpleanalysis['name']}}{{simpleanalysis['outputtag']}}.root"
 image = "pyplotting:latest"
-output = "{{simpleanalysis['name']}}_patch.json"
-options = ""
+output = "{{simpleanalysis['name']}}{{simpleanalysis['outputtag']}}_patch.json"
+options = "-c"
 
 [pyhf]
-skip = true
-likelihood = "Higgsino_2L_bkgonly.json"
+skip = false
+likelihood = "Slepton_bkgonly.json"
 image = "pyplotting:latest"
-gpu-options = "-c"
-
-[root2hdf5]
-input = "analysis/lowlevelAna.root"
-treename = "allev/lowleveltree"
+gpu-options = "-c -B jax"
+other-options = ""
```

### Comparing `mapyde-0.4.9/templates/ewkinos.toml` & `mapyde-0.5.0/templates/ewkinos.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,33 +12,31 @@
 delphes_path = "{{MAPYDE_CARDS}}/delphes/"
 madspin_path = "{{MAPYDE_CARDS}}/madspin/"
 likelihoods_path = "{{MAPYDE_LIKELIHOODS}}"
 
 [madgraph]
 skip = false
 params = "Higgsino"
-ecms = 13000
 cores = 1
-nevents = 50000
-seed = 0
 version = "madgraph:2.7.3"
 batch = false
 paramcard = "{{madgraph['params']}}.slha"
 run_without_decays = false
-
-[madgraph.generator]
 output = "run.mg5"
 
 [madgraph.masses]
 MN2 = 250
 MC1 = 250
 MN1 = 240
 
 [madgraph.run]
 card = "default_LO.dat"
+ecms = 13000
+nevents = 50000
+seed = 0
 
 [madgraph.run.options]
 mmjj = 0
 mmjjmax = -1
 deltaeta = 0
 ktdurham = -1
 ptj = 20
```

### Comparing `mapyde-0.4.9/.gitignore` & `mapyde-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/LICENSE` & `mapyde-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.9/README.md` & `mapyde-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mapyde v0.4.9
+# mapyde v0.5.0
 
 MaPyDe stands for MadGraph-Pythia-Delphes which is a utility that allows one to
 run all of the various HEP toolings or chain them together and perform a quick
 analysis with the results, such as running CERN ATLAS SimpleAnalysis or pyhf.
 
 ---
 
@@ -76,14 +76,17 @@
 configuration files significantly control how to run or execute the various
 steps in the chain of `mapyde`. Use the command line interface to get started:
 
 ```
 # display the help
 mapyde --help
 
+# open Textual TUI
+mapyde --tui
+
 # display the prefix path for data cards shipped with mapyde
 mapyde --prefix cards
 
 # parse and display the config
 mapyde config parse user.toml
 
 # run all steps
```

### Comparing `mapyde-0.4.9/pyproject.toml` & `mapyde-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,26 @@
     "Programming Language :: Python :: 3.10",
     "Development Status :: 1 - Planning",
 ]
 
 dependencies = [
     "typing_extensions >=3.7; python_version<'3.11'",
     "typer",
-    "toml",
+    "tomli; python_version<'3.11'",
+    "tomli-w",
     "jinja2",
     "in_place",
     "importlib_resources>=1.3.0; python_version<'3.9'",  # for resources in schema
+    "trogon", # tui
 ]
 
 # see https://github.com/pypi/warehouse/blob/main/warehouse/templates/packaging/detail.html
 [project.urls]
 Homepage = "https://scipp-atlas.github.io/mapyde/latest/"
-Documentation = "https://scipp-atlas.github.io/mapyde/0.4/"
+Documentation = "https://scipp-atlas.github.io/mapyde/0.5/"
 Tracker = "https://github.com/scipp-atlas/mapyde/issues"
 Source = "https://github.com/scipp-atlas/mapyde"
 
 [project.scripts]
 mapyde = "mapyde.cli:app"
 
 [tool.hatch.version]
@@ -105,15 +107,15 @@
 # pylint and pytest needs to be installed into package environment
 detached = false
 dependencies = [
     "pytest >=6",
 ]
 
 [tool.hatch.envs.dev.scripts]
-test = "pytest -ra"
+test = "pytest -ra {args}"
 
 [[tool.hatch.envs.dev.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3.8"]
 
 [tool.hatch.envs.docs]
 template = "docs"
 dependencies = [
@@ -176,14 +178,30 @@
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 
 [[tool.mypy.overrides]]
 module = 'in_place'
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+module = 'rich'
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = 'tomli'
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = 'tomli_w'
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = 'trogon'
+ignore_missing_imports = true
+
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
   "B",  "B904",  # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
   "C4",          # flake8-comprehensions
```

### Comparing `mapyde-0.4.9/PKG-INFO` & `mapyde-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mapyde
-Version: 0.4.9
+Version: 0.5.0
 Summary: Generation, simulation, analysis, and statistical inference in one go.
 Project-URL: Homepage, https://scipp-atlas.github.io/mapyde/latest/
-Project-URL: Documentation, https://scipp-atlas.github.io/mapyde/0.4/
+Project-URL: Documentation, https://scipp-atlas.github.io/mapyde/0.5/
 Project-URL: Tracker, https://github.com/scipp-atlas/mapyde/issues
 Project-URL: Source, https://github.com/scipp-atlas/mapyde
 Author-email: Giordon Stark <kratsg@gmail.com>
 Maintainer-email: Mike Hance <mhance@ucsc.edu>
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -22,20 +22,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.3.0; python_version < '3.9'
 Requires-Dist: in-place
 Requires-Dist: jinja2
-Requires-Dist: toml
+Requires-Dist: tomli-w
+Requires-Dist: tomli; python_version < '3.11'
+Requires-Dist: trogon
 Requires-Dist: typer
 Requires-Dist: typing-extensions>=3.7; python_version < '3.11'
 Description-Content-Type: text/markdown
 
-# mapyde v0.4.9
+# mapyde v0.5.0
 
 MaPyDe stands for MadGraph-Pythia-Delphes which is a utility that allows one to
 run all of the various HEP toolings or chain them together and perform a quick
 analysis with the results, such as running CERN ATLAS SimpleAnalysis or pyhf.
 
 ---
 
@@ -109,14 +111,17 @@
 configuration files significantly control how to run or execute the various
 steps in the chain of `mapyde`. Use the command line interface to get started:
 
 ```
 # display the help
 mapyde --help
 
+# open Textual TUI
+mapyde --tui
+
 # display the prefix path for data cards shipped with mapyde
 mapyde --prefix cards
 
 # parse and display the config
 mapyde config parse user.toml
 
 # run all steps
```

