# Comparing `tmp/discopy-1.1.2.tar.gz` & `tmp/discopy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discopy-1.1.2.tar", last modified: Fri May 26 07:43:50 2023, max compression
+gzip compressed data, was "discopy-1.1.3.tar", last modified: Thu Jun  1 18:45:51 2023, max compression
```

## Comparing `discopy-1.1.2.tar` & `discopy-1.1.3.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.251029 discopy-1.1.2/
--rw-r--r--   0 aleumi     (502) staff       (20)       33 2023-05-26 07:41:40.000000 discopy-1.1.2/.gitattributes
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.822315 discopy-1.1.2/.github/
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.850671 discopy-1.1.2/.github/workflows/
--rw-r--r--   0 aleumi     (502) staff       (20)     1606 2023-05-26 07:41:40.000000 discopy-1.1.2/.github/workflows/build_test.yml
--rw-r--r--   0 aleumi     (502) staff       (20)      183 2023-05-26 07:41:40.000000 discopy-1.1.2/.gitignore
--rw-r--r--   0 aleumi     (502) staff       (20)    20606 2023-05-26 07:41:40.000000 discopy-1.1.2/.pylintrc
--rw-r--r--   0 aleumi     (502) staff       (20)      744 2023-05-26 07:41:40.000000 discopy-1.1.2/.readthedocs.yaml
--rw-r--r--   0 aleumi     (502) staff       (20)     1171 2023-05-26 07:41:40.000000 discopy-1.1.2/CONTRIBUTING.md
--rw-r--r--   0 aleumi     (502) staff       (20)     1520 2023-05-26 07:41:40.000000 discopy-1.1.2/LICENSE
--rw-r--r--   0 aleumi     (502) staff       (20)     5596 2023-05-26 07:43:50.251977 discopy-1.1.2/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     4532 2023-05-26 07:41:40.000000 discopy-1.1.2/README.md
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.885085 discopy-1.1.2/discopy/
--rw-r--r--   0 aleumi     (502) staff       (20)      499 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5758 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/balanced.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8328 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/braided.py
--rw-r--r--   0 aleumi     (502) staff       (20)    28200 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/cat.py
--rw-r--r--   0 aleumi     (502) staff       (20)    10182 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/closed.py
--rw-r--r--   0 aleumi     (502) staff       (20)     4417 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/compact.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1487 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/config.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.894222 discopy-1.1.2/discopy/drawing/
--rw-r--r--   0 aleumi     (502) staff       (20)     1060 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/drawing/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13920 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/drawing/grid.py
--rw-r--r--   0 aleumi     (502) staff       (20)    36769 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/drawing/legacy.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11613 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/frobenius.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.901668 discopy-1.1.2/discopy/grammar/
--rw-r--r--   0 aleumi     (502) staff       (20)      225 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9405 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/categorial.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6890 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/cfg.py
--rw-r--r--   0 aleumi     (502) staff       (20)      926 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/dependency.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7162 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/pregroup.py
--rw-r--r--   0 aleumi     (502) staff       (20)     2410 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/grammar/thue.py
--rw-r--r--   0 aleumi     (502) staff       (20)    48318 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/hypergraph.py
--rw-r--r--   0 aleumi     (502) staff       (20)    14028 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/interaction.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8050 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/markov.py
--rw-r--r--   0 aleumi     (502) staff       (20)    16146 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/matrix.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1555 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/messages.py
--rw-r--r--   0 aleumi     (502) staff       (20)    35222 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/monoidal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6871 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/pivotal.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7845 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/python.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.916584 discopy-1.1.2/discopy/quantum/
--rw-r--r--   0 aleumi     (502) staff       (20)      667 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/__init__.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5238 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/ansatze.py
--rw-r--r--   0 aleumi     (502) staff       (20)    11626 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/channel.py
--rw-r--r--   0 aleumi     (502) staff       (20)    32818 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/circuit.py
--rw-r--r--   0 aleumi     (502) staff       (20)    24488 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/gates.py
--rw-r--r--   0 aleumi     (502) staff       (20)    15738 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/pennylane.py
--rw-r--r--   0 aleumi     (502) staff       (20)    16429 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/tk.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13451 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/quantum/zx.py
--rw-r--r--   0 aleumi     (502) staff       (20)     6916 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/ribbon.py
--rw-r--r--   0 aleumi     (502) staff       (20)    25765 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/rigid.py
--rw-r--r--   0 aleumi     (502) staff       (20)     9007 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/symmetric.py
--rw-r--r--   0 aleumi     (502) staff       (20)    23082 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/tensor.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7593 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/traced.py
--rw-r--r--   0 aleumi     (502) staff       (20)    20851 2023-05-26 07:41:40.000000 discopy-1.1.2/discopy/utils.py
--rw-r--r--   0 aleumi     (502) staff       (20)      160 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy/version.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.891931 discopy-1.1.2/discopy.egg-info/
--rw-r--r--   0 aleumi     (502) staff       (20)     5596 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/PKG-INFO
--rw-r--r--   0 aleumi     (502) staff       (20)     6584 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/SOURCES.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        1 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/dependency_links.txt
--rw-r--r--   0 aleumi     (502) staff       (20)      412 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/requires.txt
--rw-r--r--   0 aleumi     (502) staff       (20)        8 2023-05-26 07:43:49.000000 discopy-1.1.2/discopy.egg-info/top_level.txt
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.922870 discopy-1.1.2/docs/
--rw-r--r--   0 aleumi     (502) staff       (20)      634 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/Makefile
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.926526 discopy-1.1.2/docs/_ext/
--rw-r--r--   0 aleumi     (502) staff       (20)      684 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_ext/bases-fullname.py
--rw-r--r--   0 aleumi     (502) staff       (20)     3939 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_ext/youtube.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.930633 discopy-1.1.2/docs/_static/
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.938638 discopy-1.1.2/docs/_static/balanced/
--rw-r--r--   0 aleumi     (502) staff       (20)    14901 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/balanced/ribbon_twist.png
--rw-r--r--   0 aleumi     (502) staff       (20)    13367 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/balanced/twist.png
--rw-r--r--   0 aleumi     (502) staff       (20)    11712 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/balanced/twist_dual_rail.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.940632 discopy-1.1.2/docs/_static/braided/
--rw-r--r--   0 aleumi     (502) staff       (20)     8951 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/braided/hexagons.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9432 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/braided/inverse.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.944285 discopy-1.1.2/docs/_static/closed/
--rw-r--r--   0 aleumi     (502) staff       (20)    15711 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/closed/curry-left.png
--rw-r--r--   0 aleumi     (502) staff       (20)    15643 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/closed/curry-right.png
--rw-r--r--   0 aleumi     (502) staff       (20)    19051 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/closed/uncurry.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.950817 discopy-1.1.2/docs/_static/compact/
--rw-r--r--   0 aleumi     (502) staff       (20)    14358 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/reidemeister.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10190 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/snake.png
--rw-r--r--   0 aleumi     (502) staff       (20)    14358 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/yanking.png
--rw-r--r--   0 aleumi     (502) staff       (20)    14061 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/compact/yanking_cup_and_cap.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.953606 discopy-1.1.2/docs/_static/drawing/
--rw-r--r--   0 aleumi     (502) staff       (20)     5271 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/drawing/diagramize.png
--rw-r--r--   0 aleumi     (502) staff       (20)     3578 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/drawing/example.html
--rw-r--r--   0 aleumi     (502) staff       (20)    10626 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/drawing/frobenius-axioms.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.960041 discopy-1.1.2/docs/_static/frobenius/
--rw-r--r--   0 aleumi     (502) staff       (20)    17147 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/comonoid.png
--rw-r--r--   0 aleumi     (502) staff       (20)    14853 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/frobenius.png
--rw-r--r--   0 aleumi     (502) staff       (20)    17266 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/monoid.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9884 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/frobenius/special.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.963013 discopy-1.1.2/docs/_static/grammar/
--rw-r--r--   0 aleumi     (502) staff       (20)     9591 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/grammar/cfg-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)     7224 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/grammar/pregroup-example.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.968364 discopy-1.1.2/docs/_static/hypergraph/
--rw-r--r--   0 aleumi     (502) staff       (20)    16894 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/hypergraph/box.png
--rw-r--r--   0 aleumi     (502) staff       (20)    20670 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/hypergraph/diagram.png
--rw-r--r--   0 aleumi     (502) staff       (20)    15394 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/hypergraph/unfuse.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.982288 discopy-1.1.2/docs/_static/int/
--rw-r--r--   0 aleumi     (502) staff       (20)    16145 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/alice-loves-bob.png
--rw-r--r--   0 aleumi     (502) staff       (20)    18363 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/braid.png
--rw-r--r--   0 aleumi     (502) staff       (20)    16332 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/composition.png
--rw-r--r--   0 aleumi     (502) staff       (20)     8274 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/dagger.png
--rw-r--r--   0 aleumi     (502) staff       (20)    16257 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/idl.png
--rw-r--r--   0 aleumi     (502) staff       (20)    16615 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/idr.png
--rw-r--r--   0 aleumi     (502) staff       (20)    16069 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/int-snake-equations.png
--rw-r--r--   0 aleumi     (502) staff       (20)    22712 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/simplify.png
--rw-r--r--   0 aleumi     (502) staff       (20)    16278 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/int/tensor.png
--rw-r--r--   0 aleumi     (502) staff       (20)   105662 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/logo.ico
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.985865 discopy-1.1.2/docs/_static/markov/
--rw-r--r--   0 aleumi     (502) staff       (20)    13158 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/associativity.png
--rw-r--r--   0 aleumi     (502) staff       (20)    14407 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/bialgebra.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10317 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/copy_and_apply.png
--rw-r--r--   0 aleumi     (502) staff       (20)     8979 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/markov/counit.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.009502 discopy-1.1.2/docs/_static/monoidal/
--rw-r--r--   0 aleumi     (502) staff       (20)     2875 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/Eckmann-Hilton.gif
--rw-r--r--   0 aleumi     (502) staff       (20)    12008 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/EckmannHilton.gif
--rw-r--r--   0 aleumi     (502) staff       (20)     3504 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/arrow-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)     2166 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/box-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)    14662 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/bubble-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10047 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-1.png
--rw-r--r--   0 aleumi     (502) staff       (20)     7535 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-1a.png
--rw-r--r--   0 aleumi     (502) staff       (20)     7221 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-1b.png
--rw-r--r--   0 aleumi     (502) staff       (20)     4433 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/foliate-example-2.png
--rw-r--r--   0 aleumi     (502) staff       (20)     7089 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/functor-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)     2617 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/id-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)   404531 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/spiral.gif
--rw-r--r--   0 aleumi     (502) staff       (20)     2888 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/monoidal/tensor-example.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.012289 discopy-1.1.2/docs/_static/optics/
--rw-r--r--   0 aleumi     (502) staff       (20)     7259 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/optics/fusion.png
--rw-r--r--   0 aleumi     (502) staff       (20)    15302 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/optics/spider-decomp.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.018124 discopy-1.1.2/docs/_static/pivotal/
--rw-r--r--   0 aleumi     (502) staff       (20)    10105 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/axiom.png
--rw-r--r--   0 aleumi     (502) staff       (20)     6542 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/box-conjugate.png
--rw-r--r--   0 aleumi     (502) staff       (20)     7722 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/conjugate.png
--rw-r--r--   0 aleumi     (502) staff       (20)     6710 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/dagger-transpose.png
--rw-r--r--   0 aleumi     (502) staff       (20)     8451 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/dagger.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10350 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/pivotal/trace.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.020097 discopy-1.1.2/docs/_static/quantum/
--rw-r--r--   0 aleumi     (502) staff       (20)    13104 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/quantum/circuit-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)    17758 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/quantum/functor-example.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.023476 discopy-1.1.2/docs/_static/ribbon/
--rw-r--r--   0 aleumi     (502) staff       (20)     6787 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/ribbon/strict.png
--rw-r--r--   0 aleumi     (502) staff       (20)    15078 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/ribbon/twist-untwist.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.044074 discopy-1.1.2/docs/_static/rigid/
--rw-r--r--   0 aleumi     (502) staff       (20)     2296 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/cap.png
--rw-r--r--   0 aleumi     (502) staff       (20)     3223 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/caps.png
--rw-r--r--   0 aleumi     (502) staff       (20)     2352 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/cup.png
--rw-r--r--   0 aleumi     (502) staff       (20)     3131 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/cups.png
--rw-r--r--   0 aleumi     (502) staff       (20)     8834 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/curry.png
--rw-r--r--   0 aleumi     (502) staff       (20)     4537 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/diagram-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10267 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/functor-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)    11845 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/rotate.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9160 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/transpose.png
--rw-r--r--   0 aleumi     (502) staff       (20)    13976 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/transpose_box.png
--rw-r--r--   0 aleumi     (502) staff       (20)     5315 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/rigid/typed-snake-equation.png
--rw-r--r--   0 aleumi     (502) staff       (20)     5315 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/snake-equation.png
--rw-r--r--   0 aleumi     (502) staff       (20)   963196 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/spiral.gif
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.054391 discopy-1.1.2/docs/_static/symmetric/
--rw-r--r--   0 aleumi     (502) staff       (20)    13136 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/decorator.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9819 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/hexagons.png
--rw-r--r--   0 aleumi     (502) staff       (20)     6665 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/inverse.png
--rw-r--r--   0 aleumi     (502) staff       (20)     7307 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/naturality.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10124 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/symmetric/yang-baxter.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.065539 discopy-1.1.2/docs/_static/tensor/
--rw-r--r--   0 aleumi     (502) staff       (20)    17466 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/chain-rule.png
--rw-r--r--   0 aleumi     (502) staff       (20)     4810 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/frobenius-example.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10998 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/men-are-mortal.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9312 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/product-rule.png
--rw-r--r--   0 aleumi     (502) staff       (20)    13435 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/tensor/rewrite.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.081929 discopy-1.1.2/docs/_static/traced/
--rw-r--r--   0 aleumi     (502) staff       (20)    10121 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/golden.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10550 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/right-nat-trace.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9691 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/sliding-left.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9887 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/sliding-right.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10411 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/tightening-left.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10550 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/tightening-right.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10247 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/trace.png
--rw-r--r--   0 aleumi     (502) staff       (20)    12964 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_static/traced/yanking.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.084145 discopy-1.1.2/docs/_style/
--rw-r--r--   0 aleumi     (502) staff       (20)     1811 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_style/custom.css
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.091308 discopy-1.1.2/docs/_templates/
--rw-r--r--   0 aleumi     (502) staff       (20)      185 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_templates/class.rst
--rw-r--r--   0 aleumi     (502) staff       (20)      100 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_templates/function.rst
--rw-r--r--   0 aleumi     (502) staff       (20)       66 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/_templates/module.rst
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.112736 discopy-1.1.2/docs/api/
--rw-r--r--   0 aleumi     (502) staff       (20)     4581 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/architecture.html
--rw-r--r--   0 aleumi     (502) staff       (20)    56460 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/architecture.png
--rw-r--r--   0 aleumi     (502) staff       (20)      168 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/drawing.rst
--rw-r--r--   0 aleumi     (502) staff       (20)      256 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/grammar.rst
--rw-r--r--   0 aleumi     (502) staff       (20)      302 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/quantum.rst
--rw-r--r--   0 aleumi     (502) staff       (20)      222 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/semantics.rst
--rw-r--r--   0 aleumi     (502) staff       (20)      458 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/api/syntax.rst
--rw-r--r--   0 aleumi     (502) staff       (20)     3037 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/conf.py
--rw-r--r--   0 aleumi     (502) staff       (20)    13274 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/discopy.bib
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.118645 discopy-1.1.2/docs/extra/
--rw-r--r--   0 aleumi     (502) staff       (20)       57 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/bibliography.rst
--rw-r--r--   0 aleumi     (502) staff       (20)     1059 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/blogs.md
--rw-r--r--   0 aleumi     (502) staff       (20)     6077 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/papers.md
--rw-r--r--   0 aleumi     (502) staff       (20)     1492 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/extra/talks.rst
--rw-r--r--   0 aleumi     (502) staff       (20)      780 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/index.rst
--rw-r--r--   0 aleumi     (502) staff       (20)      795 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/make.bat
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.136865 discopy-1.1.2/docs/notebooks/
--rw-r--r--   0 aleumi     (502) staff       (20)   483325 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/21-05-03-tallcat.ipynb
--rw-r--r--   0 aleumi     (502) staff       (20)  1593241 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/21-05-05-tallcat.ipynb
--rw-r--r--   0 aleumi     (502) staff       (20)    42815 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/diag-diff.ipynb
--rw-r--r--   0 aleumi     (502) staff       (20)   179435 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/diagrams.ipynb
--rw-r--r--   0 aleumi     (502) staff       (20)   185975 2023-05-26 07:41:40.000000 discopy-1.1.2/docs/notebooks/qnlp.ipynb
--rw-r--r--   0 aleumi     (502) staff       (20)      140 2023-05-26 07:41:40.000000 discopy-1.1.2/pyproject.toml
--rw-r--r--   0 aleumi     (502) staff       (20)     1703 2023-05-26 07:43:50.260715 discopy-1.1.2/setup.cfg
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:49.839776 discopy-1.1.2/test/
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.139445 discopy-1.1.2/test/drawing/
--rw-r--r--   0 aleumi     (502) staff       (20)     5571 2023-05-26 07:41:40.000000 discopy-1.1.2/test/drawing/legacy.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.142325 discopy-1.1.2/test/grammar/
--rw-r--r--   0 aleumi     (502) staff       (20)     7756 2023-05-26 07:41:40.000000 discopy-1.1.2/test/grammar/categorial.py
--rw-r--r--   0 aleumi     (502) staff       (20)     2049 2023-05-26 07:41:40.000000 discopy-1.1.2/test/grammar/pregroup.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.150706 discopy-1.1.2/test/quantum/
--rw-r--r--   0 aleumi     (502) staff       (20)      425 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/ansatze.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1551 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/channel.py
--rw-r--r--   0 aleumi     (502) staff       (20)    25046 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/circuit.py
--rw-r--r--   0 aleumi     (502) staff       (20)     2510 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/eval.py
--rw-r--r--   0 aleumi     (502) staff       (20)     4296 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/tk.py
--rw-r--r--   0 aleumi     (502) staff       (20)     5804 2023-05-26 07:41:40.000000 discopy-1.1.2/test/quantum/zx.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.161254 discopy-1.1.2/test/semantics/
--rw-r--r--   0 aleumi     (502) staff       (20)     1201 2023-05-26 07:41:40.000000 discopy-1.1.2/test/semantics/matrix.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1304 2023-05-26 07:41:40.000000 discopy-1.1.2/test/semantics/python.py
--rw-r--r--   0 aleumi     (502) staff       (20)     8105 2023-05-26 07:41:40.000000 discopy-1.1.2/test/semantics/tensor.py
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.162827 discopy-1.1.2/test/src/
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.181503 discopy-1.1.2/test/src/imgs/
--rw-r--r--   0 aleumi     (502) staff       (20)    12008 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/EckmannHilton.gif
--rw-r--r--   0 aleumi     (502) staff       (20)     7553 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/bell-state.png
--rw-r--r--   0 aleumi     (502) staff       (20)    16964 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/bialgebra.png
--rw-r--r--   0 aleumi     (502) staff       (20)    25004 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/crack-eggs.png
--rw-r--r--   0 aleumi     (502) staff       (20)     2411 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/empty_diagram.png
--rw-r--r--   0 aleumi     (502) staff       (20)     5907 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/long-controlled.png
--rw-r--r--   0 aleumi     (502) staff       (20)     8810 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/sentence-as-diagram.png
--rw-r--r--   0 aleumi     (502) staff       (20)     5315 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/snake-equation.png
--rw-r--r--   0 aleumi     (502) staff       (20)    10800 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/spiral.png
--rw-r--r--   0 aleumi     (502) staff       (20)     6051 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/typed-snake-equation.png
--rw-r--r--   0 aleumi     (502) staff       (20)     9525 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/imgs/who-ansatz.png
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.210883 discopy-1.1.2/test/src/tikz/
--rw-r--r--   0 aleumi     (502) staff       (20)     2228 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bell-state.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)      153 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bell-state.tikzstyles
--rw-r--r--   0 aleumi     (502) staff       (20)     4906 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bialgebra.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)      150 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/bialgebra.tikzstyles
--rw-r--r--   0 aleumi     (502) staff       (20)     2441 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/copy.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)       86 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/copy.tikzstyles
--rw-r--r--   0 aleumi     (502) staff       (20)     3441 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/crack-eggs.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)     3338 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/long-controlled.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)     2223 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/snake-equation.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)     1906 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/spiral.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)      260 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/spiral.tikzstyles
--rw-r--r--   0 aleumi     (502) staff       (20)     3435 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tikz/who-ansatz.tikz
--rw-r--r--   0 aleumi     (502) staff       (20)    15562 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/tree2diagram.pickle
--rw-r--r--   0 aleumi     (502) staff       (20)     6324 2023-05-26 07:41:40.000000 discopy-1.1.2/test/src/zx-graph.json
-drwxr-xr-x   0 aleumi     (502) staff       (20)        0 2023-05-26 07:43:50.250191 discopy-1.1.2/test/syntax/
--rw-r--r--   0 aleumi     (502) staff       (20)      258 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/balanced.py
--rw-r--r--   0 aleumi     (502) staff       (20)      487 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/braided.py
--rw-r--r--   0 aleumi     (502) staff       (20)     7650 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/cat.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1413 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/closed.py
--rw-r--r--   0 aleumi     (502) staff       (20)      828 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/compact.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1750 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/frobenius.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1934 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/hypergraph.py
--rw-r--r--   0 aleumi     (502) staff       (20)      659 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/interaction.py
--rw-r--r--   0 aleumi     (502) staff       (20)     1532 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/markov.py
--rw-r--r--   0 aleumi     (502) staff       (20)    10159 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/monoidal.py
--rw-r--r--   0 aleumi     (502) staff       (20)      176 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/pivotal.py
--rw-r--r--   0 aleumi     (502) staff       (20)      553 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/ribbon.py
--rw-r--r--   0 aleumi     (502) staff       (20)     3278 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/rigid.py
--rw-r--r--   0 aleumi     (502) staff       (20)      962 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/symmetric.py
--rw-r--r--   0 aleumi     (502) staff       (20)      354 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/traced.py
--rw-r--r--   0 aleumi     (502) staff       (20)      953 2023-05-26 07:41:40.000000 discopy-1.1.2/test/syntax/utils.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.908706 discopy-1.1.3/
+-rw-r--r--   0 boldi      (502) staff       (20)       33 2022-09-27 14:39:16.000000 discopy-1.1.3/.gitattributes
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.847974 discopy-1.1.3/.github/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.853726 discopy-1.1.3/.github/workflows/
+-rw-r--r--   0 boldi      (502) staff       (20)     1714 2023-05-31 13:21:06.000000 discopy-1.1.3/.github/workflows/build_test.yml
+-rw-r--r--   0 boldi      (502) staff       (20)      183 2023-05-31 09:22:59.000000 discopy-1.1.3/.gitignore
+-rw-r--r--   0 boldi      (502) staff       (20)    20606 2023-05-31 09:22:59.000000 discopy-1.1.3/.pylintrc
+-rw-r--r--   0 boldi      (502) staff       (20)      744 2023-05-31 09:22:59.000000 discopy-1.1.3/.readthedocs.yaml
+-rw-r--r--   0 boldi      (502) staff       (20)     1171 2023-05-31 09:22:59.000000 discopy-1.1.3/CONTRIBUTING.md
+-rw-r--r--   0 boldi      (502) staff       (20)     1520 2023-05-31 09:22:59.000000 discopy-1.1.3/LICENSE
+-rw-r--r--   0 boldi      (502) staff       (20)     7385 2023-06-01 18:45:51.908423 discopy-1.1.3/PKG-INFO
+-rw-r--r--   0 boldi      (502) staff       (20)     4532 2023-05-31 09:22:59.000000 discopy-1.1.3/README.md
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.860295 discopy-1.1.3/discopy/
+-rw-r--r--   0 boldi      (502) staff       (20)      499 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)     5758 2023-05-31 13:40:28.000000 discopy-1.1.3/discopy/balanced.py
+-rw-r--r--   0 boldi      (502) staff       (20)     8305 2023-05-31 13:40:04.000000 discopy-1.1.3/discopy/braided.py
+-rw-r--r--   0 boldi      (502) staff       (20)    28177 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/cat.py
+-rw-r--r--   0 boldi      (502) staff       (20)    10172 2023-05-31 13:23:34.000000 discopy-1.1.3/discopy/closed.py
+-rw-r--r--   0 boldi      (502) staff       (20)     4513 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/compact.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1487 2023-06-01 16:43:13.000000 discopy-1.1.3/discopy/config.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.861686 discopy-1.1.3/discopy/drawing/
+-rw-r--r--   0 boldi      (502) staff       (20)     1060 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/drawing/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)    13859 2023-05-31 14:06:48.000000 discopy-1.1.3/discopy/drawing/grid.py
+-rw-r--r--   0 boldi      (502) staff       (20)    36817 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/drawing/legacy.py
+-rw-r--r--   0 boldi      (502) staff       (20)    11666 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/frobenius.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.863470 discopy-1.1.3/discopy/grammar/
+-rw-r--r--   0 boldi      (502) staff       (20)      225 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/grammar/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)     9422 2023-05-31 13:42:02.000000 discopy-1.1.3/discopy/grammar/categorial.py
+-rw-r--r--   0 boldi      (502) staff       (20)     6950 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/grammar/cfg.py
+-rw-r--r--   0 boldi      (502) staff       (20)      926 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/grammar/dependency.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7191 2023-05-31 14:01:32.000000 discopy-1.1.3/discopy/grammar/pregroup.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2424 2023-05-31 14:01:45.000000 discopy-1.1.3/discopy/grammar/thue.py
+-rw-r--r--   0 boldi      (502) staff       (20)    48238 2023-05-31 14:06:54.000000 discopy-1.1.3/discopy/hypergraph.py
+-rw-r--r--   0 boldi      (502) staff       (20)    14080 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/interaction.py
+-rw-r--r--   0 boldi      (502) staff       (20)     8157 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/markov.py
+-rw-r--r--   0 boldi      (502) staff       (20)    16209 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/matrix.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1555 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/messages.py
+-rw-r--r--   0 boldi      (502) staff       (20)    35290 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/monoidal.py
+-rw-r--r--   0 boldi      (502) staff       (20)     6871 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/pivotal.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7845 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/python.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.865940 discopy-1.1.3/discopy/quantum/
+-rw-r--r--   0 boldi      (502) staff       (20)      667 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/__init__.py
+-rw-r--r--   0 boldi      (502) staff       (20)     5238 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/ansatze.py
+-rw-r--r--   0 boldi      (502) staff       (20)    11626 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/channel.py
+-rw-r--r--   0 boldi      (502) staff       (20)    32776 2023-06-01 12:28:37.000000 discopy-1.1.3/discopy/quantum/circuit.py
+-rw-r--r--   0 boldi      (502) staff       (20)    24616 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/quantum/gates.py
+-rw-r--r--   0 boldi      (502) staff       (20)    15811 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/quantum/pennylane.py
+-rw-r--r--   0 boldi      (502) staff       (20)    16429 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/tk.py
+-rw-r--r--   0 boldi      (502) staff       (20)    13451 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/quantum/zx.py
+-rw-r--r--   0 boldi      (502) staff       (20)     6916 2023-05-31 09:22:59.000000 discopy-1.1.3/discopy/ribbon.py
+-rw-r--r--   0 boldi      (502) staff       (20)    25755 2023-06-01 10:54:48.000000 discopy-1.1.3/discopy/rigid.py
+-rw-r--r--   0 boldi      (502) staff       (20)     9969 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/symmetric.py
+-rw-r--r--   0 boldi      (502) staff       (20)    23157 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/tensor.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7706 2023-06-01 18:42:50.000000 discopy-1.1.3/discopy/traced.py
+-rw-r--r--   0 boldi      (502) staff       (20)    20763 2023-05-31 13:26:18.000000 discopy-1.1.3/discopy/utils.py
+-rw-r--r--   0 boldi      (502) staff       (20)      160 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy/version.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.861031 discopy-1.1.3/discopy.egg-info/
+-rw-r--r--   0 boldi      (502) staff       (20)     7385 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/PKG-INFO
+-rw-r--r--   0 boldi      (502) staff       (20)     6574 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/SOURCES.txt
+-rw-r--r--   0 boldi      (502) staff       (20)        1 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/dependency_links.txt
+-rw-r--r--   0 boldi      (502) staff       (20)      417 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/requires.txt
+-rw-r--r--   0 boldi      (502) staff       (20)        8 2023-06-01 18:45:51.000000 discopy-1.1.3/discopy.egg-info/top_level.txt
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.867089 discopy-1.1.3/docs/
+-rw-r--r--   0 boldi      (502) staff       (20)      634 2022-09-27 14:39:16.000000 discopy-1.1.3/docs/Makefile
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.867616 discopy-1.1.3/docs/_ext/
+-rw-r--r--   0 boldi      (502) staff       (20)      684 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_ext/bases-fullname.py
+-rw-r--r--   0 boldi      (502) staff       (20)     3939 2022-12-13 17:02:09.000000 discopy-1.1.3/docs/_ext/youtube.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.868799 discopy-1.1.3/docs/_static/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.870849 discopy-1.1.3/docs/_static/balanced/
+-rw-r--r--   0 boldi      (502) staff       (20)    14901 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/balanced/ribbon_twist.png
+-rw-r--r--   0 boldi      (502) staff       (20)    13367 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/balanced/twist.png
+-rw-r--r--   0 boldi      (502) staff       (20)    11712 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/balanced/twist_dual_rail.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.871142 discopy-1.1.3/docs/_static/braided/
+-rw-r--r--   0 boldi      (502) staff       (20)     8951 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/braided/hexagons.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9432 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/braided/inverse.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.871621 discopy-1.1.3/docs/_static/closed/
+-rw-r--r--   0 boldi      (502) staff       (20)    15711 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/closed/curry-left.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15643 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/closed/curry-right.png
+-rw-r--r--   0 boldi      (502) staff       (20)    19051 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/closed/uncurry.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.872535 discopy-1.1.3/docs/_static/compact/
+-rw-r--r--   0 boldi      (502) staff       (20)    14358 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/compact/reidemeister.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10190 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/compact/snake.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14358 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/compact/yanking.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14061 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/compact/yanking_cup_and_cap.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.873083 discopy-1.1.3/docs/_static/drawing/
+-rw-r--r--   0 boldi      (502) staff       (20)     5271 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/drawing/diagramize.png
+-rw-r--r--   0 boldi      (502) staff       (20)     3578 2023-06-01 16:57:36.000000 discopy-1.1.3/docs/_static/drawing/example.html
+-rw-r--r--   0 boldi      (502) staff       (20)    10626 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/drawing/frobenius-axioms.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.873664 discopy-1.1.3/docs/_static/frobenius/
+-rw-r--r--   0 boldi      (502) staff       (20)    17147 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/comonoid.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14853 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/frobenius.png
+-rw-r--r--   0 boldi      (502) staff       (20)    17266 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/monoid.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9884 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/frobenius/special.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.873973 discopy-1.1.3/docs/_static/grammar/
+-rw-r--r--   0 boldi      (502) staff       (20)     9591 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/grammar/cfg-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7224 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/grammar/pregroup-example.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.874624 discopy-1.1.3/docs/_static/hypergraph/
+-rw-r--r--   0 boldi      (502) staff       (20)    16894 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/hypergraph/box.png
+-rw-r--r--   0 boldi      (502) staff       (20)    20670 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/hypergraph/diagram.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15394 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/hypergraph/unfuse.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.876078 discopy-1.1.3/docs/_static/int/
+-rw-r--r--   0 boldi      (502) staff       (20)    16145 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/alice-loves-bob.png
+-rw-r--r--   0 boldi      (502) staff       (20)    18363 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/braid.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16332 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/composition.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8274 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/dagger.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16257 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/idl.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16615 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/idr.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16069 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/int-snake-equations.png
+-rw-r--r--   0 boldi      (502) staff       (20)    22712 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/simplify.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16278 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/int/tensor.png
+-rw-r--r--   0 boldi      (502) staff       (20)   105662 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/logo.ico
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.876767 discopy-1.1.3/docs/_static/markov/
+-rw-r--r--   0 boldi      (502) staff       (20)    13158 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/markov/associativity.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14407 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/markov/bialgebra.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10317 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/markov/copy_and_apply.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8979 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/markov/counit.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.879394 discopy-1.1.3/docs/_static/monoidal/
+-rw-r--r--   0 boldi      (502) staff       (20)     2875 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/Eckmann-Hilton.gif
+-rw-r--r--   0 boldi      (502) staff       (20)    12008 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/EckmannHilton.gif
+-rw-r--r--   0 boldi      (502) staff       (20)     3504 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/arrow-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2166 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/box-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    14662 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/bubble-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10047 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-1.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7535 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-1a.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7221 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-1b.png
+-rw-r--r--   0 boldi      (502) staff       (20)     4433 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/foliate-example-2.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7089 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/functor-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2617 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/id-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)   404531 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/monoidal/spiral.gif
+-rw-r--r--   0 boldi      (502) staff       (20)     2888 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/monoidal/tensor-example.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.879771 discopy-1.1.3/docs/_static/optics/
+-rw-r--r--   0 boldi      (502) staff       (20)     7259 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/optics/fusion.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15302 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/optics/spider-decomp.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.880838 discopy-1.1.3/docs/_static/pivotal/
+-rw-r--r--   0 boldi      (502) staff       (20)    10105 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/axiom.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6542 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/box-conjugate.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7722 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/conjugate.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6710 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/dagger-transpose.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8451 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/pivotal/dagger.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10350 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/pivotal/trace.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.881216 discopy-1.1.3/docs/_static/quantum/
+-rw-r--r--   0 boldi      (502) staff       (20)    13104 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/quantum/circuit-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    17758 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/quantum/functor-example.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.881535 discopy-1.1.3/docs/_static/ribbon/
+-rw-r--r--   0 boldi      (502) staff       (20)     6787 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/ribbon/strict.png
+-rw-r--r--   0 boldi      (502) staff       (20)    15078 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/ribbon/twist-untwist.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.883087 discopy-1.1.3/docs/_static/rigid/
+-rw-r--r--   0 boldi      (502) staff       (20)     2296 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/cap.png
+-rw-r--r--   0 boldi      (502) staff       (20)     3223 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/caps.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2352 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/cup.png
+-rw-r--r--   0 boldi      (502) staff       (20)     3131 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/cups.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8834 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/curry.png
+-rw-r--r--   0 boldi      (502) staff       (20)     4537 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/diagram-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10267 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/functor-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    11845 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/rotate.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9160 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/transpose.png
+-rw-r--r--   0 boldi      (502) staff       (20)    13976 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/transpose_box.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/rigid/typed-snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)   963196 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/spiral.gif
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.883800 discopy-1.1.3/docs/_static/symmetric/
+-rw-r--r--   0 boldi      (502) staff       (20)    13136 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/decorator.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9819 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/hexagons.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6665 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/inverse.png
+-rw-r--r--   0 boldi      (502) staff       (20)     7307 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/naturality.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10124 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/symmetric/yang-baxter.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.884570 discopy-1.1.3/docs/_static/tensor/
+-rw-r--r--   0 boldi      (502) staff       (20)    17466 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/chain-rule.png
+-rw-r--r--   0 boldi      (502) staff       (20)     4810 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/frobenius-example.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10998 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/men-are-mortal.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9312 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/product-rule.png
+-rw-r--r--   0 boldi      (502) staff       (20)    13435 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/tensor/rewrite.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.885914 discopy-1.1.3/docs/_static/traced/
+-rw-r--r--   0 boldi      (502) staff       (20)    10121 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/golden.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10550 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_static/traced/right-nat-trace.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9691 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/sliding-left.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9887 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/sliding-right.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10411 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/tightening-left.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10550 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/tightening-right.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10247 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/trace.png
+-rw-r--r--   0 boldi      (502) staff       (20)    12964 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/_static/traced/yanking.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.886065 discopy-1.1.3/docs/_style/
+-rw-r--r--   0 boldi      (502) staff       (20)     1811 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_style/custom.css
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.886661 discopy-1.1.3/docs/_templates/
+-rw-r--r--   0 boldi      (502) staff       (20)      185 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_templates/class.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      100 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_templates/function.rst
+-rw-r--r--   0 boldi      (502) staff       (20)       66 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/_templates/module.rst
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.888071 discopy-1.1.3/docs/api/
+-rw-r--r--   0 boldi      (502) staff       (20)     4581 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/architecture.html
+-rw-r--r--   0 boldi      (502) staff       (20)    56460 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/architecture.png
+-rw-r--r--   0 boldi      (502) staff       (20)      168 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/drawing.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      256 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/grammar.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      302 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/quantum.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      222 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/semantics.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      458 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/api/syntax.rst
+-rw-r--r--   0 boldi      (502) staff       (20)     3037 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/conf.py
+-rw-r--r--   0 boldi      (502) staff       (20)    13274 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/discopy.bib
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.888892 discopy-1.1.3/docs/extra/
+-rw-r--r--   0 boldi      (502) staff       (20)       57 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/bibliography.rst
+-rw-r--r--   0 boldi      (502) staff       (20)     1059 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/blogs.md
+-rw-r--r--   0 boldi      (502) staff       (20)     6077 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/papers.md
+-rw-r--r--   0 boldi      (502) staff       (20)     1492 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/extra/talks.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      780 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/index.rst
+-rw-r--r--   0 boldi      (502) staff       (20)      795 2022-09-27 14:39:16.000000 discopy-1.1.3/docs/make.bat
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.894522 discopy-1.1.3/docs/notebooks/
+-rw-r--r--   0 boldi      (502) staff       (20)   483325 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/21-05-03-tallcat.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)  1593241 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/21-05-05-tallcat.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)    42815 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/diag-diff.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)   179435 2023-05-31 09:22:59.000000 discopy-1.1.3/docs/notebooks/diagrams.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)   185975 2023-06-01 18:43:01.000000 discopy-1.1.3/docs/notebooks/qnlp.ipynb
+-rw-r--r--   0 boldi      (502) staff       (20)     2203 2023-06-01 11:23:16.000000 discopy-1.1.3/pyproject.toml
+-rw-r--r--   0 boldi      (502) staff       (20)       38 2023-06-01 18:45:51.908779 discopy-1.1.3/setup.cfg
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.851771 discopy-1.1.3/test/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.894795 discopy-1.1.3/test/drawing/
+-rw-r--r--   0 boldi      (502) staff       (20)     5573 2023-05-31 13:42:21.000000 discopy-1.1.3/test/drawing/legacy.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.896447 discopy-1.1.3/test/grammar/
+-rw-r--r--   0 boldi      (502) staff       (20)     7785 2023-05-31 13:57:44.000000 discopy-1.1.3/test/grammar/categorial.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2049 2023-05-31 09:22:59.000000 discopy-1.1.3/test/grammar/pregroup.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.898211 discopy-1.1.3/test/quantum/
+-rw-r--r--   0 boldi      (502) staff       (20)      425 2023-05-31 09:22:59.000000 discopy-1.1.3/test/quantum/ansatze.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1553 2023-05-31 13:42:16.000000 discopy-1.1.3/test/quantum/channel.py
+-rw-r--r--   0 boldi      (502) staff       (20)    25072 2023-05-31 13:59:33.000000 discopy-1.1.3/test/quantum/circuit.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2510 2023-05-31 09:22:59.000000 discopy-1.1.3/test/quantum/eval.py
+-rw-r--r--   0 boldi      (502) staff       (20)     4335 2023-06-01 10:54:48.000000 discopy-1.1.3/test/quantum/tk.py
+-rw-r--r--   0 boldi      (502) staff       (20)     5804 2023-05-31 09:22:59.000000 discopy-1.1.3/test/quantum/zx.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.899100 discopy-1.1.3/test/semantics/
+-rw-r--r--   0 boldi      (502) staff       (20)     1203 2023-05-31 13:41:31.000000 discopy-1.1.3/test/semantics/matrix.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1304 2023-05-31 09:22:59.000000 discopy-1.1.3/test/semantics/python.py
+-rw-r--r--   0 boldi      (502) staff       (20)     8107 2023-05-31 13:41:42.000000 discopy-1.1.3/test/semantics/tensor.py
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.899716 discopy-1.1.3/test/src/
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.902144 discopy-1.1.3/test/src/imgs/
+-rw-r--r--   0 boldi      (502) staff       (20)    12008 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/EckmannHilton.gif
+-rw-r--r--   0 boldi      (502) staff       (20)     7553 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/bell-state.png
+-rw-r--r--   0 boldi      (502) staff       (20)    16964 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/bialgebra.png
+-rw-r--r--   0 boldi      (502) staff       (20)    25004 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/crack-eggs.png
+-rw-r--r--   0 boldi      (502) staff       (20)     2411 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/empty_diagram.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5907 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/long-controlled.png
+-rw-r--r--   0 boldi      (502) staff       (20)     8810 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/sentence-as-diagram.png
+-rw-r--r--   0 boldi      (502) staff       (20)     5315 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)    10800 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/spiral.png
+-rw-r--r--   0 boldi      (502) staff       (20)     6051 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/typed-snake-equation.png
+-rw-r--r--   0 boldi      (502) staff       (20)     9525 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/imgs/who-ansatz.png
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.904465 discopy-1.1.3/test/src/tikz/
+-rw-r--r--   0 boldi      (502) staff       (20)     2228 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bell-state.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)      153 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bell-state.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     4906 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bialgebra.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)      150 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/bialgebra.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     2441 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/copy.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)       86 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/copy.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     3441 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/crack-eggs.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)     3338 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/long-controlled.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)     2223 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/snake-equation.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)     1906 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/spiral.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)      260 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/spiral.tikzstyles
+-rw-r--r--   0 boldi      (502) staff       (20)     3435 2023-05-31 09:22:59.000000 discopy-1.1.3/test/src/tikz/who-ansatz.tikz
+-rw-r--r--   0 boldi      (502) staff       (20)    15562 2022-09-27 14:39:16.000000 discopy-1.1.3/test/src/tree2diagram.pickle
+-rw-r--r--   0 boldi      (502) staff       (20)     6324 2022-09-27 14:39:16.000000 discopy-1.1.3/test/src/zx-graph.json
+drwxr-xr-x   0 boldi      (502) staff       (20)        0 2023-06-01 18:45:51.908131 discopy-1.1.3/test/syntax/
+-rw-r--r--   0 boldi      (502) staff       (20)      258 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/balanced.py
+-rw-r--r--   0 boldi      (502) staff       (20)      487 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/braided.py
+-rw-r--r--   0 boldi      (502) staff       (20)     7687 2023-05-31 13:45:46.000000 discopy-1.1.3/test/syntax/cat.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1413 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/closed.py
+-rw-r--r--   0 boldi      (502) staff       (20)      828 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/compact.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1750 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/frobenius.py
+-rw-r--r--   0 boldi      (502) staff       (20)     2044 2023-06-01 18:42:50.000000 discopy-1.1.3/test/syntax/hypergraph.py
+-rw-r--r--   0 boldi      (502) staff       (20)      659 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/interaction.py
+-rw-r--r--   0 boldi      (502) staff       (20)     1532 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/markov.py
+-rw-r--r--   0 boldi      (502) staff       (20)    10196 2023-05-31 13:50:28.000000 discopy-1.1.3/test/syntax/monoidal.py
+-rw-r--r--   0 boldi      (502) staff       (20)      178 2023-05-31 13:40:18.000000 discopy-1.1.3/test/syntax/pivotal.py
+-rw-r--r--   0 boldi      (502) staff       (20)      553 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/ribbon.py
+-rw-r--r--   0 boldi      (502) staff       (20)     3278 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/rigid.py
+-rw-r--r--   0 boldi      (502) staff       (20)      962 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/symmetric.py
+-rw-r--r--   0 boldi      (502) staff       (20)      391 2023-05-31 13:58:46.000000 discopy-1.1.3/test/syntax/traced.py
+-rw-r--r--   0 boldi      (502) staff       (20)      953 2023-05-31 09:22:59.000000 discopy-1.1.3/test/syntax/utils.py
```

### Comparing `discopy-1.1.2/.github/workflows/build_test.yml` & `discopy-1.1.3/.github/workflows/build_test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -21,41 +21,44 @@
     - uses: actions/checkout@v3
     - name: Setup Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install linter
       run:
