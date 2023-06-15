# Comparing `tmp/nanoqnt-0.2.1.tar.gz` & `tmp/nanoqnt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoqnt-0.2.1.tar", max compression
+gzip compressed data, was "nanoqnt-0.2.2.tar", max compression
```

## Comparing `nanoqnt-0.2.1.tar` & `nanoqnt-0.2.2.tar`

### file list

```diff
@@ -1,77 +1,79 @@
--rw-r--r--   0        0        0    32472 2023-06-14 12:31:39.675046 nanoqnt-0.2.1/LICENSE.md
--rw-r--r--   0        0        0      648 2023-06-14 14:20:59.156275 nanoqnt-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-01-02 14:34:22.063965 nanoqnt-0.2.1/nanoqnt/__init__.py
--rw-r--r--   0        0        0     4154 2023-06-12 12:02:24.898367 nanoqnt-0.2.1/nanoqnt/dispertech-logo.ico
--rw-r--r--   0        0        0     1189 2023-06-14 13:42:06.609945 nanoqnt-0.2.1/nanoqnt/main.py
--rw-r--r--   0        0        0        0 2022-12-20 12:52:00.514018 nanoqnt-0.2.1/nanoqnt/model/__init__.py
--rw-r--r--   0        0        0    15541 2023-06-14 14:52:26.989817 nanoqnt-0.2.1/nanoqnt/model/analyze_nanoqnt.py
--rw-r--r--   0        0        0      280 2023-06-12 12:02:24.900270 nanoqnt-0.2.1/nanoqnt/model/decorators.py
--rw-r--r--   0        0        0       34 2023-06-12 12:02:24.900680 nanoqnt-0.2.1/nanoqnt/model/exceptions.py
--rw-r--r--   0        0        0      385 2023-06-12 12:02:24.901046 nanoqnt-0.2.1/nanoqnt/stage_main.py
--rw-r--r--   0        0        0      351 2023-06-12 12:02:24.901498 nanoqnt-0.2.1/nanoqnt/util/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-12 12:02:24.901860 nanoqnt-0.2.1/nanoqnt/util/make_hdf5.py
--rw-r--r--   0        0        0     3759 2022-03-16 14:59:30.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
--rw-r--r--   0        0        0     4715 2022-03-16 14:59:22.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11814 - Atom.svg
--rw-r--r--   0        0        0     3727 2022-03-16 14:59:14.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11815 - Battery.svg
--rw-r--r--   0        0        0     5275 2022-03-16 14:59:06.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
--rw-r--r--   0        0        0     2802 2022-03-16 14:58:58.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
--rw-r--r--   0        0        0     4637 2022-03-16 14:58:50.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
--rw-r--r--   0        0        0     1936 2022-03-16 14:58:44.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
--rw-r--r--   0        0        0     2442 2022-03-16 14:58:36.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
--rw-r--r--   0        0        0     2191 2022-03-16 14:58:28.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
--rw-r--r--   0        0        0     2594 2022-03-16 14:58:22.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11822 - Collision.svg
--rw-r--r--   0        0        0     2347 2022-03-16 14:58:14.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
--rw-r--r--   0        0        0     2347 2022-03-16 14:58:04.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
--rw-r--r--   0        0        0     2710 2022-03-16 14:57:56.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
--rw-r--r--   0        0        0     3426 2022-03-16 15:19:36.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
--rw-r--r--   0        0        0     3508 2022-03-16 14:57:38.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
--rw-r--r--   0        0        0     3527 2022-03-16 14:57:30.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11828 - Energy.svg
--rw-r--r--   0        0        0     1821 2022-03-16 14:57:22.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11829 - Flask.svg
--rw-r--r--   0        0        0     4901 2022-03-16 14:57:14.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11830 - Float.svg
--rw-r--r--   0        0        0     1522 2022-03-16 14:57:06.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
--rw-r--r--   0        0        0     8697 2022-03-16 14:56:58.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11832 - Force.svg
--rw-r--r--   0        0        0     3310 2022-03-16 14:56:48.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11833 - Formula.svg
--rw-r--r--   0        0        0     2416 2022-03-16 14:56:40.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11834 - Gears.svg
--rw-r--r--   0        0        0     4479 2022-03-16 14:56:32.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
--rw-r--r--   0        0        0     4165 2022-03-16 14:56:24.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
--rw-r--r--   0        0        0     3653 2022-03-16 14:56:16.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
--rw-r--r--   0        0        0     2013 2022-03-16 14:56:08.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
--rw-r--r--   0        0        0     2576 2022-03-16 14:56:00.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
--rw-r--r--   0        0        0     5579 2022-03-16 14:55:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
--rw-r--r--   0        0        0     3646 2022-03-16 14:55:46.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
--rw-r--r--   0        0        0     1706 2022-03-16 14:55:38.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
--rw-r--r--   0        0        0     3307 2022-03-16 14:55:32.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
--rw-r--r--   0        0        0     2707 2022-03-16 14:55:24.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11844 - Motion.svg
--rw-r--r--   0        0        0     1163 2022-03-16 14:55:18.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
--rw-r--r--   0        0        0     5179 2022-03-16 14:55:10.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
--rw-r--r--   0        0        0     2264 2022-03-16 14:55:02.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
--rw-r--r--   0        0        0     4868 2022-03-16 14:54:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11848 - Planet.svg
--rw-r--r--   0        0        0     9381 2022-03-16 14:54:44.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
--rw-r--r--   0        0        0      806 2022-03-16 14:54:36.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11850 - Power.svg
--rw-r--r--   0        0        0     2581 2022-03-16 14:54:28.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11851 - Press.svg
--rw-r--r--   0        0        0     3090 2022-03-16 14:54:20.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11852 - Proton.svg
--rw-r--r--   0        0        0     2528 2022-03-16 14:54:12.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
--rw-r--r--   0        0        0     4144 2022-03-16 14:54:04.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
--rw-r--r--   0        0        0     3109 2022-03-16 14:53:56.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
--rw-r--r--   0        0        0     2481 2022-03-16 14:53:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
--rw-r--r--   0        0        0     3390 2022-03-16 14:53:52.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
--rw-r--r--   0        0        0     2463 2022-03-16 14:53:50.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
--rw-r--r--   0        0        0     2156 2022-03-16 14:53:48.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
--rw-r--r--   0        0        0     2552 2022-03-16 14:53:48.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
--rw-r--r--   0        0        0     2816 2022-03-16 15:41:46.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11861 - Waves.svg
--rw-r--r--   0        0        0     3799 2022-03-16 14:53:44.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
--rw-r--r--   0        0        0       43 2022-12-20 12:57:18.786580 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Icons.qrc
--rw-r--r--   0        0        0      342 2022-11-15 12:55:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Open Folder.svg
--rw-r--r--   0        0        0      559 2022-11-15 12:55:54.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Save.svg
--rw-r--r--   0        0        0      215 2020-07-27 20:54:42.000000 nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/open.svg
--rw-r--r--   0        0        0     2193 2023-06-12 12:02:24.902373 nanoqnt-0.2.1/nanoqnt/view/GUI/channel_selector.ui
--rw-r--r--   0        0        0    14862 2023-06-14 14:24:59.072757 nanoqnt-0.2.1/nanoqnt/view/GUI/data_exploration.ui
--rw-r--r--   0        0        0     5565 2023-06-14 14:20:12.278524 nanoqnt-0.2.1/nanoqnt/view/GUI/particles_widget.ui
--rw-r--r--   0        0        0     3367 2023-01-26 21:32:32.021169 nanoqnt-0.2.1/nanoqnt/view/GUI/scan_control.ui
--rw-r--r--   0        0        0       62 2023-06-12 12:02:24.903693 nanoqnt-0.2.1/nanoqnt/view/__init__.py
--rw-r--r--   0        0        0      848 2023-06-12 12:02:24.903942 nanoqnt-0.2.1/nanoqnt/view/channel_selector.py
--rw-r--r--   0        0        0    11374 2023-06-14 14:56:09.181506 nanoqnt-0.2.1/nanoqnt/view/main_window.py
--rw-r--r--   0        0        0     1947 2023-06-12 12:02:24.904552 nanoqnt-0.2.1/nanoqnt/view/particle_widget.py
--rw-r--r--   0        0        0     1359 2023-06-12 12:02:24.904821 nanoqnt-0.2.1/nanoqnt/view/stage_control.py
--rw-r--r--   0        0        0     1448 2023-06-14 14:57:22.497703 nanoqnt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 nanoqnt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-06-14 15:03:11.989086 nanoqnt-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0      648 2023-06-14 15:03:11.989297 nanoqnt-0.2.2/README.md
+-rw-r--r--   0        0        0       54 2023-06-15 10:27:00.386966 nanoqnt-0.2.2/nanoqnt/__init__.py
+-rw-r--r--   0        0        0       17 2023-06-15 10:27:26.584975 nanoqnt-0.2.2/nanoqnt/_version.py
+-rw-r--r--   0        0        0     4154 2023-06-14 15:03:11.990226 nanoqnt-0.2.2/nanoqnt/dispertech-logo.ico
+-rw-r--r--   0        0        0     1189 2023-06-14 15:03:11.990429 nanoqnt-0.2.2/nanoqnt/main.py
+-rw-r--r--   0        0        0        0 2022-12-20 12:52:00.514018 nanoqnt-0.2.2/nanoqnt/model/__init__.py
+-rw-r--r--   0        0        0    16295 2023-06-15 13:46:49.675662 nanoqnt-0.2.2/nanoqnt/model/analyze_nanoqnt.py
+-rw-r--r--   0        0        0      280 2023-06-14 15:03:11.991021 nanoqnt-0.2.2/nanoqnt/model/decorators.py
+-rw-r--r--   0        0        0       34 2023-06-14 15:03:11.991281 nanoqnt-0.2.2/nanoqnt/model/exceptions.py
+-rw-r--r--   0        0        0      385 2023-06-14 15:03:11.991605 nanoqnt-0.2.2/nanoqnt/stage_main.py
+-rw-r--r--   0        0        0      351 2023-06-14 15:03:11.991838 nanoqnt-0.2.2/nanoqnt/util/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-14 15:03:11.992107 nanoqnt-0.2.2/nanoqnt/util/make_hdf5.py
+-rw-r--r--   0        0        0     3759 2022-03-16 14:59:30.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg
+-rw-r--r--   0        0        0     4715 2022-03-16 14:59:22.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11814 - Atom.svg
+-rw-r--r--   0        0        0     3727 2022-03-16 14:59:14.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11815 - Battery.svg
+-rw-r--r--   0        0        0     5275 2022-03-16 14:59:06.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11816 - Orbit.svg
+-rw-r--r--   0        0        0     2802 2022-03-16 14:58:58.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11817 - Beaker.svg
+-rw-r--r--   0        0        0     4637 2022-03-16 14:58:50.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg
+-rw-r--r--   0        0        0     1936 2022-03-16 14:58:44.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11819 - Bounce.svg
+-rw-r--r--   0        0        0     2442 2022-03-16 14:58:36.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11820 - Caliper.svg
+-rw-r--r--   0        0        0     2191 2022-03-16 14:58:28.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11821 - Catapult.svg
+-rw-r--r--   0        0        0     2594 2022-03-16 14:58:22.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11822 - Collision.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:14.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg
+-rw-r--r--   0        0        0     2347 2022-03-16 14:58:04.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg
+-rw-r--r--   0        0        0     2710 2022-03-16 14:57:56.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg
+-rw-r--r--   0        0        0     3426 2022-03-16 15:19:36.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg
+-rw-r--r--   0        0        0     3508 2022-03-16 14:57:38.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg
+-rw-r--r--   0        0        0     3527 2022-03-16 14:57:30.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11828 - Energy.svg
+-rw-r--r--   0        0        0     1821 2022-03-16 14:57:22.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11829 - Flask.svg
+-rw-r--r--   0        0        0     4901 2022-03-16 14:57:14.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11830 - Float.svg
+-rw-r--r--   0        0        0     1522 2022-03-16 14:57:06.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg
+-rw-r--r--   0        0        0     8697 2022-03-16 14:56:58.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11832 - Force.svg
+-rw-r--r--   0        0        0     3310 2022-03-16 14:56:48.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11833 - Formula.svg
+-rw-r--r--   0        0        0     2416 2022-03-16 14:56:40.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11834 - Gears.svg
+-rw-r--r--   0        0        0     4479 2022-03-16 14:56:32.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11835 - Gravity.svg
+-rw-r--r--   0        0        0     4165 2022-03-16 14:56:24.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg
+-rw-r--r--   0        0        0     3653 2022-03-16 14:56:16.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11837 - Histogram.svg
+-rw-r--r--   0        0        0     2013 2022-03-16 14:56:08.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg
+-rw-r--r--   0        0        0     2576 2022-03-16 14:56:00.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11839 - Magnet.svg
+-rw-r--r--   0        0        0     5579 2022-03-16 14:55:54.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg
+-rw-r--r--   0        0        0     3646 2022-03-16 14:55:46.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11841 - Metronome.svg
+-rw-r--r--   0        0        0     1706 2022-03-16 14:55:38.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg
+-rw-r--r--   0        0        0     3307 2022-03-16 14:55:32.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11843 - Molecule.svg
+-rw-r--r--   0        0        0     2707 2022-03-16 14:55:24.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11844 - Motion.svg
+-rw-r--r--   0        0        0     1163 2022-03-16 14:55:18.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg
+-rw-r--r--   0        0        0     5179 2022-03-16 14:55:10.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg
+-rw-r--r--   0        0        0     2264 2022-03-16 14:55:02.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg
+-rw-r--r--   0        0        0     4868 2022-03-16 14:54:54.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11848 - Planet.svg
+-rw-r--r--   0        0        0     9381 2022-03-16 14:54:44.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg
+-rw-r--r--   0        0        0      806 2022-03-16 14:54:36.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11850 - Power.svg
+-rw-r--r--   0        0        0     2581 2022-03-16 14:54:28.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11851 - Press.svg
+-rw-r--r--   0        0        0     3090 2022-03-16 14:54:20.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11852 - Proton.svg
+-rw-r--r--   0        0        0     2528 2022-03-16 14:54:12.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11853 - Pulley.svg
+-rw-r--r--   0        0        0     4144 2022-03-16 14:54:04.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11854 - Reflection.svg
+-rw-r--r--   0        0        0     3109 2022-03-16 14:53:56.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11855 - Resistor.svg
+-rw-r--r--   0        0        0     2481 2022-03-16 14:53:54.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11856 - Rolling.svg
+-rw-r--r--   0        0        0     3390 2022-03-16 14:53:52.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11857 - Rotate.svg
+-rw-r--r--   0        0        0     2463 2022-03-16 14:53:50.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg
+-rw-r--r--   0        0        0     2156 2022-03-16 14:53:48.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11859 - Temperature.svg
+-rw-r--r--   0        0        0     2552 2022-03-16 14:53:48.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg
+-rw-r--r--   0        0        0     2816 2022-03-16 15:41:46.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11861 - Waves.svg
+-rw-r--r--   0        0        0     3799 2022-03-16 14:53:44.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg
+-rw-r--r--   0        0        0       43 2022-12-20 12:57:18.786580 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/Icons.qrc
+-rw-r--r--   0        0        0      342 2022-11-15 12:55:54.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/Open Folder.svg
+-rw-r--r--   0        0        0      559 2022-11-15 12:55:54.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/Save.svg
+-rw-r--r--   0        0        0      215 2020-07-27 20:54:42.000000 nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/open.svg
+-rw-r--r--   0        0        0     2193 2023-06-14 15:03:11.992385 nanoqnt-0.2.2/nanoqnt/view/GUI/channel_selector.ui
+-rw-r--r--   0        0        0    14793 2023-06-15 12:59:38.359897 nanoqnt-0.2.2/nanoqnt/view/GUI/data_exploration.ui
+-rw-r--r--   0        0        0     5330 2023-06-15 13:37:33.172810 nanoqnt-0.2.2/nanoqnt/view/GUI/data_vis.ui
+-rw-r--r--   0        0        0     5565 2023-06-14 15:03:11.992804 nanoqnt-0.2.2/nanoqnt/view/GUI/particles_widget.ui
+-rw-r--r--   0        0        0     3367 2023-01-26 21:32:32.021169 nanoqnt-0.2.2/nanoqnt/view/GUI/scan_control.ui
+-rw-r--r--   0        0        0       62 2023-06-14 15:03:11.993017 nanoqnt-0.2.2/nanoqnt/view/__init__.py
+-rw-r--r--   0        0        0     1931 2023-06-15 11:45:20.069350 nanoqnt-0.2.2/nanoqnt/view/channel_selector.py
+-rw-r--r--   0        0        0    11914 2023-06-15 13:41:28.165824 nanoqnt-0.2.2/nanoqnt/view/main_window.py
+-rw-r--r--   0        0        0     1947 2023-06-14 15:03:11.993600 nanoqnt-0.2.2/nanoqnt/view/particle_widget.py
+-rw-r--r--   0        0        0     3672 2023-06-15 13:26:52.612857 nanoqnt-0.2.2/nanoqnt/view/results_vis.py
+-rw-r--r--   0        0        0     1446 2023-06-15 10:27:26.588470 nanoqnt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 nanoqnt-0.2.2/PKG-INFO
```

### Comparing `nanoqnt-0.2.1/LICENSE.md` & `nanoqnt-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/README.md` & `nanoqnt-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/dispertech-logo.ico` & `nanoqnt-0.2.2/nanoqnt/dispertech-logo.ico`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/main.py` & `nanoqnt-0.2.2/nanoqnt/main.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/model/analyze_nanoqnt.py` & `nanoqnt-0.2.2/nanoqnt/model/analyze_nanoqnt.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 import trackpy as tp
 import yaml
 from scipy.spatial import KDTree
 from skimage import morphology
 from skimage.measure import label, regionprops_table
 from trackpy.find import where_close
 from trackpy.utils import pandas_concat
+from nanoqnt import __version__
 
 logger = logging.getLogger(__name__)
 
 
 class AnalyzeNanoQNT:
     def __init__(self):
         self.filename = None
         self.data = None
-        self.metadata = {}
+        self.metadata = {'Software version': __version__}
         self.particle_df = []
         self.particles = pd.DataFrame()
         self.num_frames = 0
         self.find_settings = {}
         self.filename = Path.home()
         self.concentration = {}  # pcles/ml
         self.linked_particles = None
         self.total_num_particles = 0
         self.summarized_particles = None
-
+        self.step_size = 1
         self.ignore_edge_pixels = 8
 
         self.num_channels = 1
         self.channels_data = {}
         self.channels_names = []
         self.bkg = None
 
-
     def open(self, filename):
         """ Opens the file with the data. Normally a multi-tiff file, but it can be adapted to other formats.
         It also looks for the comments.txt file (create by uManager) in order to load some metadata
 
         :param filename: The full-path to the file to be opened
         """
         self.filename = Path(filename)
@@ -68,17 +68,24 @@
             self.metadata['uManager'] = {'comments': 'file not found'}
 
         try:
             comment = self.metadata['uManager']['map']['General annotation']['scalar']['comments']['scalar']
             start = comment.index('(') + 1
             end = comment.index(')')
             self.num_channels = len(comment[start:end].split(' '))
-            self.channels_names = [i for i in range(self.num_channels)]
-        except:
-            pass
+            self.channels_names = comment[start:end].split(' ')
+
+            start = comment.index('[') + 1
+            end = comment.index(']')
+            self.step_size = abs(float(comment[start:end].split(' ')[1]))
+            self.metadata.update({'num_channels': self.num_channels,
+                                     'channels_names': self.channels_names,
+                                     'step_size': self.step_size})
+        except Exception as e:
+            print(e)
 
     def find_particles(self, frame_num, diameter, minmass, method='mask'):
         """ Finds particles in a given frame and stores the data frame in a list indexed by the frame number.
 
         :param int frame_num: The number of the frame (0-indexed) to analyze
         :param int diameter: The expected diameter of the particles. Must be an odd number and is passed directly to
         Trackpy
@@ -240,29 +247,34 @@
                     'x': [pcle.loc[ix]['x']],
                     'y': [pcle.loc[ix]['y']],
                     f'i_{channel}': [pcle['mass'].max()]
                     })
                 self.summary_data[channel] = pd.concat((self.summary_data[channel], df), ignore_index=True)
             self.summary_data[channel] = self.summary_data[channel].reset_index(drop=True)
 
-    def multi_color_link(self):  # TODO: Add max frame distance as a parameter instead of fixing it to 5
-        """ Find the same particles in every channel and add the intensity information on each """
+    def multi_color_link(self, max_dist=10):
+        """ Find the same particles in every channel and add the intensity information on each
+
+        :param int max_dist: Maximum distance between particle localizations that define a "nearest" neighbor. It is
+        assumed isotropic in X/Y and in Frames.
+
+        TODO: If the step size is very different from the spatial distance, there may be issues with the upper bound.
+            3D positions should be transformed to real-space coordinated before defining the KDTree.
+        """
+        self.metadata.update({'multi_color_link': {'max_dist': max_dist}})
         kd_trees = {}
         for channel in range(self.num_channels):
             kd_trees[channel] = KDTree(np.array(self.summary_data[channel][['x', 'y', 'frame']]))
 
         for channel in range(self.num_channels):
             for channel_2 in range(channel + 1, self.num_channels):
                 for ix, p in self.summary_data[channel].iterrows():
-                    dist, ind = kd_trees[channel_2].query((p['x'], p['y'], p['frame']), p=2, distance_upper_bound=15)
+                    dist, ind = kd_trees[channel_2].query((p['x'], p['y'], p['frame']), p=2, distance_upper_bound=max_dist)
                     if ind == kd_trees[channel_2].n:
                         continue
-                    if abs(self.summary_data[channel_2].loc[ind]['frame'] - p['frame']) > 5:
-                        logger.info('Frames too far apart with ', ix, p['x'], p['y'], p['frame'])
-                        continue
                     self.summary_data[channel].loc[ix, f'i_{channel_2}'] = \
                         self.summary_data[channel_2].loc[ind][f'i_{channel_2}']
                     self.summary_data[channel_2].loc[ind, f'i_{channel}'] = p[f'i_{channel}']
 
     def save_all_data(self, filename):
         self.linked_particles.to_csv(str(filename))
 
@@ -279,37 +291,41 @@
         for i in range(self.num_channels):
             stem = filename.stem
             file_name = filename.with_stem(f'{stem}_{i}')
             self.summary_data[i].to_csv(str(file_name))
 
         # Exporting summary data
         with open(filename.with_suffix('.md'), 'w') as f:
-            info = ""
-            for channel in range(self.num_channels):
-                info += f"# Channel {self.channels_names[channel]}\n\n"
-                info += f" - *Found particles*: {len(self.summary_data[channel])}\n"
-                if self.num_channels > 1:
-                    for sub_channel in range(self.num_channels):
-                        info += f" - Particles also in *{self.channels_names[sub_channel]}*: " \
-                                f"{len(self.summary_data[channel][f'i_{sub_channel}'].dropna())}\n"
-                info += f" - *Concentration*: {self.concentration.get(channel, 0):.2E} pcles/ml"
-                info += '\n\n'
-            f.write(info)
+
+            f.write(self.generate_info_summary())
 
         with open(filename.with_suffix('.yml'), 'w') as f:
             yaml.dump(self.metadata, f)
 
+    def generate_info_summary(self):
+        info = ""
+        for channel in range(self.num_channels):
+            info += f"# Channel {self.channels_names[channel]}\n\n"
+            info += f" - *Found particles*: {len(self.summary_data[channel])}\n"
+            if self.num_channels > 1:
+                for sub_channel in range(self.num_channels):
+                    info += f" - Particles also in *{self.channels_names[sub_channel]}*: " \
+                            f"{len(self.summary_data[channel][f'i_{sub_channel}'].dropna())}\n"
+            info += f" - *Concentration*: {self.concentration.get(channel, 0):.2E} pcles/ml"
+            info += '\n\n'
+        return info
     def calculate_concentration(self, step_size=5):
         """ Calculates the concentration on each channel in the dataset. After linking the particles,
         the concentration is calculated by simply counting the number of detections and dividing by the volume. The
         volume is derived from the field of view (given a magnification and sensor size) and the third dimension from
         the number of steps and the step size.
 
         TODO: Real-space FOV is hard-coded (as well as the region in the edges of the image that is discarded).
         """
+        self.metadata.update({'step_size': step_size})
         self.total_num_particles = {}
         self.concentration = {}
         if self.linked_particles is None:
             return
         fraction_sensor_used = (2048 - self.ignore_edge_pixels) / 2048
         field_of_view = fraction_sensor_used * (13.3 / 20) ** 2  # (Sensor size/magnification) # mm2
         for channel in range(self.num_channels):
```

