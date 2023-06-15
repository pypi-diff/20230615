# Comparing `tmp/ir_datasets-0.5.4.tar.gz` & `tmp/ir_datasets-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_datasets-0.5.4.tar", last modified: Tue Oct 18 13:16:22 2022, max compression
+gzip compressed data, was "ir_datasets-0.5.5.tar", last modified: Thu Jun 15 08:55:11 2023, max compression
```

## Comparing `ir_datasets-0.5.4.tar` & `ir_datasets-0.5.5.tar`

### file list

```diff
@@ -1,177 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.841263 ir_datasets-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11910 2022-10-18 13:16:22.841263 ir_datasets-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11554 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.825263 ir_datasets-0.5.4/ir_datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.825263 ir_datasets-0.5.4/ir_datasets/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/build_c4_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/build_clueweb_warc_indexes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/build_download_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/doc_fifos.py
--rw-r--r--   0 runner    (1001) docker     (121)    10515 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/generate_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/commands/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.833263 ir_datasets-0.5.4/ir_datasets/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5400 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/antique.py
--rw-r--r--   0 runner    (1001) docker     (121)     8175 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/aol_ia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/aquaint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/argsme.py
--rw-r--r--   0 runner    (1001) docker     (121)    13855 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8793 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/beir.py
--rw-r--r--   0 runner    (1001) docker     (121)     9055 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/c4.py
--rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/car.py
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/clinicaltrials.py
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/clirmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    13530 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/clueweb09.py
--rw-r--r--   0 runner    (1001) docker     (121)    17323 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/clueweb12.py
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/codec.py
--rw-r--r--   0 runner    (1001) docker     (121)     7164 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/codesearchnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     9911 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/cord19.py
--rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/cranfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/disks45.py
--rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/dpr_w100.py
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/gov.py
--rw-r--r--   0 runner    (1001) docker     (121)    17244 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/gov2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/hc4.py
--rw-r--r--   0 runner    (1001) docker     (121)     7613 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/highwire.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/istella22.py
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/kilt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/lotte.py
--rw-r--r--   0 runner    (1001) docker     (121)     9346 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/medline.py
--rw-r--r--   0 runner    (1001) docker     (121)     4466 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/mmarco.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/mr_tydi.py
--rw-r--r--   0 runner    (1001) docker     (121)     8696 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/msmarco_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     8671 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/msmarco_document_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    19174 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/msmarco_passage.py
--rw-r--r--   0 runner    (1001) docker     (121)    11290 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/msmarco_passage_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    16491 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/msmarco_qna.py
--rw-r--r--   0 runner    (1001) docker     (121)     9612 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/natural_questions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3830 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/neuclir.py
--rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/neumarco.py
--rw-r--r--   0 runner    (1001) docker     (121)     7238 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/nfcorpus.py
--rw-r--r--   0 runner    (1001) docker     (121)    15594 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/nyt.py
--rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/pmc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8556 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/touche.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/touche_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/trec_arabic.py
--rw-r--r--   0 runner    (1001) docker     (121)     9284 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/trec_cast.py
--rw-r--r--   0 runner    (1001) docker     (121)    11304 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/trec_fair.py
--rw-r--r--   0 runner    (1001) docker     (121)     2146 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/trec_mandarin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/trec_robust04.py
--rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/trec_spanish.py
--rw-r--r--   0 runner    (1001) docker     (121)    16281 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/tripclick.py
--rw-r--r--   0 runner    (1001) docker     (121)    18852 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/tweets2013_ia.py
--rw-r--r--   0 runner    (1001) docker     (121)     3881 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/vaswani.py
--rw-r--r--   0 runner    (1001) docker     (121)     7033 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/wapo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/wikiclir.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/datasets/wikir.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.837263 ir_datasets-0.5.4/ir_datasets/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/antique.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/aol-ia.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/aquaint.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4214 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/argsme.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16889 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/beir.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    36978 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/bibliography.bib
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/c4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/car.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2705 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/clinicaltrials.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/clirmatrix.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4530 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/clueweb09.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7470 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/clueweb12.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/codec.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/codesearchnet.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5002 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/cord19.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/cranfield.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4479 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/disks45.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2184 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/dpr-w100.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/gov.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6202 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/gov2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/hc4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/highwire.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/istella22.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/kilt.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7868 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/lotte.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/medline.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    17454 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/mmarco.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5608 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/mr-tydi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/msmarco-document-v2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5810 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/msmarco-document.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/msmarco-passage-v2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8543 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/msmarco-passage.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/msmarco-qna.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/natural-questions.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/neuclir.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/neumarco.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/nfcorpus.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/nyt.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/pmc.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/touche-image.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13241 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/touche.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/trec-arabic.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/trec-cast.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/trec-fair.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/trec-mandarin.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/trec-robust04.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/trec-spanish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9088 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/tripclick.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/tweets2013-ia.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/vaswani.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/wapo.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/wikiclir.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5125 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/docs/wikir.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.837263 ir_datasets-0.5.4/ir_datasets/etc/
--rw-r--r--   0 runner    (1001) docker     (121)   160458 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/etc/downloads.json
--rw-r--r--   0 runner    (1001) docker     (121)   112874 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/etc/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.837263 ir_datasets-0.5.4/ir_datasets/formats/
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16425 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/argsme.py
--rw-r--r--   0 runner    (1001) docker     (121)    11698 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/clirmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/csv_fmt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/extracted_cc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2979 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/ntcir.py
--rw-r--r--   0 runner    (1001) docker     (121)    22982 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/touche.py
--rw-r--r--   0 runner    (1001) docker     (121)     8694 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/touche_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    19796 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/trec.py
--rw-r--r--   0 runner    (1001) docker     (121)     7038 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/tsv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/formats/webarc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.837263 ir_datasets-0.5.4/ir_datasets/indices/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/cache_docstore.py
--rw-r--r--   0 runner    (1001) docker     (121)    11317 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/clueweb_warc.py
--rw-r--r--   0 runner    (1001) docker     (121)    11612 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/indexed_tsv_docstore.py
--rw-r--r--   0 runner    (1001) docker     (121)     9776 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/lz4_pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/numpy_sorted_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     4824 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/indices/zpickle_docstore.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/lazy_libs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.841263 ir_datasets-0.5.4/ir_datasets/util/
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16067 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/util/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     9099 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/util/fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/util/html_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/util/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.841263 ir_datasets-0.5.4/ir_datasets/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/ir_datasets/wrappers/html_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 13:16:22.825263 ir_datasets-0.5.4/ir_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11910 2022-10-18 13:16:22.000000 ir_datasets-0.5.4/ir_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5224 2022-10-18 13:16:22.000000 ir_datasets-0.5.4/ir_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 13:16:22.000000 ir_datasets-0.5.4/ir_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-18 13:16:22.000000 ir_datasets-0.5.4/ir_datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-18 13:16:22.000000 ir_datasets-0.5.4/ir_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-18 13:16:22.000000 ir_datasets-0.5.4/ir_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 13:16:22.841263 ir_datasets-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-10-18 13:16:13.000000 ir_datasets-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.187492 ir_datasets-0.5.5/ir_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.187492 ir_datasets-0.5.5/ir_datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/build_c4_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/build_clueweb_warc_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/build_download_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/doc_fifos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/generate_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/commands/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.195492 ir_datasets-0.5.5/ir_datasets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/antique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/aol_ia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/aquaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/argsme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/beir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/c4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/clinicaltrials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/clirmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/clueweb09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/clueweb12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/codesearchnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/cord19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/cranfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/disks45.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/dpr_w100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/gov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/gov2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/hc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/highwire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/istella22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/kilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/lotte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/medline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/mmarco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/mr_tydi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/msmarco_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/msmarco_document_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19477 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/msmarco_passage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/msmarco_passage_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/msmarco_qna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/natural_questions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/neuclir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/neumarco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/nfcorpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/nyt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/sara.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/touche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/touche_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/trec_arabic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/trec_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/trec_fair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/trec_mandarin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/trec_robust04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/trec_spanish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/trec_tot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/tripclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/tweets2013_ia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/vaswani.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/wapo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/wikiclir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/datasets/wikir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.199492 ir_datasets-0.5.5/ir_datasets/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/antique.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/aol-ia.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/aquaint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/argsme.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/beir.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    36428 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/c4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/car.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/clinicaltrials.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/clirmatrix.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/clueweb09.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/clueweb12.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/codec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/codesearchnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/cord19.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/cranfield.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/disks45.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/dpr-w100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/gov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/gov2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/hc4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/highwire.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/istella22.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/kilt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/lotte.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/medline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/mmarco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/mr-tydi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/msmarco-document-v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/msmarco-document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/msmarco-passage-v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/msmarco-passage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/msmarco-qna.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/natural-questions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/neuclir.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/neumarco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/nfcorpus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/nyt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/pmc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/sara.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/touche-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/touche.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/trec-arabic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/trec-cast.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/trec-fair.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/trec-mandarin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/trec-robust04.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/trec-spanish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/trec-tot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/tripclick.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/tweets2013-ia.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/vaswani.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/wapo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/wikiclir.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/docs/wikir.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.199492 ir_datasets-0.5.5/ir_datasets/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)   170067 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/etc/downloads.json
+-rw-r--r--   0 runner    (1001) docker     (123)   114497 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/etc/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/ir_datasets/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/argsme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/clirmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/csv_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/extracted_cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/ntcir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/touche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/touche_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20214 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/trec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/formats/webarc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/ir_datasets/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/cache_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/clueweb_warc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/indexed_tsv_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/lz4_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/numpy_sorted_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/indices/zpickle_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/lazy_libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/ir_datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/util/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/util/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/util/html_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/util/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/ir_datasets/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/ir_datasets/wrappers/html_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.187492 ir_datasets-0.5.5/ir_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-06-15 08:55:11.000000 ir_datasets-0.5.5/ir_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-15 08:55:11.000000 ir_datasets-0.5.5/ir_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:55:11.000000 ir_datasets-0.5.5/ir_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 08:55:11.000000 ir_datasets-0.5.5/ir_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 08:55:11.000000 ir_datasets-0.5.5/ir_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 08:55:11.000000 ir_datasets-0.5.5/ir_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:55:11.203492 ir_datasets-0.5.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-15 08:54:57.000000 ir_datasets-0.5.5/test/test_defaulttext.py
```

### Comparing `ir_datasets-0.5.4/LICENSE` & `ir_datasets-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/PKG-INFO` & `ir_datasets-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ir_datasets
-Version: 0.5.4
+Version: 0.5.5
 Summary: provides a common interface to many IR ad-hoc ranking benchmarks, training datasets, etc.
 Home-page: https://github.com/allenai/ir_datasets
 Author: Sean MacAvaney
 Author-email: sean.macavaney@glasgow.ac.uk
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ir_datasets
 
 `ir_datasets` is a python package that provides a common interface to many IR ad-hoc ranking
 benchmarks, training datasets, etc.
