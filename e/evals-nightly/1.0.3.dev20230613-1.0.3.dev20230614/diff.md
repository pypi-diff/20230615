# Comparing `tmp/evals-nightly-1.0.3.dev20230613.tar.gz` & `tmp/evals-nightly-1.0.3.dev20230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-nightly-1.0.3.dev20230613.tar", last modified: Tue Jun 13 20:51:57 2023, max compression
+gzip compressed data, was "evals-nightly-1.0.3.dev20230614.tar", last modified: Thu Jun 15 04:00:05 2023, max compression
```

## Comparing `evals-nightly-1.0.3.dev20230613.tar` & `evals-nightly-1.0.3.dev20230614.tar`

### file list

```diff
@@ -1,400 +1,417 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/LICENSE
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5697 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2965 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/api.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/cli/
--rw-r--r--   0 root         (0) root         (0)     6454 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/cli/oaieval.py
--rw-r--r--   0 root         (0) root         (0)     3863 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/cli/oaievalset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/completion_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/cot.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_llm.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_math.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/openai.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/completion_fns/retrieval.py
--rw-r--r--   0 root         (0) root         (0)     6080 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/
--rw-r--r--   0 root         (0) root         (0)     1986 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/fuzzy_match_test.py
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/includes.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/includes_test.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/json_validator.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/json_validator_test.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/match.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/match_test.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/lambada.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/base.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify_utils.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/multiple_choice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/elsuite/test/
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/test/match.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/translate.py
--rw-r--r--   0 root         (0) root         (0)     6413 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/utils.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/elsuite/utils_test.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/eval.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/formatting.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.053988 evals-nightly-1.0.3.dev20230613/evals/prompt/
--rw-r--r--   0 root         (0) root         (0)     4093 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/prompt/base.py
--rw-r--r--   0 root         (0) root         (0)    18168 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.049988 evals-nightly-1.0.3.dev20230613/evals/registry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.057988 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/cot.yaml
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/langchain_chains.yaml
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/langchain_llms.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.057988 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/logiqa-logical-reasoning-plus.yaml
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/pointer-value-retrieval.yaml
--rw-r--r--   0 root         (0) root         (0)     1652 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/raven-matrices.yaml
--rw-r--r--   0 root         (0) root         (0)      560 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      454 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/test-modelgraded.yaml
--rw-r--r--   0 root         (0) root         (0)      613 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/ukraine-gec.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.093990 evals-nightly-1.0.3.dev20230613/evals/registry/evals/
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/2d_movement.yaml
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/3d_globe_movement.yaml
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/aba-mrpc-true-false.yaml
--rw-r--r--   0 root         (0) root         (0)      863 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/abstract-causal-reasoning.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/actors-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/adultery_state_laws.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/afrikaans-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/aime_evaluation.yaml
--rw-r--r--   0 root         (0) root         (0)      457 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/algebra-word-problems.yaml
--rw-r--r--   0 root         (0) root         (0)      418 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/allergen-information.yaml
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/alternate-numeral-systems.yaml
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ambiguous-sentences.yaml
--rw-r--r--   0 root         (0) root         (0)      229 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/anagrams.yaml
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/arc.yaml
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/arithmetical_puzzles.yaml
--rw-r--r--   0 root         (0) root         (0)      280 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ascii-wordart.yaml
--rw-r--r--   0 root         (0) root         (0)      281 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/asl-classifiers.yaml
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/atpl_exams.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/balance-chemical-equation.yaml
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/banking77.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/beam-analysis.yaml
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-grammar.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-proverbs.yaml
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-russian-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-syllable-count.yaml
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/belarusian-synonyms.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/bigrams.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/bitwise.yaml
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/body-movement.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/born-first.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/brazilian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/brazilian_laws.yaml
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/building_floorplan.yaml
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/bulgarian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/canto_wu_pronunciation.yaml
--rw-r--r--   0 root         (0) root         (0)      355 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/canto_wu_pronunciation_fewshot.yaml
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cardinal-directions.yaml
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/categorize_with_distractors.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chess-piece-count.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chess.yaml
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_homonym.yaml
--rw-r--r--   0 root         (0) root         (0)      178 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_poem.yaml
--rw-r--r--   0 root         (0) root         (0)      190 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_song_ci.yaml
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_tang_poetries.yaml
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/chinese_zodiac.yaml
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cissp-study-questions.yaml
--rw-r--r--   0 root         (0) root         (0)      372 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/code_combination.yaml
--rw-r--r--   0 root         (0) root         (0)      343 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/color_theory_complementary.yaml
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/compare-countries-area.yaml
--rw-r--r--   0 root         (0) root         (0)      223 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/complex-analogies-en-ru.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/complex-replace-characters.yaml
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/comprehensive-graph-reasoning.yaml
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/connect-4.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/context-free-grammar.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/convert-hex-hsl-lightness.yaml
--rw-r--r--   0 root         (0) root         (0)     1719 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/count_intersections_polynomial.yaml
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/count_token_freq_dna.yaml
--rw-r--r--   0 root         (0) root         (0)      387 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/counterfactual-reasoning.yaml
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/countries.yaml
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/crepe.yaml
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cricket_situations.yaml
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/crontab.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cube-pack.yaml
--rw-r--r--   0 root         (0) root         (0)      553 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/cybersecurity-filepaths.yaml
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/date-booking.yaml
--rw-r--r--   0 root         (0) root         (0)      192 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/date-calculator.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/day-of-week-from-date.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/decrypt-caesar-cipher.yaml
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/detect-hshd.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/determinant.yaml
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/diabetes.yaml
--rw-r--r--   0 root         (0) root         (0)      202 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/diagrammatic_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      377 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/dice-rotation-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      199 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/direct-speech-tag.yaml
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/directions.yaml
--rw-r--r--   0 root         (0) root         (0)      316 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/dna-melting-calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/dutch-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/emoji-riddle.yaml
--rw-r--r--   0 root         (0) root         (0)      387 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/emotional-intelligence.yaml
--rw-r--r--   0 root         (0) root         (0)      195 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/escher-sentences.yaml
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/euler_problems.yaml
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/european-date-format-challenge.yaml
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/event-categories.yaml
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/fcc_amateur_extra.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/finance.yaml
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/financial-derivatives.yaml
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/find-letter.yaml
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/find-thirukkural.yaml
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/find_country_from_svg.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/finnish-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/first-letters.yaml
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/food.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/formal-grammar-to-regex.yaml
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/formal_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      928 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/forth-stack-sim.yaml
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/french-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/french-part-of-speech.yaml
--rw-r--r--   0 root         (0) root         (0)      289 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/game-theory.yaml
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/geometry_puzzle.yaml
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/german-part-of-speech.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/gol.yaml
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/gpt-protocol-buffers.yaml
--rw-r--r--   0 root         (0) root         (0)      404 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/greek-nt-manuscripts.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/greek-vocabulary.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/guess-the-singer.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/heart-disease.yaml
--rw-r--r--   0 root         (0) root         (0)      315 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hebrew-bible.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hebrew-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hebrew-same-noun-gender.yaml
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hindi_shuddha.yaml
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hindi_upsc.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/hindi_words.yaml
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/historical-kana-orthography-reading.yaml
--rw-r--r--   0 root         (0) root         (0)      313 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/human-safety.yaml
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/iambic-pentameter.yaml
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/illinois-law.yaml
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/imperial_date_to_string.yaml
--rw-r--r--   0 root         (0) root         (0)      213 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/indonesian_numbers.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/infiniteloop-match.yaml
--rw-r--r--   0 root         (0) root         (0)     1113 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/integer-sequence-predictions.yaml
--rw-r--r--   0 root         (0) root         (0)      235 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/internal_representations.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/invert_word_wise.yaml
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/invoice_due_date_leap_day_adjustment.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/invoices.yaml
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/irish-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/irony.yaml
--rw-r--r--   0 root         (0) root         (0)      370 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/islands.yaml
--rw-r--r--   0 root         (0) root         (0)      233 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/isosceles-right-triangle.yaml
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/italian-new-words.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/italian-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese-itpassport-exam01.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese-national-medical-exam01.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese-national-medical-exam02.yaml
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_city_name_pronuciation.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_driving_license.yaml
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_number_reading.yaml
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/japanese_populer_video_game_title_and_the_publisher.yaml
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/jee-math.yaml
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/json_patch_object.yaml
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/kanji-idioms.yaml
--rw-r--r--   0 root         (0) root         (0)      754 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/knot-theory.yaml
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean-consonant-vowel-combination.yaml
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean-phonetics.yaml
--rw-r--r--   0 root         (0) root         (0)      293 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean_dialects.yaml
--rw-r--r--   0 root         (0) root         (0)      191 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean_spelling.yaml
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/korean_yaminjeongeum.yaml
--rw-r--r--   0 root         (0) root         (0)      400 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/language.yaml
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/largest_country.yaml
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/last-word-nth.yaml
--rw-r--r--   0 root         (0) root         (0)      198 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/lat_long_identify.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/linear-equations.yaml
--rw-r--r--   0 root         (0) root         (0)      802 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/linear-regression.yaml
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/list_comparison_missing_name.yaml
--rw-r--r--   0 root         (0) root         (0)      814 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-grid-eval.yaml
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-liar-paradox.yaml
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-riddles.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-statements.yaml
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic.yaml
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic_and_probability.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logical_counting.yaml
--rw-r--r--   0 root         (0) root         (0)     1041 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logiqa-logical-reasoning-plus.yaml
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/logiqa.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/loss-logic.yaml
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/lunar-calendar.yaml
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mandaliof-table.yaml
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/map-electronic-component-part-to-fact.yaml
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mapping_to_matricies.yaml
--rw-r--r--   0 root         (0) root         (0)      243 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mate-in-one.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/matrix-mult-rows.yaml
--rw-r--r--   0 root         (0) root         (0)      318 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/medication_dose.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/medmcqa.yaml
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mendelian_inheritance.yaml
--rw-r--r--   0 root         (0) root         (0)      337 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/missing-operators.yaml
--rw-r--r--   0 root         (0) root         (0)    14586 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/mmlu.yaml
--rw-r--r--   0 root         (0) root         (0)      313 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/monthly_metric_comparison.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/moral_exceptQA.yaml
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/multi-step-equations.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/multistep-word-problems.yaml
--rw-r--r--   0 root         (0) root         (0)      315 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music-theory-chord-names.yaml
--rw-r--r--   0 root         (0) root         (0)      315 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music-theory-chord-notes.yaml
--rw-r--r--   0 root         (0) root         (0)      874 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music-theory.yaml
--rw-r--r--   0 root         (0) root         (0)      346 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/music_theory_scale_modes.yaml
--rw-r--r--   0 root         (0) root         (0)     1193 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/naughty_strings.yaml
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/nepali-song-singer.yaml
--rw-r--r--   0 root         (0) root         (0)      340 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/newsology.yaml
--rw-r--r--   0 root         (0) root         (0)      290 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/next-val-series.yaml
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/nfl-point-combinations.yaml
--rw-r--r--   0 root         (0) root         (0)     3875 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/non-compound-names.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/norwegian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/number-pattern.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/number-reading.yaml
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/numbers_game.yaml
--rw-r--r--   0 root         (0) root         (0)      368 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/numeral-type-comparisons.yaml
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/nutrition.yaml
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ordered-history-events.yaml
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/override-system-instruction.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pantone_to_hex.yaml
--rw-r--r--   0 root         (0) root         (0)      502 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/parable-to-moral-match.yaml
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pararule-plus-multi-step-deductive-reasoning.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/partially_solved_crossword_clues.yaml
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/passing-balls.yaml
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pattern_identification.yaml
--rw-r--r--   0 root         (0) root         (0)      287 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ph_calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      429 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/phonetics-identify-words-needing-missing-gpcs.yaml
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/physics-interaction.yaml
--rw-r--r--   0 root         (0) root         (0)     2427 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pointer-value-retrieval.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/points-on-line.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/poker_analysis.yaml
--rw-r--r--   0 root         (0) root         (0)      188 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/poker_hand_ranks.yaml
--rw-r--r--   0 root         (0) root         (0)      290 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/polish-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/polish-syllable-count.yaml
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/polish_rhymes_generation.yaml
--rw-r--r--   0 root         (0) root         (0)      579 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/population_span_extraction.yaml
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/portuguese-sarcasm.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/portuguese-syllable-count.yaml
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/positive-binary-operations.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/probability_questions.yaml
--rw-r--r--   0 root         (0) root         (0)     1847 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/product-matching.yaml
--rw-r--r--   0 root         (0) root         (0)      281 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/prompt-injection.yaml
--rw-r--r--   0 root         (0) root         (0)      235 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/pure_korean.yaml
--rw-r--r--   0 root         (0) root         (0)      334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/python_list_comprehension.yaml
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/qa.yaml
--rw-r--r--   0 root         (0) root         (0)      219 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/quartz.yaml
--rw-r--r--   0 root         (0) root         (0)      380 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rare-and-loanwords-dutch-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)    14285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/raven-matrices.yaml
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rectangles.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/regex-match.yaml
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/resistor-ohm-calculator.yaml
--rw-r--r--   0 root         (0) root         (0)      362 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/resource_id_extraction.yaml
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/reverse-polish-notation.yaml
--rw-r--r--   0 root         (0) root         (0)      370 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/reverse-sort-words-eng.yaml
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/reverse-string.yaml
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rhetorical-devices.yaml
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rock-climbing.yaml
--rw-r--r--   0 root         (0) root         (0)      255 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rot13.yaml
--rw-r--r--   0 root         (0) root         (0)      468 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ru_rhymes.yaml
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rubiks-colors.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/rucola.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russe.yaml
--rw-r--r--   0 root         (0) root         (0)      298 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-english-homonym-context-resolution.yaml
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      199 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-nlp-tasks.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian-verse.yaml
--rw-r--r--   0 root         (0) root         (0)      190 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian_medical.yaml
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/russian_sarcasm.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sarcasm.yaml
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/seating_arrangements.yaml
--rw-r--r--   0 root         (0) root         (0)      334 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/security_guide.yaml
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sexagenary-cycle-calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/shape-in-shape.yaml
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/shared-borders.yaml
--rw-r--r--   0 root         (0) root         (0)      328 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/shopping_discount_comparison.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple-knowledge-mongolian.yaml
--rw-r--r--   0 root         (0) root         (0)      377 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple-visual-understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      253 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple_math.yaml
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/simple_physics_engine.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sindarin-fluency.yaml
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/soc_codes.yaml
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/solve-for-variable.yaml
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sort-numeric.yaml
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/south-african-bands.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/spanish-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/spanish_feminine_noun_masculine_article.yaml
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/split_chinese_characters.yaml
--rw-r--r--   0 root         (0) root         (0)     1048 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/sql.yaml
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/squares-gpt.yaml
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/stats-tests.yaml
--rw-r--r--   0 root         (0) root         (0)     4472 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/superficial-patterns.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/svg_understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/swap-words.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/swedish-spelling.yaml
--rw-r--r--   0 root         (0) root         (0)      376 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/swedish_sat.yaml
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/syllables_long_words.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/syntax-check.yaml
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/taxes.yaml
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/tempo_to_measure_count.yaml
--rw-r--r--   0 root         (0) root         (0)     1169 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      400 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-comp-sci.yaml
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded-generated.yaml
--rw-r--r--   0 root         (0) root         (0)     3040 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded.yaml
--rw-r--r--   0 root         (0) root         (0)      340 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test_japanese_radical.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/test_japanese_units.yaml
--rw-r--r--   0 root         (0) root         (0)      360 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/tetris.yaml
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/three-pt-mapping.yaml
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/time-zone-conversion.yaml
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/track_objects.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/tracking-shuffled-objects.yaml
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/turkish_characters.yaml
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ukraine-eit.yaml
--rw-r--r--   0 root         (0) root         (0)     6692 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ukraine-gec.yaml
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/ukraine_electronic_petitions.yaml
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unified-patch.yaml
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unique_combinations.yaml
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unsolvable_questions.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/unwanted-rhyming.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/us-tort-law.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/utility_price_parsing.yaml
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/vigenere.yaml
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/vintage_phone_keyboard_decode.yaml
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/which-is-heavier.yaml
--rw-r--r--   0 root         (0) root         (0)      392 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/wkt_understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/evals/word_vector_over_reliance.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.093990 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      492 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/best.yaml
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 root         (0) root         (0)     1157 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 root         (0) root         (0)     2564 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/iambic_pentameter.yaml
--rw-r--r--   0 root         (0) root         (0)      887 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/regression-equation.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/rhyming.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/security.yaml
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/sql.yaml
--rw-r--r--   0 root         (0) root         (0)    10309 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.093990 evals-nightly-1.0.3.dev20230613/evals/utils/
--rw-r--r--   0 root         (0) root         (0)     2136 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/api_utils.py
--rw-r--r--   0 root         (0) root         (0)      713 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/snowflake.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/evals/utils/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16118 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-13 20:51:57.000000 evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      765 2023-06-13 20:51:54.000000 evals-nightly-1.0.3.dev20230613/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 20:51:57.097990 evals-nightly-1.0.3.dev20230613/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.439249 evals-nightly-1.0.3.dev20230614/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-15 04:00:05.439249 evals-nightly-1.0.3.dev20230614/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5697 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/api.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/cli/
+-rw-r--r--   0 root         (0) root         (0)     6454 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/cli/oaieval.py
+-rw-r--r--   0 root         (0) root         (0)     3863 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/cli/oaievalset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/completion_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/completion_fns/cot.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/completion_fns/openai.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/completion_fns/retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/elsuite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/fuzzy_match_test.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/includes.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/includes_test.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/json_validator.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/json_validator_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/match.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/match_test.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/lambada.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/elsuite/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/multiple_choice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/elsuite/test/
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/test/match.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/translate.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/utils.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/elsuite/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/eval.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/formatting.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/prompt/
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/prompt/base.py
+-rw-r--r--   0 root         (0) root         (0)    18168 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.391246 evals-nightly-1.0.3.dev20230614/evals/registry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.395247 evals-nightly-1.0.3.dev20230614/evals/registry/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.399247 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/logiqa-logical-reasoning-plus.yaml
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/mazes.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/pointer-value-retrieval.yaml
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/raven-matrices.yaml
+-rw-r--r--   0 root         (0) root         (0)      560 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/test-modelgraded.yaml
+-rw-r--r--   0 root         (0) root         (0)      613 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/ukraine-gec.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.435249 evals-nightly-1.0.3.dev20230614/evals/registry/evals/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/2d_movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/3d_globe_movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/Unfamiliar-Chinese-Character.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/abstract-causal-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/adultery_state_laws.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/afrikaans-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/aime_evaluation.yaml
+-rw-r--r--   0 root         (0) root         (0)      457 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/algebra-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      418 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/allergen-information.yaml
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/alternate-numeral-systems.yaml
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ambiguous-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      229 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/arc.yaml
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/arithmetical_puzzles.yaml
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ascii-digit-recognition.yaml
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ascii-wordart.yaml
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/asl-classifiers.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/atpl_exams.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/banking77.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/beam-analysis.yaml
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/belarusian-grammar.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/belarusian-proverbs.yaml
+-rw-r--r--   0 root         (0) root         (0)      283 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/belarusian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/belarusian-russian-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/belarusian-syllable-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/belarusian-synonyms.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/bitwise.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/body-movement.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/brazilian_laws.yaml
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/building_floorplan.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/canto_wu_pronunciation.yaml
+-rw-r--r--   0 root         (0) root         (0)      355 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/canto_wu_pronunciation_fewshot.yaml
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/cardinal-directions.yaml
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/categorize_with_distractors.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chess.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chinese_hard_translations.yaml
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chinese_homonym.yaml
+-rw-r--r--   0 root         (0) root         (0)      178 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chinese_poem.yaml
+-rw-r--r--   0 root         (0) root         (0)      190 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chinese_song_ci.yaml
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chinese_tang_poetries.yaml
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/chinese_zodiac.yaml
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/cissp-study-questions.yaml
+-rw-r--r--   0 root         (0) root         (0)      372 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/code_combination.yaml
+-rw-r--r--   0 root         (0) root         (0)      343 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/color_theory_complementary.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/compare-countries-area.yaml
+-rw-r--r--   0 root         (0) root         (0)      223 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/complex-analogies-en-ru.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/comprehensive-graph-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/consensus_summary.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/context-free-grammar.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/count_intersections_polynomial.yaml
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/count_token_freq_dna.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/counterfactual-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/countries.yaml
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/cricket_situations.yaml
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/crontab.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/cybersecurity-filepaths.yaml
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/date-booking.yaml
+-rw-r--r--   0 root         (0) root         (0)      192 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/date-calculator.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/day-of-week-from-date.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/detect-hshd.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/diabetes.yaml
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/dice-rotation-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/direct-speech-tag.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/directions.yaml
+-rw-r--r--   0 root         (0) root         (0)      316 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/dna-melting-calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/dutch-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/emoji-riddle.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/escher-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/euler_problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/european-date-format-challenge.yaml
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/event-categories.yaml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/fcc_amateur_extra.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/finance.yaml
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/financial-derivatives.yaml
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/find-letter.yaml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/find-thirukkural.yaml
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/find_country_from_svg.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/finnish-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/food.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/formal-grammar-to-regex.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      928 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/french-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/french-part-of-speech.yaml
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/game-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/geometry_puzzle.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/german-part-of-speech.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/gol.yaml
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/gpt-protocol-buffers.yaml
+-rw-r--r--   0 root         (0) root         (0)      404 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/greek-nt-manuscripts.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/greek-vocabulary.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/guess-the-singer.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/hebrew-bible.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/hebrew-same-noun-gender.yaml
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/hebrew_talmud_suka.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/hindi_shuddha.yaml
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/hindi_upsc.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/hindi_words.yaml
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/historical-kana-orthography-reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      313 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/human-safety.yaml
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/iambic-pentameter.yaml
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/indonesian_numbers.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/integer-sequence-predictions.yaml
+-rw-r--r--   0 root         (0) root         (0)      235 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/internal_representations.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/invert_word_wise.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/invoice_due_date_leap_day_adjustment.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/invoices.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/irish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/irony.yaml
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/islands.yaml
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/isosceles-right-triangle.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/italian-new-words.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/italian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese-decimal-units.yaml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese-itpassport-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese-national-medical-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese-national-medical-exam02.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese_city_name_pronuciation.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese_driving_license.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese_number_reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese_onomatopoeia.yaml
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/japanese_populer_video_game_title_and_the_publisher.yaml
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/jee-math.yaml
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/json_patch_object.yaml
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/kanji-idioms.yaml
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/knot-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/korean-consonant-vowel-combination.yaml
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/korean-phonetics.yaml
+-rw-r--r--   0 root         (0) root         (0)      293 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/korean_dialects.yaml
+-rw-r--r--   0 root         (0) root         (0)      191 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/korean_spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/korean_yaminjeongeum.yaml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/language.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/largest_country.yaml
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/linear-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/linear-regression.yaml
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/list_comparison_missing_name.yaml
+-rw-r--r--   0 root         (0) root         (0)      814 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logic-grid-eval.yaml
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logic-liar-paradox.yaml
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logic-riddles.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logic_and_probability.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logical_counting.yaml
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logical_reasoning_letter_series_test.yaml
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logiqa-logical-reasoning-plus.yaml
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/loss-logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/lunar-calendar.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/mandaliof-table.yaml
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/mapping_to_matricies.yaml
+-rw-r--r--   0 root         (0) root         (0)      243 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/mate-in-one.yaml
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/math_logic_operations.yaml
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/math_polish.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/matrix-mult-rows.yaml
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/mazes.yaml
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/medication_dose.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/medmcqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 root         (0) root         (0)      337 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/missing-operators.yaml
+-rw-r--r--   0 root         (0) root         (0)    14586 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/mmlu.yaml
+-rw-r--r--   0 root         (0) root         (0)      313 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/monthly_metric_comparison.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/multi-step-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/multistep-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/music-theory-chord-names.yaml
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/music-theory-chord-notes.yaml
+-rw-r--r--   0 root         (0) root         (0)      874 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/music-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/music_theory_scale_modes.yaml
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/nepali-song-singer.yaml
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/newsology.yaml
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/next-val-series.yaml
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/nfl-point-combinations.yaml
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/non-compound-names.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/norwegian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/numbers_game.yaml
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/numeral-type-comparisons.yaml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/nutrition.yaml
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ordered-history-events.yaml
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/override-system-instruction.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/pantone_to_hex.yaml
+-rw-r--r--   0 root         (0) root         (0)      502 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/parable-to-moral-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/pararule-plus-multi-step-deductive-reasoning.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/passing-balls.yaml
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/path_enclosed_area.yaml
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 root         (0) root         (0)      287 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ph_calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      429 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/phonetics-identify-words-needing-missing-gpcs.yaml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/physics-interaction.yaml
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/pointer-value-retrieval.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/points-on-line.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/poker_analysis.yaml
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/polish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/polish-syllable-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/polish_rhymes_generation.yaml
+-rw-r--r--   0 root         (0) root         (0)      579 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/population_span_extraction.yaml
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/portuguese-sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/portuguese-syllable-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/positive-binary-operations.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/probability_questions.yaml
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/product-matching.yaml
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/prompt-injection.yaml
+-rw-r--r--   0 root         (0) root         (0)      235 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/pure_korean.yaml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/python_list_comprehension.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/qa.yaml
+-rw-r--r--   0 root         (0) root         (0)      219 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/quartz.yaml
+-rw-r--r--   0 root         (0) root         (0)      380 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/rare-and-loanwords-dutch-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)    14285 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/raven-matrices.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/rectangles.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/resistor-ohm-calculator.yaml
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/resource_id_extraction.yaml
+-rw-r--r--   0 root         (0) root         (0)      321 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/reverse-polish-notation.yaml
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/reverse-sort-words-eng.yaml
+-rw-r--r--   0 root         (0) root         (0)      378 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/rhetorical-devices.yaml
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/rock-climbing.yaml
+-rw-r--r--   0 root         (0) root         (0)      255 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 root         (0) root         (0)      468 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ru_rhymes.yaml
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/rubiks-colors.yaml
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russe.yaml
+-rw-r--r--   0 root         (0) root         (0)      298 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russian-english-homonym-context-resolution.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russian-verse.yaml
+-rw-r--r--   0 root         (0) root         (0)      190 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russian_medical.yaml
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/russian_sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/seating_arrangements.yaml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/security_guide.yaml
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/sexagenary-cycle-calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/shape-in-shape.yaml
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/shared-borders.yaml
+-rw-r--r--   0 root         (0) root         (0)      328 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/shopping_discount_comparison.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/simple-knowledge-mongolian.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/simple-visual-understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/simple_math.yaml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/simple_physics_engine.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/sindarin-fluency.yaml
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/soc_codes.yaml
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/solve-for-variable.yaml
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/sort-numeric.yaml
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/south-african-bands.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/spanish-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/spanish_feminine_noun_masculine_article.yaml
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/split_chinese_characters.yaml
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/squares-gpt.yaml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/stats-tests.yaml
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/superficial-patterns.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/svg_to_text.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/svg_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/swap-words.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/swedish_sat.yaml
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/syllables_long_words.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/syntax-check.yaml
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/tempo_to_measure_count.yaml
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/test_japanese_radical.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/test_japanese_units.yaml
+-rw-r--r--   0 root         (0) root         (0)      360 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/tetris.yaml
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/three-pt-mapping.yaml
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/time-zone-conversion.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/track_objects.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/tracking-shuffled-objects.yaml
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/turkish_characters.yaml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 root         (0) root         (0)     6692 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ukraine-gec.yaml
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/ukraine_electronic_petitions.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/unified-patch.yaml
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/unique_combinations.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/unsolvable_questions.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/unwanted-rhyming.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/utah_real_estate.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/utility_price_parsing.yaml
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/vigenere.yaml
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/vintage_phone_keyboard_decode.yaml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/which-is-heavier.yaml
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/wkt_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/evals/word_vector_over_reliance.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.439249 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/iambic_pentameter.yaml
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/onomatopoeia.yaml
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/regression-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/rhyming.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)    10309 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.439249 evals-nightly-1.0.3.dev20230614/evals/utils/
+-rw-r--r--   0 root         (0) root         (0)     2136 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/utils/api_utils.py
+-rw-r--r--   0 root         (0) root         (0)      713 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/utils/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/evals/utils/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 04:00:05.439249 evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-15 04:00:05.000000 evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16892 2023-06-15 04:00:05.000000 evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 04:00:05.000000 evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-15 04:00:05.000000 evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-15 04:00:05.000000 evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-15 04:00:05.000000 evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      765 2023-06-15 04:00:02.000000 evals-nightly-1.0.3.dev20230614/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 04:00:05.439249 evals-nightly-1.0.3.dev20230614/setup.cfg
```

### Comparing `evals-nightly-1.0.3.dev20230613/LICENSE` & `evals-nightly-1.0.3.dev20230614/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/README.md` & `evals-nightly-1.0.3.dev20230614/README.md`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/__init__.py` & `evals-nightly-1.0.3.dev20230614/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/api.py` & `evals-nightly-1.0.3.dev20230614/evals/api.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/base.py` & `evals-nightly-1.0.3.dev20230614/evals/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/cli/oaieval.py` & `evals-nightly-1.0.3.dev20230614/evals/cli/oaieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/cli/oaievalset.py` & `evals-nightly-1.0.3.dev20230614/evals/cli/oaievalset.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/completion_fns/cot.py` & `evals-nightly-1.0.3.dev20230614/evals/completion_fns/cot.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_llm.py` & `evals-nightly-1.0.3.dev20230614/evals/completion_fns/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/completion_fns/langchain_math.py` & `evals-nightly-1.0.3.dev20230614/evals/completion_fns/langchain_math.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/completion_fns/openai.py` & `evals-nightly-1.0.3.dev20230614/evals/completion_fns/openai.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/completion_fns/retrieval.py` & `evals-nightly-1.0.3.dev20230614/evals/completion_fns/retrieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/data.py` & `evals-nightly-1.0.3.dev20230614/evals/data.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/fuzzy_match.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/fuzzy_match_test.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/fuzzy_match_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/includes.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/includes.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/includes_test.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/includes_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/json_validator.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/json_validator.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/json_validator_test.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/json_validator_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/match.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/basic/match_test.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/basic/match_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/lambada.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/lambada.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/base.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/modelgraded/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/modelgraded/classify.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/modelgraded/classify_utils.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/modelgraded/classify_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/multiple_choice.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/test/match.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/test/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/translate.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/translate.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/utils.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/elsuite/utils_test.py` & `evals-nightly-1.0.3.dev20230614/evals/elsuite/utils_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/eval.py` & `evals-nightly-1.0.3.dev20230614/evals/eval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/formatting.py` & `evals-nightly-1.0.3.dev20230614/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/metrics.py` & `evals-nightly-1.0.3.dev20230614/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/prompt/base.py` & `evals-nightly-1.0.3.dev20230614/evals/prompt/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/record.py` & `evals-nightly-1.0.3.dev20230614/evals/record.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/completion_fns/langchain_llms.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/completion_fns/langchain_llms.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/raven-matrices.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/raven-matrices.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/stock-options.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/eval_sets/ukraine-gec.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/eval_sets/ukraine-gec.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/abstract-causal-reasoning.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/abstract-causal-reasoning.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/categorize_with_distractors.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/categorize_with_distractors.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/coqa-ex.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/coqa-ex.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/cybersecurity-filepaths.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/cybersecurity-filepaths.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/euler_problems.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/euler_problems.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/forth-stack-sim.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/forth-stack-sim.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/integer-sequence-predictions.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/integer-sequence-predictions.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/knot-theory.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/knot-theory.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/linear-regression.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/linear-regression.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/logic-grid-eval.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/logic-grid-eval.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/logiqa-logical-reasoning-plus.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/logiqa-logical-reasoning-plus.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/lunar-calendar.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/lunar-calendar.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/manga-translation.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/manga-translation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/mmlu.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/mmlu.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/music-theory.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/music-theory.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/naughty_strings.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/naughty_strings.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/non-compound-names.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/non-compound-names.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/pointer-value-retrieval.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/pointer-value-retrieval.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/population_span_extraction.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/population_span_extraction.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/product-matching.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/product-matching.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/raven-matrices.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/raven-matrices.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/sql.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/stock-options.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-basic.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-basic.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/test-modelgraded.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/test-modelgraded.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/evals/ukraine-gec.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/evals/ukraine-gec.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/closedqa.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/closedqa.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/fact.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/fact.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/humor.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/humor.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/regression-equation.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/regression-equation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry/modelgraded/sql.yaml` & `evals-nightly-1.0.3.dev20230614/evals/registry/modelgraded/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/registry.py` & `evals-nightly-1.0.3.dev20230614/evals/registry.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/utils/api_utils.py` & `evals-nightly-1.0.3.dev20230614/evals/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/utils/misc.py` & `evals-nightly-1.0.3.dev20230614/evals/utils/misc.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/utils/snowflake.py` & `evals-nightly-1.0.3.dev20230614/evals/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals/utils/test.py` & `evals-nightly-1.0.3.dev20230614/evals/utils/test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230613/evals_nightly.egg-info/SOURCES.txt` & `evals-nightly-1.0.3.dev20230614/evals_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,45 +39,49 @@
 evals/prompt/base.py
 evals/registry/completion_fns/cot.yaml
 evals/registry/completion_fns/langchain_chains.yaml
 evals/registry/completion_fns/langchain_llms.yaml
 evals/registry/eval_sets/coqa-ex.yaml
 evals/registry/eval_sets/logiqa-logical-reasoning-plus.yaml
 evals/registry/eval_sets/manga-translation.yaml
+evals/registry/eval_sets/mazes.yaml
 evals/registry/eval_sets/pointer-value-retrieval.yaml
 evals/registry/eval_sets/raven-matrices.yaml
 evals/registry/eval_sets/stock-options.yaml
 evals/registry/eval_sets/test-all.yaml
 evals/registry/eval_sets/test-basic.yaml
 evals/registry/eval_sets/test-modelgraded.yaml
 evals/registry/eval_sets/ukraine-gec.yaml
 evals/registry/evals/2d_movement.yaml
 evals/registry/evals/3d_globe_movement.yaml
+evals/registry/evals/Unfamiliar-Chinese-Character.yaml
 evals/registry/evals/aba-mrpc-true-false.yaml
 evals/registry/evals/abstract-causal-reasoning.yaml
 evals/registry/evals/actors-sequence.yaml
 evals/registry/evals/adultery_state_laws.yaml
 evals/registry/evals/afrikaans-lexicon.yaml
 evals/registry/evals/aime_evaluation.yaml
 evals/registry/evals/algebra-word-problems.yaml
 evals/registry/evals/allergen-information.yaml
 evals/registry/evals/alternate-numeral-systems.yaml
 evals/registry/evals/ambiguous-sentences.yaml
 evals/registry/evals/anagrams.yaml
 evals/registry/evals/arc.yaml
 evals/registry/evals/arithmetical_puzzles.yaml
+evals/registry/evals/ascii-digit-recognition.yaml
 evals/registry/evals/ascii-wordart.yaml
 evals/registry/evals/asl-classifiers.yaml
 evals/registry/evals/atpl_exams.yaml
 evals/registry/evals/balance-chemical-equation.yaml
 evals/registry/evals/banking77.yaml
 evals/registry/evals/beam-analysis.yaml
 evals/registry/evals/belarusian-grammar.yaml
 evals/registry/evals/belarusian-lexicon.yaml
 evals/registry/evals/belarusian-proverbs.yaml
+evals/registry/evals/belarusian-rhyme.yaml
 evals/registry/evals/belarusian-russian-translation.yaml
 evals/registry/evals/belarusian-syllable-count.yaml
 evals/registry/evals/belarusian-synonyms.yaml
 evals/registry/evals/bigrams.yaml
 evals/registry/evals/bitwise.yaml
 evals/registry/evals/body-movement.yaml
 evals/registry/evals/born-first.yaml
@@ -87,27 +91,29 @@
 evals/registry/evals/bulgarian-lexicon.yaml
 evals/registry/evals/canto_wu_pronunciation.yaml
 evals/registry/evals/canto_wu_pronunciation_fewshot.yaml
 evals/registry/evals/cardinal-directions.yaml
 evals/registry/evals/categorize_with_distractors.yaml
 evals/registry/evals/chess-piece-count.yaml
 evals/registry/evals/chess.yaml
+evals/registry/evals/chinese_hard_translations.yaml
 evals/registry/evals/chinese_homonym.yaml
 evals/registry/evals/chinese_poem.yaml
 evals/registry/evals/chinese_song_ci.yaml
 evals/registry/evals/chinese_tang_poetries.yaml
 evals/registry/evals/chinese_zodiac.yaml
 evals/registry/evals/cissp-study-questions.yaml
 evals/registry/evals/code_combination.yaml
 evals/registry/evals/color_theory_complementary.yaml
 evals/registry/evals/compare-countries-area.yaml
 evals/registry/evals/complex-analogies-en-ru.yaml
 evals/registry/evals/complex-replace-characters.yaml
 evals/registry/evals/comprehensive-graph-reasoning.yaml
 evals/registry/evals/connect-4.yaml
+evals/registry/evals/consensus_summary.yaml
 evals/registry/evals/context-free-grammar.yaml
 evals/registry/evals/convert-hex-hsl-lightness.yaml
 evals/registry/evals/coqa-ex.yaml
 evals/registry/evals/count_intersections_polynomial.yaml
 evals/registry/evals/count_token_freq_dna.yaml
 evals/registry/evals/counterfactual-reasoning.yaml
 evals/registry/evals/countries.yaml
@@ -157,14 +163,15 @@
 evals/registry/evals/greek-nt-manuscripts.yaml
 evals/registry/evals/greek-vocabulary.yaml
 evals/registry/evals/guess-the-singer.yaml
 evals/registry/evals/heart-disease.yaml
 evals/registry/evals/hebrew-bible.yaml
 evals/registry/evals/hebrew-rhyme.yaml
 evals/registry/evals/hebrew-same-noun-gender.yaml
+evals/registry/evals/hebrew_talmud_suka.yaml
 evals/registry/evals/hindi_shuddha.yaml
 evals/registry/evals/hindi_upsc.yaml
 evals/registry/evals/hindi_words.yaml
 evals/registry/evals/historical-kana-orthography-reading.yaml
 evals/registry/evals/human-safety.yaml
 evals/registry/evals/iambic-pentameter.yaml
 evals/registry/evals/illinois-law.yaml
@@ -178,20 +185,22 @@
 evals/registry/evals/invoices.yaml
 evals/registry/evals/irish-lexicon.yaml
 evals/registry/evals/irony.yaml
 evals/registry/evals/islands.yaml
 evals/registry/evals/isosceles-right-triangle.yaml
 evals/registry/evals/italian-new-words.yaml
 evals/registry/evals/italian-rhyme.yaml
+evals/registry/evals/japanese-decimal-units.yaml
 evals/registry/evals/japanese-itpassport-exam01.yaml
 evals/registry/evals/japanese-national-medical-exam01.yaml
 evals/registry/evals/japanese-national-medical-exam02.yaml
 evals/registry/evals/japanese_city_name_pronuciation.yaml
 evals/registry/evals/japanese_driving_license.yaml
 evals/registry/evals/japanese_number_reading.yaml
+evals/registry/evals/japanese_onomatopoeia.yaml
 evals/registry/evals/japanese_populer_video_game_title_and_the_publisher.yaml
 evals/registry/evals/jee-math.yaml
 evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
 evals/registry/evals/json_patch_object.yaml
 evals/registry/evals/kanji-idioms.yaml
 evals/registry/evals/knot-theory.yaml
 evals/registry/evals/korean-consonant-vowel-combination.yaml
@@ -209,24 +218,28 @@
 evals/registry/evals/logic-grid-eval.yaml
 evals/registry/evals/logic-liar-paradox.yaml
 evals/registry/evals/logic-riddles.yaml
 evals/registry/evals/logic-statements.yaml
 evals/registry/evals/logic.yaml
 evals/registry/evals/logic_and_probability.yaml
 evals/registry/evals/logical_counting.yaml
+evals/registry/evals/logical_reasoning_letter_series_test.yaml
 evals/registry/evals/logiqa-logical-reasoning-plus.yaml
 evals/registry/evals/logiqa.yaml
 evals/registry/evals/loss-logic.yaml
 evals/registry/evals/lunar-calendar.yaml
 evals/registry/evals/mandaliof-table.yaml
 evals/registry/evals/manga-translation.yaml
 evals/registry/evals/map-electronic-component-part-to-fact.yaml
 evals/registry/evals/mapping_to_matricies.yaml
 evals/registry/evals/mate-in-one.yaml
+evals/registry/evals/math_logic_operations.yaml
+evals/registry/evals/math_polish.yaml
 evals/registry/evals/matrix-mult-rows.yaml
+evals/registry/evals/mazes.yaml
 evals/registry/evals/medication_dose.yaml
 evals/registry/evals/medmcqa.yaml
 evals/registry/evals/mendelian_inheritance.yaml
 evals/registry/evals/missing-operators.yaml
 evals/registry/evals/mmlu.yaml
 evals/registry/evals/monthly_metric_comparison.yaml
 evals/registry/evals/moral_exceptQA.yaml
@@ -251,14 +264,15 @@
 evals/registry/evals/ordered-history-events.yaml
 evals/registry/evals/override-system-instruction.yaml
 evals/registry/evals/pantone_to_hex.yaml
 evals/registry/evals/parable-to-moral-match.yaml
 evals/registry/evals/pararule-plus-multi-step-deductive-reasoning.yaml
 evals/registry/evals/partially_solved_crossword_clues.yaml
 evals/registry/evals/passing-balls.yaml
+evals/registry/evals/path_enclosed_area.yaml
 evals/registry/evals/pattern_identification.yaml
 evals/registry/evals/ph_calculation.yaml
 evals/registry/evals/phonetics-identify-words-needing-missing-gpcs.yaml
 evals/registry/evals/physics-interaction.yaml
 evals/registry/evals/pointer-value-retrieval.yaml
 evals/registry/evals/points-on-line.yaml
 evals/registry/evals/poker_analysis.yaml
@@ -320,14 +334,15 @@
 evals/registry/evals/spanish_feminine_noun_masculine_article.yaml
 evals/registry/evals/split_chinese_characters.yaml
 evals/registry/evals/sql.yaml
 evals/registry/evals/squares-gpt.yaml
 evals/registry/evals/stats-tests.yaml
 evals/registry/evals/stock-options.yaml
 evals/registry/evals/superficial-patterns.yaml
+evals/registry/evals/svg_to_text.yaml
 evals/registry/evals/svg_understanding.yaml
 evals/registry/evals/swap-words.yaml
 evals/registry/evals/swedish-spelling.yaml
 evals/registry/evals/swedish_sat.yaml
 evals/registry/evals/syllables_long_words.yaml
 evals/registry/evals/syntax-check.yaml
 evals/registry/evals/taxes.yaml
@@ -349,27 +364,29 @@
 evals/registry/evals/ukraine-gec.yaml
 evals/registry/evals/ukraine_electronic_petitions.yaml
 evals/registry/evals/unified-patch.yaml
 evals/registry/evals/unique_combinations.yaml
 evals/registry/evals/unsolvable_questions.yaml
 evals/registry/evals/unwanted-rhyming.yaml
 evals/registry/evals/us-tort-law.yaml
+evals/registry/evals/utah_real_estate.yaml
 evals/registry/evals/utility_price_parsing.yaml
 evals/registry/evals/vigenere.yaml
 evals/registry/evals/vintage_phone_keyboard_decode.yaml
 evals/registry/evals/which-is-heavier.yaml
 evals/registry/evals/wkt_understanding.yaml
 evals/registry/evals/word_vector_over_reliance.yaml
 evals/registry/modelgraded/battle.yaml
 evals/registry/modelgraded/best.yaml
 evals/registry/modelgraded/closedqa.yaml
 evals/registry/modelgraded/diversity.yaml
 evals/registry/modelgraded/fact.yaml
 evals/registry/modelgraded/humor.yaml
 evals/registry/modelgraded/iambic_pentameter.yaml
+evals/registry/modelgraded/onomatopoeia.yaml
 evals/registry/modelgraded/regression-equation.yaml
 evals/registry/modelgraded/rhyming.yaml
 evals/registry/modelgraded/security.yaml
 evals/registry/modelgraded/sql.yaml
 evals/utils/api_utils.py
 evals/utils/misc.py
 evals/utils/snowflake.py
```

### Comparing `evals-nightly-1.0.3.dev20230613/pyproject.toml` & `evals-nightly-1.0.3.dev20230614/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "evals-nightly"
-version = "1.0.3.dev20230613"
+version = "1.0.3.dev20230614"
 requires-python = ">=3.9"
 dependencies = [
     "mypy",
     "openai >= 0.27.2",
     "tiktoken",
     "blobfile",
     "backoff",
```