-        python -m pip install pycodestyle coverage pylint
+        python -m pip install pyproject-flake8 coverage pylint
     - name: Check for errors
       run:
         # stop the build if there are Python syntax errors or undefined names
-        pycodestyle discopy
+        pflake8 discopy
     - name: pylint
       run:
         pylint discopy
   build_and_test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [ 3.9 ]
     steps:
     - uses: actions/checkout@v3
     - name: Setup Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        cache: 'pip'  # caching pip dependencies
     - name: Install base package
-      run: python -m pip install .[test]
+      run: |
+        pip install torch --index-url https://download.pytorch.org/whl/cpu  # Install PyTorch without CUDA
+        pip install .[test]
     - name: Install coverage and pytest
       run:
-        python -m pip install coverage pytest
+        pip install coverage pytest
     - name: Test with pytest
       run:
-        coverage run --source=${{ env.SRC_DIR }} -m pytest ${{ env.SRC_DIR }} ${{ env.TEST_DIR }} --doctest-modules
+        coverage run --source=${{ env.SRC_DIR }} -m pytest --doctest-modules
     - name: Coverage report
       run:
         coverage report --fail-under=99 --show-missing
     - name: Install nbmake and test notebooks
       run: |
         python -m pip install nbmake
         pytest --nbmake ${{ env.DOCS_DIR }}/notebooks/*.ipynb
```

### Comparing `discopy-1.1.2/.pylintrc` & `discopy-1.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/.readthedocs.yaml` & `discopy-1.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/CONTRIBUTING.md` & `discopy-1.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/LICENSE` & `discopy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/PKG-INFO` & `discopy-1.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: discopy
-Version: 1.1.2
-Summary: The Python toolkit for computing with string diagrams.
-Home-page: https://discopy.org
-Download-URL: https://pypi.org/project/discopy
-Author: DisCoPy
-Author-email: contact@discopy.org
-License: BSD 3
-Project-URL: Documentation, https://docs.discopy.org
-Project-URL: Source Code, https://github.com/discopy/discopy
-Project-URL: Issue Tracker, https://github.com/discopy/discopy/issues
-Keywords: category theory,string diagrams,natural language processing,quantum computing
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-
 
 ![snake equation](https://github.com/discopy/discopy/raw/main/docs/_static/snake-equation.png)
 
 # DisCoPy
 
 [![build](https://github.com/discopy/discopy/actions/workflows/build_test.yml/badge.svg)](https://github.com/discopy/discopy/actions/workflows/build_test.yml)
 [![readthedocs](https://readthedocs.org/projects/discopy/badge/?version=main)](https://docs.discopy.org/)
```

### Comparing `discopy-1.1.2/discopy/balanced.py` & `discopy-1.1.3/discopy/balanced.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 .. image:: /_static/balanced/twist.png
 """
 
 from __future__ import annotations
 
 from discopy import monoidal, braided, traced
 from discopy.cat import factory
-from discopy.monoidal import Ty, assert_isatomic
-from discopy.utils import factory_name
+from discopy.monoidal import Ty
+from discopy.utils import factory_name, assert_isatomic
 
 
 @factory
 class Diagram(braided.Diagram, traced.Diagram):
     """
     A balanced diagram is a braided diagram with :class:`Twist`.
```

### Comparing `discopy-1.1.2/discopy/braided.py` & `discopy-1.1.3/discopy/braided.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
 from discopy import monoidal
-from discopy.cat import factory, AxiomError
-from discopy.monoidal import Ty, assert_isatomic, Match
-from discopy.utils import factory_name, from_tree, BinaryBoxConstructor
+from discopy.cat import factory
+from discopy.monoidal import Ty, Match
+from discopy.utils import factory_name, BinaryBoxConstructor, assert_isatomic
 
 
 @factory
 class Diagram(monoidal.Diagram):
     """
     A braided diagram is a monoidal diagram with :class:`Braid` boxes.
```

### Comparing `discopy-1.1.2/discopy/cat.py` & `discopy-1.1.3/discopy/cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,35 +73,36 @@
 Functors are bubble-preserving.
 
 >>> assert F(f.bubble()) == F(f).bubble()
 """
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from functools import total_ordering, cached_property
 from typing import (
-    Callable, Mapping, Iterable, Optional, TypeVar, Generic, Type)
+    Callable, Mapping, Iterable, Optional, Type, TYPE_CHECKING)
 
 from discopy import messages, utils
 from discopy.utils import (
     factory,
     factory_name,
     from_tree,
     rsubs,
     unbiased,
     MappingOrCallable,
     Composable,
-    AxiomError,
     assert_isinstance,
     assert_iscomposable,
     assert_isparallel,
 )
 
+if TYPE_CHECKING:
+    import sympy
+
 dumps, loads = utils.dumps, utils.loads
 
 
 @total_ordering
 class Ob:
     """
     An object with a string as :code:`name`.
@@ -298,15 +299,15 @@
         """
         Sequential composition, called with :code:`>>` and :code:`<<`.
 
         Parameters:
             others : The other arrows to compose.
 
         Raises:
-            cat.AxiomError : Whenever `self` and `others` do not compose.
+            AxiomError : Whenever `self` and `others` do not compose.
         """
         if any(isinstance(other, Sum) for other in others):
             return self.sum_factory((self, )).then(*others)
         inside, dom, cod = self.inside, self.dom, self.cod
         for other in others:
             assert_isinstance(other, self.factory)
             assert_isinstance(self, other.factory)
```

### Comparing `discopy-1.1.2/discopy/closed.py` & `discopy-1.1.3/discopy/closed.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 .. image:: /_static/closed/uncurry.png
     :align: center
 """
 
 from __future__ import annotations
 
-from discopy import cat, monoidal, messages
+from discopy import cat, monoidal
 from discopy.cat import Category, factory
 from discopy.utils import (
     factory_name,
     from_tree,
 )
```

### Comparing `discopy-1.1.2/discopy/compact.py` & `discopy-1.1.3/discopy/compact.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Category
     Functor
 
 Axioms
 ------
 
 >>> from discopy.drawing import Equation
+>>> Diagram.structure_preserving = True
 >>> x, y = Ty('x'), Ty('y')
 
 * Snake equations:
 
 >>> snake = Equation(Id(x.l).transpose(left=True), Id(x), Id(x.r).transpose())
 >>> assert snake
 >>> snake.draw(path="docs/_static/compact/snake.png")
@@ -54,19 +55,21 @@
 .. image:: /_static/compact/yanking_cup_and_cap.png
     :align: center
 
 * Coherence:
 
 >>> assert Diagram.caps(x @ y, y.r @ x.r)\\
 ...     == Cap(x, x.r) @ Cap(y, y.r) >> x @ Diagram.swap(x.r, y @ y.r)
+
+>>> Diagram.structure_preserving = False
 """
 
 from discopy import symmetric, ribbon
 from discopy.cat import factory
-from discopy.pivotal import Ob, Ty
+from discopy.pivotal import Ob, Ty  # noqa: F401
 
 
 @factory
 class Diagram(symmetric.Diagram, ribbon.Diagram):
     """
     A compact diagram is a symmetric diagram and a ribbon diagram.
```

### Comparing `discopy-1.1.2/discopy/config.py` & `discopy-1.1.3/discopy/config.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/drawing/__init__.py` & `discopy-1.1.3/discopy/drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/drawing/grid.py` & `discopy-1.1.3/discopy/drawing/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
+    from discopy import monoidal
     import lxml
 
 TABLE_STYLE = ".diagram .wire { border-left: 4px solid; text-align: left; } "\
               ".diagram .box { border: 4px solid; text-align: center; }"\
               ".diagram td { min-width: 20px; height: 20px; }"
 
 
@@ -38,30 +39,30 @@
     Parameters:
         start : The left of the cell.
         stop : The right of the cell.
         label : The label of the cell.
     """
     start: int
     stop: int
-    label: discopy.monoidal.Ty | discopy.monoidal.Box = None
+    label: monoidal.Ty | monoidal.Box = None
 
     def __add__(self, offset: int) -> Cell:
         return Cell(self.start + offset, self.stop + offset, self.label)
 
     def __sub__(self, offset: int) -> Cell:
         return self + (-offset)
 
     def __str__(self):
         return f"Cell({self.start}, {self.stop}, {self.label})"
 
 
 class Wire(Cell):
     """ A wire is a cell with ``stop = start``. """
 
-    def __init__(self, start: int, label: discopy.monoidal.Ty = None):
+    def __init__(self, start: int, label: monoidal.Ty = None):
         super().__init__(start, start, label)
 
     def __add__(self, offset: int) -> Wire:
         return Wire(self.start + offset, self.label)
 
     def __str__(self):
         return f"Wire({self.start}, {self.label})"
@@ -186,15 +187,14 @@
                 td.text = input_wires[0].label.name
                 input_wires = input_wires[1:]
         for i, row in list(enumerate(self.rows))[1:]:
             tr = SubElement(table, "tr")
             if row and row[0].start > 0:
                 td = SubElement(tr, "td")
                 td.set("colspan", str(row[0].start))
-            offset = 0
             for cell, next_cell in zip(row, row[1:] + [None]):
                 if cell.start == cell.stop:
                     td = SubElement(tr, "td")
                     td.set("class", "wire")
                     td.set("colspan", str(
                         width - cell.stop if next_cell is None
                         else next_cell.start - cell.stop))
@@ -206,15 +206,14 @@
                     td.set("colspan", str(cell.stop - cell.start))
                     td.text = cell.label.name
                     if cell.stop < width:
                         td = SubElement(tr, "td")
                         td.set("colspan", str(
                             width - cell.stop if next_cell is None
                             else next_cell.start - cell.stop))
-                    offset = cell.stop
         return ElementTree(root)
 
     def to_ascii(self, _debug=False) -> str:
         """
         Turn a grid into an ascii drawing.
 
         Examples
@@ -267,15 +266,15 @@
                     result += space + str(
                         cell.label.name)[:width].center(width, box_chr)
             return result
 
         return '\n'.join(map(row_to_ascii, self.rows)).strip('\n')
 
     @staticmethod
-    def from_diagram(diagram: discopy.monoidal.Diagram) -> Grid:
+    def from_diagram(diagram: monoidal.Diagram) -> Grid:
         """
         Layout a diagram on a grid.
 
         The first row is a list of :class:`Wire` cells, then for each layer of
         the diagram there are two rows: the first for the boxes and the wires
         in between them, the second is a list of :class:`Wire` for the outputs.
```

### Comparing `discopy-1.1.2/discopy/drawing/legacy.py` & `discopy-1.1.3/discopy/drawing/legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,24 +29,28 @@
 from __future__ import annotations
 
 import os
 from abc import ABC, abstractmethod
 from math import sqrt
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 
+from typing import TYPE_CHECKING
+
 import matplotlib.pyplot as plt
 from PIL import Image
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
 
-from discopy.utils import assert_isinstance
-from discopy.config import (
+from discopy.config import (  # noqa: F401
     DRAWING_ATTRIBUTES as ATTRIBUTES,
     DRAWING_DEFAULT as DEFAULT, COLORS, SHAPES)
 
+if TYPE_CHECKING:
+    from discopy import monoidal
+
 
 class Node:
     """ Node in a :class:`networkx.Graph`, can hold arbitrary data. """
     def __init__(self, kind, **data):
         self.kind, self.data = kind, data
         for key, value in data.items():
             setattr(self, key, value)
@@ -705,15 +709,15 @@
     >>> Equation(special, frobenius, symbol=', ').draw(
     ...          aspect='equal', draw_type_labels=False, figsize=(8, 2),
     ...          path='docs/_static/drawing/frobenius-axioms.png')
 
     .. image:: /_static/drawing/frobenius-axioms.png
         :align: center
     """
-    def __init__(self, *terms: discopy.monoidal.Diagram, symbol="=", space=1):
+    def __init__(self, *terms: monoidal.Diagram, symbol="=", space=1):
         self.terms, self.symbol, self.space = terms, symbol, space
 
     def __repr__(self):
         return f"Equation({', '.join(map(repr, self.terms))})"
 
     def __str__(self):
         return f" {self.symbol} ".join(map(str, self.terms))
```

### Comparing `discopy-1.1.2/discopy/frobenius.py` & `discopy-1.1.3/discopy/frobenius.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Category
     Functor
 
 Axioms
 ------
 
 >>> from discopy.drawing import Equation
-
+>>> Diagram.structure_preserving = True
 >>> x, y, z = map(Ty, "xyz")
 
 >>> split, merge = Spider(1, 2, x), Spider(2, 1, x)
 >>> unit, counit = Spider(0, 1, x), Spider(1, 0, x)
 
 * Frobenius:
 
@@ -48,26 +48,27 @@
 
 * Speciality:
 
 >>> special = Equation(split >> merge, Spider(1, 1, x), Id(x))
 >>> assert special
 >>> special.draw(path="docs/_static/frobenius/special.png")
 
+>>> Diagram.structure_preserving = False
+
 .. image:: /_static/frobenius/special.png
     :align: center
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
 from discopy import markov, compact, pivotal, hypergraph
 from discopy.cat import factory
-from discopy.monoidal import assert_isatomic
-from discopy.utils import factory_name, assert_isinstance
+from discopy.utils import factory_name, assert_isinstance, assert_isatomic
 
 
 class Ob(pivotal.Ob):
     """
     A frobenius object is a self-dual pivotal object.
 
     Parameters:
```

### Comparing `discopy-1.1.2/discopy/grammar/categorial.py` & `discopy-1.1.3/discopy/grammar/categorial.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,24 @@
         cat2ty
         tree2diagram
 """
 
 import re
 
 from discopy import closed, messages
-from discopy.cat import factory, AxiomError
+from discopy.cat import factory
 from discopy.grammar import thue
 from discopy.closed import Ty, Over, Under
 from discopy.utils import (
-    assert_isinstance, factory_name, from_tree, BinaryBoxConstructor)
+    assert_isinstance,
+    factory_name,
+    from_tree,
+    BinaryBoxConstructor,
+    AxiomError
+)
 
 
 @factory
 class Diagram(closed.Diagram):
     """
     A categorial diagram is a closed diagram with rules and words as boxes.
     """
```

### Comparing `discopy-1.1.2/discopy/grammar/cfg.py` & `discopy-1.1.3/discopy/grammar/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,25 @@
 >>> left = f(Id(x), h)(g, Id(x), Id(x))
 >>> right = f(g, Id(x))(Id(x), Id(x), h)
 >>> assert f(g, h) == left == right
 """
 
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 from discopy import monoidal
-from discopy.cat import factory, Category, Functor, AxiomError
+from discopy.cat import factory, Category, Functor
 from discopy.grammar import thue
-from discopy.monoidal import Ty, assert_isatomic
-from discopy.utils import assert_isinstance, factory_name
+from discopy.monoidal import Ty
+from discopy.utils import (
+    assert_isinstance, factory_name, assert_isatomic, AxiomError)
+
+if TYPE_CHECKING:
+    import nltk
 
 
 @factory
 class Tree:
     """
     A tree is a rule for the ``root`` and a list of trees called ``branches``.
 
@@ -100,15 +106,15 @@
     @staticmethod
     def id(dom):
         return Id(dom)
 
     def __eq__(self, other):
         return self.root == other.root and self.branches == other.branches
 
-    def to_diagram(self, contravariant=False) -> discopy.monoidal.Diagram:
+    def to_diagram(self, contravariant=False) -> monoidal.Diagram:
         """
         Interface between Tree and monoidal.Diagram.
 
         >>> x = Ty('x')
         >>> f = Rule(x @ x, x, name='f')
         >>> tree = f(f(f, f), f)
         >>> print(tree.to_diagram().foliation())
@@ -155,15 +161,15 @@
     def __eq__(self, other):
         if isinstance(other, Rule):
             return self.dom == other.dom and self.cod == other.cod \
                 and self.name == other.name
         if isinstance(other, Tree):
             return other.root == self and other.branches == []
 
-    def to_diagram(self) -> discopy.monoidal.Box:
+    def to_diagram(self) -> monoidal.Box:
         return monoidal.Box(self.name, self.dom, self.cod)
 
 
 class Word(thue.Word, Rule):
     """
     A word is a leaf in a context-free tree.
```

### Comparing `discopy-1.1.2/discopy/grammar/dependency.py` & `discopy-1.1.3/discopy/grammar/dependency.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/grammar/pregroup.py` & `discopy-1.1.3/discopy/grammar/pregroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,19 @@
         :nosignatures:
         :toctree:
 
         eager_parse
         brute_force
 """
 
-from discopy import messages, rigid, frobenius, messages
-from discopy.cat import factory, AxiomError
+from discopy import rigid, frobenius, messages
+from discopy.cat import factory
+from discopy.utils import AxiomError
 from discopy.grammar import thue
-from discopy.rigid import Ob
+from discopy.rigid import Ob  # noqa: F401
 
 
 @factory
 class Ty(rigid.Ty):
     """
     A pregroup type is a rigid type.
```

### Comparing `discopy-1.1.2/discopy/grammar/thue.py` & `discopy-1.1.3/discopy/grammar/thue.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 >>> sentence = Jane @ loves @ John >> n @ r1 >> r0
 >>> sentence.draw(figsize=(4, 3), path='docs/_static/grammar/cfg-example.png')
 
 .. image:: /_static/grammar/cfg-example.png
     :align: center
 """
 from discopy import monoidal
-from discopy.monoidal import Ty
+from discopy.monoidal import Ty  # noqa: F401
 from discopy.utils import factory_name
 
 
 class Rule(monoidal.Box):
     """
     A rule is a box with monoidal types as ``dom`` and ``cod`` and an
     optional ``name``.
```

### Comparing `discopy-1.1.2/discopy/hypergraph.py` & `discopy-1.1.3/discopy/hypergraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,18 @@
     spring_layout,
     draw_networkx,
     dag_longest_path_length,
     weisfeiler_lehman_graph_hash,
 )
 from networkx.algorithms.isomorphism import is_isomorphic
 
-from discopy import drawing, messages
+from discopy import messages
 from discopy.cat import Category
 from discopy.drawing import Node
 from discopy.utils import (
-    factory,
     factory_name,
     assert_isinstance,
     pushout,
     unbiased,
     NamedGeneric,
     AxiomError,
     Composable,
@@ -777,15 +776,14 @@
         >>> from discopy.frobenius import Ty, Box, Hypergraph as H, Spider
         >>> h = H.spiders(2, 3, Ty('x')).make_polygynous()
         >>> assert h.boxes == (Spider(2, 1, Ty('x')), )
         >>> assert h.wires == (0, 1) + (0, 1, 2) + (2, 2, 2)
         """
         for spider, (typ, (input_wires, output_wires)) in enumerate(
                 zip(self.spider_types, self.spider_wires)):
-            n_legs = len(input_wires) + len(output_wires)
             if len(input_wires) == 1:
                 continue
             depth = getattr(self.ports[max(input_wires)], "depth", -1) + 1\
                 if input_wires else 0
             boxes = self.boxes[:depth] + (self.category.ar.spider_factory(
                 len(input_wires), 1, typ), ) + self.boxes[depth:]
             offsets = self.offsets[:depth] + (None, ) + self.offsets[depth:]
```

### Comparing `discopy-1.1.2/discopy/interaction.py` & `discopy-1.1.3/discopy/interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,21 @@
 """
 
 from __future__ import annotations
 from dataclasses import dataclass
 from functools import wraps
 
 from discopy import (
-    balanced, traced, rigid, pivotal, ribbon, frobenius, messages)
+    balanced,
+    traced,
+    rigid,
+    pivotal,
+    ribbon,
+    messages
+)
 from discopy.cat import Composable, assert_iscomposable
 from discopy.monoidal import Whiskerable
 from discopy.utils import (
     NamedGeneric, unbiased, assert_isinstance, factory_name)
 
 
 @dataclass
@@ -368,14 +374,15 @@
 
     def simplify(self):
         """
         Simplify by going back and forth to :class:`Hypergraph`.
 
         Example
         -------
+        >>> from discopy import frobenius
         >>> x = Ty[frobenius.Ty]('x')
         >>> D = Diagram[frobenius.Diagram]
         >>> left_snake = D.id(-x).transpose(left=True)
         >>> right_snake = D.id(-x).transpose(left=False)
         >>> assert left_snake.simplify() == D.id(x) == right_snake.simplify()
 
         >>> from discopy.drawing import Equation
```

### Comparing `discopy-1.1.2/discopy/markov.py` & `discopy-1.1.3/discopy/markov.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Functor
 
 
 Axioms
 ------
 
 >>> from discopy.drawing import Equation
+>>> Diagram.structure_preserving = True
 >>> x = Ty('x')
 
 >>> copy, merge = Copy(x), Merge(x)
 >>> unit, delete = Merge(x, n=0), Copy(x, n=0)
 
 * Commutative monoid:
 
@@ -58,26 +59,29 @@
 >>> assert Diagram.copy(x @ x, n=0) == delete @ delete
 >>> assert Diagram.copy(x @ x)\\
 ...     == copy @ copy >> x @ Swap(x, x) @ x
 >>> assert Diagram.merge(x @ x, n=0) == unit @ unit
 >>> assert Diagram.merge(x @ x)\\
 ...     == x @ Swap(x, x) @ x >> merge @ merge
 
+>>> Diagram.structure_preserving = False
+
 Note
 ----
 Equality of Markov diagrams is computed by translation to hypergraph.
 Both copy and merge boxes are translated to spiders, thus when they appear
 in the same diagram they automatically satisfy the :mod:`frobenius` axioms.
 """
 
 from __future__ import annotations
 
 from discopy import symmetric, monoidal, hypergraph
 from discopy.cat import factory
-from discopy.monoidal import Ty, assert_isatomic
+from discopy.monoidal import Ty
+from discopy.utils import assert_isatomic
 
 
 @factory
 class Diagram(symmetric.Diagram):
     """
     A Markov diagram is a symmetric diagram with :class:`Copy` boxes.
```

### Comparing `discopy-1.1.2/discopy/matrix.py` & `discopy-1.1.3/discopy/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,27 +35,28 @@
 * :class:`Matrix` is used to evaluate :class:`quantum.optics.Diagram`.
 
 """
 from __future__ import annotations
 
 from contextlib import contextmanager
 from types import ModuleType
-from typing import Union, Literal as L
+from typing import Union, Literal as L, Callable, TYPE_CHECKING
 
-from discopy import cat, monoidal, config, messages
+from discopy import monoidal, config, messages
 from discopy.cat import (
     factory,
     Composable,
     assert_iscomposable,
     assert_isparallel,
 )
 from discopy.monoidal import Whiskerable
 from discopy.utils import assert_isinstance, unbiased, NamedGeneric
 
-import numpy as np
+if TYPE_CHECKING:
+    import sympy
 
 
 @factory
 class Matrix(Composable[int], Whiskerable, NamedGeneric['dtype']):
     """
     A matrix is an ``array`` with natural numbers as ``dom`` and ``cod``.
 
@@ -91,14 +92,15 @@
     >>> Matrix[complex].id(1)
     Matrix[complex]([1.+0.j], dom=1, cod=1)
     >>> assert Matrix[complex].id(1) != Matrix[float].id(1)
 
     The default data type is determined by underlying array datastructure of
     the backend used. An array is initialised with ``array`` as parameter and
     the dtype of the ``Matrix`` object is the data type of this array.
+    >>> import numpy as np
     >>> assert Matrix([1, 0], dom=1, cod=2).dtype == np.int64
     >>> assert Matrix([0.5, 0.5], dom=1, cod=2).dtype == np.float64
     >>> assert Matrix([0.5j], dom=1, cod=1).dtype == np.complex128
 
     The data type needs to have the structure of a rig (riNg with no negatives)
     i.e. with methods ``__add__`` and ``__mul__`` as well as an ``__init__``
     that can accept both ``0`` and ``1`` as input.
```

### Comparing `discopy-1.1.2/discopy/messages.py` & `discopy-1.1.3/discopy/messages.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/monoidal.py` & `discopy-1.1.3/discopy/monoidal.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,31 +49,33 @@
 .. image:: /_static/monoidal/EckmannHilton.gif
     :align: center
 """
 
 from __future__ import annotations
 
 import itertools
-from typing import Iterator, Callable
+from typing import Iterator, Callable, TYPE_CHECKING
 from dataclasses import dataclass
 from warnings import warn
 
 from discopy import cat, drawing, hypergraph, messages
-from discopy.cat import Ob, AxiomError
+from discopy.cat import Ob
 from discopy.utils import (
     factory,
     factory_name,
     from_tree,
     assert_isinstance,
     assert_iscomposable,
-    assert_isatomic,
-    Composable,
     Whiskerable,
+    AxiomError,
 )
 
+if TYPE_CHECKING:
+    import sympy
+
 
 @factory
 class Ty(cat.Ob):
     """
     A type is a tuple of objects with :meth:`Ty.tensor` as concatenation.
 
     Parameters:
@@ -324,14 +326,17 @@
 
     def __getitem__(self, key):
         return self.boxes_or_types[key]
 
     def __eq__(self, other):
         return isinstance(other, type(self)) and tuple(self) == tuple(other)
 
+    def __hash__(self):
+        return hash(tuple(self))
+
     def __repr__(self):
         return factory_name(type(self))\
             + f"({', '.join(map(repr, self))})"
 
     def __matmul__(self, other: Ty) -> Layer:
         *tail, head = self
         return type(self)(*tail + [head @ other])
@@ -414,15 +419,15 @@
                 (self, other), self.dom, other.cod).to_staircases())
         except NotImplementedError as exception:  # Eckmann-Hilton argument.
             diagram = exception.last_step
         boxes_or_types, offset = [self.dom[:0]], 0
         for layer in diagram.inside:
             left, box, right = layer
             if len(left) < offset:
-                raise cat.AxiomError(
+                raise AxiomError(
                     messages.NOT_MERGEABLE.format(self, other))
             boxes_or_types[-1] @= left[offset:]
             boxes_or_types += [box, right[:0]]
             offset = len(left @ box.cod)
         boxes_or_types[-1] @= layer.cod[offset:]
         return type(self)(*boxes_or_types)
 
@@ -675,15 +680,15 @@
                     self.inside, self.inside[1:])):
                 try:
                     inside = self.inside[:i] + (first.merge(second), )\
                         + self.inside[i + 2:]
                     self = self.factory(inside, self.dom, self.cod)
                     keep_on_going = True
                     break
-                except cat.AxiomError:
+                except AxiomError:
                     continue
             if not keep_on_going:
                 break
         return self
 
     def depth(self):
         """
```

### Comparing `discopy-1.1.2/discopy/pivotal.py` & `discopy-1.1.3/discopy/pivotal.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/python.py` & `discopy-1.1.3/discopy/python.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/quantum/__init__.py` & `discopy-1.1.3/discopy/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/quantum/ansatze.py` & `discopy-1.1.3/discopy/quantum/ansatze.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/quantum/channel.py` & `discopy-1.1.3/discopy/quantum/channel.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/quantum/circuit.py` & `discopy-1.1.3/discopy/quantum/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,17 +66,16 @@
 .. image:: /_static/quantum/functor-example.png
     :align: center
 """
 
 from __future__ import annotations
 
 from collections.abc import Mapping
-from math import pi
 
-from discopy import messages, rigid, tensor, frobenius
+from discopy import messages, tensor, frobenius
 from discopy.cat import factory, Category
 from discopy.matrix import backend
 from discopy.tensor import Dim, Tensor
 from discopy.utils import factory_name, assert_isinstance
 
 
 class Ob(frobenius.Ob):
@@ -287,15 +286,14 @@
                 return channel.Channel(array, f(self.dom), f(self.cod))
             f = tensor.Functor(
                 lambda x: x.inside[0].dim, {},
                 dtype=complex, dom=Category(Ty, Circuit))
             return Tensor[complex](array, f(self.dom), f(self.cod))
 
         from discopy.quantum import channel
-        from discopy.quantum.gates import Bits
         if backend is None:
             if others:
                 return [circuit.eval(mixed=mixed, **params)
                         for circuit in (self, ) + others]
             if mixed or self.is_mixed:
                 return channel.Functor(
                     {}, {}, dom=Category(Ty, Circuit), dtype=complex)(self)
@@ -672,14 +670,15 @@
 
         Returns
         -------
         circuit : `discopy.quantum.circuit.Sum`
 
         Examples
         --------
+        >>> from math import pi
         >>> from sympy.abc import phi
         >>> from discopy.quantum import *
         >>> circuit = Rz(phi / 2) @ Rz(phi + 1) >> CX
         >>> assert circuit.grad(phi, mixed=False)\\
         ...     == (scalar(pi/2) @ Rz(phi/2 + .5) @ Rz(phi + 1) >> CX)\\
         ...     + (Rz(phi / 2) @ scalar(pi) @ Rz(phi + 1.5) >> CX)
         """
```

### Comparing `discopy-1.1.2/discopy/quantum/gates.py` & `discopy-1.1.3/discopy/quantum/gates.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from math import e, pi
 
 from discopy import messages
 from discopy.cat import rsubs
 from discopy.matrix import get_backend
 from discopy.quantum.circuit import (
     Circuit, Digit, Ty, bit, qubit, Box, Swap, Sum, Id)
-from discopy.tensor import Dim, Tensor, backend
+from discopy.tensor import backend
 from discopy.utils import factory_name, assert_isinstance
 
 
 def format_number(data):
     """ Tries to format a number. """
     try:
         return f'{data:.3g}'
@@ -256,14 +256,15 @@
 
 class Digits(ClassicalGate):
     """
     Classical state for a given string of digits of a given dimension.
 
     Examples
     --------
+    >>> from discopy.tensor import Dim, Tensor
     >>> assert Digits(2, dim=4).eval()\\
     ...     == Tensor[complex](dom=Dim(1), cod=Dim(4), array=[0, 0, 1, 0])
     """
     draw_as_brakets = True
 
     def __init__(self, *digits, dim=None, is_dagger=False):
         if not isinstance(dim, int):
@@ -315,14 +316,15 @@
     return Digits(*bitstring, dim=2, is_dagger=is_dagger)
 
 
 class Ket(SelfConjugate, QuantumGate):
     """
     Implements qubit preparation for a given bitstring.
 
+    >>> from discopy.tensor import Dim, Tensor
     >>> assert Ket(1, 0).cod == qubit ** 2
     >>> assert Ket(1, 0).eval()\\
     ...     == Tensor[complex](dom=Dim(1), cod=Dim(2, 2), array=[0, 0, 1, 0])
     """
     to_drawing = Digits.to_drawing
     array = Digits.array
 
@@ -347,14 +349,15 @@
         return Id().tensor(*[Ket(b) for b in self.bitstring])
 
 
 class Bra(SelfConjugate, QuantumGate):
     """
     Implements qubit post-selection for a given bitstring.
 
+    >>> from discopy.tensor import Dim, Tensor
     >>> assert Bra(1, 0).dom == qubit ** 2
     >>> assert Bra(1, 0).eval()\\
     ...     == Tensor[complex](dom=Dim(2, 2), cod=Dim(1), array=[0, 0, 1, 0])
     """
     to_drawing = Digits.to_drawing
     array = Digits.array
```

### Comparing `discopy-1.1.2/discopy/quantum/pennylane.py` & `discopy-1.1.3/discopy/quantum/pennylane.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,24 +42,28 @@
 concrete parameters (i.e. no symbolic parameters), no arguments
 should be passed to `eval()`. If the circuit contains symbolic
 parameters, a list of the symbolic parameters and a list of their
 associated weights should be passed to `eval()` as `symbols=` and
 `weights=`.
 """
 
+from __future__ import annotations
+
 from itertools import product
-import numpy as np
 import pennylane as qml
 import sympy
 import torch
 from pytket import OpType
+from typing import TYPE_CHECKING
 
-from discopy.quantum import Circuit
 from discopy.quantum.gates import Scalar
 
+if TYPE_CHECKING:
+    from discopy.quantum import Circuit
+
 OP_MAP = {
     OpType.X: qml.PauliX,
     OpType.Y: qml.PauliY,
     OpType.Z: qml.PauliZ,
     OpType.S: qml.S,
     OpType.Sdg: lambda wires: qml.S(wires=wires).inv(),
     OpType.T: qml.T,
```

### Comparing `discopy-1.1.2/discopy/quantum/tk.py` & `discopy-1.1.3/discopy/quantum/tk.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/quantum/zx.py` & `discopy-1.1.3/discopy/quantum/zx.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/ribbon.py` & `discopy-1.1.3/discopy/ribbon.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/discopy/rigid.py` & `discopy-1.1.3/discopy/rigid.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,18 +40,25 @@
     :align: center
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
+from typing import Iterator
+
 from discopy import cat, monoidal, closed, messages
-from discopy.cat import AxiomError, factory
-from discopy.monoidal import assert_isatomic
-from discopy.utils import assert_isinstance, factory_name, BinaryBoxConstructor
+from discopy.cat import factory
+from discopy.utils import (
+    assert_isinstance,
+    factory_name,
+    BinaryBoxConstructor,
+    AxiomError,
+    assert_isatomic
+)
 
 
 class Ob(cat.Ob):
     """
     A rigid object has adjoints :meth:`Ob.l` and :meth:`Ob.r`.
 
     Parameters:
@@ -277,15 +284,14 @@
 
         .. image:: /_static/rigid/curry.png
             :align: center
         """
         if left:
             base, exponent = self.dom[:-n], self.dom[-n:]
             return base @ self.caps(exponent, exponent.l) >> self @ exponent.l
-        offset = len(self.dom) - n
         base, exponent = self.dom[n:], self.dom[:n]
         return self.caps(exponent.r, exponent) @ base >> exponent.r @ self
 
     def rotate(self, left=False):
         """
         The half-turn rotation of a diagram, called with ``.l`` and ``.r``.
```

### Comparing `discopy-1.1.2/discopy/symmetric.py` & `discopy-1.1.3/discopy/symmetric.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Category
     Functor
 
 Axioms
 ------
 
 >>> from discopy.drawing import Equation
+>>> Diagram.structure_preserving = True
 >>> x, y, z, w = map(Ty, "xyzw")
 >>> f, g = Box("f", x, y), Box("g", z, w)
 
 * Triangle:
 
 >>> assert Diagram.swap(Ty(), x) == Id(x) == Diagram.swap(x, Ty())
 
@@ -61,36 +62,55 @@
 
 >>> yang_baxter_left = Swap(x, y) @ z >> y @ Swap(x, z) >> Swap(y, z) @ x
 >>> yang_baxter_right = x @ Swap(y, z) >> Swap(x, z) @ y >> z @ Swap(x, y)
 >>> assert yang_baxter_left == yang_baxter_right
 >>> Equation(yang_baxter_left, yang_baxter_right).draw(
 ...     path='docs/_static/symmetric/yang-baxter.png', figsize=(3, 2))
 
+>>> Diagram.structure_preserving = False
+
 .. image:: /_static/symmetric/yang-baxter.png
     :align: center
 """
 
 from __future__ import annotations
 
-from discopy import monoidal, balanced, hypergraph, messages
+from discopy import monoidal, balanced, messages
 from discopy.cat import factory
-from discopy.monoidal import Ob, Ty, PRO
+from discopy.monoidal import Ob, Ty, PRO  # noqa: F401
 
 
 @factory
 class Diagram(balanced.Diagram):
     """
     A symmetric diagram is a balanced diagram with :class:`Swap` boxes.
 
     Parameters:
         inside(Layer) : The layers inside the diagram.
         dom (monoidal.Ty) : The domain of the diagram, i.e. its input.
         cod (monoidal.Ty) : The codomain of the diagram, i.e. its output.
 
     Note
+    ____
+    Symmetric diagrams have a class property `structure_preserving`, that
+    changes the behaviour of equality and hashing.
+    When set to `False`, two diagrams equal if they are built from the same
+    layers.
+    When set to `True`, the underlying hypergraphs are used for hashing and
+    equality checking.
+    The default value of `structure_preserving` is `False`.
+    >>> x, y = Ty("x"), Ty("y")
+    >>> id_hash = hash(Id(x @ y))
+    >>> assert Swap(x, y) >> Swap(y, x) != Id(x @ y)
+    >>> Diagram.structure_preserving = True
+    >>> assert Swap(x, y) >> Swap(y, x) == Id(x @ y)
+    >>> assert id_hash != hash(Id(x @ y))
+    >>> Diagram.structure_preserving = False
+
+    Note
     ----
     Symmetric diagrams can be defined using the standard syntax for functions.
 
     >>> x = Ty('x')
     >>> f = Box('f', x @ x, x)
     >>> g = Box('g', x, x @ x)
 
@@ -123,14 +143,15 @@
 
     Note
     ----
     As for :class:`discopy.balanced.Diagram`, our symmetric diagrams are traced
     by default. However now we have that the axioms for trace hold on the nose.
     """
     twist_factory = classmethod(lambda cls, dom: cls.id(dom))
+    structure_preserving = False
 
     @classmethod
     def swap(cls, left: monoidal.Ty, right: monoidal.Ty) -> Diagram:
         """
         The diagram that swaps the ``left`` and ``right`` wires.
 
         Parameters:
@@ -183,20 +204,24 @@
         functor = self.hypergraph_factory.functor
         return self.hypergraph_factory[category, functor].from_diagram(self)
 
     def simplify(self):
         """ Simplify by translating back and forth to hypergraph. """
         return self.to_hypergraph().to_diagram()
 
+    def _get_structure(self):
+        return self.to_hypergraph() if self.structure_preserving else (
+            self.inside, self.cod, self.dom)
+
     def __eq__(self, other):
         return isinstance(other, self.factory)\
-            and self.to_hypergraph() == other.to_hypergraph()
+            and self._get_structure() == other._get_structure()
 
     def __hash__(self):
-        return hash(self.to_hypergraph())
+        return hash(self._get_structure())
 
     def depth(self):
         """
         The depth of a symmetric diagram.
 
         Examples
         --------
```

### Comparing `discopy-1.1.2/discopy/tensor.py` & `discopy-1.1.3/discopy/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,28 @@
     Spider
     Sum
     Bubble
 """
 
 from __future__ import annotations
 
-from typing import Callable
+from typing import Callable, TYPE_CHECKING
 
 from discopy import (
     cat, monoidal, rigid, symmetric, frobenius)
 from discopy.cat import factory, assert_iscomposable
 from discopy.frobenius import Dim, Cup, Category
-from discopy.matrix import Matrix, backend, set_backend, get_backend
-from discopy.monoidal import assert_isatomic
-from discopy.utils import factory_name, assert_isinstance, product
+from discopy.matrix import (  # noqa: F401
+    Matrix, backend, set_backend, get_backend)
+from discopy.utils import (
+    factory_name, assert_isinstance, product, assert_isatomic)
+
+if TYPE_CHECKING:
+    import sympy
+    import tensornetwork
 
 
 @factory
 class Tensor(Matrix):
     """
     A tensor is a :class:`Matrix` with dimensions as domain and codomain and
     the Kronecker product as tensor.
@@ -316,15 +321,15 @@
         :align: center
 
     >>> assert F(diagram) == F(rewrite)
     """
     dom, cod = frobenius.Category(), Category(Dim, Tensor)
 
     def __init__(
-            self, ob: dict[cat.Ob, Dim], ar: dict[cat.Box, array],
+            self, ob: dict[cat.Ob, Dim], ar: dict[cat.Box, list],
             dom: cat.Category = None, dtype: type = int):
         self.dtype = dtype
         cod = Category(type(self).cod.ob, type(self).cod.ar[dtype])
         super().__init__(ob, ar, dom=dom or type(self).dom, cod=cod)
 
     def __repr__(self):
         return factory_name(type(self)) + f"(ob={self.ob}, ar={self.ar}, "\
```

### Comparing `discopy-1.1.2/discopy/traced.py` & `discopy-1.1.3/discopy/traced.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,20 @@
     Functor
 
 Axioms
 ------
 
 >>> from discopy.drawing import Equation
 >>> from discopy.symmetric import Ty, Box, Swap, Id
+>>> from discopy import symmetric
+>>> symmetric.Diagram.structure_preserving = True
 >>> x = Ty('x')
 >>> f, g = Box('f', x @ x, x @ x), Box('g', x, x)
 
 * Vanishing
-
 >>> assert f.trace(n=0) == f == f.trace(n=0, left=True)
 >>> assert f.trace(n=2) == f.trace().trace()
 >>> assert f.trace(n=2, left=True) == f.trace(left=True).trace(left=True)
 
 * Superposing
 
 >>> assert (x @ f).trace() == x @ f.trace()
@@ -94,18 +95,20 @@
 >>> sliding_right.draw(
 ...     path='docs/_static/traced/sliding-right.png', draw_type_labels=False)
 
 .. image:: /_static/traced/sliding-right.png
     :align: center
 
 >>> assert sliding_left and sliding_right
+
+>>> symmetric.Diagram.structure_preserving = False
 """
 
-from discopy import monoidal, messages
-from discopy.cat import factory, AxiomError
+from discopy import monoidal
+from discopy.cat import factory
 from discopy.monoidal import Ty
 from discopy.utils import factory_name, assert_isinstance, assert_istraceable
 
 
 @factory
 class Diagram(monoidal.Diagram):
     """
```

### Comparing `discopy-1.1.2/discopy/utils.py` & `discopy-1.1.3/discopy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 # -*- coding: utf-8 -*-
 
 """ DisCoPy utility functions. """
 
 from __future__ import annotations
 
-import os
 import json
-from functools import wraps
+import os
 from abc import ABC, abstractmethod
+from functools import wraps
 from typing import (
     Callable,
     Generic,
     Mapping,
     Iterable,
     TypeVar,
     Any,
-    Hashable,
-    Literal,
-    cast,
-    Union,
     Collection,
     Type,
     Optional,
     TYPE_CHECKING,
 )
 
-import json
-from functools import wraps
-from networkx import Graph, connected_components
 from matplotlib.testing.compare import compare_images
+from networkx import Graph, connected_components
 
 from discopy import messages
 from discopy.config import DRAWING_DEFAULT
 
 if TYPE_CHECKING:
     from discopy.monoidal import Ty, Diagram
```

### Comparing `discopy-1.1.2/discopy.egg-info/SOURCES.txt` & `discopy-1.1.3/discopy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .gitignore
 .pylintrc
 .readthedocs.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 .github/workflows/build_test.yml
 discopy/__init__.py
 discopy/balanced.py
 discopy/braided.py
 discopy/cat.py
 discopy/closed.py
 discopy/compact.py
```

### Comparing `discopy-1.1.2/docs/Makefile` & `discopy-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_ext/bases-fullname.py` & `discopy-1.1.3/docs/_ext/bases-fullname.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_ext/youtube.py` & `discopy-1.1.3/docs/_ext/youtube.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/balanced/ribbon_twist.png` & `discopy-1.1.3/docs/_static/balanced/ribbon_twist.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/balanced/twist.png` & `discopy-1.1.3/docs/_static/balanced/twist.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/balanced/twist_dual_rail.png` & `discopy-1.1.3/docs/_static/balanced/twist_dual_rail.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/braided/hexagons.png` & `discopy-1.1.3/docs/_static/braided/hexagons.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/braided/inverse.png` & `discopy-1.1.3/docs/_static/braided/inverse.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/closed/curry-left.png` & `discopy-1.1.3/docs/_static/closed/curry-left.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/closed/curry-right.png` & `discopy-1.1.3/docs/_static/closed/curry-right.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/closed/uncurry.png` & `discopy-1.1.3/docs/_static/closed/uncurry.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/compact/reidemeister.png` & `discopy-1.1.3/docs/_static/compact/reidemeister.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/compact/snake.png` & `discopy-1.1.3/docs/_static/compact/snake.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/compact/yanking.png` & `discopy-1.1.3/docs/_static/compact/yanking.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/compact/yanking_cup_and_cap.png` & `discopy-1.1.3/docs/_static/compact/yanking_cup_and_cap.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/drawing/diagramize.png` & `discopy-1.1.3/docs/_static/drawing/diagramize.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/drawing/example.html` & `discopy-1.1.3/docs/_static/drawing/example.html`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/drawing/frobenius-axioms.png` & `discopy-1.1.3/docs/_static/drawing/frobenius-axioms.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/frobenius/comonoid.png` & `discopy-1.1.3/docs/_static/frobenius/comonoid.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/frobenius/frobenius.png` & `discopy-1.1.3/docs/_static/frobenius/frobenius.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/frobenius/monoid.png` & `discopy-1.1.3/docs/_static/frobenius/monoid.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/frobenius/special.png` & `discopy-1.1.3/docs/_static/frobenius/special.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/grammar/cfg-example.png` & `discopy-1.1.3/docs/_static/grammar/cfg-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/grammar/pregroup-example.png` & `discopy-1.1.3/docs/_static/grammar/pregroup-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/hypergraph/box.png` & `discopy-1.1.3/docs/_static/hypergraph/box.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/hypergraph/diagram.png` & `discopy-1.1.3/docs/_static/hypergraph/diagram.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/hypergraph/unfuse.png` & `discopy-1.1.3/docs/_static/hypergraph/unfuse.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/alice-loves-bob.png` & `discopy-1.1.3/docs/_static/int/alice-loves-bob.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/braid.png` & `discopy-1.1.3/docs/_static/int/braid.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/composition.png` & `discopy-1.1.3/docs/_static/int/composition.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/dagger.png` & `discopy-1.1.3/docs/_static/int/dagger.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/idl.png` & `discopy-1.1.3/docs/_static/int/idl.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/idr.png` & `discopy-1.1.3/docs/_static/int/idr.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/int-snake-equations.png` & `discopy-1.1.3/docs/_static/int/int-snake-equations.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/simplify.png` & `discopy-1.1.3/docs/_static/int/simplify.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/int/tensor.png` & `discopy-1.1.3/docs/_static/int/tensor.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/logo.ico` & `discopy-1.1.3/docs/_static/logo.ico`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/markov/associativity.png` & `discopy-1.1.3/docs/_static/markov/associativity.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/markov/bialgebra.png` & `discopy-1.1.3/docs/_static/markov/bialgebra.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/markov/copy_and_apply.png` & `discopy-1.1.3/docs/_static/markov/copy_and_apply.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/markov/counit.png` & `discopy-1.1.3/docs/_static/markov/counit.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/Eckmann-Hilton.gif` & `discopy-1.1.3/docs/_static/monoidal/Eckmann-Hilton.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/EckmannHilton.gif` & `discopy-1.1.3/docs/_static/monoidal/EckmannHilton.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/arrow-example.png` & `discopy-1.1.3/docs/_static/monoidal/arrow-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/box-example.png` & `discopy-1.1.3/docs/_static/monoidal/box-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/bubble-example.png` & `discopy-1.1.3/docs/_static/monoidal/bubble-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/foliate-example-1.png` & `discopy-1.1.3/docs/_static/monoidal/foliate-example-1.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/foliate-example-1a.png` & `discopy-1.1.3/docs/_static/monoidal/foliate-example-1a.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/foliate-example-1b.png` & `discopy-1.1.3/docs/_static/monoidal/foliate-example-1b.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/foliate-example-2.png` & `discopy-1.1.3/docs/_static/monoidal/foliate-example-2.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/functor-example.png` & `discopy-1.1.3/docs/_static/monoidal/functor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/id-example.png` & `discopy-1.1.3/docs/_static/monoidal/id-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/spiral.gif` & `discopy-1.1.3/docs/_static/monoidal/spiral.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/monoidal/tensor-example.png` & `discopy-1.1.3/docs/_static/monoidal/tensor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/optics/fusion.png` & `discopy-1.1.3/docs/_static/optics/fusion.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/optics/spider-decomp.png` & `discopy-1.1.3/docs/_static/optics/spider-decomp.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/pivotal/axiom.png` & `discopy-1.1.3/docs/_static/pivotal/axiom.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/pivotal/box-conjugate.png` & `discopy-1.1.3/docs/_static/pivotal/box-conjugate.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/pivotal/conjugate.png` & `discopy-1.1.3/docs/_static/pivotal/conjugate.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/pivotal/dagger-transpose.png` & `discopy-1.1.3/docs/_static/pivotal/dagger-transpose.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/pivotal/dagger.png` & `discopy-1.1.3/docs/_static/pivotal/dagger.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/pivotal/trace.png` & `discopy-1.1.3/docs/_static/pivotal/trace.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/quantum/circuit-example.png` & `discopy-1.1.3/docs/_static/quantum/circuit-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/quantum/functor-example.png` & `discopy-1.1.3/docs/_static/quantum/functor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/ribbon/strict.png` & `discopy-1.1.3/docs/_static/ribbon/strict.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/ribbon/twist-untwist.png` & `discopy-1.1.3/docs/_static/ribbon/twist-untwist.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/cap.png` & `discopy-1.1.3/docs/_static/rigid/cap.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/caps.png` & `discopy-1.1.3/docs/_static/rigid/caps.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/cup.png` & `discopy-1.1.3/docs/_static/rigid/cup.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/cups.png` & `discopy-1.1.3/docs/_static/rigid/cups.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/curry.png` & `discopy-1.1.3/docs/_static/rigid/curry.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/diagram-example.png` & `discopy-1.1.3/docs/_static/rigid/diagram-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/functor-example.png` & `discopy-1.1.3/docs/_static/rigid/functor-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/rotate.png` & `discopy-1.1.3/docs/_static/rigid/rotate.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/transpose.png` & `discopy-1.1.3/docs/_static/rigid/transpose.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/transpose_box.png` & `discopy-1.1.3/docs/_static/rigid/transpose_box.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/rigid/typed-snake-equation.png` & `discopy-1.1.3/docs/_static/rigid/typed-snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/snake-equation.png` & `discopy-1.1.3/docs/_static/snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/spiral.gif` & `discopy-1.1.3/docs/_static/spiral.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/symmetric/decorator.png` & `discopy-1.1.3/docs/_static/symmetric/decorator.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/symmetric/hexagons.png` & `discopy-1.1.3/docs/_static/symmetric/hexagons.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/symmetric/inverse.png` & `discopy-1.1.3/docs/_static/symmetric/inverse.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/symmetric/naturality.png` & `discopy-1.1.3/docs/_static/symmetric/naturality.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/symmetric/yang-baxter.png` & `discopy-1.1.3/docs/_static/symmetric/yang-baxter.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/tensor/chain-rule.png` & `discopy-1.1.3/docs/_static/tensor/chain-rule.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/tensor/frobenius-example.png` & `discopy-1.1.3/docs/_static/tensor/frobenius-example.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/tensor/men-are-mortal.png` & `discopy-1.1.3/docs/_static/tensor/men-are-mortal.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/tensor/product-rule.png` & `discopy-1.1.3/docs/_static/tensor/product-rule.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/tensor/rewrite.png` & `discopy-1.1.3/docs/_static/tensor/rewrite.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/golden.png` & `discopy-1.1.3/docs/_static/traced/golden.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/right-nat-trace.png` & `discopy-1.1.3/docs/_static/traced/right-nat-trace.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/sliding-left.png` & `discopy-1.1.3/docs/_static/traced/sliding-left.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/sliding-right.png` & `discopy-1.1.3/docs/_static/traced/sliding-right.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/tightening-left.png` & `discopy-1.1.3/docs/_static/traced/tightening-left.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/tightening-right.png` & `discopy-1.1.3/docs/_static/traced/tightening-right.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/trace.png` & `discopy-1.1.3/docs/_static/traced/trace.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_static/traced/yanking.png` & `discopy-1.1.3/docs/_static/traced/yanking.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/_style/custom.css` & `discopy-1.1.3/docs/_style/custom.css`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/api/architecture.html` & `discopy-1.1.3/docs/api/architecture.html`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/api/architecture.png` & `discopy-1.1.3/docs/api/architecture.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/conf.py` & `discopy-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/discopy.bib` & `discopy-1.1.3/docs/discopy.bib`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/extra/blogs.md` & `discopy-1.1.3/docs/extra/blogs.md`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/extra/papers.md` & `discopy-1.1.3/docs/extra/papers.md`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/extra/talks.rst` & `discopy-1.1.3/docs/extra/talks.rst`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/index.rst` & `discopy-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/make.bat` & `discopy-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/notebooks/21-05-03-tallcat.ipynb` & `discopy-1.1.3/docs/notebooks/21-05-03-tallcat.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/notebooks/21-05-05-tallcat.ipynb` & `discopy-1.1.3/docs/notebooks/21-05-05-tallcat.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/notebooks/diag-diff.ipynb` & `discopy-1.1.3/docs/notebooks/diag-diff.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/notebooks/diagrams.ipynb` & `discopy-1.1.3/docs/notebooks/diagrams.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/docs/notebooks/qnlp.ipynb` & `discopy-1.1.3/docs/notebooks/qnlp.ipynb`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/drawing/legacy.py` & `discopy-1.1.3/test/drawing/legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from pytest import raises
 
 from discopy import utils
-from discopy.cat import AxiomError
+from discopy.utils import AxiomError
 from discopy.compact import *
 from discopy.drawing import *
 
 IMG_FOLDER, TIKZ_FOLDER, TOL = 'test/src/imgs/', 'test/src/tikz/', 10
 
 
 def draw_and_compare(file, **params):
```

### Comparing `discopy-1.1.2/test/grammar/categorial.py` & `discopy-1.1.3/test/grammar/categorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,16 @@
             BC(x >> y, y >> x),
             FX(x << y, z >> y),
             BX(y << x, y >> z)]:
         assert from_tree(diagram.to_tree()) == diagram
 
 
 def pregroup_diagram():
-    from discopy.grammar.pregroup import Ob, Ty, Box, Cup, Diagram
+    from discopy.grammar.pregroup import Ty, Box, Cup, Diagram
+    from discopy.rigid import Ob
 
     boxes = [
         Box('that', Ty(), Ty('NP')),
         Box("'s", Ty(), Ty(Ob('NP', z=1), 'S', Ob('NP', z=-1))),
         Box('exactly', Ty(), Ty(Ob('S', z=1), Ob('NP', z=2), Ob('NP', z=1), 'S')),
         Box('bx', Ty(Ob('NP', z=1), 'S', Ob('NP', z=-1), Ob('S', z=1), Ob('NP', z=2), Ob('NP', z=1), 'S'), Ty(Ob('NP', z=1), 'S', Ob('NP', z=-1))),
         Box('what', Ty(), Ty('NP', Ob('NP', z=-2), Ob('S', z=-1))),
```

### Comparing `discopy-1.1.2/test/grammar/pregroup.py` & `discopy-1.1.3/test/grammar/pregroup.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/quantum/channel.py` & `discopy-1.1.3/test/quantum/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from discopy.cat import AxiomError
+from discopy.utils import AxiomError
 from pytest import raises
 
 from discopy.quantum import *
 from discopy.quantum.channel import *
 
 
 def test_CQ():
```

### Comparing `discopy-1.1.2/test/quantum/circuit.py` & `discopy-1.1.3/test/quantum/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sympy
 import torch
 from pytest import raises
 
 from discopy.quantum.channel import *
 from discopy.quantum.circuit import *
 from discopy.quantum.gates import *
+from discopy import rigid
 
 
 def test_index2bitstring():
     with raises(ValueError):
         index2bitstring(1, 0)
     assert index2bitstring(42, 8) == (0, 0, 1, 0, 1, 0, 1, 0)
```

### Comparing `discopy-1.1.2/test/quantum/eval.py` & `discopy-1.1.3/test/quantum/eval.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/quantum/tk.py` & `discopy-1.1.3/test/quantum/tk.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from unittest.mock import Mock
 
 import numpy as np
 from pytest import raises
 
 from discopy.quantum import tk
 from discopy.quantum.gates import *
+from discopy.tensor import Tensor, Dim
 
 
 def test_Circuit_to_tk():
     bell_state = Circuit.caps(qubit, qubit)
     bell_effect = bell_state[::-1]
     snake = (bell_state @ qubit >> qubit @ bell_effect)[::-1]
     tk_circ = snake.to_tk()
```

### Comparing `discopy-1.1.2/test/quantum/zx.py` & `discopy-1.1.3/test/quantum/zx.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/semantics/matrix.py` & `discopy-1.1.3/test/semantics/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from pytest import raises
 
-from discopy.cat import AxiomError
 from discopy.matrix import Matrix, backend
+from discopy.utils import AxiomError
 
 
 def test_bad_composition():
     m = Matrix([1, 2, 3, 4, 5, 6], 2, 3)
 
     with raises(TypeError):
         m >> 1
```

### Comparing `discopy-1.1.2/test/semantics/python.py` & `discopy-1.1.3/test/semantics/python.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/semantics/tensor.py` & `discopy-1.1.3/test/semantics/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import tensornetwork as tn
 from pytest import raises
 
-from discopy.cat import AxiomError
+from discopy.utils import AxiomError
 from discopy.tensor import *
 from discopy import frobenius
 
 
 def test_backend():
     import jax.numpy
     import torch
```

### Comparing `discopy-1.1.2/test/src/imgs/EckmannHilton.gif` & `discopy-1.1.3/test/src/imgs/EckmannHilton.gif`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/bell-state.png` & `discopy-1.1.3/test/src/imgs/bell-state.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/bialgebra.png` & `discopy-1.1.3/test/src/imgs/bialgebra.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/crack-eggs.png` & `discopy-1.1.3/test/src/imgs/crack-eggs.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/empty_diagram.png` & `discopy-1.1.3/test/src/imgs/empty_diagram.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/long-controlled.png` & `discopy-1.1.3/test/src/imgs/long-controlled.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/sentence-as-diagram.png` & `discopy-1.1.3/test/src/imgs/sentence-as-diagram.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/snake-equation.png` & `discopy-1.1.3/test/src/imgs/snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/spiral.png` & `discopy-1.1.3/test/src/imgs/spiral.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/typed-snake-equation.png` & `discopy-1.1.3/test/src/imgs/typed-snake-equation.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/imgs/who-ansatz.png` & `discopy-1.1.3/test/src/imgs/who-ansatz.png`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/bell-state.tikz` & `discopy-1.1.3/test/src/tikz/bell-state.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/bialgebra.tikz` & `discopy-1.1.3/test/src/tikz/bialgebra.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/copy.tikz` & `discopy-1.1.3/test/src/tikz/copy.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/crack-eggs.tikz` & `discopy-1.1.3/test/src/tikz/crack-eggs.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/long-controlled.tikz` & `discopy-1.1.3/test/src/tikz/long-controlled.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/snake-equation.tikz` & `discopy-1.1.3/test/src/tikz/snake-equation.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/spiral.tikz` & `discopy-1.1.3/test/src/tikz/spiral.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tikz/who-ansatz.tikz` & `discopy-1.1.3/test/src/tikz/who-ansatz.tikz`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/tree2diagram.pickle` & `discopy-1.1.3/test/src/tree2diagram.pickle`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/src/zx-graph.json` & `discopy-1.1.3/test/src/zx-graph.json`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/cat.py` & `discopy-1.1.3/test/syntax/cat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pytest import raises
 
 from discopy.cat import *
+from discopy.utils import AxiomError
 
 
 def test_main():
     x, y, z = Ob('x'), Ob('y'), Ob('z')
     f, g, h = Box('f', x, y), Box('g', y, z), Box('h', z, x)
     assert Id(x) >> f == f == f >> Id(y)
     assert (f >> g).dom == f.dom and (f >> g).cod == g.cod
```

### Comparing `discopy-1.1.2/test/syntax/closed.py` & `discopy-1.1.3/test/syntax/closed.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/compact.py` & `discopy-1.1.3/test/syntax/compact.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/frobenius.py` & `discopy-1.1.3/test/syntax/frobenius.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/hypergraph.py` & `discopy-1.1.3/test/syntax/hypergraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 
 
 def test_Hypergraph_bijection():
     with raises(ValueError):
         H.spiders(1, 2, Ty('x')).bijection
 
 
+def test_Hypergraph_rotate():
+    assert H.id() == \
+           H.id().rotate(left=False).rotate(left=True)
+
+
 def test_Box():
     box = Box('box', Ty('x'), Ty('y')).to_hypergraph()
     assert box == box and box == box @ H.id() and box != 1
 
 
 def test_AxiomError():
     x, y = map(Ty, "xy")
```

### Comparing `discopy-1.1.2/test/syntax/interaction.py` & `discopy-1.1.3/test/syntax/interaction.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/markov.py` & `discopy-1.1.3/test/syntax/markov.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/monoidal.py` & `discopy-1.1.3/test/syntax/monoidal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from pytest import raises
 
 from discopy.cat import *
 from discopy.monoidal import *
 from discopy.drawing import spiral
+from discopy.utils import AxiomError
 
 
 def test_Ty():
     x, y, z = Ty('x'), Ty('y'), Ty('z')
     assert x @ y != y @ x
     assert x @ Ty() == x == Ty() @ x
     assert (x @ y) @ z == x @ y @ z == x @ (y @ z)
```

### Comparing `discopy-1.1.2/test/syntax/ribbon.py` & `discopy-1.1.3/test/syntax/ribbon.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/rigid.py` & `discopy-1.1.3/test/syntax/rigid.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/symmetric.py` & `discopy-1.1.3/test/syntax/symmetric.py`

 * *Files identical despite different names*

### Comparing `discopy-1.1.2/test/syntax/utils.py` & `discopy-1.1.3/test/syntax/utils.py`

 * *Files identical despite different names*