@@ -51,15 +51,15 @@
 ```
 $ git clone https://github.com/allenai/ir_datasets
 $ cd ir_datasets
 $ python setup.py bdist_wheel
 $ pip install dist/ir_datasets-*.whl
 ```
 
-Tested with python versions 3.6 and 3.7
+Tested with python versions 3.7, 3.8, 3.9, and 3.10. (Mininum python version is 3.7.)
 
 ## Features
 
 **Python and Command Line Interfaces**. Access datasts both through a simple Python API and
 via the command line.
 
 ```python
```

### Comparing `ir_datasets-0.5.4/README.md` & `ir_datasets-0.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ```
 $ git clone https://github.com/allenai/ir_datasets
 $ cd ir_datasets
 $ python setup.py bdist_wheel
 $ pip install dist/ir_datasets-*.whl
 ```
 
-Tested with python versions 3.6 and 3.7
+Tested with python versions 3.7, 3.8, 3.9, and 3.10. (Mininum python version is 3.7.)
 
 ## Features
 
 **Python and Command Line Interfaces**. Access datasts both through a simple Python API and
 via the command line.
 
 ```python
```

### Comparing `ir_datasets-0.5.4/ir_datasets/__init__.py` & `ir_datasets-0.5.5/ir_datasets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,8 +97,8 @@
     commands.COMMANDS[args[0]](args[1:])
 
 
 def main_cli():
     import sys
     main(sys.argv[1:])
 