### Comparing `nanoqnt-0.2.1/nanoqnt/util/make_hdf5.py` & `nanoqnt-0.2.2/nanoqnt/util/make_hdf5.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11813 - Amplifier.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11814 - Atom.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11814 - Atom.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11815 - Battery.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11815 - Battery.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11816 - Orbit.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11816 - Orbit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11817 - Beaker.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11817 - Beaker.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11818 - Black Hole.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11819 - Bounce.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11819 - Bounce.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11820 - Caliper.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11820 - Caliper.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11821 - Catapult.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11821 - Catapult.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11822 - Collision.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11822 - Collision.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11823 - Communicating Vessels.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11824 - Cylinder.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11825 - Dispersion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11826 - Elasticity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11827 - Electrical Circuit.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11828 - Energy.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11828 - Energy.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11829 - Flask.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11829 - Flask.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11830 - Float.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11830 - Float.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11831 - Fluid Mechanics.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11832 - Force.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11832 - Force.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11833 - Formula.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11833 - Formula.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11834 - Gears.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11834 - Gears.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11835 - Gravity.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11835 - Gravity.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11836 - Gyroscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11837 - Histogram.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11837 - Histogram.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11838 - Law Of Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11839 - Magnet.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11839 - Magnet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11840 - Magnetic Field.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11841 - Metronome.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11841 - Metronome.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11842 - Micrometer.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11843 - Molecule.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11843 - Molecule.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11844 - Motion.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11844 - Motion.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11845 - Nuclear.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11846 - Oscilloscope.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11847 - Pendulum.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11848 - Planet.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11848 - Planet.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11849 - Plasma Ball.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11850 - Power.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11850 - Power.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11851 - Press.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11851 - Press.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11852 - Proton.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11852 - Proton.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11853 - Pulley.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11853 - Pulley.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11854 - Reflection.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11854 - Reflection.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11855 - Resistor.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11855 - Resistor.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11856 - Rolling.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11856 - Rolling.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11857 - Rotate.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11857 - Rotate.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11858 - Seesaw.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11859 - Temperature.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11859 - Temperature.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11860 - Voltmeter.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11861 - Waves.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11861 - Waves.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/11862 - Weight Scale.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/Icons/Save.svg` & `nanoqnt-0.2.2/nanoqnt/view/GUI/Icons/Save.svg`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/channel_selector.ui` & `nanoqnt-0.2.2/nanoqnt/view/GUI/channel_selector.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/data_exploration.ui` & `nanoqnt-0.2.2/nanoqnt/view/GUI/data_exploration.ui`

 * *Files 1% similar despite different names*

#### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/data_exploration.ui` & `nanoqnt-0.2.2/nanoqnt/view/GUI/data_exploration.ui`

```diff
@@ -41,24 +41,14 @@
               </property>
               <property name="rightMargin">
                 <number>0</number>
               </property>
               <property name="bottomMargin">
                 <number>0</number>
               </property>
-              <item row="0" column="0" colspan="2">
-                <widget class="QCheckBox" name="find_particles_check">
-                  <property name="toolTip">
-                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Whether to mark the particles on the images&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                  </property>
-                  <property name="text">
-                    <string>Find Particles</string>
-                  </property>
-                </widget>
-              </item>
               <item row="1" column="0">
                 <widget class="QLabel" name="label_9">
                   <property name="text">
                     <string>Frame Range</string>
                   </property>
                   <property name="buddy">
                     <cstring>start_frame_line</cstring>
@@ -170,47 +160,57 @@
               <item row="9" column="0" colspan="2">
                 <widget class="Line" name="line">
                   <property name="orientation">
                     <enum>Qt::Horizontal</enum>
                   </property>
                 </widget>
               </item>
-              <item row="10" column="0">
+              <item row="11" column="0">
                 <widget class="QLabel" name="label_8">
                   <property name="text">
                     <string>Step Size (µm)</string>
                   </property>
                   <property name="buddy">
                     <cstring>step_size_line</cstring>
                   </property>
                 </widget>
               </item>
-              <item row="10" column="1">
+              <item row="11" column="1">
                 <widget class="QLineEdit" name="step_size_line">
                   <property name="toolTip">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Step size during the scan&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                   <property name="text">
                     <string>5</string>
                   </property>
                 </widget>
               </item>
-              <item row="11" column="1">
+              <item row="12" column="1">
                 <spacer name="verticalSpacer">
                   <property name="orientation">
                     <enum>Qt::Vertical</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
                       <width>20</width>
                       <height>40</height>
                     </size>
                   </property>
                 </spacer>
               </item>
+              <item row="10" column="0">
+                <widget class="QCheckBox" name="find_particles_check">
+                  <property name="toolTip">
+                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Whether to mark the particles on the images&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                  </property>
+                  <property name="text">
+                    <string>Find Particles</string>
+                  </property>
+                </widget>
+              </item>
             </layout>
           </widget>
         </item>
         <item>
           <widget class="QWidget" name="widget" native="true">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Preferred">
@@ -309,15 +309,15 @@
       <attribute name="toolBarArea">
         <enum>TopToolBarArea</enum>
       </attribute>
       <attribute name="toolBarBreak">
         <bool>false</bool>
       </attribute>
       <addaction name="action_open"/>
-      <addaction name="action_mass_histogram"/>
+      <addaction name="action_data_vis"/>
       <addaction name="action_data_plots"/>
       <addaction name="action_save_data"/>
     </widget>
     <widget class="QMenuBar" name="menuBar">
       <property name="geometry">
         <rect>
           <x>0</x>
@@ -366,26 +366,26 @@
       <property name="toolTip">
         <string>Open data file</string>
       </property>
       <property name="shortcut">
         <string>Ctrl+O</string>
       </property>
     </action>
-    <action name="action_mass_histogram">
+    <action name="action_data_vis">
       <property name="icon">
         <iconset>
           <normaloff>Icons/11837 - Histogram.svg</normaloff>
           Icons/11837 - Histogram.svg
         </iconset>
       </property>
       <property name="text">
-        <string>Mass Histogram</string>
+        <string>Open Data Vis Window</string>
       </property>
       <property name="toolTip">
-        <string>Histogram of Intensities for the current frame</string>
+        <string>Opens the tools to visualize results</string>
       </property>
     </action>
     <action name="action_data_frame">
       <property name="icon">
         <iconset>
           <normaloff>Icons/11831 - Fluid Mechanics.svg</normaloff>
           Icons/11831 - Fluid Mechanics.svg
@@ -471,15 +471,14 @@
     <action name="action_show_bkg">
       <property name="text">
         <string>Show Background</string>
       </property>
     </action>
   </widget>
   <tabstops>
-    <tabstop>find_particles_check</tabstop>
     <tabstop>start_frame_line</tabstop>
     <tabstop>end_frame_line</tabstop>
     <tabstop>engine_box</tabstop>
     <tabstop>search_radius_line</tabstop>
     <tabstop>min_frames_line</tabstop>
     <tabstop>calculate_button</tabstop>
     <tabstop>step_size_line</tabstop>
```

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/particles_widget.ui` & `nanoqnt-0.2.2/nanoqnt/view/GUI/particles_widget.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/GUI/scan_control.ui` & `nanoqnt-0.2.2/nanoqnt/view/GUI/scan_control.ui`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/nanoqnt/view/main_window.py` & `nanoqnt-0.2.2/nanoqnt/view/main_window.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import pyqtgraph as pg
 from PyQt5 import uic
-from PyQt5.QtCore import Qt
+from PyQt5.QtCore import Qt, QThread
 from PyQt5.QtWidgets import QApplication, QFileDialog, QMainWindow, QMessageBox
 
 from nanoqnt.view import VIEW_FOLDER
 from nanoqnt.view.channel_selector import ChannelSelector
 from nanoqnt.view.particle_widget import ParticleWidget
+from nanoqnt.view.results_vis import DataVis
 
 home_path = Path.home()
 
 
 class NanoQNTMainWindow(QMainWindow):
     def __init__(self, model=None):
         """
         :param AnalyzeNanoQNT model: Model used to analyze the data
         """
         super().__init__(parent=None)
         uic.loadUi(str(VIEW_FOLDER / 'GUI' / 'data_exploration.ui'), self)
         self.setWindowTitle('NanoQNT Analysis')
 
         self.analyze_model = model
+        self.channel_widget = ChannelSelector()
+        self.data_vis_window = DataVis(analyze_model=model)
 
         self.action_open.triggered.connect(self.open)
-        self.action_mass_histogram.triggered.connect(self.histogram_mass)
+        self.action_data_vis.triggered.connect(self.data_vis_window.show)
         self.action_data_frame.triggered.connect(self.data_over_frame)
         self.action_data_plots.triggered.connect(self.total_histograms)
         self.action_export_all_data.triggered.connect(self.export_all_data)
         self.action_save_data.triggered.connect(self.export_data)
         self.action_calculate_bkg.triggered.connect(self.calculate_background)
         self.action_show_bkg.triggered.connect(self.show_background)
 
@@ -38,31 +41,33 @@
         self.find_particles_check.toggled.connect(self.update_images)
         self.calculate_button.clicked.connect(self.calculate_all)
         self.action_about.triggered.connect(self.show_about)
 
         self.circles = []
         self.curr_index = 0
 
-        self.channel_widget = ChannelSelector()
+
         self.channel_widget.accept_button.clicked.connect(self.channels_updated)
 
         self.nanoqnt_images = []
 
     def open(self):
         last_dir = self.analyze_model.metadata.get('last_dir', home_path)
         file = QFileDialog.getOpenFileName(self, 'Open Data', str(last_dir), filter='*.tif')[0]
         if file != '':
             file = Path(file)
         else:
             return
 
+        self.analyze_model.open(str(file))
+        self.channel_widget.update_info(self.analyze_model.num_channels, self.analyze_model.channels_names)
         self.channel_widget.show()
 
-        self.analyze_model.open(str(file))
         self.setWindowTitle(f'NanoQNT Analysis: {file.name}')
+        self.step_size_line.setText(str(self.analyze_model.step_size))
 
     def update_slider(self, index):
         self.curr_index = index - 1
         self.frame_num.setText(str(index))
         self.update_images()
 
     def update_images(self, auto_range=False, auto_levels=False):
@@ -98,28 +103,37 @@
         self.analyze_model.find_particles(index, diameter, minmass)
 
         fig, ax = plt.subplots(1)
         ax.hist(self.analyze_model.particle_df[index]['mass'], bins=50)
         fig.suptitle(f'Mass Histogram Frame Number: {self.curr_index}')
         fig.show()
 
-    def calculate_all(self):
+    def start_calculate_all(self):
         QApplication.setOverrideCursor(Qt.BusyCursor)
+
+
+        self.calculate_thread = QThread.create(self.calculate_all)
+        self.calculate_thread.finished.connect(self.calculate_finish)
+        self.calculate_thread.start()
+
+    def calculate_finish(self):
+        QApplication.setOverrideCursor(Qt.ArrowCursor)
+
+    def calculate_all(self):
         diameter = [int(channel_image.size_line.text()) for channel_image in self.nanoqnt_images]
         minmass = [int(channel_image.min_mass_line.text()) for channel_image in self.nanoqnt_images]
         engine = self.engine_box.currentText()
         frames_no = [int(self.start_frame_line.text()) - 1, int(self.end_frame_line.text())]
         self.analyze_model.find_all_particles(frames_no, diameter, minmass, engine)
         search_radius = int(self.search_radius_line.text())
         min_frames = int(self.min_frames_line.text())
         self.analyze_model.link_particles(search_radius, memory=0, min_frames=min_frames)
         self.analyze_model.calculate_intensities()
         self.analyze_model.multi_color_link()
         self.calculate_concentration()
-        QApplication.setOverrideCursor(Qt.ArrowCursor)
 
     def data_over_frame(self):
         t1 = self.analyze_model.linked_particles
 
         fig, ax = plt.subplots(3, sharex=True)
         ax[0].plot(t1['ecc'].groupby('frame').mean())
         ax[0].set_ylabel('Eccentricity')
```

