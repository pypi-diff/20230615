# Comparing `tmp/stdatamodels-1.5.0.tar.gz` & `tmp/stdatamodels-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdatamodels-1.5.0.tar", last modified: Tue May 16 18:38:14 2023, max compression
+gzip compressed data, was "stdatamodels-1.6.0.tar", last modified: Thu Jun 15 17:45:38 2023, max compression
```

## Comparing `stdatamodels-1.5.0.tar` & `stdatamodels-1.6.0.tar`

### file list

```diff
@@ -1,440 +1,442 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.982864 stdatamodels-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.838863 stdatamodels-1.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.838863 stdatamodels-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-16 18:38:14.978864 stdatamodels-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.838863 stdatamodels-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.838863 stdatamodels-1.5.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/asdf_in_fits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.834863 stdatamodels-1.5.0/docs/source/jwst/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.842863 stdatamodels-1.5.0/docs/source/jwst/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/jwst/datamodels/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/jwst/datamodels/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/jwst/datamodels/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/jwst/datamodels/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/jwst/datamodels/new_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/jwst/datamodels/structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.842863 stdatamodels-1.5.0/docs/source/jwst/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/docs/source/jwst/transforms/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:38:14.982864 stdatamodels-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.842863 stdatamodels-1.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.846863 stdatamodels-1.5.0/src/stdatamodels/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 18:38:14.000000 stdatamodels-1.5.0/src/stdatamodels/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/asdf_in_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/dynamicdq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)    29597 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/fits_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.846863 stdatamodels-1.5.0/src/stdatamodels/jwst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.866863 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/abvega_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/amilg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/apcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/asn.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/barshadow.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/combinedspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/dark.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/darkMIRI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/drizpars.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/drizproduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/extract1dimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/fringe.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/fringefreq.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/guider.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ifucube.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ifucubepars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ifuimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/irs2.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/lastframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/level1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.866863 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/metaschema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/metaschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/metaschema/fits-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multiexposure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multiextract1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multiprod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multislit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multispec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/outlierpars.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/pathloss.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/persat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/photom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/pixelarea.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/psfmask.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/readnoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/rscd.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57881 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schema_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.902864 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/asn.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/combinedspectable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/contrast.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    90805 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/dq_def.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/flatcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/gain.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ipc.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_channel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_gainfact.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_grating.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_groupgap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampmode.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_module.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nframes.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ngroups.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nints.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_noutputs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pchannel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pgrating.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_photmjsr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_tsovisit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mask.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multiexposure.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multislit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/pixelarea.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/psfmask.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/readnoise.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/regions.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/resolution.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/segmap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/slit.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/sosswavegrid.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/spec.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specprofile.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/spectrace.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/spectracesingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/spectracetable.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/straylight.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/throughput.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/trapdensity.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/trapsfilled.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wavemap.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27691 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/segmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/slit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/sosswavegrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/speckernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/specprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/spectrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/straylight.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/superbias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.906864 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.930864 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/association.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits
--rw-r--r--   0 runner    (1001) docker     (123) 16801920 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits
--rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/throughput.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/trapdensity.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/trappars.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/trapsfilled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tsophot.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/wavemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/wfssbkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.938864 stdatamodels-1.5.0/src/stdatamodels/jwst/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/library/basic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.938864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.938864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.942864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.942864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    62824 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.942864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.946864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.834863 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.834863 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.954864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.954864 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    38542 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/src/stdatamodels/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.846863 stdatamodels-1.5.0/src/stdatamodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-16 18:38:14.000000 stdatamodels-1.5.0/src/stdatamodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-05-16 18:38:14.000000 stdatamodels-1.5.0/src/stdatamodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:38:14.000000 stdatamodels-1.5.0/src/stdatamodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-16 18:38:14.000000 stdatamodels-1.5.0/src/stdatamodels.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-16 18:38:14.000000 stdatamodels-1.5.0/src/stdatamodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 18:38:14.000000 stdatamodels-1.5.0/src/stdatamodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:38:13.000000 stdatamodels-1.5.0/src/stdatamodels.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.962864 stdatamodels-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.966864 stdatamodels-1.5.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/association.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/association_w_cat.json
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/headers.fits
--rw-r--r--   0 runner    (1001) docker     (123)   501120 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/jwst_image.fits
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/mask.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/nircam_abvega_offset.asdf
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/nonstandard_primary_array.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/nonstandard_primary_array.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-16 18:38:01.000000 stdatamodels-1.5.0/tests/data/sip.fits
--rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/data/test.fits
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:14.978864 stdatamodels-1.5.0/tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/anyof_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/basic_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/core_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/deprecated_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/fits_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/required_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/table_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/transform_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/schemas/validation_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_asdf_in_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_embedded_asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-16 18:38:02.000000 stdatamodels-1.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/asdf_in_fits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.427204 stdatamodels-1.6.0/docs/source/jwst/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/source/jwst/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/new_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/datamodels/structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/docs/source/jwst/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/docs/source/jwst/transforms/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.431204 stdatamodels-1.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.435204 stdatamodels-1.6.0/src/stdatamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/asdf_in_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/dynamicdq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29344 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/fits_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.435204 stdatamodels-1.6.0/src/stdatamodels/jwst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.443204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/abvega_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/amilg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/apcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/asn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/barshadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/combinedspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/darkMIRI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/drizpars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/drizproduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/extract1dimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/fringe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/fringefreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/guider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucubepars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifuimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/irs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/lastframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/level1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.443204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/metaschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/metaschema/fits-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiexposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiextract1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiprod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multislit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/outlierifuoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/outlierpars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pathloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/persat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/photom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pixelarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/psfmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/readnoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rscd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57881 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.467204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/asn.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/combinedspectable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/contrast.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    90805 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/dq_def.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/flatcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/gain.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ipc.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_channel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_gainfact.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_grating.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_groupgap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampmode.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_module.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nframes.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ngroups.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_nints.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_noutputs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pchannel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pgrating.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_photmjsr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_tsovisit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mask.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multiexposure.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multislit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/outlierifuoutput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pixelarea.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/psfmask.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/readnoise.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/regions.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/resolution.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/segmap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slit.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/sosswavegrid.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spec.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specprofile.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectrace.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectracesingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectracetable.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/straylight.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/throughput.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trapdensity.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trapsfilled.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavemap.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27691 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/segmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/slit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/sosswavegrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/speckernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/specprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/spectrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/straylight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/superbias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.467204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.483204 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 16801920 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/throughput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trapdensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trappars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trapsfilled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tsophot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wavemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wfssbkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/library/basic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62822 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.491204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.427204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.427204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.495204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.495204 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38513 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/src/stdatamodels/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.435204 stdatamodels-1.6.0/src/stdatamodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 17:45:38.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:45:37.000000 stdatamodels-1.6.0/src/stdatamodels.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.499204 stdatamodels-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.499204 stdatamodels-1.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/association.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/association_w_cat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/headers.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   501120 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/jwst_image.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/mask.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/nircam_abvega_offset.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/sip.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  5405760 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/data/test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:45:38.507204 stdatamodels-1.6.0/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/anyof_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/basic_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/core_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/deprecated_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/fits_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/required_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/table_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/transform_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/schemas/validation_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_asdf_in_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_embedded_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-15 17:45:28.000000 stdatamodels-1.6.0/tox.ini
```

### Comparing `stdatamodels-1.5.0/.github/pull_request_template.md` & `stdatamodels-1.6.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/.github/workflows/ci.yml` & `stdatamodels-1.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/.github/workflows/ci_cron.yml` & `stdatamodels-1.6.0/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/.github/workflows/publish-to-pypi.yml` & `stdatamodels-1.6.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/.gitignore` & `stdatamodels-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/CHANGES.rst` & `stdatamodels-1.6.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,48 @@
+1.6.1 (unreleased)
+==================
+
+- 
+
+1.6.0 (2023-06-15)
+==================
+
+Other
+-----
+
+- Update jwst outlierpars schema to support new IFU outlier detection algorithm
+  and add new ``OutlierIFUOutputModel`` data model. [#164]
+
+- Reduce interpolation vector length in NIRCam backwards transform
+  to improve computation times [#165]
+
+- Update of JWST/MIRI MRS photom datamodel to include the time dependent correction. [#166]
+
+- Add a parameter to jwst outlierpars schema to support a second level of
+  flagging outliers for JWST MIRI/MRS and NIRSpec IFU data. [#167]
+
+- Close for opened files [#169]
+
+
 1.5.0 (2023-05-16)
 ==================
 
 Other
 -----
 
 - Provide second-order polynomial transforms for NIRCam WFSS grisms. [#124]
 
-
 - Deprecate ``stdatamodels.jwst.datamodels.DataModel`` in favor of
   ``stdatamodels.jwst.datamodels.JwstDataModel``. [#160]
 
 - Provide backwards compatibility for grism transform schemas; remove inverse
   models from required properties of transform schemas. [#161]
 
 - Add wavelength tables for NIRSpec Drizzle cubepars reference file model. [#162]
 
-
 1.4.0 (2023-04-19)
 ==================
 
 Other
 -----
 
 - Add pixel replacement step keyword to jwst.datamodels core schema, and change
```

### Comparing `stdatamodels-1.5.0/CODE_OF_CONDUCT.md` & `stdatamodels-1.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/CONTRIBUTING.md` & `stdatamodels-1.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/LICENSE` & `stdatamodels-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/PKG-INFO` & `stdatamodels-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdatamodels
-Version: 1.5.0
+Version: 1.6.0
 Summary: Core support for DataModel classes used in calibration pipelines
 Author: STScI
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stdatamodels-1.5.0/README.md` & `stdatamodels-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/Makefile` & `stdatamodels-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/asdf_in_fits.rst` & `stdatamodels-1.6.0/docs/source/asdf_in_fits.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/conf.py` & `stdatamodels-1.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/jwst/datamodels/attributes.rst` & `stdatamodels-1.6.0/docs/source/jwst/datamodels/attributes.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/jwst/datamodels/metadata.rst` & `stdatamodels-1.6.0/docs/source/jwst/datamodels/metadata.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/jwst/datamodels/models.rst` & `stdatamodels-1.6.0/docs/source/jwst/datamodels/models.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/jwst/datamodels/new_model.rst` & `stdatamodels-1.6.0/docs/source/jwst/datamodels/new_model.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/jwst/datamodels/structure.rst` & `stdatamodels-1.6.0/docs/source/jwst/datamodels/structure.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/docs/source/jwst/transforms/index.rst` & `stdatamodels-1.6.0/docs/source/jwst/transforms/index.rst`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/pyproject.toml` & `stdatamodels-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/asdf_in_fits.py` & `stdatamodels-1.6.0/src/stdatamodels/asdf_in_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/basic_utils.py` & `stdatamodels-1.6.0/src/stdatamodels/basic_utils.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/dqflags.py` & `stdatamodels-1.6.0/src/stdatamodels/dqflags.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/dynamicdq.py` & `stdatamodels-1.6.0/src/stdatamodels/dynamicdq.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/filetype.py` & `stdatamodels-1.6.0/src/stdatamodels/filetype.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/fits_support.py` & `stdatamodels-1.6.0/src/stdatamodels/fits_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,21 +679,14 @@
         When `True` and the FITS file has an ASDF extension, the
         loading/validation of the FITS header will be skipped, loading
         the model only from the ASDF extension.
         When `None`, the value is taken from the environmental SKIP_FITS_UPDATE.
         Otherwise, the default is `False`
     """
     try:
-        return _from_fits(hdulist, schema, context, skip_fits_update=skip_fits_update, **kwargs)
-    except Exception as exc:
-        hdulist.close()
-        raise exc
-
-def _from_fits(hdulist, schema, context, skip_fits_update=None, **kwargs):
-    try:
         ff = from_fits_asdf(hdulist, **kwargs)
     except Exception as exc:
         raise exc.__class__("ERROR loading embedded ASDF: " + str(exc)) from exc
 
     # Determine whether skipping the FITS loading can be done.
     skip_fits_update = _verify_skip_fits_update(
         skip_fits_update, hdulist, ff, context
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/history.py` & `stdatamodels-1.6.0/src/stdatamodels/history.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/__init__.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from .multiexposure import MultiExposureModel
 from .multiextract1d import MultiExtract1dImageModel
 from .multiprod import MultiProductModel
 from .multislit import MultiSlitModel
 from .multispec import MultiSpecModel
 from .nirspec_flat import NirspecFlatModel, NirspecQuadFlatModel
 from .outlierpars import OutlierParsModel
+from .outlierifuoutput import OutlierIFUOutputModel
 from .pathloss import PathlossModel, MirLrsPathlossModel
 from .persat import PersistenceSatModel
 from .photom import FgsImgPhotomModel
 from .photom import MirImgPhotomModel, MirLrsPhotomModel, MirMrsPhotomModel
 from .photom import NrcImgPhotomModel, NrcWfssPhotomModel
 from .photom import NisImgPhotomModel, NisSossPhotomModel, NisWfssPhotomModel
 from .photom import NrsFsPhotomModel, NrsMosPhotomModel
@@ -117,15 +118,15 @@
     'LinearityModel', 'MaskModel', 'MSAModel',
     'MultiCombinedSpecModel', 'MultiExposureModel',
     'MultiExtract1dImageModel', 'MultiSlitModel',
     'MultiProductModel',
     'MultiSpecModel',
     'NIRCAMGrismModel', 'NIRISSGrismModel',
     'OTEModel',
-    'OutlierParsModel',
+    'OutlierParsModel','OutlierIFUOutputModel',
     'PathlossModel', 'MirLrsPathlossModel',
     'PersistenceSatModel',
     'PixelAreaModel', 'NirspecSlitAreaModel', 'NirspecMosAreaModel', 'NirspecIfuAreaModel',
     'FgsImgPhotomModel',
     'MirImgPhotomModel', 'MirLrsPhotomModel', 'MirMrsPhotomModel',
     'NrcImgPhotomModel', 'NrcWfssPhotomModel',
     'NisImgPhotomModel', 'NisSossPhotomModel', 'NisWfssPhotomModel',
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/abvega_offset.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/abvega_offset.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/amilg.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/amilg.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/apcorr.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/apcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/asn.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/asn.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/barshadow.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/barshadow.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/cube.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/cube.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/dark.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dark.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/darkMIRI.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/darkMIRI.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/dqflags.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/dqflags.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/extract1d_spec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/flat.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/flat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/fringe.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/fringe.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/gls_rampfit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/guider.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/guider.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ifucube.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucube.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ifucubepars.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifucubepars.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ifuimage.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ifuimage.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/image.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/image.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/integration.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/integration.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/irs2.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/irs2.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/lastframe.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/lastframe.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/level1b.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/level1b.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/linearity.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/linearity.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/mask.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mask.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/model_base.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/model_base.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsptcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/mrsxartcorr.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multicombinedspec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multiexposure.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiexposure.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multiextract1d.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multiextract1d.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multislit.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multislit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/multispec.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/multispec.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/nirspec_flat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/pathloss.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pathloss.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/persat.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/persat.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/photom.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/photom.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,31 @@
 
     dq_def : numpy array
         A table-like object containing the data quality definitions table.
 
     pixsiz : numpy array
         An array-like object containing pixel-by-pixel size values, in units of
         square arcseconds (arcsec^2).
+
+    timecoeff_ch1 : numpy table
+        A table of time and wavelength dependent throughput corrections
+        for channel 1
+
+    timecoeff_ch2 : numpy table
+        A table of time and wavelength dependent throughput corrections
+        for channel 2
+
+    timecoeff_ch3 : numpy table
+        A table of time and wavelength dependent throughput corrections
+        for channel 3
+
+    timecoeff_ch4 : numpy table
+        A table of time and wavelength dependent throughput corrections
+        for channel 4
+
     """
     schema_url = "http://stsci.edu/schemas/jwst_datamodel/mirmrs_photom.schema"
 
     def __init__(self, init=None, **kwargs):
         super(MirMrsPhotomModel, self).__init__(init=init, **kwargs)
 
         self.dq = dynamic_mask(self, pixel)
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/pixelarea.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/pixelarea.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/quad.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/quad.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/ramp.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/ramp.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rampfitoutput.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/reference.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reference.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/reset.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/reset.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/resolution.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/resolution.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/rscd.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/rscd.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/saturation.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/saturation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schema.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schema_editor.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schema_editor.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/abvegaoffset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/amilg.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/barshadow.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/bunit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/camera.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cheby.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/collimator.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/combinedspec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/core.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/cube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/dark.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/darkMIRI.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/disperser.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/distortion_mrs.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/drizpars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1difu.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/extract1dimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fgsimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/filteroffset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fore.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fpa.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/fringe_freq.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/gls_rampfit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/group.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_cal.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_meta.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/guider_raw.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifufore.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifupost.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ifuslicer.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/image.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/int_times.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/irs2.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_band.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_coronmsk.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_exptype.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_filter.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_lampstate.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pband.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pdetector.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pexptype.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pfilter.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pixelarea.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_ppupil.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_preadpatt.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_psubarray.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_pupil.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/keyword_readpatt.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/lastframe.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/level1b.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/linearity.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsptcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_mrsxartcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/miri_resolution.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_pathloss.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirlrs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_extract1d.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/mirmrs_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,29 @@
 %YAML 1.1
 ---
 $schema: "http://stsci.edu/schemas/fits-schema/fits-schema"
-id: "http://stsci.edu/schemas/jwst_datamodel/mirmrs_photom.schema"
-title: MIRI MRS photometric flux conversion data model
+id: "http://stsci.edu/schemas/jwst_datamodel/superbias.schema"
 allOf:
 - $ref: referencefile.schema
-- $ref: keyword_exptype.schema
-- $ref: keyword_pexptype.schema
-- $ref: keyword_band.schema
-- $ref: keyword_photmjsr.schema
-- $ref: keyword_pixelarea.schema
+- $ref: subarray.schema
+- $ref: keyword_readpatt.schema
+- $ref: keyword_preadpatt.schema
+- $ref: keyword_gainfact.schema
 - type: object
   properties:
     data:
-      title: Flux conversion array
+      title: The science data
       fits_hdu: SCI
-      default: 1.0
-      ndim: 2
-      datatype: float32
-    err:
-      title: Uncertainty array
-      fits_hdu: ERR
       default: 0.0
       ndim: 2
       datatype: float32
     dq:
       title: Data quality array
       fits_hdu: DQ
       default: 0
-      ndim: 2
       datatype: uint32
-- $ref: dq_def.schema
-- type: object
-  properties:
-    pixsiz:
-      title: Pixel size array
-      fits_hdu: PIXSIZ
-      default: 1.0
-      ndim: 2
+    err:
+      title: Error array
+      fits_hdu: ERR
+      default: 0.0
       datatype: float32
+- $ref: dq_def.schema
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/moving_target.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msa.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/msatargacq.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multicombinedspec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multiextract1d.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/multispec.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_ifu.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_mos.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_area_slit.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_ifucubepars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nirspec_quad_flat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nisimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nissoss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/niswfss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcimg_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -53,8 +53,13 @@
         datatype: float32
       - name: snr
         datatype: [ascii, 20]
       - name: scale
         datatype: [ascii, 10]
       - name: backg
         datatype: float32
-
+      - name: threshold_percent
+        datatype: float32
+      - name: kernel_size
+        datatype: [ascii, 10]
+      - name: ifu_second_check
+        datatype: bool8
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/quad.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/ramp.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rampfitoutput.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencecube.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencefile.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referenceimage.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/referencequad.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/reset.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/rscd.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/saturation.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitdata.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/slitmeta.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/sossextractmodel.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/speckernel.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specprofilesingle.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/spectable.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_nircam_grism.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/specwcs_niriss_grism.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/subarray.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/superbias.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wfssbkg.schema.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 %YAML 1.1
 ---
 $schema: "http://stsci.edu/schemas/fits-schema/fits-schema"
-id: "http://stsci.edu/schemas/jwst_datamodel/superbias.schema"
+id: "http://stsci.edu/schemas/jwst_datamodel/wfssbkg.schema"
 allOf:
 - $ref: referencefile.schema
+- $ref: keyword_exptype.schema
+- $ref: keyword_filter.schema
+- $ref: keyword_pupil.schema
 - $ref: subarray.schema
-- $ref: keyword_readpatt.schema
-- $ref: keyword_preadpatt.schema
-- $ref: keyword_gainfact.schema
+- $ref: bunit.schema
 - type: object
   properties:
     data:
       title: The science data
       fits_hdu: SCI
       default: 0.0
       ndim: 2
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/trappars.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/tsophot.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/variance.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavecorr.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavelengthrange.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wavemapsingle.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/schemas/wcsinfo.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/slit.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/slit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/sossextractmodel.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/specprofile.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/specprofile.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/spectrace.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/spectrace.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/superbias.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/superbias.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/association.json` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/association_w_cat.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/headers.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/jwst_nircam_mask_ref.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nircam_abvega_offset.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/nonstandard_primary_array.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/sip.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/data/test.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_models.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,18 +46,17 @@
 
 
 def test_init_from_pathlib(tmp_path):
     """Test initializing model from a Path object"""
     path = tmp_path / "pathlib.fits"
     model1 = datamodels.ImageModel((50, 50))
     model1.save(path)
-    model = datamodels.open(path)
-
-    # Test is basically, did we open the model?
-    assert isinstance(model, ImageModel)
+    with datamodels.open(path) as model:
+        # Test is basically, did we open the model?
+        assert isinstance(model, ImageModel)
 
 
 @pytest.mark.parametrize('which_file, skip_fits_update, expected_exp_type',
                          [
                              ('just_fits', None, 'FGS_DARK'),
                              ('just_fits', False, 'FGS_DARK'),
                              ('just_fits', True, 'FGS_DARK'),
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_multislit.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_open.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_open.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Test datamodel.open
 """
 
+import contextlib
 import os
 import os.path
 from pathlib import Path, PurePath
 import warnings
 
 import pytest
 import numpy as np
@@ -250,26 +251,29 @@
 def test_open_asdf_no_datamodel_class(tmp_path, suffix):
     path = str(tmp_path / f"no_model.{suffix}")
     model = DataModel()
     model.save(path)
 
     # Note: only the fits open emits a "model_type not found" warning.  Both
     # fits and asdf should behave the same
-    with datamodels.open(path) as m:
-        assert isinstance(m, DataModel)
+    ctx = pytest.warns(util.NoTypeWarning) if suffix == 'fits' else contextlib.nullcontext()
+    with ctx:
+        with datamodels.open(path) as m:
+            assert isinstance(m, DataModel)
 
 
 def test_open_asdf(tmp_path):
     path = str(tmp_path / "straight_asdf.asdf")
     tree = {"foo": 42, "bar": 13, "seq": np.arange(100)}
     with asdf.AsdfFile(tree) as af:
         af.write_to(path)
 
-    with datamodels.open(path) as m:
-        assert isinstance(m, DataModel)
+    with pytest.warns(util.NoTypeWarning):
+        with datamodels.open(path) as m:
+            assert isinstance(m, DataModel)
 
 
 def test_open_kwargs_asdf(tmp_path):
     """
     Test that unrecognized kwargs to the datamodels.open function
     are passed on to the model class constructor.
     """
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_schema_against_crds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import logging
 from collections.abc import Iterable
 from stdatamodels.jwst import datamodels as dm
 import pytest
 import warnings
-from ..util import NoTypeWarning
 
 os.environ["CRDS_SERVER_URL"] = "https://jwst-crds.stsci.edu"
 
 # the CRDS_SERVER_URL environment variable must be set before
 # crds is imported
 import crds  # noqa: E402
 from crds.client.api import cache_references, dump_files  # noqa: E402
@@ -202,15 +201,15 @@
                 # Ensure filetype is kind to be loaded into datamodel
                 if 'fits' in f or 'asdf' in f:
                     # Find datamodel appropriate for this reference file
                     # If reftype has multiple datamodels possible, do some guesswork
                     if reftype in ref_to_multiples_dict.keys():
                         model_map = ref_to_multiples_dict[reftype]
                         with warnings.catch_warnings():
-                            warnings.simplefilter('ignore', NoTypeWarning)
+                            warnings.simplefilter('ignore', dm.util.NoTypeWarning)
                             refs = cache_references(context, {reftype: f})
                             with dm.open(refs[reftype]) as model:
                                 try:
                                     ref_exptype = model.meta.exposure.type
                                 except AttributeError:
                                     ref_exptype = None
                                 ref_instrument = model.meta.instrument.name
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/trapdensity.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trapdensity.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/trappars.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/trappars.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/tsophot.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/tsophot.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/util.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,20 @@
     # Log a message about how the model was opened
     if file_name:
         log.debug(f'Opening {file_name} as {new_class}')
     else:
         log.debug(f'Opening as {new_class}')
 
     # Actually open the model
-    model = new_class(init, **kwargs)
+    try:
+        model = new_class(init, **kwargs)
+    except Exception:
+        if file_to_close is not None:
+            file_to_close.close()
+        raise
 
     # Close the hdulist if we opened it
     if file_to_close is not None:
         # TODO: We need a better solution than messing with DataModel
         # internals.
         model._file_references.append(_FileReference(file_to_close))
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/wavemap.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wavemap.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wcs_ref_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/datamodels/wfssbkg.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/datamodels/wfssbkg.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/library/basic_utils.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/library/basic_utils.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/__init__.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/jwst_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/data/niriss_soss.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/converters/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/extensions.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/extensions.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/integration.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/integration.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/models.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,15 +941,15 @@
 
         dx = assess_model(xmodel, x, y, t)
         dy = assess_model(ymodel, x, y, t)
         return x + dx, y + dy, x, y, order
 
     def invdisp_interp(self, model, x0, y0, wavelength):
 
-        t0 = np.linspace(0., 1., 1000)
+        t0 = np.linspace(0., 1., 40)
         t_re = np.reshape(t0, [len(t0), *map(int, np.ones_like(np.shape(x0)))])
 
         if len(model) == 2:
             xr = (np.ones_like(t_re) * model[0](x0, y0)) + (t_re * model[1](x0, y0))
         elif len(model) == 3:
             xr = (np.ones_like(t_re) * model[0](x0, y0)) + (t_re * model[1](x0, y0)) + \
                  (t_re ** 2 * model[2](x0, y0))
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/manifests/jwst_transforms-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/coords-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/grating_equation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/gwa_to_slit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/logical-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/miri_ab2slice-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/nircam_grism_dispersion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_grism_dispersion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/niriss_soss-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/refraction_index_from_prism-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/rotation_sequence-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/slit_to_msa-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/snell-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/resources/schemas/stsci.edu/jwst_pipeline/v23tosky-0.7.0.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/jwst/transforms/tests/tests.py` & `stdatamodels-1.6.0/src/stdatamodels/jwst/transforms/tests/tests.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/model_base.py` & `stdatamodels-1.6.0/src/stdatamodels/model_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,18 +228,18 @@
                 init = str(init)
             if isinstance(init, bytes):
                 init = init.decode(sys.getfilesystemencoding())
             file_type = filetype.check(init)
 
             if file_type == "fits":
                 hdulist = fits.open(init, memmap=memmap)
+                self._file_references.append(_FileReference(hdulist))
                 asdffile = fits_support.from_fits(
                     hdulist, self._schema, self._ctx, **kwargs
                 )
-                self._file_references.append(_FileReference(hdulist))
 
             elif file_type == "asdf":
                 asdffile = self.open_asdf(init=init, **kwargs)
 
             else:
                 # TODO handle json files as well
                 raise IOError(
@@ -382,15 +382,14 @@
             target._asdf = source._asdf
             target._instance = source._instance
             for file_reference in source._file_references:
                 file_reference.increment()
                 target._file_references.append(file_reference)
 
         target._shape = source._shape
-        target._ctx = target
         target._no_asdf_extension = source._no_asdf_extension
 
     def copy(self, memo=None):
         """
         Returns a deep copy of this model.
         """
         result = self.__class__(init=None,
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels/properties.py` & `stdatamodels-1.6.0/src/stdatamodels/properties.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/schema.py` & `stdatamodels-1.6.0/src/stdatamodels/schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/util.py` & `stdatamodels-1.6.0/src/stdatamodels/util.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels/validate.py` & `stdatamodels-1.6.0/src/stdatamodels/validate.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/src/stdatamodels.egg-info/PKG-INFO` & `stdatamodels-1.6.0/src/stdatamodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdatamodels
-Version: 1.5.0
+Version: 1.6.0
 Summary: Core support for DataModel classes used in calibration pipelines
 Author: STScI
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stdatamodels-1.5.0/src/stdatamodels.egg-info/SOURCES.txt` & `stdatamodels-1.6.0/src/stdatamodels.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 src/stdatamodels/jwst/datamodels/multicombinedspec.py
 src/stdatamodels/jwst/datamodels/multiexposure.py
 src/stdatamodels/jwst/datamodels/multiextract1d.py
 src/stdatamodels/jwst/datamodels/multiprod.py
 src/stdatamodels/jwst/datamodels/multislit.py
 src/stdatamodels/jwst/datamodels/multispec.py
 src/stdatamodels/jwst/datamodels/nirspec_flat.py
+src/stdatamodels/jwst/datamodels/outlierifuoutput.py
 src/stdatamodels/jwst/datamodels/outlierpars.py
 src/stdatamodels/jwst/datamodels/pathloss.py
 src/stdatamodels/jwst/datamodels/persat.py
 src/stdatamodels/jwst/datamodels/photom.py
 src/stdatamodels/jwst/datamodels/pixelarea.py
 src/stdatamodels/jwst/datamodels/psfmask.py
 src/stdatamodels/jwst/datamodels/quad.py
@@ -252,14 +253,15 @@
 src/stdatamodels/jwst/datamodels/schemas/nrcwfss_photom.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsfs_apcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsfs_photom.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsifu_apcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsmos_apcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/nrsmos_photom.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/ote.schema.yaml
+src/stdatamodels/jwst/datamodels/schemas/outlierifuoutput.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/outlierpars.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/pathloss.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/pathlosscorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/persat.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/photomcorr.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/photometry.schema.yaml
 src/stdatamodels/jwst/datamodels/schemas/pixelarea.schema.yaml
```

### Comparing `stdatamodels-1.5.0/tests/conftest.py` & `stdatamodels-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/association.json` & `stdatamodels-1.6.0/tests/data/association.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/association_w_cat.json` & `stdatamodels-1.6.0/tests/data/association_w_cat.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/headers.fits` & `stdatamodels-1.6.0/tests/data/headers.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/jwst_image.fits` & `stdatamodels-1.6.0/tests/data/jwst_image.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/mask.fits` & `stdatamodels-1.6.0/tests/data/mask.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/nircam_abvega_offset.asdf` & `stdatamodels-1.6.0/tests/data/nircam_abvega_offset.asdf`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/nonstandard_primary_array.schema.json` & `stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.json`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/nonstandard_primary_array.schema.yaml` & `stdatamodels-1.6.0/tests/data/nonstandard_primary_array.schema.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/sip.fits` & `stdatamodels-1.6.0/tests/data/sip.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/data/test.fits` & `stdatamodels-1.6.0/tests/data/test.fits`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/models.py` & `stdatamodels-1.6.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/schemas/basic_model.yaml` & `stdatamodels-1.6.0/tests/schemas/basic_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/schemas/deprecated_model.yaml` & `stdatamodels-1.6.0/tests/schemas/deprecated_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/schemas/fits_model.yaml` & `stdatamodels-1.6.0/tests/schemas/fits_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/schemas/table_model.yaml` & `stdatamodels-1.6.0/tests/schemas/table_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/schemas/validation_model.yaml` & `stdatamodels-1.6.0/tests/schemas/validation_model.yaml`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_asdf_in_fits.py` & `stdatamodels-1.6.0/tests/test_asdf_in_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_dq.py` & `stdatamodels-1.6.0/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_embedded_asdf.py` & `stdatamodels-1.6.0/tests/test_embedded_asdf.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_filetype.py` & `stdatamodels-1.6.0/tests/test_filetype.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_fits.py` & `stdatamodels-1.6.0/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_history.py` & `stdatamodels-1.6.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_models.py` & `stdatamodels-1.6.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_resources.py` & `stdatamodels-1.6.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_schema.py` & `stdatamodels-1.6.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_util.py` & `stdatamodels-1.6.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tests/test_validation.py` & `stdatamodels-1.6.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `stdatamodels-1.5.0/tox.ini` & `stdatamodels-1.6.0/tox.ini`

 * *Files identical despite different names*