-__version__ = "0.5.4" # NOTE: keep this in sync with setup.py
+__version__ = "0.5.5" # NOTE: keep this in sync with setup.py
```

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/__init__.py` & `ir_datasets-0.5.5/ir_datasets/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/build_c4_checkpoints.py` & `ir_datasets-0.5.5/ir_datasets/commands/build_c4_checkpoints.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/build_clueweb_warc_indexes.py` & `ir_datasets-0.5.5/ir_datasets/commands/build_clueweb_warc_indexes.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/build_download_cache.py` & `ir_datasets-0.5.5/ir_datasets/commands/build_download_cache.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/clean.py` & `ir_datasets-0.5.5/ir_datasets/commands/clean.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/doc_fifos.py` & `ir_datasets-0.5.5/ir_datasets/commands/doc_fifos.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/export.py` & `ir_datasets-0.5.5/ir_datasets/commands/export.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/generate_metadata.py` & `ir_datasets-0.5.5/ir_datasets/commands/generate_metadata.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/commands/lookup.py` & `ir_datasets-0.5.5/ir_datasets/commands/lookup.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/__init__.py` & `ir_datasets-0.5.5/ir_datasets/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,19 @@
 from . import pmc
 from . import touche_image
 from . import touche  # must be after argsme,clueweb12,touche_image
 from . import trec_arabic
 from . import trec_mandarin
 from . import trec_spanish
 from . import trec_robust04
+from . import trec_tot
 from . import tripclick
 from . import tweets2013_ia
 from . import vaswani
 from . import wapo
 from . import wikiclir
 from . import wikir
 from . import trec_fair
 from . import trec_cast # must be after wapo,car,msmarco_passage
 from . import hc4
-from . import neuclir # must be after hc4
+from . import neuclir # must be after hc4
+from . import sara
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/antique.py` & `ir_datasets-0.5.5/ir_datasets/datasets/antique.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/aol_ia.py` & `ir_datasets-0.5.5/ir_datasets/datasets/aol_ia.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
 class AolIaDoc(NamedTuple):
     doc_id: str
     title: str
     text: str
     url: str
     ia_url: str
+    def default_text(self):
+        """
+        title and text
+        """
+        return f'{self.title} {self.text}'
 
 
 class AolQlogs(BaseQlogs):
     def __init__(self, dlc):
         self.dlc = dlc
 
     def qlogs_iter(self):
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/aquaint.py` & `ir_datasets-0.5.5/ir_datasets/datasets/aquaint.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/argsme.py` & `ir_datasets-0.5.5/ir_datasets/datasets/argsme.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/base.py` & `ir_datasets-0.5.5/ir_datasets/datasets/base.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/beir.py` & `ir_datasets-0.5.5/ir_datasets/datasets/beir.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,41 @@
 
 
 class BeirDoc(NamedTuple):
     doc_id: str
     text: str
     title: str
     metadata: Dict[str, str]
+    def default_text(self):
+        """
+        title text
+        """
+        return f'{self.title} {self.text}'
 
 
 class BeirTitleDoc(NamedTuple):
     doc_id: str
     text: str
     title: str
+    def default_text(self):
+        """
+        title text
+        """
+        return f'{self.title} {self.text}'
 
 class BeirTitleUrlDoc(NamedTuple):
     doc_id: str
     text: str
     title: str
     url: str
+    def default_text(self):
+        """
+        title text
+        """
+        return f'{self.title} {self.text}'
 
 class BeirSciDoc(NamedTuple):
     doc_id: str
     text: str
     title: str
     authors: List[str]
     year: int
@@ -42,27 +57,37 @@
 
 class BeirCordDoc(NamedTuple):
     doc_id: str
     text: str
     title: str
     url: str
     pubmed_id: str
+    def default_text(self):
+        """
+        title text
+        """
+        return f'{self.title} {self.text}'
 
 class BeirToucheDoc(NamedTuple):
     doc_id: str
     text: str
     title: str
     stance: str
     url: str
 
 class BeirCqaDoc(NamedTuple):
     doc_id: str
     text: str
     title: str
     tags: List[str]
+    def default_text(self):
+        """
+        title text
+        """
+        return f'{self.title} {self.text}'
 
 class BeirUrlQuery(NamedTuple):
     query_id: str
     text: str
     url: str
 
 class BeirSciQuery(NamedTuple):
@@ -80,19 +105,29 @@
     narrative: str
 
 class BeirCovidQuery(NamedTuple):
     query_id: str
     text: str
     query: str
     narrative: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 class BeirCqaQuery(NamedTuple):
     query_id: str
     text: str
     tags: List[str]
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 def _map_field(field, data):
     if field in ('doc_id', 'query_id'):
         return data['_id']
     if field == 'text':
         return data['text']
     if field == 'title':
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/c4.py` & `ir_datasets-0.5.5/ir_datasets/datasets/c4.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,34 @@
 
 
 class C4Doc(NamedTuple):
     doc_id: str
     text: str
     url: str
     timestamp: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class MisinfoQuery(NamedTuple):
     query_id: str
     text: str
     description: str
     narrative: str
     disclaimer: str
     stance: str
     evidence: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class C4Source(DocSource):
     def __init__(self, name, dlc, checkpoint_dlc, doc_count, checkpoint_freq, size_hint, cache_path):
         self.name = name # e.g., en.noclean.c4-train.01234-of-07168
         self.dlc = dlc
         self.checkpoint_dlc = checkpoint_dlc
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/car.py` & `ir_datasets-0.5.5/ir_datasets/datasets/car.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 
 class CarQuery(NamedTuple):
     query_id: str
     text: str
     title: str
     headings: Tuple[str, ...]
+    def default_text(self):
+        """
+        text (which is title + headings)
+        """
+        return self.text
 
 
 class CarDocs(BaseDocs):
     def __init__(self, streamer, count_hint=None):
         super().__init__()
         self._streamer = streamer
         self._count_hint = count_hint
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/clinicaltrials.py` & `ir_datasets-0.5.5/ir_datasets/datasets/clinicaltrials.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/clirmatrix.py` & `ir_datasets-0.5.5/ir_datasets/datasets/clirmatrix.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/clueweb09.py` & `ir_datasets-0.5.5/ir_datasets/datasets/clueweb09.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 
 class TrecWebTrackQuery(NamedTuple):
     query_id: str
     query: str
     description: str
     type: str
     subtopics: Tuple[TrecSubtopic, ...]
+    def default_text(self):
+        """
+        query
+        """
+        return self.query
 
 
 class ClueWeb09Docs(WarcDocs):
     def __init__(self, docs_dlc, chk_dlc, dirs=None, lang=None):
         super().__init__(warc_cw09=True, lang=lang)
         self.docs_dlc = docs_dlc
         self.chk_dlc = chk_dlc
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/clueweb12.py` & `ir_datasets-0.5.5/ir_datasets/datasets/clueweb12.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,28 +56,43 @@
 
 class TrecWebTrackQuery(NamedTuple):
     query_id: str
     query: str
     description: str
     type: str
     subtopics: Tuple[TrecSubtopic, ...]
+    def default_text(self):
+        """
+        query
+        """
+        return self.query
 
 
 class NtcirQuery(NamedTuple):
     query_id: str
     title: str
     description: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class MisinfoQuery(NamedTuple):
     query_id: str
     title: str
     cochranedoi: str
     description: str
     narrative: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class MisinfoQrel(NamedTuple):
     query_id: str
     doc_id: str
     relevance: int
     effectiveness: int
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/codec.py` & `ir_datasets-0.5.5/ir_datasets/datasets/codec.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,19 @@
         return f'{self.title} {self.text}'
 
 class CodecQuery(NamedTuple):
     query_id: str
     query: str
     domain: str
     guidelines: str
+    def default_text(self):
+        """
+        query
+        """
+        return self.query
 
 
 class CodecQueries(BaseQueries):
     def __init__(self, streamer, qid_filter=None):
         super().__init__()
         self._streamer = streamer
         self._qid_filter = qid_filter
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/codesearchnet.py` & `ir_datasets-0.5.5/ir_datasets/datasets/codesearchnet.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/cord19.py` & `ir_datasets-0.5.5/ir_datasets/datasets/cord19.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,39 @@
 
 class Cord19Doc(NamedTuple):
     doc_id: str
     title: str
     doi: str
     date: str
     abstract: str
+    def default_text(self):
+        """
+        title + abstract
+        """
+        return f'{self.title} {self.abstract}'
 
 
 class Cord19FullTextSection(NamedTuple):
     title: str
     text: str
 
 
 class Cord19FullTextDoc(NamedTuple):
     doc_id: str
     title: str
     doi: str
     date: str
     abstract: str
     body: Tuple[Cord19FullTextSection, ...]
+    def default_text(self):
+        """
+        title + abstract + body
+        """
+        body = ' '.join(f'{b.title} {b.text}' for b in self.body)
+        return f'{self.title} {self.abstract} {body}'
 
 
 
 QRELS_DEFS = {
     2: 'Relevant: the article is fully responsive to the information need as expressed by the topic, i.e. answers the Question in the topic. The article need not contain all information on the topic, but must, on its own, provide an answer to the question.',
     1: 'Partially Relevant: the article answers part of the question but would need to be combined with other information to get a complete answer.',
     0: 'Not Relevant: everything else.',
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/cranfield.py` & `ir_datasets-0.5.5/ir_datasets/datasets/cranfield.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 class CranfieldDoc(NamedTuple):
     doc_id: str
     title: str
     text: str
     author: str
     bib: str
+    def default_text(self):
+        """
+        title + text
+        """
+        return f'{self.title} {self.text}'
 
 
 def prefix_sentinel_splitter(it, sentinel):
     lines = None
     for is_sentinel, group in itertools.groupby(it, lambda l: l.startswith(sentinel)):
         if is_sentinel:
             lines = [list(group)[0].replace(sentinel, '')]
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/disks45.py` & `ir_datasets-0.5.5/ir_datasets/datasets/disks45.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/dpr_w100.py` & `ir_datasets-0.5.5/ir_datasets/datasets/dpr_w100.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,20 +20,30 @@
 }
 
 
 class DprW100Doc(NamedTuple):
     doc_id: str
     text: str
     title: str
+    def default_text(self):
+        """
+        title + text
+        """
+        return f'{self.title} {self.text}'
 
 
 class DprW100Query(NamedTuple):
     query_id: str
     text: str
     answers: Tuple[str, ]
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class DprW100Manager:
     def __init__(self, dlc, base_path, passage_id_key='passage_id'):
         self._dlc = dlc
         self._base_path = base_path
         self._base_path.mkdir(parents=True, exist_ok=True)
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/gov.py` & `ir_datasets-0.5.5/ir_datasets/datasets/gov.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,29 @@
     '<title>': 'text',
 }
 
 class GovWeb02Query(NamedTuple):
     query_id: str
     title: str
     description: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class GovDoc(NamedTuple):
     doc_id: str
     url: str
     http_headers: str
     body: bytes
     body_content_type: str
+    def default_text(self):
+        return ir_datasets.util.sax_html_parser(self.body, headers=self.http_headers, fields=[{'title', 'body'}])[0]
 
 
 class GovDocs(BaseDocs):
     def __init__(self, docs_dlc):
         super().__init__()
         self.docs_dlc = docs_dlc
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/gov2.py` & `ir_datasets-0.5.5/ir_datasets/datasets/gov2.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
 class Gov2Doc(NamedTuple):
     doc_id: str
     url: str
     http_headers: str
     body: bytes
     body_content_type: str
+    def default_text(self):
+        return ir_datasets.util.sax_html_parser(self.body, headers=self.http_headers, fields=[{'title', 'body'}])[0]
 
 
 
 class Gov2DocIter:
     def __init__(self, gov2_docs, slice):
         self.gov2_docs = gov2_docs
         self.slice = slice
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/hc4.py` & `ir_datasets-0.5.5/ir_datasets/datasets/hc4.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/highwire.py` & `ir_datasets-0.5.5/ir_datasets/datasets/highwire.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 
 
 class HighwireDoc(NamedTuple):
     doc_id: str
     journal: str
     title: str
     spans: Tuple[HighwireSpan, ...]
+    def default_text(self):
+        """
+        title + spans
+        """
+        return self.title + ' ' + ' '.join(s.text for s in self.spans)
 
 
 class TrecGenomicsQrel(NamedTuple):
     query_id: str
     doc_id: str
     span_start: int
     span_len: int
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/istella22.py` & `ir_datasets-0.5.5/ir_datasets/datasets/istella22.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     doc_id: str
     title: str
     url: str
     text: str
     extra_text: str
     lang: str
     lang_pct: int
+    def default_text(self):
+        """
+        title + text + extra_text
+        """
+        return f'{self.title} {self.text} {self.extra_text}'
 
 
 NAME = 'istella22'
 QREL_DEFS = {1: 'Least relevant', 2: 'Somewhat relevant', 3: 'Mostly relevant', 4: 'Perfectly relevant'}
 
 DUA = ("To use the Istella22 dataset, you must read and accept the Istella22 Licence Agreement, found here: "
        "<https://istella.ai/data/istella22-dataset/>")
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/kilt.py` & `ir_datasets-0.5.5/ir_datasets/datasets/kilt.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,19 @@
     categories: Tuple[str, ...]
     wikidata_id: str
     history_revid: str
     history_timestamp: str
     history_parentid: str
     history_pageid: str
     history_url: str
+    def default_text(self):
+        """
+        title + text
+        """
+        return f'{self.title} {self.text}'
 
 
 def strip_markup(text):
     if text.startswith('Section::::'):
         return text.replace('Section::::', '').replace(':', ' ')
     if text.startswith('BULLET::::-'):
         return text.replace('BULLET::::-', '-')
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/lotte.py` & `ir_datasets-0.5.5/ir_datasets/datasets/lotte.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/medline.py` & `ir_datasets-0.5.5/ir_datasets/datasets/medline.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,36 +32,56 @@
 NAME = 'medline'
 
 
 class MedlineDoc(NamedTuple):
     doc_id: str
     title: str
     abstract: str
+    def default_text(self):
+        """
+        title + abstract
+        """
+        return f'{self.title} {self.abstract}'
 
 
 class TrecGenomicsQuery(NamedTuple):
     query_id: str
     title: str
     need: str
     context: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class TrecPm2017Query(NamedTuple):
     query_id: str
     disease: str
     gene: str
     demographic: str
     other: str
+    def default_text(self):
+        """
+        disease, gene, demographic, and other
+        """
+        return f'{self.disease} {self.gene} {self.demographic} {self.other}'
 
 
 class TrecPmQuery(NamedTuple):
     query_id: str
     disease: str
     gene: str
     demographic: str
+    def default_text(self):
+        """
+        disease, gene, and demographic
+        """
+        return f'{self.disease} {self.gene} {self.demographic}'
 
 
 class ConcatFile:
     """
     Simulates a sequence of file-like objects that are cat'd.
     Only supports read operations.
     """
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/mmarco.py` & `ir_datasets-0.5.5/ir_datasets/datasets/mmarco.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/mr_tydi.py` & `ir_datasets-0.5.5/ir_datasets/datasets/mr_tydi.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/msmarco_document.py` & `ir_datasets-0.5.5/ir_datasets/datasets/msmarco_document.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 }
 
 class MsMarcoDocument(NamedTuple):
     doc_id: str
     url: str
     title: str
     body: str
+    def default_text(self):
+        """
+        title + body
+        """
+        return f'{self.title} {self.body}'
 
 
 # Use the TREC-formatted docs so we get all the available formatting (namely, line breaks)
 class MsMarcoTrecDocs(TrecDocs):
     def __init__(self, docs_dlc):
         super().__init__(docs_dlc, parser='text', lang='en', docstore_size_hint=14373971970, count_hint=ir_datasets.util.count_hint(NAME))
 
@@ -59,14 +64,19 @@
         return NAME
 
 
 class MsMarcoAnchorTextDocument(NamedTuple):
     doc_id: str
     text: str
     anchors: List[str]
+    def default_text(self):
+        """
+        text + anchors
+        """
+        return f'{self.text} ' + ' '.join(self.anchors)
 
 
 class MsMarcoAnchorTextDocs(BaseDocs):
     def __init__(self, dlc, count_hint):
         super().__init__()
         self._dlc = dlc
         self._count_hint = count_hint
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/msmarco_document_v2.py` & `ir_datasets-0.5.5/ir_datasets/datasets/msmarco_document_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 class MsMarcoV2Document(NamedTuple):
     doc_id: str
     url: str
     title: str
     headings: str
     body: str
+    def default_text(self):
+        """
+        title + headings + body
+        """
+        return f'{self.title} {self.headings} {self.body}'
 
 
 class MsMarcoV2Docs(BaseDocs):
     def __init__(self, dlc):
         super().__init__()
         self._dlc = dlc
 
@@ -97,14 +102,19 @@
 
 
 
 class MsMarcoV2AnchorTextDocument(NamedTuple):
     doc_id: str
     text: str
     anchors: List[str]
+    def default_text(self):
+        """
+        text + anchors
+        """
+        return f'{self.text} ' + ' '.join(self.anchors)
 
 
 class MsMarcoV2AnchorTextDocs(BaseDocs):
     def __init__(self, dlc, count_hint):
         super().__init__()
         self._dlc = dlc
         self._count_hint = count_hint
@@ -196,16 +206,23 @@
         FilteredQueries(subsets['trec-dl-2021'].queries_handler(), dl21_judged),
         FilteredScoredDocs(subsets['trec-dl-2021'].scoreddocs_handler(), dl21_judged),
         subsets['trec-dl-2021'],
     )
     subsets['trec-dl-2022'] = Dataset(
         collection,
         TsvQueries(dlc['trec-dl-2022/queries'], namespace='msmarco', lang='en'),
+        TrecQrels(dlc['trec-dl-2022/qrels'], TREC_DL_QRELS_DEFS),
         TrecScoredDocs(GzipExtract(dlc['trec-dl-2022/scoreddocs'])),
     )
+    dl22_judged = Lazy(lambda: {q.query_id for q in subsets['trec-dl-2022'].qrels_iter()})
+    subsets['trec-dl-2022/judged'] = Dataset(
+        FilteredQueries(subsets['trec-dl-2022'].queries_handler(), dl22_judged),
+        FilteredScoredDocs(subsets['trec-dl-2022'].scoreddocs_handler(), dl22_judged),
+        subsets['trec-dl-2022'],
+    )
 
     subsets['anchor-text'] = Dataset(
         MsMarcoV2AnchorTextDocs(
             Cache(GzipExtract(dlc['anchor-text']), base_path / "anchor-text.json"),
             count_hint=4821244
         ),
         documentation('anchor-text')
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/msmarco_passage.py` & `ir_datasets-0.5.5/ir_datasets/datasets/msmarco_passage.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,14 +270,21 @@
         FilteredQueries(subsets['train'].queries_handler(), split200, mode='include'),
         FilteredScoredDocs(subsets['train'].scoreddocs_handler(), split200, mode='include'),
         FilteredQrels(subsets['train'].qrels_handler(), split200, mode='include'),
         FilteredDocPairs(subsets['train'].docpairs_handler(), split200, mode='include'),
         subsets['train'],
     )
 
+    dev2_qids = Lazy(lambda: {q.query_id for q in ir_datasets.load('msmarco-passage-v2/dev2').queries})
+    subsets['dev/2'] = Dataset(
+        FilteredQueries(subsets['dev'].queries_handler(), dev2_qids),
+        FilteredQrels(subsets['dev'].qrels_handler(), dev2_qids),
+        subsets['dev'],
+    )
+
     # Medical subset
     def train_med():
         with dlc['medmarco_ids'].stream() as stream:
             stream = codecs.getreader('utf8')(stream)
             return {l.rstrip() for l in stream}
     train_med = Lazy(train_med)
     subsets['train/medical'] = Dataset(
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/msmarco_passage_v2.py` & `ir_datasets-0.5.5/ir_datasets/datasets/msmarco_passage_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 
 class MsMarcoV2Passage(NamedTuple):
     doc_id: str
     text: str
     spans: Tuple[Tuple[int, int], ...]
     msmarco_document_id: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 def parse_msmarco_passage(line):
     data = json.loads(line)
     # extract spans in the format of "(123,456),(789,101123)"
     spans = tuple((int(a), int(b)) for a, b in re.findall(r'\((\d+),(\d+)\)', data['spans']))
     return MsMarcoV2Passage(
@@ -271,16 +276,23 @@
         FilteredQueries(subsets['trec-dl-2021'].queries_handler(), dl21_judged),
         FilteredScoredDocs(subsets['trec-dl-2021'].scoreddocs_handler(), dl21_judged),
         subsets['trec-dl-2021'],
     )
     subsets['trec-dl-2022'] = Dataset(
         collection,
         TsvQueries(dlc['trec-dl-2022/queries'], namespace='msmarco', lang='en'),
+        TrecQrels(dlc['trec-dl-2022/qrels'], TREC_DL_QRELS_DEFS),
         TrecScoredDocs(GzipExtract(dlc['trec-dl-2022/scoreddocs'])),
     )
+    dl22_judged = Lazy(lambda: {q.query_id for q in subsets['trec-dl-2022'].qrels_iter()})
+    subsets['trec-dl-2022/judged'] = Dataset(
+        FilteredQueries(subsets['trec-dl-2022'].queries_handler(), dl22_judged),
+        FilteredScoredDocs(subsets['trec-dl-2022'].scoreddocs_handler(), dl22_judged),
+        subsets['trec-dl-2022'],
+    )
 
     ir_datasets.registry.register(NAME, Dataset(collection, documentation("_")))
     for s in sorted(subsets):
         ir_datasets.registry.register(f'{NAME}/{s}', Dataset(subsets[s], documentation(s)))
 
     return collection, subsets
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/msmarco_qna.py` & `ir_datasets-0.5.5/ir_datasets/datasets/msmarco_qna.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,28 +26,43 @@
 NO_ANSWER_PLACEHOLDER = 'No Answer Present.'
 
 class MsMarcoQnAQuery(NamedTuple):
     query_id: str
     text: str
     type: str
     answers: Tuple[str, ...]
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class MsMarcoQnAEvalQuery(NamedTuple):
     query_id: str
     text: str
     type: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class MsMarcoQnADoc(NamedTuple):
     doc_id: str
     text: str
     url: str
     msmarco_passage_id: str
     msmarco_document_id: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 # The MS MARCO QnA data files are in a super inconvenient format. They have a script to convert it
 # to JSONL format, but it involves loading the entire collection into memory and doing merging via
 # pandas, which is a non-starter. So we'll incrementally process the dataset using ijson.
 # Format:
 #     {
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/natural_questions.py` & `ir_datasets-0.5.5/ir_datasets/datasets/natural_questions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
     start_byte: int # the following are from the `long_answer_candidates` objects and may be useful for something
     end_byte: int
     start_token: int
     end_token: int
     document_title: str # from document itself
     document_url: str # from document itself
     parent_doc_id: str # doc_id of the largest passage it's under (e.g., a sentence under a paragraph), or None if it's a top-level passage
+    def default_text(self):
+        """
+        document_title and text
+        """
+        return f'{self.document_title} {self.text}'
+
 
 
 class NqQrel(NamedTuple):
     query_id: str
     doc_id: str
     relevance: int # always 1
     short_answers: List[str] # the **string** representations of the answers (this is similar to how DPH evaluates)
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/neuclir.py` & `ir_datasets-0.5.5/ir_datasets/datasets/neuclir.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/neumarco.py` & `ir_datasets-0.5.5/ir_datasets/datasets/neumarco.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/nfcorpus.py` & `ir_datasets-0.5.5/ir_datasets/datasets/nfcorpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,39 @@
 }
 
 class NfCorpusDoc(NamedTuple):
     doc_id: str
     url: str
     title: str
     abstract: str
+    def default_text(self):
+        """
+        title and abstract
+        """
+        return f'{self.title} {self.abstract}'
 
 class NfCorpusQuery(NamedTuple):
     query_id: str
     title: str
     all: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 class NfCorpusVideoQuery(NamedTuple):
     query_id: str
     title: str
     desc: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 class ZipQueries(BaseQueries):
     def __init__(self, queries, idxs, qtype):
         self._queries = queries
         self._idxs = idxs
         self._qtype = qtype
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/nyt.py` & `ir_datasets-0.5.5/ir_datasets/datasets/nyt.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 
 
 class NytDoc(NamedTuple):
     doc_id: str
     headline: str
     body: str
     source_xml: str
+    def default_text(self):
+        """
+        headline and body
+        """
+        return f'{self.headline} {self.body}'
+
 
 
 class NytDocs(BaseDocs):
     def __init__(self, dlc):
         self._dlc = dlc
 
     def docs_path(self, force=True):
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/pmc.py` & `ir_datasets-0.5.5/ir_datasets/datasets/pmc.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,29 +32,44 @@
 
 class PmcDoc(NamedTuple):
     doc_id: str
     journal: str
     title: str
     abstract: str
     body: str
+    def default_text(self):
+        """
+        title, abstract, and body
+        """
+        return f'{self.title} {self.abstract} {self.body}'
 
 
 class TrecCdsQuery(NamedTuple):
     query_id: str
     type: str
     description: str
     summary: str
+    def default_text(self):
+        """
+        description
+        """
+        return self.description
 
 
 class TrecCds2016Query(NamedTuple):
     query_id: str
     type: str
     note: str
     description: str
     summary: str
+    def default_text(self):
+        """
+        description
+        """
+        return self.description
 
 
 class PmcDocs(BaseDocs):
     def __init__(self, dlcs, path, duplicate_dlcs=[], count_hint=None):
         self._dlcs = dlcs
         self._path = path
         self._duplicate_dlcs = duplicate_dlcs
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/touche.py` & `ir_datasets-0.5.5/ir_datasets/datasets/touche.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/touche_image.py` & `ir_datasets-0.5.5/ir_datasets/datasets/touche_image.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/trec_arabic.py` & `ir_datasets-0.5.5/ir_datasets/datasets/trec_arabic.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/trec_cast.py` & `ir_datasets-0.5.5/ir_datasets/datasets/trec_cast.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,34 @@
 class Cast2019Query(NamedTuple):
     query_id: str
     raw_utterance: str
     topic_number: int
     turn_number: int
     topic_title: str
     topic_description: str
+    def default_text(self):
+        """
+        raw_utterance
+        """
+        return self.raw_utterance
 
 
 class Cast2020Query(NamedTuple):
     query_id: str
     raw_utterance: str
     automatic_rewritten_utterance: str
     manual_rewritten_utterance: str
     manual_canonical_result_id: str
     topic_number: int
     turn_number: int
+    def default_text(self):
+        """
+        raw_utterance
+        """
+        return self.raw_utterance
 
 
 class CastDocs(BaseDocs):
     def __init__(self, corpus_name, docs_mapping, count_hint=None):
         super().__init__()
         self._corpus_name = corpus_name
         self._docs_mapping = docs_mapping
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/trec_fair.py` & `ir_datasets-0.5.5/ir_datasets/datasets/trec_fair.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     title: str
     text: str
     marked_up_text: str
     url: str
     quality_score: Optional[float]
     geographic_locations: Optional[List[str]]
     quality_score_disk: Optional[str]
+    def default_text(self):
+        """
+        title and text
+        """
+        return f"{self.title} {self.text}"
 
 
 class FairTrec2022Doc(NamedTuple):
     doc_id: str
     title: str
     text: str
     url: str
@@ -63,26 +68,41 @@
 
 class FairTrecQuery(NamedTuple):
     query_id: str
     text: str
     keywords: List[str]
     scope: str
     homepage: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 class FairTrec2022TrainQuery(NamedTuple):
     query_id: str
     text: str
     url: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class FairTrecEvalQuery(NamedTuple):
     query_id: str
     text: str
     keywords: List[str]
     scope: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class FairTrecDocs(BaseDocs):
     def __init__(self, dlc, mlc):
         super().__init__()
         self._dlc = dlc
         self._mlc = mlc
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/trec_mandarin.py` & `ir_datasets-0.5.5/ir_datasets/datasets/trec_mandarin.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     query_id: str
     title_en: str
     title_zh: str
     description_en: str
     description_zh: str
     narrative_en: str
     narrative_zh: str
+    def default_text(self):
+        """
+        title_zh
+        """
+        return self.title_zh
 
 
 QREL_DEFS = {
     1: 'relevant',
     0: 'not relevant',
 }
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/trec_robust04.py` & `ir_datasets-0.5.5/ir_datasets/datasets/trec_robust04.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/trec_spanish.py` & `ir_datasets-0.5.5/ir_datasets/datasets/trec_spanish.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,45 @@
 
 
 NAME = 'trec-spanish'
 
 class TrecDescOnlyQuery(NamedTuple):
     query_id: str
     description: str
+    def default_text(self):
+        """
+        description
+        """
+        return self.description
 
 class TrecSpanish3Query(NamedTuple):
     query_id: str
     title_es: str
     title_en: str
     description_es: str
     description_en: str
     narrative_es: str
     narrative_en: str
+    def default_text(self):
+        """
+        title_es
+        """
+        return self.title_es
 
 class TrecSpanish4Query(NamedTuple):
     query_id: str
     description_es1: str
     description_en1: str
     description_es2: str
     description_en2: str
+    def default_text(self):
+        """
+        description_es1
+        """
+        return self.description_es1
 
 QREL_DEFS = {
     1: 'relevant',
     0: 'not relevant',
 }
 
 QTYPE_MAP_3 = {
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/tripclick.py` & `ir_datasets-0.5.5/ir_datasets/datasets/tripclick.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,19 @@
     time: datetime
     items: Tuple[LogItem, ...]
 
 class TripClickPartialDoc(NamedTuple):
     doc_id: str
     title: str
     url: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class TripClickQlogs(BaseQlogs):
     def __init__(self, dlc):
         self.dlc = dlc
 
     def qlogs_iter(self):
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/tweets2013_ia.py` & `ir_datasets-0.5.5/ir_datasets/datasets/tweets2013_ia.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,29 +52,44 @@
     user_id: str
     created_at: str
     lang: str
     reply_doc_id: str
     retweet_doc_id: str
     source: bytes
     source_content_type: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class TrecMb13Query(NamedTuple):
     query_id: str
     query: str
     time: str
     tweet_time: str
+    def default_text(self):
+        """
+        query
+        """
+        return self.query
 
 
 class TrecMb14Query(NamedTuple):
     query_id: str
     query: str
     time: str
     tweet_time: str
     description: str
+    def default_text(self):
+        """
+        query
+        """
+        return self.query
 
 
 """
 About the tweets2013-ia collection:
 
 This collection uses tweets distributed by the Internet Archive. These archives are not /exactly/ the same
 that were used for the TREC Microblog 2013--14 shared tasks, but Sequiera and Lin [1] show that it's close enough.
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/vaswani.py` & `ir_datasets-0.5.5/ir_datasets/datasets/vaswani.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/wapo.py` & `ir_datasets-0.5.5/ir_datasets/datasets/wapo.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,19 @@
     title: str
     author: str
     published_date: int
     kicker: str
     body: str
     body_paras_html: Tuple[str, ...]
     body_media: Tuple[WapoDocMedia, ...]
+    def default_text(self):
+        """
+        title and body
+        """
+        return f'{self.title} {self.body}'
 
 
 class TrecBackgroundLinkingQuery(NamedTuple):
     query_id: str
     doc_id: str
     url: str
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/wikiclir.py` & `ir_datasets-0.5.5/ir_datasets/datasets/wikiclir.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,30 @@
 }
 
 
 class WikiClirQuery(NamedTuple):
     query_id: str
     title: str
     first_sent: str
+    def default_text(self):
+        """
+        title
+        """
+        return f"{self.title}"
 
 
 class WikiClirDoc(NamedTuple):
     doc_id: str
     title: str
     text: str
+    def default_text(self):
+        """
+        title and text
+        """
+        return f"{self.title} {self.text}"
 
 
 def _init():
     base_path = ir_datasets.util.home_path()/NAME
     dlc = DownloadConfig.context(NAME, base_path)
     documentation = YamlDocumentation(f'docs/{NAME}.yaml')
```