### Comparing `nanoqnt-0.2.1/nanoqnt/view/particle_widget.py` & `nanoqnt-0.2.2/nanoqnt/view/particle_widget.py`

 * *Files identical despite different names*

### Comparing `nanoqnt-0.2.1/pyproject.toml` & `nanoqnt-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanoqnt"
-version = "0.2.1"
+version = "0.2.2"
 description = "Software for analysing the data generated with the nanoQNT device. It includes a practical GUI as well as a module that can be extended and used in custom scripts. "
 authors = ["Aquiles Carattino <carattino@dispertech.com>"]
 maintainers = ["Aron Opheij <opheij@dispertech.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 homepage = "https://www.dispertech.com"
 repository = "https://www.github.com/dispertech/NanoQNTPy"
@@ -14,16 +14,14 @@
     "Environment :: MacOS X",
     "Environment :: Win32 (MS Windows)",
     "Environment :: X11 Applications :: Qt",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "Operating System :: MacOS :: MacOS X",
-
-
 ]
 [tool.poetry.dependencies]
 python = ">3.9, <3.12"
 pyqtgraph = "^0.13.3"
 numpy = "~1.24"
 scipy = "~1.10.1"
 scikit-image = "^0.21"
@@ -32,16 +30,17 @@
 h5py = "^3.8.0"
 matplotlib = "^3.7.1"
 pyqt5 = "^5.15"
 pyyaml = "^6.0"
 numba = "^0.57.0"
 pandas = "^2.0.2"
 
+
 [tool.poetry.scripts]
 nanoqnt = 'nanoqnt.main:start_nanoqnt'
 
 [tool.poetry.group.dev.dependencies]
 pyinstaller = "^5.10.1"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nanoqnt-0.2.1/PKG-INFO` & `nanoqnt-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoqnt
-Version: 0.2.1
+Version: 0.2.2
 Summary: Software for analysing the data generated with the nanoQNT device. It includes a practical GUI as well as a module that can be extended and used in custom scripts. 
 Home-page: https://www.dispertech.com
 License: GPL-3.0
 Keywords: extracellular vesicles,light-sheet microscopy,data analysis
 Author: Aquiles Carattino
 Author-email: carattino@dispertech.com
 Maintainer: Aron Opheij
```