### Comparing `ir_datasets-0.5.4/ir_datasets/datasets/wikir.py` & `ir_datasets-0.5.5/ir_datasets/datasets/wikir.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/antique.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/antique.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/aol-ia.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/aol-ia.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/aquaint.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/aquaint.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/argsme.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/argsme.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/beir.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/beir.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/bibliography.bib` & `ir_datasets-0.5.5/ir_datasets/docs/bibliography.bib`

 * *Files 1% similar despite different names*

```diff
@@ -450,28 +450,14 @@
 @inproceedings{Hersh2005TrecGenomics,
   title={TREC 2005 Genomics Track Overview},
   author={William Hersh and Aaron Cohen and Jianji Yang and Ravi Teja Bhupatiraju and Phoebe Roberts and Marti Hearst},
   booktitle={TREC},
   year={2007}
 }
 
-@inproceedings{Roberts2017TrecPm,
-  title={Overview of the TREC 2017 Precision Medicine Track},
-  author={Kirk Roberts and Dina Demner-Fushman and Ellen M. Voorhees and William R. Hersh and Steven Bedrick and Alexander J. Lazar and Shubham Pant},
-  booktitle={TREC},
-  year={2017}
-}
-
-@inproceedings{Roberts2018TrecPm,
-  title={Overview of the TREC 2018 Precision Medicine Track},
-  author={Kirk Roberts and Dina Demner-Fushman and Ellen M. Voorhees and William R. Hersh and Steven Bedrick and Alexander J. Lazar},
-  booktitle={TREC},
-  year={2018}
-}
-
 @article{Craswell2020Orcas,
   title={ORCAS: 18 Million Clicked Query-Document Pairs for Analyzing Search},
   author={Craswell, Nick and Campos, Daniel and Mitra, Bhaskar and Yilmaz, Emine and Billerbeck, Bodo},
   journal={arXiv preprint arXiv:2006.05324},
   year={2020}
 }
 
@@ -966,8 +952,8 @@
   booktitle = {{Advances in Information Retrieval. 44th European Conference on IR Research (ECIR 2022)},
   year = {2022},
   month = apr,
   publisher = {Springer},
   series = {Lecture Notes in Computer Science},
   site = {Stavanger, Norway},
   url = {https://arxiv.org/abs/2201.09992}
-}
+}
```

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/c4.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/c4.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/car.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/car.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/clinicaltrials.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/clinicaltrials.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/clirmatrix.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/clirmatrix.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/clueweb09.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/clueweb09.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/clueweb12.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/clueweb12.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/codec.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/codec.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/codesearchnet.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/codesearchnet.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/cord19.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/cord19.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/disks45.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/disks45.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/dpr-w100.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/dpr-w100.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/gov.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/gov.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/gov2.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/gov2.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/hc4.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/hc4.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/highwire.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/highwire.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/istella22.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/istella22.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/kilt.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/kilt.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/lotte.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/lotte.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/medline.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/medline.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/mmarco.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/mmarco.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/mr-tydi.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/mr-tydi.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/msmarco-document-v2.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/msmarco-document-v2.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,26 @@
   official_measures: ['AP@100', 'nDCG@10', 'P@10', 'RR(rel=2)']
 
 trec-dl-2022:
   desc: '
 <p>
 Official topics for the TREC Deep Learning (DL) 2022 shared task.
 </p>
+<p>
+Note that these qrels are <i>inferred</i> from the passage ranking task; a document''s relevance
+label is the maximum of the labels of its passages.
+</p>
+'
+
+trec-dl-2022/judged:
+  desc: '
+<p>
+<a class="ds-ref">msmarco-document-v2/trec-dl-2022</a>, but filtered down to only the queries
+with qrels.
+</p>
 '
 
 anchor-text:
   pretty_name: "Anchor Text for version 2 of MS Marco"
   desc: '
 <p>
 For version 2 of MS MARCO, the anchor text collection enriches 4,821,244 documents with anchor text extracted from six Common Crawl snapshots. To keep the collection size reasonable, we sampled 1,000 anchor texts for documents with more than 1,000 anchor texts (this sampling yields that all anchor text is included for 97% of the documents). The <code>text</code> field contains the anchor texts concatenated and the <code>anchors</code> field contains the anchor texts as list. The raw dataset with additional information (roughly 100GB) is <a href="https://github.com/webis-de/ecir22-anchor-text">available online</a>.
```

#### html2text {}

```diff
@@ -38,14 +38,19 @@
 msmarco-document-v2/trec-dl-2021, but filtered down to the 57 queries with
 qrels.
 Note that at this time, this is only available to those with TREC active
 participant login credentials.
 ' official_measures: ['AP@100', 'nDCG@10', 'P@10', 'RR(rel=2)'] trec-dl-2022:
 desc: '
 Official topics for the TREC Deep Learning (DL) 2022 shared task.
+Note that these qrels are inferred from the passage ranking task; a document''s
+relevance label is the maximum of the labels of its passages.
+' trec-dl-2022/judged: desc: '
+msmarco-document-v2/trec-dl-2022, but filtered down to only the queries with
+qrels.
 ' anchor-text: pretty_name: "Anchor Text for version 2 of MS Marco" desc: '
 For version 2 of MS MARCO, the anchor text collection enriches 4,821,244
 documents with anchor text extracted from six Common Crawl snapshots. To keep
 the collection size reasonable, we sampled 1,000 anchor texts for documents
 with more than 1,000 anchor texts (this sampling yields that all anchor text is
 included for 97% of the documents). The text field contains the anchor texts
 concatenated and the anchors field contains the anchor texts as list. The raw
```

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/msmarco-document.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/msmarco-document.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/msmarco-passage-v2.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/msmarco-passage-v2.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -79,8 +79,22 @@
   official_measures: ['AP@100', 'nDCG@10', 'P(rel=2)@10', 'RR(rel=2)']
 
 trec-dl-2022:
   desc: '
 <p>
 Official topics for the TREC Deep Learning (DL) 2022 shared task.
 </p>
+<p>
+Note that the officially-released qrels <i>include</i> relevance labels propagated to
+duplicate passages, while results presented in the notebook papers remove duplicate documents.
+This means that the results are not directly comparable, and extra care should be taken when
+making comparisions among systems to ensure that they were evaluated in the same settings.
+</p>
+'
+
+trec-dl-2022/judged:
+  desc: '
+<p>
+<a class="ds-ref">msmarco-passage-v2/trec-dl-2022</a>, but filtered down to only the queries
+with qrels.
+</p>
 '
```

#### html2text {}

```diff
@@ -30,8 +30,16 @@
 ' official_measures: ['AP@100', 'nDCG@10', 'P(rel=2)@10', 'RR(rel=2)'] trec-dl-
 2021/judged: desc: '
 msmarco-passage-v2/trec-dl-2021, but filtered down to the 53 queries with
 qrels.
 ' official_measures: ['AP@100', 'nDCG@10', 'P(rel=2)@10', 'RR(rel=2)'] trec-dl-
 2022: desc: '
 Official topics for the TREC Deep Learning (DL) 2022 shared task.
+Note that the officially-released qrels include relevance labels propagated to
+duplicate passages, while results presented in the notebook papers remove
+duplicate documents. This means that the results are not directly comparable,
+and extra care should be taken when making comparisions among systems to ensure
+that they were evaluated in the same settings.
+' trec-dl-2022/judged: desc: '
+msmarco-passage-v2/trec-dl-2022, but filtered down to only the queries with
+qrels.
 '
```

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/msmarco-passage.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/msmarco-passage.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 dev:
   desc: '
 <p>
 Official dev set.
 </p>
 <p>
 scoreddocs are the top 1000 results from BM25. These are used for the "re-ranking" setting. Note
-that these are sub-sampled to about 1/8 of the total avaialable dev queries by the MSMARCO authors
+that these are sub-sampled to about 1/8 of the total available dev queries by the MSMARCO authors
 for faster evaluation. The BM25 scores from scoreddocs are not available (all have a score of 0).
 </p>
 '
   bibtex_ids: ['Bajaj2016Msmarco']
   official_measures: ['RR@10']
 
 dev/small:
@@ -51,23 +51,31 @@
 Subset of <a class="ds-ref">msmarco-passage/dev</a> that only includes queries that have at least
 one qrel.
 </p>
 '
   bibtex_ids: ['Bajaj2016Msmarco']
   official_measures: ['RR@10']
 
+dev/2:
+  desc: '
+<p>
+"Dev2" split of the <a class="ds-ref">msmarco-passage/dev</a> set. Originally released as part of the v2 corpus.
+</p>
+'
+  bibtex_ids: ['Bajaj2016Msmarco']
+  official_measures: ['RR@10']
 
 eval:
   desc: '
 <p>
 Official eval set for submission to MS MARCO leaderboard. Relevance judgments are hidden.
 </p>
 <p>
 scoreddocs are the top 1000 results from BM25. These are used for the "re-ranking" setting. Note
-that these are sub-sampled to about 1/8 of the total avaialable eval queries by the MSMARCO authors
+that these are sub-sampled to about 1/8 of the total available eval queries by the MSMARCO authors
 for faster evaluation. The BM25 scores from scoreddocs are not available (all have a score of 0).
 </p>
 '
   bibtex_ids: ['Bajaj2016Msmarco']
   official_measures: ['RR@10']
 
 eval/small:
@@ -87,15 +95,15 @@
 </p>
 <p>
 Not all queries have relevance judgments. Use <a class="ds-ref">msmarco-passage/train/judged</a> for
 a filtered list that only includes documents that have at least one qrel.
 </p>
 <p>
 scoreddocs are the top 1000 results from BM25. These are used for the "re-ranking" setting. Note
-that these are sub-sampled to about 1/8 of the total avaialable train queries by the MSMARCO authors
+that these are sub-sampled to about 1/8 of the total available train queries by the MSMARCO authors
 for faster evaluation. The BM25 scores from scoreddocs are not available (all have a score of 0).
 </p>
 <p>
 docpairs provides access to the "official" sequence for pairwise training.
 </p>
 '
   bibtex_ids: ['Bajaj2016Msmarco']
```

#### html2text {}

```diff
@@ -12,42 +12,45 @@
     * Queries: Natural language questions (from query log)
     * Leaderboard
     * Dataset_Paper
 ' bibtex_ids: ['Bajaj2016Msmarco'] dev: desc: '
 Official dev set.
 scoreddocs are the top 1000 results from BM25. These are used for the "re-
 ranking" setting. Note that these are sub-sampled to about 1/8 of the total
-avaialable dev queries by the MSMARCO authors for faster evaluation. The BM25
+available dev queries by the MSMARCO authors for faster evaluation. The BM25
 scores from scoreddocs are not available (all have a score of 0).
 ' bibtex_ids: ['Bajaj2016Msmarco'] official_measures: ['RR@10'] dev/small:
 desc: '
 Official "small" version of the dev set, consisting of 6,980 queries (6.9% of
 the full dev set).
 ' bibtex_ids: ['Bajaj2016Msmarco'] official_measures: ['RR@10'] dev/judged:
 desc: '
 Subset of msmarco-passage/dev that only includes queries that have at least one
 qrel.
+' bibtex_ids: ['Bajaj2016Msmarco'] official_measures: ['RR@10'] dev/2: desc: '
+"Dev2" split of the msmarco-passage/dev set. Originally released as part of the
+v2 corpus.
 ' bibtex_ids: ['Bajaj2016Msmarco'] official_measures: ['RR@10'] eval: desc: '
 Official eval set for submission to MS MARCO leaderboard. Relevance judgments
 are hidden.
 scoreddocs are the top 1000 results from BM25. These are used for the "re-
 ranking" setting. Note that these are sub-sampled to about 1/8 of the total
-avaialable eval queries by the MSMARCO authors for faster evaluation. The BM25
+available eval queries by the MSMARCO authors for faster evaluation. The BM25
 scores from scoreddocs are not available (all have a score of 0).
 ' bibtex_ids: ['Bajaj2016Msmarco'] official_measures: ['RR@10'] eval/small:
 desc: '
 Official "small" version of the eval set, consisting of 6,837 queries (6.8% of
 the full eval set).
 ' bibtex_ids: ['Bajaj2016Msmarco'] official_measures: ['RR@10'] train: desc: '
 Official train set.
 Not all queries have relevance judgments. Use msmarco-passage/train/judged for
 a filtered list that only includes documents that have at least one qrel.
 scoreddocs are the top 1000 results from BM25. These are used for the "re-
 ranking" setting. Note that these are sub-sampled to about 1/8 of the total
-avaialable train queries by the MSMARCO authors for faster evaluation. The BM25
+available train queries by the MSMARCO authors for faster evaluation. The BM25
 scores from scoreddocs are not available (all have a score of 0).
 docpairs provides access to the "official" sequence for pairwise training.
 ' bibtex_ids: ['Bajaj2016Msmarco'] official_measures: ['RR@10'] train/triples-
 v2: desc: '
 Version of msmarco-passage/train, but with version 2 of the triples file.
 This version of the triples file includes rows that were accidently missing
 from version 1 of the file (see discussion here).
```

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/msmarco-qna.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/msmarco-qna.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/natural-questions.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/natural-questions.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/neuclir.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/neuclir.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/neumarco.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/neumarco.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/nfcorpus.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/nfcorpus.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/nyt.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/nyt.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/pmc.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/pmc.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/touche-image.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/touche-image.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/touche.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/touche.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     often come to a point where one side challenges the other with a why-question,
     which is a prompt to justify some stance based on arguments.
     Since technologies for argument mining are maturing at a rapid pace,
     also ad-hoc argument retrieval becomes a feasible task in reach.
     Touché 2022 is the third lab on argument retrieval at CLEF 2022 featuring three tasks.
     </p>
     <p>
-    Given a controversial topic, the task is to retrieve images (from <a class="ds-ref">touche-image-search/2022-06-13</a>) for each stance (pro/con) that show support for that stance.
+    Given a controversial topic, the task is to retrieve images (from <a class="ds-ref">touche-image/2022-06-13</a>) for each stance (pro/con) that show support for that stance.
     </p>
     <p>
     Systems are evaluated on Touché topics 1-50 by the ratio of images among the 20 retrieved images for each topic (10 images for each stance) that are all three: relevant to the topic, argumentative, and have the associated stance.
     </p>
     <ul>
     <li><a href="https://touche.webis.de/clef22/touche22-web/image-retrieval-for-arguments.html">Task 3 website</a></li>
     <li><a href="https://touche.webis.de/clef22/touche22-web/">Lab website</a></li>
```

#### html2text {}

```diff
@@ -145,16 +145,16 @@
 3: Argument Retrieval for Comparative Questions" desc: |
 Decision making processes, be it at the societal or at the personal level,
 often come to a point where one side challenges the other with a why-question,
 which is a prompt to justify some stance based on arguments. Since technologies
 for argument mining are maturing at a rapid pace, also ad-hoc argument
 retrieval becomes a feasible task in reach. TouchÃ© 2022 is the third lab on
 argument retrieval at CLEF 2022 featuring three tasks.
-Given a controversial topic, the task is to retrieve images (from touche-image-
-search/2022-06-13) for each stance (pro/con) that show support for that stance.
+Given a controversial topic, the task is to retrieve images (from touche-image/
+2022-06-13) for each stance (pro/con) that show support for that stance.
 Systems are evaluated on TouchÃ© topics 1-50 by the ratio of images among the
 20 retrieved images for each topic (10 images for each stance) that are all
 three: relevant to the topic, argumentative, and have the associated stance.
     * Task_3_website
     * Lab_website
     * Overview_paper
 bibtex_ids: - Bondarenko2022Touche - Kiesel2021Image - Dimitrov2021SemEval -
```

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/trec-arabic.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/trec-arabic.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/trec-cast.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/trec-cast.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/trec-fair.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/trec-fair.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/trec-mandarin.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/trec-mandarin.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/trec-robust04.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/trec-robust04.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/trec-spanish.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/trec-spanish.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/tripclick.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/tripclick.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/tweets2013-ia.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/tweets2013-ia.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/wapo.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/wapo.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/wikiclir.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/wikiclir.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/docs/wikir.yaml` & `ir_datasets-0.5.5/ir_datasets/docs/wikir.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/etc/downloads.json` & `ir_datasets-0.5.5/ir_datasets/etc/downloads.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9619433421516754%*

 * *Differences: {"'msmarco-document-v2'": "{'trec-dl-2022/qrels': OrderedDict([('url', "*

 * *                          "'https://trec.nist.gov/data/deep/2022.qrels.docs.inferred.txt'), "*

 * *                          "('irds_mirror', True), ('size_hint', 13808681), ('expected_md5', "*

 * *                          "'cca2e4db9d842e6262500532809bd571'), ('cache_path', "*

 * *                          "'trec-dl-2022/qrels.inferred.txt')])}",*

 * * "'msmarco-passage-v2'": "{'trec-dl-2022/qrels': OrderedDict([('url', "*

 * *                         "'http […]*

```diff
@@ -2652,14 +2652,21 @@
         },
         "trec-dl-2021/scoreddocs": {
             "cache_path": "trec-dl-2021/top100.trec.gz",
             "expected_md5": "0bc85e3f2a6f798b91e18f0cd4a6bc6b",
             "size_hint": 618228,
             "url": "https://msmarco.blob.core.windows.net/msmarcoranking/2021_document_top100.txt.gz"
         },
+        "trec-dl-2022/qrels": {
+            "cache_path": "trec-dl-2022/qrels.inferred.txt",
+            "expected_md5": "cca2e4db9d842e6262500532809bd571",
+            "irds_mirror": true,
+            "size_hint": 13808681,
+            "url": "https://trec.nist.gov/data/deep/2022.qrels.docs.inferred.txt"
+        },
         "trec-dl-2022/queries": {
             "cache_path": "trec-dl-2022/queries.tsv",
             "expected_md5": "f1bfd53d80e81e58207ce557fd2211a0",
             "size_hint": 21508,
             "url": "https://msmarco.blob.core.windows.net/msmarcoranking/2022_queries.tsv"
         },
         "trec-dl-2022/scoreddocs": {
@@ -2902,14 +2909,21 @@
         },
         "trec-dl-2021/scoreddocs": {
             "cache_path": "trec-dl-2021/top100.trec.gz",
             "expected_md5": "e2be2d307da26d1a3f76eb95507672a3",
             "size_hint": 604533,
             "url": "https://msmarco.blob.core.windows.net/msmarcoranking/2021_passage_top100.txt.gz"
         },
+        "trec-dl-2022/qrels": {
+            "cache_path": "trec-dl-2022/qrels.withDupes.txt",
+            "expected_md5": "b36484d6cfd039664a570a4bf04f0eeb",
+            "irds_mirror": true,
+            "size_hint": 15800539,
+            "url": "https://trec.nist.gov/data/deep/2022.qrels.pass.withDupes.txt"
+        },
         "trec-dl-2022/queries": {
             "cache_path": "trec-dl-2022/queries.tsv",
             "expected_md5": "f1bfd53d80e81e58207ce557fd2211a0",
             "size_hint": 21508,
             "url": "https://msmarco.blob.core.windows.net/msmarcoranking/2022_queries.tsv"
         },
         "trec-dl-2022/scoreddocs": {
@@ -3476,14 +3490,30 @@
         "v2/source3": {
             "cache_path": "v2/pmc-text-03.tar.gz",
             "expected_md5": "231de843bb5334c3c885d75f2ca3240b",
             "size_hint": 6443033629,
             "url": "https://ceb.nlm.nih.gov/~robertske/pmc-03.tar.gz"
         }
     },
+    "sara": {
+        "docs": {
+            "expected_md5": "f880a35b54bf9fa4d18d1eee8da6f179",
+            "url": "https://bailando.berkeley.edu/enron/enron_with_categories.tar.gz"
+        },
+        "qrels": {
+            "cache_path": "qrels.txt",
+            "expected_md5": "49589ab65d1eaf78dbbadfc5ae56ef72",
+            "url": "https://raw.githubusercontent.com/JackMcKechnie/SARA-A-Collection-of-Sensitivity-Aware-Relevance-Assessments/main/repeated_qrels.txt"
+        },
+        "queries": {
+            "cache_path": "queries.csv",
+            "expected_md5": "fc0247928a0b93bb344068fa238a5e3f",
+            "url": "https://raw.githubusercontent.com/JackMcKechnie/SARA-A-Collection-of-Sensitivity-Aware-Relevance-Assessments/main/repeated_queries.tsv"
+        }
+    },
     "touche": {
         "2020/task-1/qrels": {
             "expected_md5": "6a645e2ebd4f1d6c44da4d9509624598",
             "size_hint": 62058,
             "url": "https://zenodo.org/record/6862281/files/touche2020-task1-relevance-args-me-corpus-version-2020-04-01-corrected.qrels"
         },
         "2020/task-1/qrels-argsme-1.0-uncorrected": {
@@ -3855,14 +3885,21 @@
             "cache_path": "trec4/querie.gz",
             "expected_md5": "dfd9685cce559e33ab397c1878a6a1f8",
             "irds_mirror": true,
             "size_hint": 2091,
             "url": "https://trec.nist.gov/data/topics_noneng/topics.SP26-SP50.spanish.english.gz"
         }
     },
+    "trec-tot": {
+        "main": {
+            "cache_path": "trec-tot.zip",
+            "expected_md5": "f84fe82cb80e3ee1072576c8d6c4a417",
+            "url": "https://surfdrive.surf.nl/files/index.php/s/FaEK4xc6Xp2JcAJ/download"
+        }
+    },
     "tripclick": {
         "benchmark": {
             "cache_path": "benchmark.tar.gz",
             "expected_md5": "6e5d3deeba138750e9a148b538f30a8f",
             "instructions": "To use this dataset, you need to request the source files from the Trip Database here: <https://tripdatabase.github.io/tripclick/#getting-the-data>.\nMore details about the procedure can be found here: <https://ir-datasets.com/tripclick.html#DataAccess>.\nTo proceed, symlink the source file here: {path}"
         },
         "dlfiles": {
```

### Comparing `ir_datasets-0.5.4/ir_datasets/etc/metadata.json` & `ir_datasets-0.5.5/ir_datasets/etc/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9872881355932204%*

 * *Differences: {"'msmarco-document-v2/trec-dl-2022'": "{'qrels': OrderedDict([('count', 369638), ('fields', "*

 * *                                       "OrderedDict([('relevance', "*

 * *                                       "OrderedDict([('counts_by_value', OrderedDict([('0', "*

 * *                                       "274971), ('1', 49016), ('2', 44255), ('3', "*

 * *                                       '1396)]))]))]))])}',*

 * * "'msmarco-document-v2/trec-dl-2022/judged'": "OrderedDict([('docs', OrderedDict([('_ref', "*

 * *                 […]*

```diff
@@ -7337,21 +7337,48 @@
             "count": 5700
         }
     },
     "msmarco-document-v2/trec-dl-2022": {
         "docs": {
             "_ref": "msmarco-document-v2"
         },
+        "qrels": {
+            "count": 369638,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 274971,
+                        "1": 49016,
+                        "2": 44255,
+                        "3": 1396
+                    }
+                }
+            }
+        },
         "queries": {
             "count": 500
         },
         "scoreddocs": {
             "count": 50000
         }
     },
+    "msmarco-document-v2/trec-dl-2022/judged": {
+        "docs": {
+            "_ref": "msmarco-document-v2"
+        },
+        "qrels": {
+            "_ref": "msmarco-document-v2/trec-dl-2022"
+        },
+        "queries": {
+            "count": 76
+        },
+        "scoreddocs": {
+            "count": 7600
+        }
+    },
     "msmarco-document/anchor-text": {
         "docs": {
             "count": 1703834,
             "fields": {
                 "doc_id": {
                     "common_prefix": "D",
                     "max_len": 8
@@ -7758,21 +7785,48 @@
             "count": 5300
         }
     },
     "msmarco-passage-v2/trec-dl-2022": {
         "docs": {
             "_ref": "msmarco-passage-v2"
         },
+        "qrels": {
+            "count": 386416,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 286459,
+                        "1": 52218,
+                        "2": 46080,
+                        "3": 1659
+                    }
+                }
+            }
+        },
         "queries": {
             "count": 500
         },
         "scoreddocs": {
             "count": 50000
         }
     },
+    "msmarco-passage-v2/trec-dl-2022/judged": {
+        "docs": {
+            "_ref": "msmarco-passage-v2"
+        },
+        "qrels": {
+            "_ref": "msmarco-passage-v2/trec-dl-2022"
+        },
+        "queries": {
+            "count": 76
+        },
+        "scoreddocs": {
+            "count": 7600
+        }
+    },
     "msmarco-passage/dev": {
         "docs": {
             "_ref": "msmarco-passage"
         },
         "qrels": {
             "count": 59273,
             "fields": {
@@ -7783,14 +7837,32 @@
                 }
             }
         },
         "queries": {
             "count": 101093
         }
     },
+    "msmarco-passage/dev/2": {
+        "docs": {
+            "_ref": "msmarco-passage"
+        },
+        "qrels": {
+            "count": 4655,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "1": 4655
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 4281
+        }
+    },
     "msmarco-passage/dev/judged": {
         "docs": {
             "_ref": "msmarco-passage"
         },
         "qrels": {
             "_ref": "msmarco-passage/dev"
         },
@@ -9054,14 +9126,40 @@
                 }
             }
         },
         "queries": {
             "count": 30
         }
     },
+    "sara": {
+        "docs": {
+            "count": 1702,
+            "fields": {
+                "doc_id": {
+                    "common_prefix": "",
+                    "max_len": 6
+                }
+            }
+        },
+        "qrels": {
+            "count": 34413,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 32706,
+                        "1": 999,
+                        "2": 708
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 150
+        }
+    },
     "touche-image": {},
     "touche-image/2022-06-13": {
         "docs": {
             "count": 23841,
             "fields": {
                 "doc_id": {
                     "common_prefix": "I",
@@ -9614,14 +9712,74 @@
                 }
             }
         },
         "queries": {
             "count": 25
         }
     },
+    "trec-tot": {},
+    "trec-tot/2023": {
+        "docs": {
+            "count": 231852,
+            "fields": {
+                "doc_id": {
+                    "common_prefix": "",
+                    "max_len": 8
+                }
+            }
+        }
+    },
+    "trec-tot/2023/dev": {
+        "docs": {
+            "count": 231852,
+            "fields": {
+                "doc_id": {
+                    "common_prefix": "",
+                    "max_len": 8
+                }
+            }
+        },
+        "qrels": {
+            "count": 150,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "1": 150
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 150
+        }
+    },
+    "trec-tot/2023/train": {
+        "docs": {
+            "count": 231852,
+            "fields": {
+                "doc_id": {
+                    "common_prefix": "",
+                    "max_len": 8
+                }
+            }
+        },
+        "qrels": {
+            "count": 150,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "1": 150
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 150
+        }
+    },
     "tripclick": {
         "docs": {
             "count": 1523878,
             "fields": {
                 "doc_id": {
                     "common_prefix": "",
                     "max_len": 8
```

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/__init__.py` & `ir_datasets-0.5.5/ir_datasets/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/argsme.py` & `ir_datasets-0.5.5/ir_datasets/formats/argsme.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,20 @@
     date: Optional[datetime]
     author: Optional[str]
     author_image_url: Optional[str]
     author_organization: Optional[str]
     author_role: Optional[str]
     mode: Optional[ArgsMeMode]
 
+    def default_text(self):
+        """
+        premises + conclusion
+        """
+        return f"{self.premises_texts} {self.conclusion}"
+
     @staticmethod
     def from_json(json: dict) -> "ArgsMeDoc":
         context_json = json["context"]
 
         doc_id = str(json["id"])
         conclusion = str(json["conclusion"])
```

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/base.py` & `ir_datasets-0.5.5/ir_datasets/formats/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 import ir_datasets
 
 _logger = ir_datasets.log.easy()
 
 class GenericDoc(NamedTuple):
     doc_id: str
     text: str
+    def default_text(self):
+        return self.text
 
 class GenericQuery(NamedTuple):
     query_id: str
     text: str
+    def default_text(self):
+        return self.text
 
 class GenericQrel(NamedTuple):
     query_id: str
     doc_id: str
     relevance: int
 
 class GenericScoredDoc(NamedTuple):
```

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/clirmatrix.py` & `ir_datasets-0.5.5/ir_datasets/formats/clirmatrix.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/csv_fmt.py` & `ir_datasets-0.5.5/ir_datasets/formats/csv_fmt.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/extracted_cc.py` & `ir_datasets-0.5.5/ir_datasets/formats/extracted_cc.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 class ExctractedCCDoc(NamedTuple):
     doc_id: str
     title: str
     text: str
     url: str
     time: str
     cc_file: str
+    def default_text(self):
+        """
+        title and text
+        """
+        return f'{self.title} {self.text}'
 
 
 class ExctractedCCDocs(BaseDocs):
     
     def __init__(self, docs_dlc, subset_lang, namespace=None, count=None):
         self._docs_dlc = docs_dlc
         self._subset_lang = subset_lang
@@ -79,14 +84,19 @@
     mt_title: str
     mt_description: str
     narrative_by_relevance: Dict[str, str]
     report: str
     report_url: str
     report_date: str
     translation_lang: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 class ExctractedCCQueries(BaseQueries):
     def __init__(self, queries_dlc, subset_lang, namespace=None):
         self._queries_dlc = queries_dlc if isinstance(queries_dlc, list) else [queries_dlc]
         self._subset_lang = subset_lang
         self._namespace = namespace
```

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/jsonl.py` & `ir_datasets-0.5.5/ir_datasets/formats/jsonl.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/ntcir.py` & `ir_datasets-0.5.5/ir_datasets/formats/ntcir.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/touche.py` & `ir_datasets-0.5.5/ir_datasets/formats/touche.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,42 @@
 
 
 class ToucheQuery(NamedTuple):
     query_id: str
     title: str
     description: str
     narrative: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class ToucheTitleQuery(NamedTuple):
     query_id: str
     title: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class ToucheComparativeQuery(NamedTuple):
     query_id: str
     title: str
     objects: Tuple[str, str]
     description: str
     narrative: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 
 class ToucheQualityQrel(NamedTuple):
     query_id: str
     doc_id: str
     relevance: int
     quality: int
@@ -75,14 +90,19 @@
     stance: ToucheControversialStance
 
 
 class TouchePassageDoc(NamedTuple):
     doc_id: str
     text: str
     chatnoir_url: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 
 class ToucheQueries(BaseQueries):
     _source: Any
     _namespace: Optional[str]
     _language: Optional[str]
```

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/touche_image.py` & `ir_datasets-0.5.5/ir_datasets/formats/touche_image.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/trec.py` & `ir_datasets-0.5.5/ir_datasets/formats/trec.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,32 +13,52 @@
 from .base import GenericDoc, GenericQuery, GenericScoredDoc, BaseDocs, BaseQueries, BaseScoredDocs, BaseQrels
 
 
 class TrecDoc(NamedTuple):
     doc_id: str
     text: str
     marked_up_doc: str
+    def default_text(self):
+        """
+        text
+        """
+        return self.text
 
 class TitleUrlTextDoc(NamedTuple):
     doc_id: str
     title: str
     url: str
     text: str
+    def default_text(self):
+        """
+        title and text
+        """
+        return f'{self.title} {self.text}'
 
 class TrecParsedDoc(NamedTuple):
     doc_id: str
     title: str
     body: str
     marked_up_doc: bytes
+    def default_text(self):
+        """
+        title and body
+        """
+        return f'{self.title} {self.body}'
 
 class TrecQuery(NamedTuple):
     query_id: str
     title: str
     description: str
     narrative: str
+    def default_text(self):
+        """
+        title
+        """
+        return self.title
 
 class TrecSubtopic(NamedTuple):
     number: str
     text: str
     type: str
 
 class TrecQrel(NamedTuple):
```

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/tsv.py` & `ir_datasets-0.5.5/ir_datasets/formats/tsv.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/formats/webarc.py` & `ir_datasets-0.5.5/ir_datasets/formats/webarc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import gzip
 import re
 from contextlib import contextmanager, ExitStack
 from typing import NamedTuple
 import ir_datasets
 from ir_datasets.formats import BaseDocs
 
+_logger = ir_datasets.log.easy()
 
 class WarcDoc(NamedTuple):
     doc_id: str
     url: str
     date: str
     http_headers: bytes
     body: bytes
     body_content_type: str
+    def default_text(self):
+        try:
+            return ir_datasets.util.sax_html_parser(self.body, headers=self.http_headers, fields=[{'title', 'body'}])[0]
+        except UnicodeDecodeError:
+            _logger.info(f'UnicodeDecodeError when parsing doc_id={self.doc_id}')
+            return ''
 
 
 class WarcDocs(BaseDocs):
     def __init__(self, id_header='WARC-TREC-ID', warc_cw09=False, lang=None):
         super().__init__()
         self.id_header = id_header
         self.warc_cw09 = warc_cw09
```

### Comparing `ir_datasets-0.5.4/ir_datasets/indices/base.py` & `ir_datasets-0.5.5/ir_datasets/indices/base.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/indices/cache_docstore.py` & `ir_datasets-0.5.5/ir_datasets/indices/cache_docstore.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/indices/clueweb_warc.py` & `ir_datasets-0.5.5/ir_datasets/indices/clueweb_warc.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/indices/indexed_tsv_docstore.py` & `ir_datasets-0.5.5/ir_datasets/indices/indexed_tsv_docstore.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/indices/lz4_pickle.py` & `ir_datasets-0.5.5/ir_datasets/indices/lz4_pickle.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/indices/numpy_sorted_index.py` & `ir_datasets-0.5.5/ir_datasets/indices/numpy_sorted_index.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/indices/zpickle_docstore.py` & `ir_datasets-0.5.5/ir_datasets/indices/zpickle_docstore.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/lazy_libs.py` & `ir_datasets-0.5.5/ir_datasets/lazy_libs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,21 @@
 def bs4():
     if 'bs4' not in _cache:
         import bs4
         _cache['bs4'] = bs4
     return _cache['bs4']
 
 
+def inscriptis():
+    if 'inscriptis' not in _cache:
+        import inscriptis
+        _cache['inscriptis'] = inscriptis
+    return _cache['inscriptis']
+
+
 def yaml():
     if 'yaml' not in _cache:
         import yaml
         _cache['yaml'] = yaml
     return _cache['yaml']
```

### Comparing `ir_datasets-0.5.4/ir_datasets/log.py` & `ir_datasets-0.5.5/ir_datasets/log.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/util/__init__.py` & `ir_datasets-0.5.5/ir_datasets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/util/download.py` & `ir_datasets-0.5.5/ir_datasets/util/download.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/util/fileio.py` & `ir_datasets-0.5.5/ir_datasets/util/fileio.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/util/hash.py` & `ir_datasets-0.5.5/ir_datasets/util/hash.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/util/html_parsing.py` & `ir_datasets-0.5.5/ir_datasets/util/html_parsing.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/util/metadata.py` & `ir_datasets-0.5.5/ir_datasets/util/metadata.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/util/registry.py` & `ir_datasets-0.5.5/ir_datasets/util/registry.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.4/ir_datasets/wrappers/html_extractor.py` & `ir_datasets-0.5.5/ir_datasets/wrappers/html_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     soup = bs4.BeautifulSoup(html, 'html.parser')
     output = ''
     for t in soup.find_all(text=True):
         if t.parent.name not in ignore and not isinstance(t, bs4.element.Comment):
             output += '{} '.format(t)
     return output
 
+def inscriptis_extract(html):
+    get_text = ir_datasets.lazy_libs.inscriptis().get_text
+    return get_text(html.decode("utf-8",'ignore'))
+
 
 class HtmlDocIter:
     def __init__(self, it, extractor):
         self.it = it
         self.extractor = extractor
         self.mapped_it = _doc_map_it(it, self.extractor)
 
@@ -69,14 +73,15 @@
 
     def docs_store(self):
         return HtmlDocExtractorDocStoreWrapper(self._dataset.docs_store(), self)
 
 
 class HtmlDocExtractorDocStoreWrapper(ir_datasets.indices.Docstore):
     def __init__(self, docstore, extractor):
+        super().__init__(docstore._doc_cls, docstore._id_field)
         self.docstore = docstore
         self.extractor = extractor
 
     def get_many_iter(self, doc_ids):
         return _doc_map_it(self.docstore.get_many_iter(doc_ids), self.extractor)
 
     def clear_cache(self):
@@ -114,15 +119,16 @@
 
     return it_out()
 
 
 def _doc_map(args):
     doc, field_content_type, extractor, docs_cls = args
     extractor = {
-        'bs4': bs4_extract
+        'bs4': bs4_extract,
+        'inscriptis': inscriptis_extract,
     }[extractor]
     result = list(doc)
     any_updates = False
     for content_idx, type_idx in field_content_type:
         if result[type_idx] in ('text/html', 'application/xhtml+xml'):
             result[content_idx] = extractor(result[content_idx])
             result[type_idx] = 'text/plain'
```

### Comparing `ir_datasets-0.5.4/ir_datasets.egg-info/PKG-INFO` & `ir_datasets-0.5.5/ir_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ir-datasets
-Version: 0.5.4
+Version: 0.5.5
 Summary: provides a common interface to many IR ad-hoc ranking benchmarks, training datasets, etc.
 Home-page: https://github.com/allenai/ir_datasets
 Author: Sean MacAvaney
 Author-email: sean.macavaney@glasgow.ac.uk
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ir_datasets
 
 `ir_datasets` is a python package that provides a common interface to many IR ad-hoc ranking
 benchmarks, training datasets, etc.
@@ -51,15 +51,15 @@
 ```
 $ git clone https://github.com/allenai/ir_datasets
 $ cd ir_datasets
 $ python setup.py bdist_wheel
 $ pip install dist/ir_datasets-*.whl
 ```
 
-Tested with python versions 3.6 and 3.7
+Tested with python versions 3.7, 3.8, 3.9, and 3.10. (Mininum python version is 3.7.)
 
 ## Features
 
 **Python and Command Line Interfaces**. Access datasts both through a simple Python API and
 via the command line.
 
 ```python
```

### Comparing `ir_datasets-0.5.4/ir_datasets.egg-info/SOURCES.txt` & `ir_datasets-0.5.5/ir_datasets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,24 @@
 ir_datasets/datasets/msmarco_qna.py
 ir_datasets/datasets/natural_questions.py
 ir_datasets/datasets/neuclir.py
 ir_datasets/datasets/neumarco.py
 ir_datasets/datasets/nfcorpus.py
 ir_datasets/datasets/nyt.py
 ir_datasets/datasets/pmc.py
+ir_datasets/datasets/sara.py
 ir_datasets/datasets/touche.py
 ir_datasets/datasets/touche_image.py
 ir_datasets/datasets/trec_arabic.py
 ir_datasets/datasets/trec_cast.py
 ir_datasets/datasets/trec_fair.py
 ir_datasets/datasets/trec_mandarin.py
 ir_datasets/datasets/trec_robust04.py
 ir_datasets/datasets/trec_spanish.py
+ir_datasets/datasets/trec_tot.py
 ir_datasets/datasets/tripclick.py
 ir_datasets/datasets/tweets2013_ia.py
 ir_datasets/datasets/vaswani.py
 ir_datasets/datasets/wapo.py
 ir_datasets/datasets/wikiclir.py
 ir_datasets/datasets/wikir.py
 ir_datasets/docs/antique.yaml
@@ -112,22 +114,24 @@
 ir_datasets/docs/msmarco-qna.yaml
 ir_datasets/docs/natural-questions.yaml
 ir_datasets/docs/neuclir.yaml
 ir_datasets/docs/neumarco.yaml
 ir_datasets/docs/nfcorpus.yaml
 ir_datasets/docs/nyt.yaml
 ir_datasets/docs/pmc.yaml
+ir_datasets/docs/sara.yaml
 ir_datasets/docs/touche-image.yaml
 ir_datasets/docs/touche.yaml
 ir_datasets/docs/trec-arabic.yaml
 ir_datasets/docs/trec-cast.yaml
 ir_datasets/docs/trec-fair.yaml
 ir_datasets/docs/trec-mandarin.yaml
 ir_datasets/docs/trec-robust04.yaml
 ir_datasets/docs/trec-spanish.yaml
+ir_datasets/docs/trec-tot.yaml
 ir_datasets/docs/tripclick.yaml
 ir_datasets/docs/tweets2013-ia.yaml
 ir_datasets/docs/vaswani.yaml
 ir_datasets/docs/wapo.yaml
 ir_datasets/docs/wikiclir.yaml
 ir_datasets/docs/wikir.yaml
 ir_datasets/etc/downloads.json
@@ -157,8 +161,9 @@
 ir_datasets/util/download.py
 ir_datasets/util/fileio.py
 ir_datasets/util/hash.py
 ir_datasets/util/html_parsing.py
 ir_datasets/util/metadata.py
 ir_datasets/util/registry.py
 ir_datasets/wrappers/__init__.py
-ir_datasets/wrappers/html_extractor.py
+ir_datasets/wrappers/html_extractor.py
+test/test_defaulttext.py
```

### Comparing `ir_datasets-0.5.4/setup.py` & `ir_datasets-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ir_datasets",
-    version="0.5.4", # NOTE: keep this in sync with ir_datasets/__init__.py
+    version="0.5.5", # NOTE: keep this in sync with ir_datasets/__init__.py
     author="Sean MacAvaney",
     author_email="sean.macavaney@glasgow.ac.uk",
     description="provides a common interface to many IR ad-hoc ranking benchmarks, training datasets, etc.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allenai/ir_datasets",
     include_package_data = True,
     packages=setuptools.find_packages(include=['ir_datasets', 'ir_datasets.*']),
     install_requires=list(open('requirements.txt')),
     classifiers=[],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     entry_points={
         'console_scripts': ['ir_datasets=ir_datasets:main_cli'],
     },
     package_data={
         'ir_datasets': glob('docs/*.yaml') + glob('etc/*.json'),
         '': ['requirements.txt', 'LICENSE'],
     },
```

