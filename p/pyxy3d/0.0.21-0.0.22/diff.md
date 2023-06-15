# Comparing `tmp/pyxy3d-0.0.21.tar.gz` & `tmp/pyxy3d-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.0.21.tar", max compression
+gzip compressed data, was "pyxy3d-0.0.22.tar", max compression
```

## Comparing `pyxy3d-0.0.21.tar` & `pyxy3d-0.0.22.tar`

### file list

```diff
@@ -1,233 +1,233 @@
--rw-r--r--   0        0        0    35184 2023-03-13 23:46:36.918754 pyxy3d-0.0.21/LICENSE.md
--rw-r--r--   0        0        0      925 2023-06-12 22:16:34.127513 pyxy3d-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     2007 2023-05-20 12:18:55.240529 pyxy3d-0.0.21/pyxy3d/__init__.py
--rw-r--r--   0        0        0      934 2023-06-12 22:15:42.388447 pyxy3d-0.0.21/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.0.21/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.21/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.0.21/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.0.21/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0    11255 2023-06-10 20:05:09.592548 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.0.21/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.0.21/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.0.21/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.0.21/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    15573 2023-06-10 20:04:49.722607 pyxy3d-0.0.21/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.0.21/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.0.21/pyxy3d/export.py
--rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5684 2023-06-12 18:45:02.565389 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
--rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8098 2023-06-12 18:45:07.819053 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0    10204 2023-06-12 18:45:08.757113 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
--rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0    11941 2023-06-12 18:45:08.751113 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.0.21/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0     7438 2023-06-12 22:15:42.390444 pyxy3d-0.0.21/pyxy3d/gui/calibration_widget.py
--rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.0.21/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.0.21/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.0.21/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    10279 2023-06-12 16:49:05.520130 pyxy3d-0.0.21/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0     9807 2023-06-02 14:30:41.606273 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    14193 2023-06-02 00:29:03.392704 pyxy3d-0.0.21/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.21/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.0.21/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    14273 2023-06-12 16:49:05.521130 pyxy3d-0.0.21/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.0.21/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.0.21/pyxy3d/gui/playback_widget.py
--rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.0.21/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.0.21/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    14618 2023-06-12 16:49:05.522130 pyxy3d-0.0.21/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.0.21/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.0.21/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.0.21/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.0.21/pyxy3d/helper.py
--rw-r--r--   0        0        0     6646 2023-06-01 14:21:56.755811 pyxy3d-0.0.21/pyxy3d/interface.py
--rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.0.21/pyxy3d/logger.py
--rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.0.21/pyxy3d/post_processor.py
--rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.0.21/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.0.21/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.0.21/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
--rw-r--r--   0        0        0    15728 2023-06-12 22:04:21.160455 pyxy3d-0.0.21/pyxy3d/session/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0    20849 2023-06-12 22:15:55.087470 pyxy3d-0.0.21/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.0.21/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
--rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.0.21/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.0.21/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.0.21/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.0.21/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.0.21/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.0.21/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.0.21/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
--rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
--rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
--rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
--rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
--rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
--rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
--rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
--rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
--rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
--rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
--rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
--rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
--rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
--rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
--rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
--rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
--rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
--rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
--rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
--rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
--rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
--rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
--rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
--rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.0.21/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.0.21/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.0.21/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     9401 2023-06-12 22:15:42.383443 pyxy3d-0.0.21/README.md
--rw-r--r--   0        0        0    10203 1970-01-01 00:00:00.000000 pyxy3d-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.0.22/LICENSE.md
+-rw-r--r--   0        0        0      925 2023-06-15 18:45:52.069743 pyxy3d-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     2007 2023-05-20 12:18:55.240529 pyxy3d-0.0.22/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-12 22:15:42.388447 pyxy3d-0.0.22/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.0.22/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.22/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.0.22/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.0.22/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     9900 2023-06-15 18:19:09.634902 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.0.22/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.0.22/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.0.22/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.0.22/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    13543 2023-06-15 18:45:15.726954 pyxy3d-0.0.22/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.0.22/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.0.22/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5691 2023-06-15 17:55:45.122373 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8558 2023-06-15 17:55:46.699957 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    11710 2023-06-15 18:19:11.391906 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    11942 2023-06-15 17:55:47.202676 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.0.22/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0     7459 2023-06-15 18:45:15.727954 pyxy3d-0.0.22/pyxy3d/gui/calibration_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.0.22/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.0.22/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.0.22/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.0.22/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.0.22/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.0.22/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9669 2023-06-15 17:02:49.032222 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.0.22/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.22/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.22/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.22/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.0.22/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    16047 2023-06-15 18:45:15.731956 pyxy3d-0.0.22/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.0.22/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.0.22/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.0.22/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.0.22/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    14740 2023-06-15 18:45:15.732954 pyxy3d-0.0.22/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.0.22/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.0.22/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.0.22/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.0.22/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.0.22/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.0.22/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.0.22/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.0.22/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.22/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.0.22/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.22/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.0.22/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.0.22/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.0.22/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    16304 2023-06-15 17:47:03.005005 pyxy3d-0.0.22/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    21437 2023-06-15 18:45:15.733955 pyxy3d-0.0.22/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.0.22/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.0.22/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.0.22/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.0.22/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.0.22/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.0.22/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.0.22/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.0.22/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.0.22/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.0.22/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.0.22/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     5883 2023-06-15 18:45:15.718953 pyxy3d-0.0.22/README.md
+-rw-r--r--   0        0        0     6737 1970-01-01 00:00:00.000000 pyxy3d-0.0.22/PKG-INFO
```

### Comparing `pyxy3d-0.0.21/LICENSE.md` & `pyxy3d-0.0.22/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+
+
                     GNU AFFERO GENERAL PUBLIC LICENSE
                        Version 3, 19 November 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
```

### Comparing `pyxy3d-0.0.21/pyproject.toml` & `pyxy3d-0.0.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.0.21"
+version = "0.0.22"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
```

### Comparing `pyxy3d-0.0.21/pyxy3d/__init__.py` & `pyxy3d-0.0.22/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/__main__.py` & `pyxy3d-0.0.22/pyxy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.0.22/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/charuco.py` & `pyxy3d-0.0.22/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.0.22/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.0.22/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.0.22/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun 10 20:04:49 2023 UTC, .py size: 15573 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,704 +1,691 @@
-00000000: 6f0d 0d0a 0000 0000 61d7 8464 d53c 0000  o.......a..d.<..
+00000000: 550d 0d0a 0000 0000 384a 3864 fa38 0000  U.......8J8d.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 3602 0000 6400  .....@...s6...d.
+00000020: 0009 0000 0040 0000 0073 5002 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
-00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
-00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
-00000060: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6401 6c0e  m.Z.m.Z...d.d.l.
-00000080: 5a0e 6400 6401 6c0f 5a10 6400 6405 6c11  Z.d.d.l.Z.d.d.l.
-00000090: 6d12 5a12 0100 6406 5a13 4700 6407 6408  m.Z...d.Z.G.d.d.
-000000a0: 8400 6408 8302 5a14 6504 6409 6b02 9001  ..d...Z.e.d.k...
-000000b0: 7219 6400 640a 6c15 6d16 5a16 0100 6400  r.d.d.l.m.Z...d.
-000000c0: 640b 6c17 6d18 5a18 0100 6400 640c 6c19  d.l.m.Z...d.d.l.
-000000d0: 6d1a 5a1a 6d1b 5a1b 0100 6400 640d 6c1c  m.Z.m.Z...d.d.l.
-000000e0: 6d1d 5a1d 0100 6400 6401 6c06 5a06 6400  m.Z...d.d.l.Z.d.
-000000f0: 640e 6c01 6d1e 5a1e 0100 640f 5a1f 651f  d.l.m.Z...d.Z.e.
-00000100: 7295 6508 651e 6410 6411 8303 5a20 651d  r.e.e.d.d...Z e.
-00000110: 6520 8301 5a21 6521 a022 a100 0100 6521  e ..Z!e!."....e!
-00000120: 6a23 a024 a100 4400 5d0a 5c02 5a25 5a26  j#.$..D.].\.Z%Z&
-00000130: 6412 6526 5f27 6412 6526 5f28 717d 6502  d.e&_'d.e&_(q}e.
-00000140: a029 6413 a101 0100 6514 6521 6a23 6414  .)d.....e.e!j#d.
-00000150: 6415 8d02 5a2a 6e2d 6700 6416 a201 5a2b  d...Z*n-g.d...Z+
-00000160: 6508 651e 6410 6417 6411 8304 5a2c 6516  e.e.d.d.d...Z,e.
-00000170: 6418 6414 6419 641a 641b 641c 6412 641d  d.d.d.d.d.d.d.d.
-00000180: 8d07 5a2d 651b 652b 652c 652d 641e 8d03  ..Z-e.e+e,e-d...
-00000190: 5a2e 6502 a029 6413 a101 0100 6514 652e  Z.e..)d.....e.e.
-000001a0: 6a23 641f 6415 8d02 5a2a 652e a02f a100  j#d.d...Z*e../..
-000001b0: 0100 650a 8300 5a30 652a a031 6530 a101  ..e...Z0e*.1e0..
-000001c0: 0100 6502 a029 6420 6506 a032 a100 9b00  ..e..)d e..2....
-000001d0: 9d02 a101 0100 652a 6a33 a034 a100 9001  ......e*j3.4....
-000001e0: 730d 6530 a003 a100 5a35 652a 6a36 5a37  s.e0....Z5e*j6Z7
-000001f0: 6537 6a38 a024 a100 4400 5d10 5c02 5a25  e7j8.$..D.].\.Z%
-00000200: 5a39 6539 72f6 650e a03a 6421 6525 9b00  Z9e9r.e..:d!e%..
-00000210: 9d02 6539 6a3b a102 0100 71e6 650e a03c  ..e9j;....q.e..<
-00000220: 6422 a101 5a3d 653d 653e 6423 8301 6b02  d"..Z=e=e>d#..k.
-00000230: 9001 7208 650e a03f a100 0100 6e05 652a  ..r.e..?....n.e*
-00000240: 6a33 a034 a100 72da 6502 a029 6424 6506  j3.4..r.e..)d$e.
-00000250: a032 a100 9b00 9d02 a101 0100 6401 5300  .2..........d.S.
-00000260: 6401 5300 2925 e900 0000 004e 2901 da04  d.S.)%.....N)...
-00000270: 5061 7468 2901 da05 5175 6575 6529 02da  Path)...Queue)..
-00000280: 0654 6872 6561 64da 0545 7665 6e74 2901  .Thread..Event).
-00000290: da0a 5379 6e63 5061 636b 6574 e964 0000  ..SyncPacket.d..
-000002a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000002b0: 0000 0400 0000 4000 0000 73be 0000 0065  ......@...s....e
-000002c0: 005a 0164 005a 0264 2d64 0265 0366 0264  .Z.d.Z.d-d.e.f.d
-000002d0: 0364 0484 055a 0464 0565 0566 0264 0664  .d...Z.d.e.f.d.d
-000002e0: 0784 045a 0664 0864 0984 005a 0765 0864  ...Z.d.d...Z.e.d
-000002f0: 0a64 0b84 0083 015a 0964 0c64 0d84 005a  .d.....Z.d.d...Z
-00000300: 0a64 0e64 0f84 005a 0b64 1064 1184 005a  .d.d...Z.d.d...Z
-00000310: 0c64 1264 1384 005a 0d64 1464 1584 005a  .d.d...Z.d.d...Z
-00000320: 0e64 1664 1784 005a 0f64 1864 1984 005a  .d.d...Z.d.d...Z
-00000330: 1064 1a64 1b84 005a 1164 1c64 1d84 005a  .d.d...Z.d.d...Z
-00000340: 1264 1e64 1f84 005a 1364 2064 2184 005a  .d.d...Z.d d!..Z
-00000350: 1464 2264 2384 005a 1564 2464 2584 005a  .d"d#..Z.d$d%..Z
-00000360: 1664 2664 2784 005a 1764 2864 2984 005a  .d&d'..Z.d(d)..Z
-00000370: 1864 2a64 2b84 005a 1964 2c53 0029 2eda  .d*d+..Z.d,S.)..
-00000380: 0c53 796e 6368 726f 6e69 7a65 72e9 0600  .Synchronizer...
-00000390: 0000 da07 7374 7265 616d 7363 0300 0000  ....streamsc....
-000003a0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
-000003b0: 4300 0000 73b2 0000 007c 017c 005f 0064  C...s....|.|._.d
-000003c0: 007c 005f 0167 007c 005f 0267 007c 005f  .|._.g.|._.g.|._
-000003d0: 0369 007c 005f 0474 0583 007c 005f 0664  .i.|._.t...|._.d
-000003e0: 017c 005f 0767 007c 005f 0869 007c 005f  .|._.g.|._.i.|._
-000003f0: 097c 006a 00a0 0aa1 0044 005d 135c 027d  .|.j.....D.].\.}
-00000400: 037d 047c 006a 08a0 0b7c 03a1 0101 0074  .}.|.j...|.....t
-00000410: 0c64 0283 017d 057c 057c 006a 097c 033c  .d...}.|.|.j.|.<
-00000420: 0071 2164 017c 005f 0d7c 00a0 0ea1 0001  .q!d.|._.|......
-00000430: 007c 00a0 0f7c 02a1 0101 007c 027c 005f  .|...|.....|.|._
-00000440: 1064 0364 0484 0074 117c 006a 0883 0144  .d.d...t.|.j...D
-00000450: 0083 017c 005f 127c 00a0 13a1 0001 007c  ...|._.|.......|
-00000460: 00a0 14a1 0001 0064 0053 0029 054e 46e9  .......d.S.).NF.
-00000470: ffff ffff 6301 0000 0000 0000 0000 0000  ....c...........
-00000480: 0002 0000 0004 0000 0053 0000 0073 1200  .........S...s..
-00000490: 0000 6900 7c00 5d05 7d01 7c01 6700 9302  ..i.|.].}.|.g...
-000004a0: 7102 5300 a900 720c 0000 00a9 02da 022e  q.S...r.........
-000004b0: 30da 0470 6f72 7472 0c00 0000 720c 0000  0..portr....r...
-000004c0: 00fa 3f43 3a5c 5573 6572 735c 4d61 6320  ..?C:\Users\Mac 
-000004d0: 5072 6962 6c65 5c72 6570 6f73 5c70 7978  Prible\repos\pyx
-000004e0: 7933 645c 7079 7879 3364 5c63 616d 6572  y3d\pyxy3d\camer
-000004f0: 6173 5c73 796e 6368 726f 6e69 7a65 722e  as\synchronizer.
-00000500: 7079 da0a 3c64 6963 7463 6f6d 703e 3100  py..<dictcomp>1.
-00000510: 0000 f302 0000 0012 007a 2953 796e 6368  .........z)Synch
-00000520: 726f 6e69 7a65 722e 5f5f 696e 6974 5f5f  ronizer.__init__
-00000530: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00000540: 6f6d 703e 2915 720a 0000 005a 1663 7572  omp>).r....Z.cur
-00000550: 7265 6e74 5f73 796e 6368 6564 5f66 7261  rent_synched_fra
-00000560: 6d65 73da 1773 796e 635f 6e6f 7469 6365  mes..sync_notice
-00000570: 5f73 7562 7363 7269 6265 7273 da1a 7379  _subscribers..sy
-00000580: 6e63 6865 645f 6672 616d 6573 5f73 7562  nched_frames_sub
-00000590: 7363 7269 6265 7273 da11 616c 6c5f 6672  scribers..all_fr
-000005a0: 616d 655f 7061 636b 6574 7372 0500 0000  ame_packetsr....
-000005b0: da0a 7374 6f70 5f65 7665 6e74 da0f 6672  ..stop_event..fr
-000005c0: 616d 6573 5f63 6f6d 706c 6574 65da 0570  ames_complete..p
-000005d0: 6f72 7473 da13 6672 616d 655f 7061 636b  orts..frame_pack
-000005e0: 6574 5f71 7565 7565 73da 0569 7465 6d73  et_queues..items
-000005f0: da06 6170 7065 6e64 7203 0000 00da 1573  ..appendr......s
-00000600: 7562 7363 7269 6265 645f 746f 5f73 7472  ubscribed_to_str
-00000610: 6561 6d73 da14 7375 6273 6372 6962 655f  eams..subscribe_
-00000620: 746f 5f73 7472 6561 6d73 da0e 7365 745f  to_streams..set_
-00000630: 7374 7265 616d 5f66 7073 da08 6670 735f  stream_fps..fps_
-00000640: 6d65 616e da06 736f 7274 6564 da15 6472  mean..sorted..dr
-00000650: 6f70 7065 645f 6672 616d 655f 6869 7374  opped_frame_hist
-00000660: 6f72 79da 1269 6e69 7469 616c 697a 655f  ory..initialize_
-00000670: 6c65 6467 6572 73da 0573 7461 7274 2906  ledgers..start).
-00000680: da04 7365 6c66 720a 0000 00da 0a66 7073  ..selfr......fps
-00000690: 5f74 6172 6765 7472 0f00 0000 da06 7374  _targetr......st
-000006a0: 7265 616d da01 7172 0c00 0000 720c 0000  ream..qr....r...
-000006b0: 0072 1000 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
-000006c0: 1400 0000 732c 0000 0006 0106 0102 0304  ....s,..........
-000006d0: ff02 0404 ff06 0408 0106 0106 0206 0112  ................
-000006e0: 010c 0108 010c 0106 0208 010a 0206 0116  ................
-000006f0: 0308 020c 017a 1553 796e 6368 726f 6e69  .....z.Synchroni
-00000700: 7a65 722e 5f5f 696e 6974 5f5f da05 7472  zer.__init__..tr
-00000710: 6163 6b63 0200 0000 0000 0000 0000 0000  ackc............
-00000720: 0400 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
-00000730: 007c 006a 00a0 01a1 0044 005d 095c 027d  .|.j.....D.].\.}
-00000740: 027d 037c 03a0 027c 01a1 0101 0071 0564  .}.|...|.....q.d
-00000750: 0053 00a9 014e 2903 720a 0000 0072 1a00  .S...N).r....r..
-00000760: 0000 da0f 7365 745f 7472 6163 6b69 6e67  ....set_tracking
-00000770: 5f6f 6e29 0472 2400 0000 7229 0000 0072  _on).r$...r)...r
-00000780: 0f00 0000 7226 0000 0072 0c00 0000 720c  ....r&...r....r.
-00000790: 0000 0072 1000 0000 da17 7365 745f 7472  ...r......set_tr
-000007a0: 6163 6b69 6e67 5f6f 6e5f 7374 7265 616d  acking_on_stream
-000007b0: 7336 0000 0073 0600 0000 1201 0c01 04ff  s6...s..........
-000007c0: 7a24 5379 6e63 6872 6f6e 697a 6572 2e73  z$Synchronizer.s
-000007d0: 6574 5f74 7261 636b 696e 675f 6f6e 5f73  et_tracking_on_s
-000007e0: 7472 6561 6d73 6301 0000 0000 0000 0000  treamsc.........
-000007f0: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
-00000800: 4800 0000 7c00 6a00 6a01 7d01 7c01 a002  H...|.j.j.}.|...
-00000810: a100 4400 5d19 5c02 7d02 7d03 7c00 6a03  ..D.].\.}.}.|.j.
-00000820: 7c02 1900 a004 7c03 a101 0100 7c00 6a03  |.....|.....|.j.
-00000830: 7c02 1900 7405 0b00 6400 8502 1900 7c00  |...t...d.....|.
-00000840: 6a03 7c02 3c00 7108 6400 5300 722a 0000  j.|.<.q.d.S.r*..
-00000850: 0029 06da 1363 7572 7265 6e74 5f73 796e  .)...current_syn
-00000860: 635f 7061 636b 6574 da07 6472 6f70 7065  c_packet..droppe
-00000870: 6472 1a00 0000 7221 0000 0072 1b00 0000  dr....r!...r....
-00000880: da1a 4452 4f50 5045 445f 4652 414d 455f  ..DROPPED_FRAME_
-00000890: 5452 4143 4b5f 5749 4e44 4f57 2904 7224  TRACK_WINDOW).r$
-000008a0: 0000 005a 0f63 7572 7265 6e74 5f64 726f  ...Z.current_dro
-000008b0: 7070 6564 720f 0000 0072 2e00 0000 720c  ppedr....r....r.
-000008c0: 0000 0072 0c00 0000 7210 0000 00da 1c75  ...r....r......u
-000008d0: 7064 6174 655f 6472 6f70 7065 645f 6672  pdate_dropped_fr
-000008e0: 616d 655f 6869 7374 6f72 793a 0000 0073  ame_history:...s
-000008f0: 0a00 0000 0801 1002 1001 1c01 04fe 7a29  ..............z)
-00000900: 5379 6e63 6872 6f6e 697a 6572 2e75 7064  Synchronizer.upd
-00000910: 6174 655f 6472 6f70 7065 645f 6672 616d  ate_dropped_fram
-00000920: 655f 6869 7374 6f72 7963 0100 0000 0000  e_historyc......
-00000930: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000940: 0000 7314 0000 0064 0164 0284 007c 006a  ..s....d.d...|.j
-00000950: 00a0 01a1 0044 0083 0153 0029 037a 4a0a  .....D...S.).zJ.
-00000960: 2020 2020 2020 2020 4176 6572 6167 6573          Averages
-00000970: 2064 726f 7070 6564 2066 7261 6d65 2063   dropped frame c
-00000980: 6f75 6e74 2061 6372 6f73 7320 7468 6520  ount across the 
-00000990: 6f62 7365 7276 6564 2068 6973 746f 7279  observed history
-000009a0: 0a20 2020 2020 2020 2063 0100 0000 0000  .        c......
-000009b0: 0000 0000 0000 0300 0000 0600 0000 5300  ..............S.
-000009c0: 0000 731c 0000 0069 007c 005d 0a5c 027d  ..s....i.|.].\.}
-000009d0: 017d 027c 0174 00a0 017c 02a1 0193 0271  .}.|.t...|.....q
-000009e0: 0253 0072 0c00 0000 2902 da02 6e70 da04  .S.r....)...np..
-000009f0: 6d65 616e 2903 720e 0000 0072 0f00 0000  mean).r....r....
-00000a00: 5a0c 6472 6f70 5f68 6973 746f 7279 720c  Z.drop_historyr.
-00000a10: 0000 0072 0c00 0000 7210 0000 0072 1100  ...r....r....r..
-00000a20: 0000 4600 0000 7302 0000 001c 007a 2c53  ..F...s......z,S
-00000a30: 796e 6368 726f 6e69 7a65 722e 6472 6f70  ynchronizer.drop
-00000a40: 7065 645f 6670 732e 3c6c 6f63 616c 733e  ped_fps.<locals>
-00000a50: 2e3c 6469 6374 636f 6d70 3e29 0272 2100  .<dictcomp>).r!.
-00000a60: 0000 721a 0000 00a9 0172 2400 0000 720c  ..r......r$...r.
-00000a70: 0000 0072 0c00 0000 7210 0000 00da 0b64  ...r....r......d
-00000a80: 726f 7070 6564 5f66 7073 4100 0000 7302  ropped_fpsA...s.
-00000a90: 0000 0014 057a 1853 796e 6368 726f 6e69  .....z.Synchroni
-00000aa0: 7a65 722e 6472 6f70 7065 645f 6670 7363  zer.dropped_fpsc
-00000ab0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000ac0: 0400 0000 4300 0000 7338 0000 007c 017c  ....C...s8...|.|
-00000ad0: 005f 0074 01a0 0264 017c 019b 009d 02a1  ._.t...d.|......
-00000ae0: 0101 007c 006a 03a0 04a1 0044 005d 095c  ...|.j.....D.].\
-00000af0: 027d 027d 037c 03a0 057c 01a1 0101 0071  .}.}.|...|.....q
-00000b00: 1064 0053 0029 024e 7a2e 4174 7465 6d70  .d.S.).Nz.Attemp
-00000b10: 7469 6e67 2074 6f20 6368 616e 6765 2074  ting to change t
-00000b20: 6172 6765 7420 6670 7320 696e 2073 7472  arget fps in str
-00000b30: 6561 6d73 2074 6f20 2906 7225 0000 00da  eams to ).r%....
-00000b40: 066c 6f67 6765 72da 0469 6e66 6f72 0a00  .logger..infor..
-00000b50: 0000 721a 0000 00da 0e73 6574 5f66 7073  ..r......set_fps
-00000b60: 5f74 6172 6765 7429 0472 2400 0000 7225  _target).r$...r%
-00000b70: 0000 0072 0f00 0000 7226 0000 0072 0c00  ...r....r&...r..
-00000b80: 0000 720c 0000 0072 1000 0000 721e 0000  ..r....r....r...
-00000b90: 0049 0000 0073 0a00 0000 0601 1001 1201  .I...s..........
-00000ba0: 0c01 04ff 7a1b 5379 6e63 6872 6f6e 697a  ....z.Synchroniz
-00000bb0: 6572 2e73 6574 5f73 7472 6561 6d5f 6670  er.set_stream_fp
-00000bc0: 7363 0100 0000 0000 0000 0000 0000 0300  sc..............
-00000bd0: 0000 0500 0000 4300 0000 732e 0000 007c  ......C...s....|
-00000be0: 006a 00a0 01a1 0044 005d 0c5c 027d 017d  .j.....D.].\.}.}
-00000bf0: 027c 02a0 027c 006a 037c 0119 00a1 0101  .|...|.j.|......
-00000c00: 0071 0564 017c 005f 0464 0053 0029 024e  .q.d.|._.d.S.).N
-00000c10: 5429 0572 0a00 0000 721a 0000 00da 0973  T).r....r......s
-00000c20: 7562 7363 7269 6265 7219 0000 0072 1c00  ubscriber....r..
-00000c30: 0000 a903 7224 0000 0072 0f00 0000 7226  ....r$...r....r&
-00000c40: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-00000c50: 0000 721d 0000 004f 0000 0073 0600 0000  ..r....O...s....
-00000c60: 1201 1201 0a01 7a21 5379 6e63 6872 6f6e  ......z!Synchron
-00000c70: 697a 6572 2e73 7562 7363 7269 6265 5f74  izer.subscribe_t
-00000c80: 6f5f 7374 7265 616d 7363 0100 0000 0000  o_streamsc......
-00000c90: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000ca0: 0000 733e 0000 007c 006a 00a0 01a1 0044  ..s>...|.j.....D
-00000cb0: 005d 145c 027d 017d 0274 02a0 0364 017c  .].\.}.}.t...d.|
-00000cc0: 019b 009d 02a1 0101 007c 02a0 047c 006a  .........|...|.j
-00000cd0: 057c 0119 00a1 0101 0071 0564 027c 005f  .|.......q.d.|._
-00000ce0: 0664 0053 0029 034e 7a23 756e 7375 6273  .d.S.).Nz#unsubs
-00000cf0: 6372 6962 6520 7379 6e63 6872 6f6e 697a  cribe synchroniz
-00000d00: 6572 2066 726f 6d20 706f 7274 2046 2907  er from port F).
-00000d10: 720a 0000 0072 1a00 0000 7235 0000 0072  r....r....r5...r
-00000d20: 3600 0000 da0b 756e 7375 6273 6372 6962  6.....unsubscrib
-00000d30: 6572 1900 0000 721c 0000 0072 3900 0000  er....r....r9...
-00000d40: 720c 0000 0072 0c00 0000 7210 0000 00da  r....r....r.....
-00000d50: 1875 6e73 7562 7363 7269 6265 5f66 726f  .unsubscribe_fro
-00000d60: 6d5f 7374 7265 616d 7354 0000 0073 0800  m_streamsT...s..
-00000d70: 0000 1201 1001 1201 0a01 7a25 5379 6e63  ..........z%Sync
-00000d80: 6872 6f6e 697a 6572 2e75 6e73 7562 7363  hronizer.unsubsc
-00000d90: 7269 6265 5f66 726f 6d5f 7374 7265 616d  ribe_from_stream
-00000da0: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
-00000db0: 0000 0300 0000 4300 0000 732c 0000 007c  ......C...s,...|
-00000dc0: 006a 00a0 01a1 0001 007c 006a 02a0 03a1  .j.......|.j....
-00000dd0: 0001 007c 006a 0444 005d 067d 017c 01a0  ...|.j.D.].}.|..
-00000de0: 03a1 0001 0071 0d64 0053 0072 2a00 0000  .....q.d.S.r*...
-00000df0: 2905 7216 0000 00da 0373 6574 da06 7468  ).r......set..th
-00000e00: 7265 6164 da04 6a6f 696e da07 7468 7265  read..join..thre
-00000e10: 6164 7329 0272 2400 0000 da01 7472 0c00  ads).r$.....tr..
-00000e20: 0000 720c 0000 0072 1000 0000 da04 7374  ..r....r......st
-00000e30: 6f70 5a00 0000 730a 0000 000a 010a 010a  opZ...s.........
-00000e40: 010a 0104 ff7a 1153 796e 6368 726f 6e69  .....z.Synchroni
-00000e50: 7a65 722e 7374 6f70 6301 0000 0000 0000  zer.stopc.......
-00000e60: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000e70: 0073 2e00 0000 6401 6402 8400 7c00 6a00  .s....d.d...|.j.
-00000e80: 4400 8301 7c00 5f01 6403 6402 8400 7c00  D...|._.d.d...|.
-00000e90: 6a00 4400 8301 7c00 5f02 6700 7c00 5f03  j.D...|._.g.|._.
-00000ea0: 6400 5300 2904 4e63 0100 0000 0000 0000  d.S.).Nc........
-00000eb0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00000ec0: f312 0000 0069 007c 005d 057d 017c 0164  .....i.|.].}.|.d
-00000ed0: 0093 0271 0253 00a9 0172 0100 0000 720c  ...q.S...r....r.
-00000ee0: 0000 0072 0d00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000ef0: 0000 7210 0000 0072 1100 0000 6200 0000  ..r....r....b...
-00000f00: 7212 0000 007a 3353 796e 6368 726f 6e69  r....z3Synchroni
-00000f10: 7a65 722e 696e 6974 6961 6c69 7a65 5f6c  zer.initialize_l
-00000f20: 6564 6765 7273 2e3c 6c6f 6361 6c73 3e2e  edgers.<locals>.
-00000f30: 3c64 6963 7463 6f6d 703e 6301 0000 0000  <dictcomp>c.....
-00000f40: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00000f50: 0000 0072 4200 0000 7243 0000 0072 0c00  ...rB...rC...r..
-00000f60: 0000 720d 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000f70: 0072 1000 0000 7211 0000 0063 0000 0072  .r....r....c...r
-00000f80: 1200 0000 2904 7218 0000 00da 1070 6f72  ....).r......por
-00000f90: 745f 6672 616d 655f 636f 756e 74da 1270  t_frame_count..p
-00000fa0: 6f72 745f 6375 7272 656e 745f 6672 616d  ort_current_fram
-00000fb0: 65da 106d 6561 6e5f 6672 616d 655f 7469  e..mean_frame_ti
-00000fc0: 6d65 7372 3300 0000 720c 0000 0072 0c00  mesr3...r....r..
-00000fd0: 0000 7210 0000 0072 2200 0000 6000 0000  ..r....r"...`...
-00000fe0: 7306 0000 0012 0212 010a 017a 1f53 796e  s..........z.Syn
-00000ff0: 6368 726f 6e69 7a65 722e 696e 6974 6961  chronizer.initia
-00001000: 6c69 7a65 5f6c 6564 6765 7273 6301 0000  lize_ledgersc...
-00001010: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00001020: 0043 0000 0073 7e00 0000 7400 a001 6401  .C...s~...t...d.
-00001030: a101 0100 6700 7c00 5f02 7c00 6a03 a004  ....g.|._.|.j...
-00001040: a100 4400 5d17 5c02 7d01 7d02 7405 7c00  ..D.].\.}.}.t.|.
-00001050: 6a06 7c02 6601 6402 6403 8d03 7d03 7c03  j.|.f.d.d...}.|.
-00001060: a007 a100 0100 7c00 6a02 a008 7c03 a101  ......|.j...|...
-00001070: 0100 710d 7400 a001 6404 a101 0100 7400  ..q.t...d.....t.
-00001080: a001 6405 a101 0100 7405 7c00 6a09 6406  ..d.....t.|.j.d.
-00001090: 6402 6403 8d03 7c00 5f0a 7c00 6a0a a007  d.d...|._.|.j...
-000010a0: a100 0100 6400 5300 2907 4e7a 2e41 626f  ....d.S.).Nz.Abo
-000010b0: 7574 2074 6f20 7375 626d 6974 2054 6872  ut to submit Thr
-000010c0: 6561 6470 6f6f 6c20 6f66 2066 7261 6d65  eadpool of frame
-000010d0: 2048 6172 7665 7374 6572 7354 2903 da06   HarvestersT)...
-000010e0: 7461 7267 6574 da04 6172 6773 da06 6461  target..args..da
-000010f0: 656d 6f6e 7a1f 4672 616d 6520 6861 7276  emonz.Frame harv
-00001100: 6573 7465 7273 206a 7573 7420 7375 626d  esters just subm
-00001110: 6974 7465 647a 1e53 7461 7274 696e 6720  ittedz.Starting 
-00001120: 6672 616d 6520 7379 6e63 6872 6f6e 697a  frame synchroniz
-00001130: 6572 2e2e 2e72 0c00 0000 290b 7235 0000  er...r....).r5..
-00001140: 0072 3600 0000 723f 0000 0072 0a00 0000  .r6...r?...r....
-00001150: 721a 0000 0072 0400 0000 da15 6861 7276  r....r......harv
-00001160: 6573 745f 6672 616d 655f 7061 636b 6574  est_frame_packet
-00001170: 7372 2300 0000 721b 0000 00da 1373 796e  sr#...r......syn
-00001180: 6368 5f66 7261 6d65 735f 776f 726b 6572  ch_frames_worker
-00001190: 723d 0000 0029 0472 2400 0000 720f 0000  r=...).r$...r...
-000011a0: 0072 2600 0000 7240 0000 0072 0c00 0000  .r&...r@...r....
-000011b0: 720c 0000 0072 1000 0000 7223 0000 0066  r....r....r#...f
-000011c0: 0000 0073 1400 0000 0a02 0601 1201 1201  ...s............
-000011d0: 0801 0e01 0a01 0a02 1201 0e01 7a12 5379  ............z.Sy
-000011e0: 6e63 6872 6f6e 697a 6572 2e73 7461 7274  nchronizer.start
-000011f0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001200: 0003 0000 0043 0000 00f3 1a00 0000 7400  .....C........t.
-00001210: a001 6401 a101 0100 7c00 6a02 a003 7c01  ..d.....|.j...|.
-00001220: a101 0100 6400 5300 2902 4e7a 3741 6464  ....d.S.).Nz7Add
-00001230: 696e 6720 7175 6575 6520 746f 2072 6563  ing queue to rec
-00001240: 6569 7665 206e 6f74 6963 6520 6f66 2073  eive notice of s
-00001250: 796e 6368 6564 2066 7261 6d65 7320 7570  ynched frames up
-00001260: 6461 7465 2904 7235 0000 0072 3600 0000  date).r5...r6...
-00001270: 7213 0000 0072 1b00 0000 a902 7224 0000  r....r......r$..
-00001280: 0072 2700 0000 720c 0000 0072 0c00 0000  .r'...r....r....
-00001290: 7210 0000 00da 1373 7562 7363 7269 6265  r......subscribe
-000012a0: 5f74 6f5f 6e6f 7469 6365 7400 0000 f304  _to_noticet.....
-000012b0: 0000 000a 0410 017a 2053 796e 6368 726f  .......z Synchro
-000012c0: 6e69 7a65 722e 7375 6273 6372 6962 655f  nizer.subscribe_
-000012d0: 746f 5f6e 6f74 6963 6563 0200 0000 0000  to_noticec......
-000012e0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000012f0: 0000 724c 0000 0029 024e 7a46 5265 6d6f  ..rL...).NzFRemo
-00001300: 7669 6e67 2071 7565 7565 2074 6861 7420  ving queue that 
-00001310: 6861 6420 6265 656e 2072 6563 6569 7669  had been receivi
-00001320: 6e67 206e 6f74 6963 6520 6f66 2073 796e  ng notice of syn
-00001330: 6368 6564 2066 7261 6d65 7320 7570 6461  ched frames upda
-00001340: 7465 2904 7235 0000 0072 3600 0000 7213  te).r5...r6...r.
-00001350: 0000 00da 0672 656d 6f76 6572 4d00 0000  .....removerM...
-00001360: 720c 0000 0072 0c00 0000 7210 0000 00da  r....r....r.....
-00001370: 1575 6e73 7562 7363 7269 6265 5f74 6f5f  .unsubscribe_to_
-00001380: 6e6f 7469 6365 7b00 0000 724f 0000 007a  notice{...rO...z
-00001390: 2253 796e 6368 726f 6e69 7a65 722e 756e  "Synchronizer.un
-000013a0: 7375 6273 6372 6962 655f 746f 5f6e 6f74  subscribe_to_not
-000013b0: 6963 6563 0200 0000 0000 0000 0000 0000  icec............
-000013c0: 0200 0000 0300 0000 4300 0000 724c 0000  ........C...rL..
-000013d0: 0029 024e 7a26 4164 6469 6e67 2071 7565  .).Nz&Adding que
-000013e0: 7565 2074 6f20 7265 6365 6976 6520 7379  ue to receive sy
-000013f0: 6e63 6865 6420 6672 616d 6573 2904 7235  nched frames).r5
-00001400: 0000 0072 3600 0000 7214 0000 0072 1b00  ...r6...r....r..
-00001410: 0000 724d 0000 0072 0c00 0000 720c 0000  ..rM...r....r...
-00001420: 0072 1000 0000 da19 7375 6273 6372 6962  .r......subscrib
-00001430: 655f 746f 5f73 796e 635f 7061 636b 6574  e_to_sync_packet
-00001440: 7383 0000 00f3 0400 0000 0a01 1001 7a26  s.............z&
-00001450: 5379 6e63 6872 6f6e 697a 6572 2e73 7562  Synchronizer.sub
-00001460: 7363 7269 6265 5f74 6f5f 7379 6e63 5f70  scribe_to_sync_p
-00001470: 6163 6b65 7473 6302 0000 0000 0000 0000  acketsc.........
-00001480: 0000 0002 0000 0003 0000 0043 0000 0072  ...........C...r
-00001490: 4c00 0000 2902 4e7a 1652 656c 6561 7369  L...).Nz.Releasi
-000014a0: 6e67 2072 6563 6f72 6420 7175 6575 6529  ng record queue)
-000014b0: 0472 3500 0000 7236 0000 0072 1400 0000  .r5...r6...r....
-000014c0: 7250 0000 0072 4d00 0000 720c 0000 0072  rP...rM...r....r
-000014d0: 0c00 0000 7210 0000 00da 1572 656c 6561  ....r......relea
-000014e0: 7365 5f73 796e 635f 7061 636b 6574 5f71  se_sync_packet_q
-000014f0: 8700 0000 7253 0000 007a 2253 796e 6368  ....rS...z"Synch
-00001500: 726f 6e69 7a65 722e 7265 6c65 6173 655f  ronizer.release_
-00001510: 7379 6e63 5f70 6163 6b65 745f 7163 0200  sync_packet_qc..
-00001520: 0000 0000 0000 0000 0000 0500 0000 0800  ................
-00001530: 0000 4300 0000 73a8 0000 007c 016a 007d  ..C...s....|.j.}
-00001540: 0274 01a0 0264 017c 029b 009d 02a1 0101  .t...d.|........
-00001550: 007c 006a 03a0 04a1 0073 497c 006a 057c  .|.j.....sI|.j.|
-00001560: 0219 00a0 06a1 007d 037c 006a 077c 0219  .......}.|.j.|..
-00001570: 007d 047c 047c 035f 087c 037c 006a 097c  .}.|.|._.|.|.j.|
-00001580: 029b 0064 027c 036a 089b 009d 033c 007c  ...d.|.j.....<.|
-00001590: 006a 077c 0205 0019 0064 0337 0003 003c  .j.|.....d.7...<
-000015a0: 0074 01a0 0a64 047c 036a 009b 0064 057c  .t...d.|.j...d.|
-000015b0: 036a 089b 0064 067c 036a 0b9b 009d 06a1  .j...d.|.j......
-000015c0: 0101 007c 006a 03a0 04a1 0072 1074 01a0  ...|.j.....r.t..
-000015d0: 0264 077c 029b 0064 089d 03a1 0101 0064  .d.|...d.......d
-000015e0: 0053 0029 094e 7a2c 4265 6769 6e6e 696e  .S.).Nz,Beginnin
-000015f0: 6720 746f 2063 6f6c 6c65 6374 2064 6174  g to collect dat
-00001600: 6120 6765 6e65 7261 7465 6420 6174 2070  a generated at p
-00001610: 6f72 7420 da01 5fe9 0100 0000 7a1f 4672  ort .._.....z.Fr
-00001620: 616d 6520 6461 7461 2068 6172 7665 7374  ame data harvest
-00001630: 6564 2066 726f 6d20 7265 656c 207a 0c20  ed from reel z. 
-00001640: 7769 7468 2069 6e64 6578 207a 1320 616e  with index z. an
-00001650: 6420 6672 616d 6520 7469 6d65 206f 6620  d frame time of 
-00001660: 7a19 4672 616d 6520 6861 7276 6573 7465  z.Frame harveste
-00001670: 7220 666f 7220 706f 7274 207a 0a20 636f  r for port z. co
-00001680: 6d70 6c65 7465 6429 0c72 0f00 0000 7235  mpleted).r....r5
-00001690: 0000 0072 3600 0000 7216 0000 00da 0669  ...r6...r......i
-000016a0: 735f 7365 7472 1900 0000 da03 6765 7472  s_setr......getr
-000016b0: 4400 0000 da0b 6672 616d 655f 696e 6465  D.....frame_inde
-000016c0: 7872 1500 0000 da05 6465 6275 67da 0a66  xr......debug..f
-000016d0: 7261 6d65 5f74 696d 6529 0572 2400 0000  rame_time).r$...
-000016e0: 7226 0000 0072 0f00 0000 da0c 6672 616d  r&...r......fram
-000016f0: 655f 7061 636b 6574 7259 0000 0072 0c00  e_packetrY...r..
-00001700: 0000 720c 0000 0072 1000 0000 724a 0000  ..r....r....rJ..
-00001710: 008b 0000 0073 1a00 0000 0601 1002 0a02  .....s..........
-00001720: 0e01 0a01 0601 1602 1201 0402 1a01 04ff  ................
-00001730: 0af8 160c 7a22 5379 6e63 6872 6f6e 697a  ....z"Synchroniz
-00001740: 6572 2e68 6172 7665 7374 5f66 7261 6d65  er.harvest_frame
-00001750: 5f70 6163 6b65 7473 6302 0000 0000 0000  _packetsc.......
-00001760: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
-00001770: 0073 e200 0000 6700 7d02 7c00 6a00 4400  .s....g.}.|.j.D.
-00001780: 5d67 7d03 7c00 6a01 7c03 1900 6401 1700  ]g}.|.j.|...d...
-00001790: 7d04 7c03 9b00 6402 7c04 9b00 9d03 7d05  }.|...d.|.....}.
-000017a0: 7c05 7c00 6a02 a003 a100 7601 7248 7404  |.|.j.....v.rHt.
-000017b0: a005 6403 7c05 9b00 9d02 a101 0100 7c00  ..d.|.........|.
-000017c0: 6a06 722d 7407 a008 6404 a101 0100 6e14  j.r-t...d.....n.
-000017d0: 7409 7407 a007 a100 8301 6405 1600 6406  t.t.......d...d.
-000017e0: 6b02 723c 7404 a00a 6407 a101 0100 7407  k.r<t...d.....t.
-000017f0: a008 6401 a101 0100 7c05 7c00 6a02 a003  ..d.....|.|.j...
-00001800: a100 7601 731c 7c00 6a02 7c05 1900 6a0b  ..v.s.|.j.|...j.
-00001810: 7d06 7c06 6408 6b02 7263 7404 a00a 6409  }.|.d.k.rct...d.
-00001820: 7c03 9b00 640a 9d03 a101 0100 640b 7c00  |...d.......d.|.
-00001830: 5f0c 7c00 6a0d a00e a100 0100 7c03 7c01  _.|.j.......|.|.
-00001840: 6b03 726c 7c02 a00f 7c06 a101 0100 7105  k.rl|...|.....q.
-00001850: 7410 7c02 8301 5300 290c 7a75 4c6f 6f6b  t.|...S.).zuLook
-00001860: 7320 6174 206e 6578 7420 756e 6173 7369  s at next unassi
-00001870: 676e 6564 2066 7261 6d65 2061 6372 6f73  gned frame acros
-00001880: 7320 7468 6520 706f 7274 7320 746f 2064  s the ports to d
-00001890: 6574 6572 6d69 6e65 0a20 2020 2020 2020  etermine.       
-000018a0: 2074 6865 2065 6172 6c69 6573 7420 7469   the earliest ti
-000018b0: 6d65 2061 7420 7768 6963 6820 6561 6368  me at which each
-000018c0: 206f 6620 7468 656d 2077 6173 2072 6561   of them was rea
-000018d0: 6472 5600 0000 7255 0000 007a 3757 6169  drV...rU...z7Wai
-000018e0: 7469 6e67 2069 6e20 6120 6c6f 6f70 2066  ting in a loop f
-000018f0: 6f72 2066 7261 6d65 2064 6174 6120 746f  or frame data to
-00001900: 2070 6f70 756c 6174 6520 7769 7468 206b   populate with k
-00001910: 6579 3a20 679a 9999 9999 99b9 3fe9 0a00  ey: g.......?...
-00001920: 0000 7201 0000 007a 3e53 796e 6368 726f  ..r....z>Synchro
-00001930: 6e69 7a65 7220 6e6f 7420 7375 6273 6372  nizer not subscr
-00001940: 6962 6564 2074 6f20 616e 7920 7374 7265  ibed to any stre
-00001950: 616d 7320 616e 6420 6275 7379 2077 6169  ams and busy wai
-00001960: 7469 6e67 2e2e 2e72 0b00 0000 7a16 456e  ting...r....z.En
-00001970: 6420 6f66 2066 7261 6d65 7320 6174 2070  d of frames at p
-00001980: 6f72 7420 7a21 2064 6574 6563 7465 643b  ort z! detected;
-00001990: 2065 6e64 696e 6720 7379 6e63 6872 6f6e   ending synchron
-000019a0: 697a 6174 696f 6e54 2911 7218 0000 0072  izationT).r....r
-000019b0: 4500 0000 7215 0000 00da 046b 6579 7372  E...r......keysr
-000019c0: 3500 0000 725a 0000 0072 1c00 0000 da04  5...rZ...r......
-000019d0: 7469 6d65 da05 736c 6565 70da 0369 6e74  time..sleep..int
-000019e0: 7236 0000 0072 5b00 0000 7217 0000 0072  r6...r[...r....r
-000019f0: 1600 0000 723c 0000 0072 1b00 0000 da03  ....r<...r......
-00001a00: 6d69 6e29 0772 2400 0000 720f 0000 005a  min).r$...r....Z
-00001a10: 1474 696d 6573 5f6f 665f 6e65 7874 5f66  .times_of_next_f
-00001a20: 7261 6d65 73da 0170 da0a 6e65 7874 5f69  rames..p..next_i
-00001a30: 6e64 6578 da0e 6672 616d 655f 6461 7461  ndex..frame_data
-00001a40: 5f6b 6579 5a0f 6e65 7874 5f66 7261 6d65  _keyZ.next_frame
-00001a50: 5f74 696d 6572 0c00 0000 720c 0000 0072  _timer....r....r
-00001a60: 1000 0000 da13 6561 726c 6965 7374 5f6e  ......earliest_n
-00001a70: 6578 745f 6672 616d 659f 0000 0073 3200  ext_frame....s2.
-00001a80: 0000 0403 0a01 0e01 0e01 0e03 0401 0801  ................
-00001a90: 04ff 0603 0c01 1403 0a01 0a01 0ef6 0c0c  ................
-00001aa0: 0802 0401 0a01 04ff 0604 0a01 0802 0a01  ................
-00001ab0: 0280 0802 7a20 5379 6e63 6872 6f6e 697a  ....z Synchroniz
-00001ac0: 6572 2e65 6172 6c69 6573 745f 6e65 7874  er.earliest_next
-00001ad0: 5f66 7261 6d65 6302 0000 0000 0000 0000  _framec.........
-00001ae0: 0000 0007 0000 0004 0000 0043 0000 0073  ...........C...s
-00001af0: 4e00 0000 6700 7d02 7c00 6a00 4400 5d1d  N...g.}.|.j.D.].
-00001b00: 7d03 7c00 6a01 7c03 1900 7d04 7c03 9b00  }.|.j.|...}.|...
-00001b10: 6401 7c04 9b00 9d03 7d05 7c00 6a02 7c05  d.|.....}.|.j.|.
-00001b20: 1900 6a03 7d06 7c03 7c01 6b03 7222 7c02  ..j.}.|.|.k.r"|.
-00001b30: a004 7c06 a101 0100 7105 7405 7c02 8301  ..|.....q.t.|...
-00001b40: 5300 2902 7a57 5072 6f76 6964 6573 2074  S.).zWProvides t
-00001b50: 6865 206c 6174 6573 7420 6672 616d 655f  he latest frame_
-00001b60: 7469 6d65 206f 6620 7468 6520 6375 7272  time of the curr
-00001b70: 656e 7420 6672 616d 6573 206e 6f74 2069  ent frames not i
-00001b80: 6e63 6c75 7369 7665 206f 6620 7468 6520  nclusive of the 
-00001b90: 7072 6f76 6964 6564 2070 6f72 7472 5500  provided portrU.
-00001ba0: 0000 2906 7218 0000 0072 4500 0000 7215  ..).r....rE...r.
-00001bb0: 0000 0072 5b00 0000 721b 0000 00da 036d  ...r[...r......m
-00001bc0: 6178 2907 7224 0000 0072 0f00 0000 5a17  ax).r$...r....Z.
-00001bd0: 7469 6d65 735f 6f66 5f63 7572 7265 6e74  times_of_current
-00001be0: 5f66 7261 6d65 7372 6300 0000 da0d 6375  _framesrc.....cu
-00001bf0: 7272 656e 745f 696e 6465 7872 6500 0000  rrent_indexre...
-00001c00: 5a12 6375 7272 656e 745f 6672 616d 655f  Z.current_frame_
-00001c10: 7469 6d65 720c 0000 0072 0c00 0000 7210  timer....r....r.
-00001c20: 0000 00da 146c 6174 6573 745f 6375 7272  .....latest_curr
-00001c30: 656e 745f 6672 616d 65c3 0000 0073 1200  ent_frame....s..
-00001c40: 0000 0402 0a01 0a01 0e01 0c01 0801 0a01  ................
-00001c50: 0280 0802 7a21 5379 6e63 6872 6f6e 697a  ....z!Synchroniz
-00001c60: 6572 2e6c 6174 6573 745f 6375 7272 656e  er.latest_curren
-00001c70: 745f 6672 616d 6563 0100 0000 0000 0000  t_framec........
-00001c80: 0000 0000 0200 0000 0400 0000 0300 0000  ................
-00001c90: 732c 0000 0087 0066 0164 0164 0284 0888  s,.....f.d.d....
-00001ca0: 006a 0044 0083 017d 0174 01a0 0264 037c  .j.D...}.t...d.|
-00001cb0: 019b 009d 02a1 0101 0074 037c 0183 0153  .........t.|...S
-00001cc0: 0029 047a 4244 6574 6572 6d69 6e65 2068  .).zBDetermine h
-00001cd0: 6f77 206d 616e 7920 756e 6173 7369 676e  ow many unassign
-00001ce0: 6564 2066 7261 6d65 7320 6172 6520 7369  ed frames are si
-00001cf0: 7474 696e 6720 696e 2073 656c 662e 6461  tting in self.da
-00001d00: 7461 6672 616d 6563 0100 0000 0000 0000  taframec........
-00001d10: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-00001d20: 7320 0000 0067 007c 005d 0c7d 0188 006a  s ...g.|.].}...j
-00001d30: 007c 0119 0088 006a 017c 0119 0018 0091  .|.....j.|......
-00001d40: 0271 0253 0072 0c00 0000 2902 7244 0000  .q.S.r....).rD..
-00001d50: 0072 4500 0000 720d 0000 0072 3300 0000  .rE...r....r3...
-00001d60: 720c 0000 0072 1000 0000 da0a 3c6c 6973  r....r......<lis
-00001d70: 7463 6f6d 703e d100 0000 7308 0000 0006  tcomp>....s.....
-00001d80: 0002 0212 ff06 ff7a 2c53 796e 6368 726f  .......z,Synchro
-00001d90: 6e69 7a65 722e 6672 616d 655f 736c 6163  nizer.frame_slac
-00001da0: 6b2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  k.<locals>.<list
-00001db0: 636f 6d70 3e7a 1353 6c61 636b 2069 6e20  comp>z.Slack in 
-00001dc0: 6672 616d 6573 2069 7320 2904 7218 0000  frames is ).r...
-00001dd0: 0072 3500 0000 725a 0000 0072 6200 0000  .r5...rZ...rb...
-00001de0: 2902 7224 0000 005a 0573 6c61 636b 720c  ).r$...Z.slackr.
-00001df0: 0000 0072 3300 0000 7210 0000 00da 0b66  ...r3...r......f
-00001e00: 7261 6d65 5f73 6c61 636b cf00 0000 730a  rame_slack....s.
-00001e10: 0000 000a 0204 0206 fe10 0408 017a 1853  .............z.S
-00001e20: 796e 6368 726f 6e69 7a65 722e 6672 616d  ynchronizer.fram
-00001e30: 655f 736c 6163 6b63 0100 0000 0000 0000  e_slackc........
-00001e40: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-00001e50: 733c 0000 0074 007c 006a 0183 0164 016b  s<...t.|.j...d.k
-00001e60: 0472 0f7c 006a 0164 0264 0085 0219 007c  .r.|.j.d.d.....|
-00001e70: 005f 0174 02a0 037c 006a 01a1 017d 0174  ._.t...|.j...}.t
-00001e80: 02a0 047c 01a1 017d 0264 037c 021b 0053  ...|...}.d.|...S
-00001e90: 0029 044e 725d 0000 0069 f6ff ffff 7256  .).Nr]...i....rV
-00001ea0: 0000 0029 05da 036c 656e 7246 0000 0072  ...)...lenrF...r
-00001eb0: 3100 0000 da04 6469 6666 7232 0000 0029  1.....diffr2...)
-00001ec0: 0372 2400 0000 5a07 6465 6c74 615f 745a  .r$...Z.delta_tZ
-00001ed0: 0c6d 6561 6e5f 6465 6c74 615f 7472 0c00  .mean_delta_tr..
-00001ee0: 0000 720c 0000 0072 1000 0000 da0b 6176  ..r....r......av
-00001ef0: 6572 6167 655f 6670 73d8 0000 0073 0a00  erage_fps....s..
-00001f00: 0000 0e01 1001 0c02 0a01 0802 7a18 5379  ............z.Sy
-00001f10: 6e63 6872 6f6e 697a 6572 2e61 7665 7261  nchronizer.avera
-00001f20: 6765 5f66 7073 6301 0000 0000 0000 0000  ge_fpsc.........
-00001f30: 0000 000c 0000 0009 0000 0043 0000 0073  ...........C...s
-00001f40: 8e02 0000 7400 a001 6401 a101 0100 6402  ....t...d.....d.
-00001f50: 7d01 7400 a001 6403 a101 0100 7c00 6a02  }.t...d.....|.j.
-00001f60: a003 a100 9001 7340 6900 7d02 6700 7d03  ......s@i.}.g.}.
-00001f70: 6900 7d04 6900 7d05 7c00 6a04 4400 5d15  i.}.i.}.|.j.D.].
-00001f80: 7d06 7c00 a005 7c06 a101 7c04 7c06 3c00  }.|...|...|.|.<.
-00001f90: 7c00 a006 7c06 a101 7c05 7c06 3c00 7c00  |...|...|.|.<.|.
-00001fa0: 6a07 7c06 1900 7d07 711d 7c00 6a04 4400  j.|...}.q.|.j.D.
-00001fb0: 5d68 7d06 7c00 6a07 7c06 1900 7d07 7c06  ]h}.|.j.|...}.|.
-00001fc0: 9b00 6404 7c07 9b00 9d03 7d08 7c00 6a08  ..d.|.....}.|.j.
-00001fd0: 7c08 1900 7d09 7c09 6a09 7d0a 7c0a 7c04  |...}.|.j.}.|.|.
-00001fe0: 7c06 1900 6b04 7260 6400 7c02 7c06 3c00  |...k.r`d.|.|.<.
-00001ff0: 7400 a00a 6405 7c06 9b00 6406 9d03 a101  t...d.|...d.....
-00002000: 0100 7136 7c04 7c06 1900 7c0a 1800 7c0a  ..q6|.|...|...|.
-00002010: 7c05 7c06 1900 1800 6b00 727a 6400 7c02  |.|.....k.rzd.|.
-00002020: 7c06 3c00 7400 a00a 6405 7c06 9b00 6407  |.<.t...d.|...d.
-00002030: 9d03 a101 0100 7136 7c00 6a08 a00b 7c08  ......q6|.j...|.
-00002040: a101 7c02 7c06 3c00 7c00 6a07 7c06 0500  ..|.|.<.|.j.|...
-00002050: 1900 6408 3700 0300 3c00 7c03 a00c 7c0a  ..d.7...<.|...|.
-00002060: a101 0100 7400 a00d 6409 7c06 9b00 640a  ....t...d.|...d.
-00002070: 7c07 9b00 640b 7c0a 9b00 9d06 a101 0100  |...d.|.........
-00002080: 7136 7400 a00d 640c 740e 7c00 6a08 8301  q6t...d.t.|.j...
-00002090: 9b00 9d02 a101 0100 7c00 6a0f a00c 7410  ........|.j...t.
-000020a0: a011 7c03 a101 a101 0100 7412 7c01 7c02  ..|.......t.|.|.
-000020b0: 8302 7c00 5f13 7c00 a014 a100 0100 7c01  ..|._.|.......|.
-000020c0: 6408 3700 7d01 7c00 6a02 a003 a100 72ce  d.7.}.|.j.....r.
-000020d0: 7400 a001 640d a101 0100 6400 7c00 5f13  t...d.....d.|._.
-000020e0: 7c00 6a15 4400 5d0c 7d0b 7400 a00d 640e  |.j.D.].}.t...d.
-000020f0: a101 0100 7c0b a016 640f a101 0100 71d1  ....|...d.....q.
-00002100: 7c00 6a17 4400 5d54 7d0b 7c0b a016 7c00  |.j.D.]T}.|...|.
-00002110: 6a13 a101 0100 7c00 6a13 6400 7501 9001  j.....|.j.d.u...
-00002120: 7218 7400 a00d 6410 7c00 6a13 6a18 9b00  r.t...d.|.j.j...
-00002130: 6411 9d03 a101 0100 7400 a00d 6412 7c00  d.......t...d.|.
-00002140: 6a13 6a19 9b00 9d02 a101 0100 7c00 6a13  j.j.........|.j.
-00002150: 6a19 6413 1600 6402 6b02 9001 7217 7400  j.d...d.k...r.t.
-00002160: a001 6412 7c00 6a13 6a19 9b00 9d02 a101  ..d.|.j.j.......
-00002170: 0100 71e1 7400 a001 6414 a101 0100 7c00  ..q.t...d.....|.
-00002180: 6a1a a01b a100 4400 5d12 5c02 7d06 7d0b  j.....D.].\.}.}.
-00002190: 7400 a001 6415 7c0b a01c a100 9b00 6416  t...d.|.......d.
-000021a0: 7c06 9b00 9d04 a101 0100 9001 7122 71e1  |...........q"q.
-000021b0: 7c00 a01d a100 7c00 5f1e 7c00 6a02 a003  |.....|._.|.j...
-000021c0: a100 7212 7400 a001 6417 a101 0100 6400  ..r.t...d.....d.
-000021d0: 5300 2918 4e7a 3457 6169 7469 6e67 2066  S.).Nz4Waiting f
-000021e0: 6f72 2061 6c6c 2070 6f72 7473 2074 6f20  or all ports to 
-000021f0: 6265 6769 6e20 6861 7276 6573 7469 6e67  begin harvesting
-00002200: 2063 6f72 6e65 7273 2e2e 2e72 0100 0000   corners...r....
-00002210: 7a26 4162 6f75 7420 746f 2073 7461 7274  z&About to start
-00002220: 2073 796e 6368 726f 6e69 7a69 6e67 2066   synchronizing f
-00002230: 7261 6d65 732e 2e2e 7255 0000 007a 1653  rames...rU...z.S
-00002240: 6b69 7070 6564 2066 7261 6d65 2061 7420  kipped frame at 
-00002250: 706f 7274 207a 113a 203e 2065 6172 6c69  port z.: > earli
-00002260: 6573 745f 6e65 7874 7a1d 3a20 6465 6c74  est_nextz.: delt
-00002270: 6120 3c20 7469 6d65 2d6c 6174 6573 745f  a < time-latest_
-00002280: 6375 7272 656e 7472 5600 0000 7a1a 4164  currentrV...z.Ad
-00002290: 6469 6e67 2074 6f20 6c61 7965 7220 6672  ding to layer fr
-000022a0: 6f6d 2070 6f72 7420 7a0a 2061 7420 696e  om port z. at in
-000022b0: 6465 7820 7a11 2061 6e64 2066 7261 6d65  dex z. and frame
-000022c0: 2074 696d 653a 207a 1355 6e61 7373 6967   time: z.Unassig
-000022d0: 6e65 6420 4672 616d 6573 3a20 7a37 5365  ned Frames: z7Se
-000022e0: 6e64 696e 6720 604e 6f6e 6560 206f 6e20  nding `None` on 
-000022f0: 7175 6575 6520 746f 2073 6967 6e61 6c20  queue to signal 
-00002300: 656e 6420 6f66 2073 796e 6365 6420 6672  end of synced fr
-00002310: 616d 6573 2e7a 3447 6976 696e 6720 6e6f  ames.z4Giving no
-00002320: 7469 6365 206f 6620 6e65 7720 7379 6e63  tice of new sync
-00002330: 6865 6420 6672 616d 6573 2070 6163 6b65  hed frames packe
-00002340: 7420 7669 6120 7175 6575 657a 1c6e 6577  t via queuez.new
-00002350: 2073 796e 6368 6564 2066 7261 6d65 7320   synched frames 
-00002360: 6176 6169 6c61 626c 657a 3050 6c61 6369  availablez0Placi
-00002370: 6e67 206e 6577 2073 796e 6368 6564 2066  ng new synched f
-00002380: 7261 6d65 7320 7061 636b 6574 206f 6e20  rames packet on 
-00002390: 7175 6575 6520 7769 7468 207a 0720 6672  queue with z. fr
-000023a0: 616d 6573 7a26 506c 6163 696e 6720 6e65  amesz&Placing ne
-000023b0: 7720 7379 6e63 6865 6420 6672 616d 6573  w synched frames
-000023c0: 2077 6974 6820 696e 6465 7820 7207 0000   with index r...
-000023d0: 007a 3f73 6967 6e61 6c69 6e67 2065 6e64  .z?signaling end
-000023e0: 206f 6620 6672 616d 6573 2077 6974 6820   of frames with 
-000023f0: 604e 6f6e 6560 2070 6163 6b65 7420 6f6e  `None` packet on
-00002400: 2073 7562 7363 7269 6265 7220 7175 6575   subscriber queu
-00002410: 652e 7a0a 4375 7272 656e 746c 7920 7a24  e.z.Currently z$
-00002420: 2066 7261 6d65 2070 6163 6b65 7473 2075   frame packets u
-00002430: 6e70 726f 6365 7373 6564 2066 6f72 2070  nprocessed for p
-00002440: 6f72 7420 7a25 4672 616d 6520 7379 6e63  ort z%Frame sync
-00002450: 6820 776f 726b 6572 2073 7563 6365 7373  h worker success
-00002460: 6675 6c6c 7920 656e 6465 6429 1f72 3500  fully ended).r5.
-00002470: 0000 7236 0000 0072 1600 0000 7257 0000  ..r6...r....rW..
-00002480: 0072 1800 0000 7266 0000 0072 6900 0000  .r....rf...ri...
-00002490: 7245 0000 0072 1500 0000 725b 0000 00da  rE...r....r[....
-000024a0: 0777 6172 6e69 6e67 da03 706f 7072 1b00  .warning..popr..
-000024b0: 0000 725a 0000 0072 6c00 0000 7246 0000  ..rZ...rl...rF..
-000024c0: 0072 3100 0000 7232 0000 0072 0600 0000  .r1...r2...r....
-000024d0: 722d 0000 0072 3000 0000 7213 0000 00da  r-...r0...r.....
-000024e0: 0370 7574 7214 0000 00da 1266 7261 6d65  .putr......frame
-000024f0: 5f70 6163 6b65 745f 636f 756e 74da 0a73  _packet_count..s
-00002500: 796e 635f 696e 6465 7872 1900 0000 721a  ync_indexr....r.
-00002510: 0000 00da 0571 7369 7a65 726e 0000 0072  .....qsizern...r
-00002520: 1f00 0000 290c 7224 0000 0072 7300 0000  ....).r$...rs...
-00002530: 5a15 6375 7272 656e 745f 6672 616d 655f  Z.current_frame_
-00002540: 7061 636b 6574 735a 116c 6179 6572 5f66  packetsZ.layer_f
-00002550: 7261 6d65 5f74 696d 6573 5a0d 6561 726c  rame_timesZ.earl
-00002560: 6965 7374 5f6e 6578 745a 0e6c 6174 6573  iest_nextZ.lates
-00002570: 745f 6375 7272 656e 7472 0f00 0000 5a13  t_currentr....Z.
-00002580: 6375 7272 656e 745f 6672 616d 655f 696e  current_frame_in
-00002590: 6465 785a 0e70 6f72 745f 696e 6465 785f  dexZ.port_index_
-000025a0: 6b65 795a 1463 7572 7265 6e74 5f66 7261  keyZ.current_fra
-000025b0: 6d65 5f70 6163 6b65 7472 5b00 0000 7227  me_packetr[...r'
-000025c0: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-000025d0: 0000 724b 0000 00e1 0000 0073 7800 0000  ..rK.......sx...
-000025e0: 0a02 0402 0a02 0c01 0402 0402 0404 0401  ................
-000025f0: 0a02 0e01 0e01 0c01 0a02 0a01 0e02 0a01  ................
-00002600: 0601 0c03 0802 1401 1602 02ff 0805 0401  ................
-00002610: 0a01 06ff 0605 0201 08ff 1204 0a01 0401  ................
-00002620: 1401 06ff 1604 1202 0c02 0802 0802 0a02  ................
-00002630: 0a01 0601 0a04 0a01 0c01 0a02 0c01 0c01  ................
-00002640: 1601 1401 1203 1401 0280 0a02 1201 1e01  ................
-00002650: 02ff 0a03 0aad 0e55 7a20 5379 6e63 6872  .......Uz Synchr
-00002660: 6f6e 697a 6572 2e73 796e 6368 5f66 7261  onizer.synch_fra
-00002670: 6d65 735f 776f 726b 6572 4e29 0172 0900  mes_workerN).r..
-00002680: 0000 291a da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-00002690: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000026a0: 616c 6e61 6d65 5f5f da04 6469 6374 7228  alname__..dictr(
-000026b0: 0000 00da 0462 6f6f 6c72 2c00 0000 7230  .....boolr,...r0
-000026c0: 0000 00da 0870 726f 7065 7274 7972 3400  .....propertyr4.
-000026d0: 0000 721e 0000 0072 1d00 0000 723b 0000  ..r....r....r;..
-000026e0: 0072 4100 0000 7222 0000 0072 2300 0000  .rA...r"...r#...
-000026f0: 724e 0000 0072 5100 0000 7252 0000 0072  rN...rQ...rR...r
-00002700: 5400 0000 724a 0000 0072 6600 0000 7269  T...rJ...rf...ri
-00002710: 0000 0072 6b00 0000 726e 0000 0072 4b00  ...rk...rn...rK.
-00002720: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00002730: 0072 1000 0000 7208 0000 0013 0000 0073  .r....r........s
-00002740: 2c00 0000 0800 1001 0e22 0804 0207 0a01  ,........"......
-00002750: 0807 0806 0805 0806 0806 0806 080e 0807  ................
-00002760: 0808 0804 0804 0814 0824 080c 0809 0c09  .........$......
-00002770: 7208 0000 00da 085f 5f6d 6169 6e5f 5f29  r......__main__)
-00002780: 01da 0743 6861 7275 636f 2901 da0e 4368  ...Charuco)...Ch
-00002790: 6172 7563 6f54 7261 636b 6572 2902 da0e  arucoTracker)...
-000027a0: 5265 636f 7264 6564 5374 7265 616d da12  RecordedStream..
-000027b0: 5265 636f 7264 6564 5374 7265 616d 506f  RecordedStreamPo
-000027c0: 6f6c 2901 da07 5365 7373 696f 6e29 01da  ol)...Session)..
-000027d0: 085f 5f72 6f6f 745f 5f46 da05 7465 7374  .__root__F..test
-000027e0: 735a 0332 3137 547a 1543 7265 6174 696e  sZ.217Tz.Creatin
-000027f0: 6720 5379 6e63 6872 6f6e 697a 6572 e905  g Synchronizer..
-00002800: 0000 0029 0172 2500 0000 2905 7201 0000  ...).r%...).r...
-00002810: 0072 5600 0000 e902 0000 00e9 0300 0000  .rV.............
-00002820: e904 0000 005a 0873 6573 7369 6f6e 7372  .....Z.sessionsr
-00002830: 8600 0000 e90b 0000 0067 0000 0000 0000  .........g......
-00002840: 2140 6700 0000 0000 00e8 3f67 0000 0000  !@g.......?g....
-00002850: 0000 1540 2903 da0b 6172 7563 6f5f 7363  ...@)...aruco_sc
-00002860: 616c 65da 1673 7175 6172 655f 7369 7a65  ale..square_size
-00002870: 5f6f 7665 7269 6465 5f63 6dda 0869 6e76  _overide_cm..inv
-00002880: 6572 7465 6429 01da 0763 6861 7275 636f  erted)...charuco
-00002890: e914 0000 007a 1642 6567 696e 6e69 6e67  .....z.Beginning
-000028a0: 2070 6c61 7962 6163 6b20 6174 207a 0550   playback at z.P
-000028b0: 6f72 7420 7256 0000 0072 2700 0000 7a15  ort rV...r'...z.
-000028c0: 506c 6179 6261 636b 2066 696e 6973 6865  Playback finishe
-000028d0: 6420 6174 2029 40da 0d70 7978 7933 642e  d at )@..pyxy3d.
-000028e0: 6c6f 6767 6572 da06 7079 7879 3364 7235  logger..pyxy3dr5
-000028f0: 0000 0072 5800 0000 7275 0000 00da 076c  ...rX...ru.....l
-00002900: 6f67 6769 6e67 725f 0000 00da 0770 6174  oggingr_.....pat
-00002910: 686c 6962 7202 0000 00da 0571 7565 7565  hlibr......queue
-00002920: 7203 0000 00da 0974 6872 6561 6469 6e67  r......threading
-00002930: 7204 0000 0072 0500 0000 da03 6376 32da  r....r......cv2.
-00002940: 056e 756d 7079 7231 0000 00da 1070 7978  .numpyr1.....pyx
-00002950: 7933 642e 696e 7465 7266 6163 6572 0600  y3d.interfacer..
-00002960: 0000 722f 0000 0072 0800 0000 da1a 7079  ..r/...r......py
-00002970: 7879 3364 2e63 616c 6962 7261 7469 6f6e  xy3d.calibration
-00002980: 2e63 6861 7275 636f 727c 0000 00da 1f70  .charucor|.....p
-00002990: 7978 7933 642e 7472 6163 6b65 7273 2e63  yxy3d.trackers.c
-000029a0: 6861 7275 636f 5f74 7261 636b 6572 727d  haruco_trackerr}
-000029b0: 0000 005a 2070 7978 7933 642e 7265 636f  ...Z pyxy3d.reco
-000029c0: 7264 696e 672e 7265 636f 7264 6564 5f73  rding.recorded_s
-000029d0: 7472 6561 6d72 7e00 0000 727f 0000 00da  treamr~...r.....
-000029e0: 1670 7978 7933 642e 7365 7373 696f 6e2e  .pyxy3d.session.
-000029f0: 7365 7373 696f 6e72 8000 0000 7281 0000  sessionr....r...
-00002a00: 005a 0974 6573 745f 6c69 7665 da11 7365  .Z.test_live..se
-00002a10: 7373 696f 6e5f 6469 7265 6374 6f72 79da  ssion_directory.
-00002a20: 0773 6573 7369 6f6e da11 6c6f 6164 5f73  .session..load_s
-00002a30: 7472 6561 6d5f 746f 6f6c 7372 0a00 0000  tream_toolsr....
-00002a40: 721a 0000 0072 0f00 0000 7226 0000 00da  r....r....r&....
-00002a50: 095f 7368 6f77 5f66 7073 5a0d 5f73 686f  ._show_fpsZ._sho
-00002a60: 775f 6368 6172 7563 6f72 3600 0000 5a05  w_charucor6...Z.
-00002a70: 7379 6e63 7272 1800 0000 5a13 7265 636f  syncrr....Z.reco
-00002a80: 7264 696e 675f 6469 7265 6374 6f72 79da  rding_directory.
-00002a90: 0774 7261 636b 6572 5a14 7265 636f 7264  .trackerZ.record
-00002aa0: 6564 5f73 7472 6561 6d5f 706f 6f6c 5a0b  ed_stream_poolZ.
-00002ab0: 706c 6179 5f76 6964 656f 735a 0e6e 6f74  play_videosZ.not
-00002ac0: 6966 6963 6174 696f 6e5f 7172 4e00 0000  ification_qrN...
-00002ad0: da0c 7065 7266 5f63 6f75 6e74 6572 7216  ..perf_counterr.
-00002ae0: 0000 0072 5700 0000 5a15 7379 6e63 6865  ...rW...Z.synche
-00002af0: 645f 6672 616d 6573 5f6e 6f74 6963 6572  d_frames_noticer
-00002b00: 2d00 0000 5a0b 7379 6e63 5f70 6163 6b65  -...Z.sync_packe
-00002b10: 74da 0d66 7261 6d65 5f70 6163 6b65 7473  t..frame_packets
-00002b20: 725c 0000 00da 0669 6d73 686f 77da 0566  r\.....imshow..f
-00002b30: 7261 6d65 da07 7761 6974 4b65 79da 036b  rame..waitKey..k
-00002b40: 6579 da03 6f72 64da 1164 6573 7472 6f79  ey..ord..destroy
-00002b50: 416c 6c57 696e 646f 7773 720c 0000 0072  AllWindowsr....r
-00002b60: 0c00 0000 720c 0000 0072 1000 0000 da08  ....r....r......
-00002b70: 3c6d 6f64 756c 653e 0100 0000 7376 0000  <module>....sv..
-00002b80: 0008 000c 0208 0108 040c 010c 0110 0108  ................
-00002b90: 0208 010c 0104 020e 0200 7f00 7f0a 2f0c  ............../.
-00002ba0: 010c 0110 010c 0208 010c 0204 0404 020c  ................
-00002bb0: 0208 0208 0212 0306 0108 010a 0210 0108  ................
-00002bc0: 020e 0202 010e 0106 ff02 0306 0106 ff0a  ................
-00002bd0: 030e 0108 0106 020a 0214 010c 0208 0106  ................
-00002be0: 0112 0104 0214 0102 800a 020e 0208 0102  ................
-00002bf0: 010a f418 0e04 c2                        .......
+00000040: 5a02 6400 6401 6c05 5a05 6502 a006 6505  Z.d.d.l.Z.e...e.
+00000050: 6a07 a101 0100 6400 6401 6c08 5a08 6400  j.....d.d.l.Z.d.
+00000060: 6402 6c09 6d0a 5a0a 0100 6400 6403 6c0b  d.l.m.Z...d.d.l.
+00000070: 6d0c 5a0c 0100 6400 6404 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000080: 6d0f 5a0f 0100 6400 6401 6c10 5a10 6400  m.Z...d.d.l.Z.d.
+00000090: 6401 6c11 5a12 6400 6405 6c13 6d14 5a14  d.l.Z.d.d.l.m.Z.
+000000a0: 0100 6406 5a15 4700 6407 6408 8400 6408  ..d.Z.G.d.d...d.
+000000b0: 8302 5a16 6504 6409 6b02 9002 724c 6400  ..Z.e.d.k...rLd.
+000000c0: 640a 6c17 6d18 5a18 0100 6400 640b 6c19  d.l.m.Z...d.d.l.
+000000d0: 6d1a 5a1a 0100 6400 640c 6c1b 6d1c 5a1c  m.Z...d.d.l.m.Z.
+000000e0: 6d1d 5a1d 0100 6400 640d 6c1e 6d1f 5a1f  m.Z...d.d.l.m.Z.
+000000f0: 0100 6400 6401 6c08 5a08 6400 640e 6c01  ..d.d.l.Z.d.d.l.
+00000100: 6d20 5a20 0100 640f 5a21 6521 9001 7242  m Z ..d.Z!e!..rB
+00000110: 650a 6520 6410 6411 8303 5a22 651f 6522  e.e d.d...Z"e.e"
+00000120: 8301 5a23 6523 a024 a100 0100 6523 a025  ..Z#e#.$....e#.%
+00000130: a100 0100 6523 6a26 a027 a100 4400 5d16  ....e#j&.'..D.].
+00000140: 5c02 5a28 5a29 6412 6529 5f2a 6412 6529  \.Z(Z)d.e)_*d.e)
+00000150: 5f2b 9001 7110 6502 a02c 6413 a101 0100  _+..q.e..,d.....
+00000160: 6516 6523 6a26 6414 6415 8d02 5a2d 6e60  e.e#j&d.d...Z-n`
+00000170: 6400 6416 6417 6418 6419 6705 5a2e 650a  d.d.d.d.d.g.Z.e.
+00000180: 6520 6410 641a 6411 8304 5a2f 6518 6419  e d.d.d...Z/e.d.
+00000190: 6414 641b 641c 641d 641e 6412 641f 8d07  d.d.d.d.d.d.d...
+000001a0: 5a30 651d 652e 652f 6530 6420 8d03 5a31  Z0e.e.e/e0d ..Z1
+000001b0: 6502 a02c 6413 a101 0100 6516 6531 6a26  e..,d.....e.e1j&
+000001c0: 6421 6415 8d02 5a2d 6531 a032 a100 0100  d!d...Z-e1.2....
+000001d0: 650c 8300 5a33 652d a034 6533 a101 0100  e...Z3e-.4e3....
+000001e0: 6502 a02c 6422 6508 a035 a100 9b00 9d02  e..,d"e..5......
+000001f0: a101 0100 652d 6a36 a037 a100 9002 7338  ....e-j6.7....s8
+00000200: 6533 a003 a100 5a38 652d 6a39 5a3a 653a  e3....Z8e-j9Z:e:
+00000210: 6a3b a027 a100 4400 5d24 5c02 5a28 5a3c  j;.'..D.]$\.Z(Z<
+00000220: 653c 9001 72ea 6510 a03d 6423 6528 9b00  e<..r.e..=d#e(..
+00000230: 9d02 653c 6a3e a102 0100 9001 71ea 6510  ..e<j>......q.e.
+00000240: a03f 6416 a101 5a40 6540 6541 6424 8301  .?d...Z@e@eAd$..
+00000250: 6b02 9001 72c6 6510 a042 a100 0100 9002  k...r.e..B......
+00000260: 7138 9001 71c6 6502 a02c 6425 6508 a035  q8..q.e..,d%e..5
+00000270: a100 9b00 9d02 a101 0100 6401 5300 2926  ..........d.S.)&
+00000280: e900 0000 004e 2901 da04 5061 7468 2901  .....N)...Path).
+00000290: da05 5175 6575 6529 02da 0654 6872 6561  ..Queue)...Threa
+000002a0: 64da 0545 7665 6e74 2901 da0a 5379 6e63  d..Event)...Sync
+000002b0: 5061 636b 6574 e964 0000 0063 0000 0000  Packet.d...c....
+000002c0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000002d0: 4000 0000 73c6 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+000002e0: 0264 2f65 0364 029c 0164 0364 0484 055a  .d/e.d...d.d...Z
+000002f0: 0465 0564 059c 0164 0664 0784 045a 0664  .e.d...d.d...Z.d
+00000300: 0864 0984 005a 0764 0a64 0b84 005a 0865  .d...Z.d.d...Z.e
+00000310: 0964 0c64 0d84 0083 015a 0a64 0e64 0f84  .d.d.....Z.d.d..
+00000320: 005a 0b64 1064 1184 005a 0c64 1264 1384  .Z.d.d...Z.d.d..
+00000330: 005a 0d64 1464 1584 005a 0e64 1664 1784  .Z.d.d...Z.d.d..
+00000340: 005a 0f64 1864 1984 005a 1064 1a64 1b84  .Z.d.d...Z.d.d..
+00000350: 005a 1164 1c64 1d84 005a 1264 1e64 1f84  .Z.d.d...Z.d.d..
+00000360: 005a 1364 2064 2184 005a 1464 2264 2384  .Z.d d!..Z.d"d#.
+00000370: 005a 1564 2464 2584 005a 1664 2664 2784  .Z.d$d%..Z.d&d'.
+00000380: 005a 1764 2864 2984 005a 1864 2a64 2b84  .Z.d(d)..Z.d*d+.
+00000390: 005a 1964 2c64 2d84 005a 1a64 2e53 0029  .Z.d,d-..Z.d.S.)
+000003a0: 30da 0c53 796e 6368 726f 6e69 7a65 72e9  0..Synchronizer.
+000003b0: 0600 0000 2901 da07 7374 7265 616d 7363  ....)...streamsc
+000003c0: 0300 0000 0000 0000 0000 0000 0600 0000  ................
+000003d0: 0400 0000 4300 0000 73ba 0000 007c 017c  ....C...s....|.|
+000003e0: 005f 0064 007c 005f 0167 007c 005f 0267  ._.d.|._.g.|._.g
+000003f0: 007c 005f 0369 007c 005f 0474 0583 007c  .|._.i.|._.t...|
+00000400: 005f 0664 017c 005f 0767 007c 005f 0869  ._.d.|._.g.|._.i
+00000410: 007c 005f 097c 006a 00a0 0aa1 0044 005d  .|._.|.j.....D.]
+00000420: 265c 027d 037d 047c 006a 08a0 0b7c 03a1  &\.}.}.|.j...|..
+00000430: 0101 0074 0c64 0283 017d 057c 057c 006a  ...t.d...}.|.|.j
+00000440: 097c 033c 0071 4264 017c 005f 0d7c 00a0  .|.<.qBd.|._.|..
+00000450: 0ea1 0001 007c 027c 005f 0f7c 00a0 107c  .....|.|._.|...|
+00000460: 006a 0fa1 0101 007c 027c 005f 1164 0364  .j.....|.|._.d.d
+00000470: 0484 0074 127c 006a 0883 0144 0083 017c  ...t.|.j...D...|
+00000480: 005f 137c 00a0 14a1 0001 007c 00a0 15a1  ._.|.......|....
+00000490: 0001 0064 0053 0029 054e 46e9 ffff ffff  ...d.S.).NF.....
+000004a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000004b0: 0004 0000 0053 0000 0073 1200 0000 6900  .....S...s....i.
+000004c0: 7c00 5d0a 7d01 7c01 6700 9302 7104 5300  |.].}.|.g...q.S.
+000004d0: a900 720c 0000 00a9 02da 022e 30da 0470  ..r.........0..p
+000004e0: 6f72 7472 0c00 0000 720c 0000 00fa 3f43  ortr....r.....?C
+000004f0: 3a5c 5573 6572 735c 4d61 6320 5072 6962  :\Users\Mac Prib
+00000500: 6c65 5c72 6570 6f73 5c70 7978 7933 645c  le\repos\pyxy3d\
+00000510: 7079 7879 3364 5c63 616d 6572 6173 5c73  pyxy3d\cameras\s
+00000520: 796e 6368 726f 6e69 7a65 722e 7079 da0a  ynchronizer.py..
+00000530: 3c64 6963 7463 6f6d 703e 3200 0000 7306  <dictcomp>2...s.
+00000540: 0000 0006 0002 0002 007a 2953 796e 6368  .........z)Synch
+00000550: 726f 6e69 7a65 722e 5f5f 696e 6974 5f5f  ronizer.__init__
+00000560: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00000570: 6f6d 703e 2916 720a 0000 005a 1663 7572  omp>).r....Z.cur
+00000580: 7265 6e74 5f73 796e 6368 6564 5f66 7261  rent_synched_fra
+00000590: 6d65 73da 1773 796e 635f 6e6f 7469 6365  mes..sync_notice
+000005a0: 5f73 7562 7363 7269 6265 7273 da1a 7379  _subscribers..sy
+000005b0: 6e63 6865 645f 6672 616d 6573 5f73 7562  nched_frames_sub
+000005c0: 7363 7269 6265 7273 da11 616c 6c5f 6672  scribers..all_fr
+000005d0: 616d 655f 7061 636b 6574 7372 0500 0000  ame_packetsr....
+000005e0: da0a 7374 6f70 5f65 7665 6e74 da0f 6672  ..stop_event..fr
+000005f0: 616d 6573 5f63 6f6d 706c 6574 65da 0570  ames_complete..p
+00000600: 6f72 7473 da13 6672 616d 655f 7061 636b  orts..frame_pack
+00000610: 6574 5f71 7565 7565 73da 0569 7465 6d73  et_queues..items
+00000620: da06 6170 7065 6e64 7203 0000 00da 1573  ..appendr......s
+00000630: 7562 7363 7269 6265 645f 746f 5f73 7472  ubscribed_to_str
+00000640: 6561 6d73 da14 7375 6273 6372 6962 655f  eams..subscribe_
+00000650: 746f 5f73 7472 6561 6d73 da0b 5f66 7073  to_streams.._fps
+00000660: 5f74 6172 6765 74da 0e73 6574 5f66 7073  _target..set_fps
+00000670: 5f74 6172 6765 74da 0866 7073 5f6d 6561  _target..fps_mea
+00000680: 6eda 0673 6f72 7465 64da 1564 726f 7070  n..sorted..dropp
+00000690: 6564 5f66 7261 6d65 5f68 6973 746f 7279  ed_frame_history
+000006a0: da12 696e 6974 6961 6c69 7a65 5f6c 6564  ..initialize_led
+000006b0: 6765 7273 da05 7374 6172 7429 06da 0473  gers..start)...s
+000006c0: 656c 6672 0a00 0000 da0a 6670 735f 7461  elfr......fps_ta
+000006d0: 7267 6574 720f 0000 00da 0673 7472 6561  rgetr......strea
+000006e0: 6dda 0171 720c 0000 0072 0c00 0000 7210  m..qr....r....r.
+000006f0: 0000 00da 085f 5f69 6e69 745f 5f14 0000  .....__init__...
+00000700: 0073 2e00 0000 0001 0601 0603 02ff 0404  .s..............
+00000710: 02ff 0404 0601 0801 0602 0601 0601 1201  ................
+00000720: 0c01 0801 0c02 0601 0802 0601 0c01 0603  ................
+00000730: 1602 0801 7a15 5379 6e63 6872 6f6e 697a  ....z.Synchroniz
+00000740: 6572 2e5f 5f69 6e69 745f 5f29 01da 0574  er.__init__)...t
+00000750: 7261 636b 6302 0000 0000 0000 0000 0000  rackc...........
+00000760: 0004 0000 0004 0000 0043 0000 0073 2200  .........C...s".
+00000770: 0000 7c00 6a00 a001 a100 4400 5d12 5c02  ..|.j.....D.].\.
+00000780: 7d02 7d03 7c03 a002 7c01 a101 0100 710a  }.}.|...|.....q.
+00000790: 6400 5300 a901 4e29 0372 0a00 0000 7219  d.S...N).r....r.
+000007a0: 0000 00da 0f73 6574 5f74 7261 636b 696e  .....set_trackin
+000007b0: 675f 6f6e 2904 7224 0000 0072 2900 0000  g_on).r$...r)...
+000007c0: 720f 0000 0072 2600 0000 720c 0000 0072  r....r&...r....r
+000007d0: 0c00 0000 7210 0000 00da 1773 6574 5f74  ....r......set_t
+000007e0: 7261 636b 696e 675f 6f6e 5f73 7472 6561  racking_on_strea
+000007f0: 6d73 3700 0000 7304 0000 0000 0112 017a  ms7...s........z
+00000800: 2453 796e 6368 726f 6e69 7a65 722e 7365  $Synchronizer.se
+00000810: 745f 7472 6163 6b69 6e67 5f6f 6e5f 7374  t_tracking_on_st
+00000820: 7265 616d 7363 0100 0000 0000 0000 0000  reamsc..........
+00000830: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00000840: 0000 007c 006a 0053 0072 2a00 0000 2901  ...|.j.S.r*...).
+00000850: 721d 0000 00a9 0172 2400 0000 720c 0000  r......r$...r...
+00000860: 0072 0c00 0000 7210 0000 00da 0e67 6574  .r....r......get
+00000870: 5f66 7073 5f74 6172 6765 743b 0000 0073  _fps_target;...s
+00000880: 0200 0000 0001 7a1b 5379 6e63 6872 6f6e  ......z.Synchron
+00000890: 697a 6572 2e67 6574 5f66 7073 5f74 6172  izer.get_fps_tar
+000008a0: 6765 7463 0100 0000 0000 0000 0000 0000  getc............
+000008b0: 0400 0000 0400 0000 4300 0000 7348 0000  ........C...sH..
+000008c0: 007c 006a 006a 017d 017c 01a0 02a1 0044  .|.j.j.}.|.....D
+000008d0: 005d 325c 027d 027d 037c 006a 037c 0219  .]2\.}.}.|.j.|..
+000008e0: 00a0 047c 03a1 0101 007c 006a 037c 0219  ...|.....|.j.|..
+000008f0: 0074 050b 0064 0085 0219 007c 006a 037c  .t...d.....|.j.|
+00000900: 023c 0071 1064 0053 0072 2a00 0000 2906  .<.q.d.S.r*...).
+00000910: da13 6375 7272 656e 745f 7379 6e63 5f70  ..current_sync_p
+00000920: 6163 6b65 74da 0764 726f 7070 6564 7219  acket..droppedr.
+00000930: 0000 0072 2100 0000 721a 0000 00da 1a44  ...r!...r......D
+00000940: 524f 5050 4544 5f46 5241 4d45 5f54 5241  ROPPED_FRAME_TRA
+00000950: 434b 5f57 494e 444f 5729 0472 2400 0000  CK_WINDOW).r$...
+00000960: 5a0f 6375 7272 656e 745f 6472 6f70 7065  Z.current_droppe
+00000970: 6472 0f00 0000 7230 0000 0072 0c00 0000  dr....r0...r....
+00000980: 720c 0000 0072 1000 0000 da1c 7570 6461  r....r......upda
+00000990: 7465 5f64 726f 7070 6564 5f66 7261 6d65  te_dropped_frame
+000009a0: 5f68 6973 746f 7279 3e00 0000 7308 0000  _history>...s...
+000009b0: 0000 0108 0210 0110 017a 2953 796e 6368  .........z)Synch
+000009c0: 726f 6e69 7a65 722e 7570 6461 7465 5f64  ronizer.update_d
+000009d0: 726f 7070 6564 5f66 7261 6d65 5f68 6973  ropped_frame_his
+000009e0: 746f 7279 6301 0000 0000 0000 0000 0000  toryc...........
+000009f0: 0001 0000 0003 0000 0043 0000 0073 1400  .........C...s..
+00000a00: 0000 6401 6402 8400 7c00 6a00 a001 a100  ..d.d...|.j.....
+00000a10: 4400 8301 5300 2903 7a4a 0a20 2020 2020  D...S.).zJ.     
+00000a20: 2020 2041 7665 7261 6765 7320 6472 6f70     Averages drop
+00000a30: 7065 6420 6672 616d 6520 636f 756e 7420  ped frame count 
+00000a40: 6163 726f 7373 2074 6865 206f 6273 6572  across the obser
+00000a50: 7665 6420 6869 7374 6f72 790a 2020 2020  ved history.    
+00000a60: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+00000a70: 0003 0000 0006 0000 0053 0000 0073 1c00  .........S...s..
+00000a80: 0000 6900 7c00 5d14 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+00000a90: 7400 a001 7c02 a101 9302 7104 5300 720c  t...|.....q.S.r.
+00000aa0: 0000 0029 02da 026e 70da 046d 6561 6e29  ...)...np..mean)
+00000ab0: 0372 0e00 0000 720f 0000 005a 0c64 726f  .r....r....Z.dro
+00000ac0: 705f 6869 7374 6f72 7972 0c00 0000 720c  p_historyr....r.
+00000ad0: 0000 0072 1000 0000 7211 0000 004a 0000  ...r....r....J..
+00000ae0: 0073 0600 0000 0600 0600 0200 7a2c 5379  .s..........z,Sy
+00000af0: 6e63 6872 6f6e 697a 6572 2e64 726f 7070  nchronizer.dropp
+00000b00: 6564 5f66 7073 2e3c 6c6f 6361 6c73 3e2e  ed_fps.<locals>.
+00000b10: 3c64 6963 7463 6f6d 703e 2902 7221 0000  <dictcomp>).r!..
+00000b20: 0072 1900 0000 722d 0000 0072 0c00 0000  .r....r-...r....
+00000b30: 720c 0000 0072 1000 0000 da0b 6472 6f70  r....r......drop
+00000b40: 7065 645f 6670 7345 0000 0073 0200 0000  ped_fpsE...s....
+00000b50: 0005 7a18 5379 6e63 6872 6f6e 697a 6572  ..z.Synchronizer
+00000b60: 2e64 726f 7070 6564 5f66 7073 6302 0000  .dropped_fpsc...
+00000b70: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00000b80: 0043 0000 0073 3800 0000 7c01 7c00 5f00  .C...s8...|.|._.
+00000b90: 7401 a002 6401 7c01 9b00 9d02 a101 0100  t...d.|.........
+00000ba0: 7c00 6a03 a004 a100 4400 5d12 5c02 7d02  |.j.....D.].\.}.
+00000bb0: 7d03 7c03 a005 7c01 a101 0100 7120 6400  }.|...|.....q d.
+00000bc0: 5300 2902 4e7a 2e41 7474 656d 7074 696e  S.).Nz.Attemptin
+00000bd0: 6720 746f 2063 6861 6e67 6520 7461 7267  g to change targ
+00000be0: 6574 2066 7073 2069 6e20 7374 7265 616d  et fps in stream
+00000bf0: 7320 746f 2029 0672 1d00 0000 da06 6c6f  s to ).r......lo
+00000c00: 6767 6572 da04 696e 666f 720a 0000 0072  gger..infor....r
+00000c10: 1900 0000 721e 0000 0029 0472 2400 0000  ....r....).r$...
+00000c20: da06 7461 7267 6574 720f 0000 0072 2600  ..targetr....r&.
+00000c30: 0000 720c 0000 0072 0c00 0000 7210 0000  ..r....r....r...
+00000c40: 0072 1e00 0000 4d00 0000 7308 0000 0000  .r....M...s.....
+00000c50: 0106 0110 0112 017a 1b53 796e 6368 726f  .......z.Synchro
+00000c60: 6e69 7a65 722e 7365 745f 6670 735f 7461  nizer.set_fps_ta
+00000c70: 7267 6574 6301 0000 0000 0000 0000 0000  rgetc...........
+00000c80: 0003 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
+00000c90: 0000 7c00 6a00 a001 a100 4400 5d18 5c02  ..|.j.....D.].\.
+00000ca0: 7d01 7d02 7c02 a002 7c00 6a03 7c01 1900  }.}.|...|.j.|...
+00000cb0: a101 0100 710a 6401 7c00 5f04 6400 5300  ....q.d.|._.d.S.
+00000cc0: 2902 4e54 2905 720a 0000 0072 1900 0000  ).NT).r....r....
+00000cd0: da09 7375 6273 6372 6962 6572 1800 0000  ..subscriber....
+00000ce0: 721b 0000 00a9 0372 2400 0000 720f 0000  r......r$...r...
+00000cf0: 0072 2600 0000 720c 0000 0072 0c00 0000  .r&...r....r....
+00000d00: 7210 0000 0072 1c00 0000 5300 0000 7306  r....r....S...s.
+00000d10: 0000 0000 0112 0112 017a 2153 796e 6368  .........z!Synch
+00000d20: 726f 6e69 7a65 722e 7375 6273 6372 6962  ronizer.subscrib
+00000d30: 655f 746f 5f73 7472 6561 6d73 6301 0000  e_to_streamsc...
+00000d40: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000d50: 0043 0000 0073 3e00 0000 7c00 6a00 a001  .C...s>...|.j...
+00000d60: a100 4400 5d28 5c02 7d01 7d02 7402 a003  ..D.](\.}.}.t...
+00000d70: 6401 7c01 9b00 9d02 a101 0100 7c02 a004  d.|.........|...
+00000d80: 7c00 6a05 7c01 1900 a101 0100 710a 6402  |.j.|.......q.d.
+00000d90: 7c00 5f06 6400 5300 2903 4e7a 2375 6e73  |._.d.S.).Nz#uns
+00000da0: 7562 7363 7269 6265 2073 796e 6368 726f  ubscribe synchro
+00000db0: 6e69 7a65 7220 6672 6f6d 2070 6f72 7420  nizer from port 
+00000dc0: 4629 0772 0a00 0000 7219 0000 0072 3600  F).r....r....r6.
+00000dd0: 0000 7237 0000 00da 0b75 6e73 7562 7363  ..r7.....unsubsc
+00000de0: 7269 6265 7218 0000 0072 1b00 0000 723a  riber....r....r:
+00000df0: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
+00000e00: 0000 da16 756e 7375 6273 6372 6962 655f  ....unsubscribe_
+00000e10: 746f 5f73 7472 6561 6d73 5800 0000 7308  to_streamsX...s.
+00000e20: 0000 0000 0112 0110 0112 017a 2353 796e  ...........z#Syn
+00000e30: 6368 726f 6e69 7a65 722e 756e 7375 6273  chronizer.unsubs
+00000e40: 6372 6962 655f 746f 5f73 7472 6561 6d73  cribe_to_streams
+00000e50: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000e60: 0003 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
+00000e70: 6a00 a001 a100 0100 7c00 6a02 a003 a100  j.......|.j.....
+00000e80: 0100 7c00 6a04 4400 5d0c 7d01 7c01 a003  ..|.j.D.].}.|...
+00000e90: a100 0100 711a 6400 5300 722a 0000 0029  ....q.d.S.r*...)
+00000ea0: 0572 1500 0000 da03 7365 74da 0674 6872  .r......set..thr
+00000eb0: 6561 64da 046a 6f69 6eda 0774 6872 6561  ead..join..threa
+00000ec0: 6473 2902 7224 0000 00da 0174 720c 0000  ds).r$.....tr...
+00000ed0: 0072 0c00 0000 7210 0000 00da 0473 746f  .r....r......sto
+00000ee0: 705e 0000 0073 0800 0000 0001 0a01 0a01  p^...s..........
+00000ef0: 0a01 7a11 5379 6e63 6872 6f6e 697a 6572  ..z.Synchronizer
+00000f00: 2e73 746f 7063 0100 0000 0000 0000 0000  .stopc..........
+00000f10: 0000 0100 0000 0200 0000 4300 0000 732e  ..........C...s.
+00000f20: 0000 0064 0164 0284 007c 006a 0044 0083  ...d.d...|.j.D..
+00000f30: 017c 005f 0164 0364 0284 007c 006a 0044  .|._.d.d...|.j.D
+00000f40: 0083 017c 005f 0267 007c 005f 0364 0053  ...|._.g.|._.d.S
+00000f50: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000f60: 0002 0000 0004 0000 0053 0000 0073 1200  .........S...s..
+00000f70: 0000 6900 7c00 5d0a 7d01 7c01 6400 9302  ..i.|.].}.|.d...
+00000f80: 7104 5300 a901 7201 0000 0072 0c00 0000  q.S...r....r....
+00000f90: 720d 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000fa0: 1000 0000 7211 0000 0066 0000 0073 0600  ....r....f...s..
+00000fb0: 0000 0600 0200 0200 7a33 5379 6e63 6872  ........z3Synchr
+00000fc0: 6f6e 697a 6572 2e69 6e69 7469 616c 697a  onizer.initializ
+00000fd0: 655f 6c65 6467 6572 732e 3c6c 6f63 616c  e_ledgers.<local
+00000fe0: 733e 2e3c 6469 6374 636f 6d70 3e63 0100  s>.<dictcomp>c..
+00000ff0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001000: 0000 5300 0000 7312 0000 0069 007c 005d  ..S...s....i.|.]
+00001010: 0a7d 017c 0164 0093 0271 0453 0072 4300  .}.|.d...q.S.rC.
+00001020: 0000 720c 0000 0072 0d00 0000 720c 0000  ..r....r....r...
+00001030: 0072 0c00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001040: 6700 0000 7306 0000 0006 0002 0002 0029  g...s..........)
+00001050: 0472 1700 0000 da10 706f 7274 5f66 7261  .r......port_fra
+00001060: 6d65 5f63 6f75 6e74 da12 706f 7274 5f63  me_count..port_c
+00001070: 7572 7265 6e74 5f66 7261 6d65 da10 6d65  urrent_frame..me
+00001080: 616e 5f66 7261 6d65 5f74 696d 6573 722d  an_frame_timesr-
+00001090: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
+000010a0: 0000 7222 0000 0064 0000 0073 0600 0000  ..r"...d...s....
+000010b0: 0002 1201 1201 7a1f 5379 6e63 6872 6f6e  ......z.Synchron
+000010c0: 697a 6572 2e69 6e69 7469 616c 697a 655f  izer.initialize_
+000010d0: 6c65 6467 6572 7363 0100 0000 0000 0000  ledgersc........
+000010e0: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+000010f0: 737e 0000 0074 00a0 0164 01a1 0101 0067  s~...t...d.....g
+00001100: 007c 005f 027c 006a 03a0 04a1 0044 005d  .|._.|.j.....D.]
+00001110: 2e5c 027d 017d 0274 057c 006a 067c 0266  .\.}.}.t.|.j.|.f
+00001120: 0164 0264 038d 037d 037c 03a0 07a1 0001  .d.d...}.|......
+00001130: 007c 006a 02a0 087c 03a1 0101 0071 1a74  .|.j...|.....q.t
+00001140: 00a0 0164 04a1 0101 0074 00a0 0164 05a1  ...d.....t...d..
+00001150: 0101 0074 057c 006a 0964 0664 0264 038d  ...t.|.j.d.d.d..
+00001160: 037c 005f 0a7c 006a 0aa0 07a1 0001 0064  .|._.|.j.......d
+00001170: 0053 0029 074e 7a2e 4162 6f75 7420 746f  .S.).Nz.About to
+00001180: 2073 7562 6d69 7420 5468 7265 6164 706f   submit Threadpo
+00001190: 6f6c 206f 6620 6672 616d 6520 4861 7276  ol of frame Harv
+000011a0: 6573 7465 7273 5429 0372 3800 0000 da04  estersT).r8.....
+000011b0: 6172 6773 da06 6461 656d 6f6e 7a1f 4672  args..daemonz.Fr
+000011c0: 616d 6520 6861 7276 6573 7465 7273 206a  ame harvesters j
+000011d0: 7573 7420 7375 626d 6974 7465 647a 1e53  ust submittedz.S
+000011e0: 7461 7274 696e 6720 6672 616d 6520 7379  tarting frame sy
+000011f0: 6e63 6872 6f6e 697a 6572 2e2e 2e72 0c00  nchronizer...r..
+00001200: 0000 290b 7236 0000 0072 3700 0000 7240  ..).r6...r7...r@
+00001210: 0000 0072 0a00 0000 7219 0000 0072 0400  ...r....r....r..
+00001220: 0000 da15 6861 7276 6573 745f 6672 616d  ....harvest_fram
+00001230: 655f 7061 636b 6574 7372 2300 0000 721a  e_packetsr#...r.
+00001240: 0000 00da 1373 796e 6368 5f66 7261 6d65  .....synch_frame
+00001250: 735f 776f 726b 6572 723e 0000 0029 0472  s_workerr>...).r
+00001260: 2400 0000 720f 0000 0072 2600 0000 7241  $...r....r&...rA
+00001270: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
+00001280: 0000 7223 0000 006a 0000 0073 1400 0000  ..r#...j...s....
+00001290: 0002 0a01 0601 1201 1201 0801 0e01 0a02  ................
+000012a0: 0a01 1201 7a12 5379 6e63 6872 6f6e 697a  ....z.Synchroniz
+000012b0: 6572 2e73 7461 7274 6302 0000 0000 0000  er.startc.......
+000012c0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+000012d0: 0073 1a00 0000 7400 a001 6401 a101 0100  .s....t...d.....
+000012e0: 7c00 6a02 a003 7c01 a101 0100 6400 5300  |.j...|.....d.S.
+000012f0: 2902 4e7a 3741 6464 696e 6720 7175 6575  ).Nz7Adding queu
+00001300: 6520 746f 2072 6563 6569 7665 206e 6f74  e to receive not
+00001310: 6963 6520 6f66 2073 796e 6368 6564 2066  ice of synched f
+00001320: 7261 6d65 7320 7570 6461 7465 2904 7236  rames update).r6
+00001330: 0000 0072 3700 0000 7212 0000 0072 1a00  ...r7...r....r..
+00001340: 0000 a902 7224 0000 0072 2700 0000 720c  ....r$...r'...r.
+00001350: 0000 0072 0c00 0000 7210 0000 00da 1373  ...r....r......s
+00001360: 7562 7363 7269 6265 5f74 6f5f 6e6f 7469  ubscribe_to_noti
+00001370: 6365 7800 0000 7304 0000 0000 040a 017a  cex...s........z
+00001380: 2053 796e 6368 726f 6e69 7a65 722e 7375   Synchronizer.su
+00001390: 6273 6372 6962 655f 746f 5f6e 6f74 6963  bscribe_to_notic
+000013a0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+000013b0: 0000 0300 0000 4300 0000 731a 0000 0074  ......C...s....t
+000013c0: 00a0 0164 01a1 0101 007c 006a 02a0 037c  ...d.....|.j...|
+000013d0: 01a1 0101 0064 0053 0029 024e 7a46 5265  .....d.S.).NzFRe
+000013e0: 6d6f 7669 6e67 2071 7565 7565 2074 6861  moving queue tha
+000013f0: 7420 6861 6420 6265 656e 2072 6563 6569  t had been recei
+00001400: 7669 6e67 206e 6f74 6963 6520 6f66 2073  ving notice of s
+00001410: 796e 6368 6564 2066 7261 6d65 7320 7570  ynched frames up
+00001420: 6461 7465 2904 7236 0000 0072 3700 0000  date).r6...r7...
+00001430: 7212 0000 00da 0672 656d 6f76 6572 4b00  r......removerK.
+00001440: 0000 720c 0000 0072 0c00 0000 7210 0000  ..r....r....r...
+00001450: 00da 1575 6e73 7562 7363 7269 6265 5f74  ...unsubscribe_t
+00001460: 6f5f 6e6f 7469 6365 7f00 0000 7304 0000  o_notice....s...
+00001470: 0000 040a 017a 2253 796e 6368 726f 6e69  .....z"Synchroni
+00001480: 7a65 722e 756e 7375 6273 6372 6962 655f  zer.unsubscribe_
+00001490: 746f 5f6e 6f74 6963 6563 0200 0000 0000  to_noticec......
+000014a0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000014b0: 0000 731a 0000 0074 00a0 0164 01a1 0101  ..s....t...d....
+000014c0: 007c 006a 02a0 037c 01a1 0101 0064 0053  .|.j...|.....d.S
+000014d0: 0029 024e 7a26 4164 6469 6e67 2071 7565  .).Nz&Adding que
+000014e0: 7565 2074 6f20 7265 6365 6976 6520 7379  ue to receive sy
+000014f0: 6e63 6865 6420 6672 616d 6573 2904 7236  nched frames).r6
+00001500: 0000 0072 3700 0000 7213 0000 0072 1a00  ...r7...r....r..
+00001510: 0000 724b 0000 0072 0c00 0000 720c 0000  ..rK...r....r...
+00001520: 0072 1000 0000 da19 7375 6273 6372 6962  .r......subscrib
+00001530: 655f 746f 5f73 796e 635f 7061 636b 6574  e_to_sync_packet
+00001540: 7387 0000 0073 0400 0000 0001 0a01 7a26  s....s........z&
+00001550: 5379 6e63 6872 6f6e 697a 6572 2e73 7562  Synchronizer.sub
+00001560: 7363 7269 6265 5f74 6f5f 7379 6e63 5f70  scribe_to_sync_p
+00001570: 6163 6b65 7473 6302 0000 0000 0000 0000  acketsc.........
+00001580: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00001590: 1a00 0000 7400 a001 6401 a101 0100 7c00  ....t...d.....|.
+000015a0: 6a02 a003 7c01 a101 0100 6400 5300 2902  j...|.....d.S.).
+000015b0: 4e7a 1652 656c 6561 7369 6e67 2072 6563  Nz.Releasing rec
+000015c0: 6f72 6420 7175 6575 6529 0472 3600 0000  ord queue).r6...
+000015d0: 7237 0000 0072 1300 0000 724d 0000 0072  r7...r....rM...r
+000015e0: 4b00 0000 720c 0000 0072 0c00 0000 7210  K...r....r....r.
+000015f0: 0000 00da 1572 656c 6561 7365 5f73 796e  .....release_syn
+00001600: 635f 7061 636b 6574 5f71 8b00 0000 7304  c_packet_q....s.
+00001610: 0000 0000 010a 017a 2253 796e 6368 726f  .......z"Synchro
+00001620: 6e69 7a65 722e 7265 6c65 6173 655f 7379  nizer.release_sy
+00001630: 6e63 5f70 6163 6b65 745f 7163 0200 0000  nc_packet_qc....
+00001640: 0000 0000 0000 0000 0500 0000 0800 0000  ................
+00001650: 4300 0000 73a0 0000 007c 016a 007d 0274  C...s....|.j.}.t
+00001660: 01a0 0264 017c 029b 009d 02a1 0101 007c  ...d.|.........|
+00001670: 006a 03a0 04a1 0073 8a7c 006a 057c 0219  .j.....s.|.j.|..
+00001680: 00a0 06a1 007d 037c 006a 077c 0219 007d  .....}.|.j.|...}
+00001690: 047c 047c 035f 087c 037c 006a 097c 029b  .|.|._.|.|.j.|..
+000016a0: 0064 027c 036a 089b 009d 033c 007c 006a  .d.|.j.....<.|.j
+000016b0: 077c 0205 0019 0064 0337 0003 003c 0074  .|.....d.7...<.t
+000016c0: 01a0 0a64 047c 036a 009b 0064 057c 036a  ...d.|.j...d.|.j
+000016d0: 089b 0064 067c 036a 0b9b 009d 06a1 0101  ...d.|.j........
+000016e0: 0071 1674 01a0 0264 077c 029b 0064 089d  .q.t...d.|...d..
+000016f0: 03a1 0101 0064 0053 0029 094e 7a2c 4265  .....d.S.).Nz,Be
+00001700: 6769 6e6e 696e 6720 746f 2063 6f6c 6c65  ginning to colle
+00001710: 6374 2064 6174 6120 6765 6e65 7261 7465  ct data generate
+00001720: 6420 6174 2070 6f72 7420 da01 5fe9 0100  d at port .._...
+00001730: 0000 7a1f 4672 616d 6520 6461 7461 2068  ..z.Frame data h
+00001740: 6172 7665 7374 6564 2066 726f 6d20 7265  arvested from re
+00001750: 656c 207a 0c20 7769 7468 2069 6e64 6578  el z. with index
+00001760: 207a 1320 616e 6420 6672 616d 6520 7469   z. and frame ti
+00001770: 6d65 206f 6620 7a19 4672 616d 6520 6861  me of z.Frame ha
+00001780: 7276 6573 7465 7220 666f 7220 706f 7274  rvester for port
+00001790: 207a 0a20 636f 6d70 6c65 7465 6429 0c72   z. completed).r
+000017a0: 0f00 0000 7236 0000 0072 3700 0000 7215  ....r6...r7...r.
+000017b0: 0000 00da 0669 735f 7365 7472 1800 0000  .....is_setr....
+000017c0: da03 6765 7472 4400 0000 da0b 6672 616d  ..getrD.....fram
+000017d0: 655f 696e 6465 7872 1400 0000 da05 6465  e_indexr......de
+000017e0: 6275 67da 0a66 7261 6d65 5f74 696d 6529  bug..frame_time)
+000017f0: 0572 2400 0000 7226 0000 0072 0f00 0000  .r$...r&...r....
+00001800: da0c 6672 616d 655f 7061 636b 6574 7255  ..frame_packetrU
+00001810: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
+00001820: 0000 7249 0000 008f 0000 0073 1800 0000  ..rI.......s....
+00001830: 0001 0602 1002 0a01 0e01 0a01 0602 1601  ................
+00001840: 1202 0401 1aff 0604 7a22 5379 6e63 6872  ........z"Synchr
+00001850: 6f6e 697a 6572 2e68 6172 7665 7374 5f66  onizer.harvest_f
+00001860: 7261 6d65 5f70 6163 6b65 7473 6302 0000  rame_packetsc...
+00001870: 0000 0000 0000 0000 0007 0000 0006 0000  ................
+00001880: 0043 0000 0073 b800 0000 6700 7d02 7c00  .C...s....g.}.|.
+00001890: 6a00 4400 5da4 7d03 7c00 6a01 7c03 1900  j.D.].}.|.j.|...
+000018a0: 6401 1700 7d04 7c03 9b00 6402 7c04 9b00  d...}.|...d.|...
+000018b0: 9d03 7d05 7c05 7c00 6a02 a003 a100 6b07  ..}.|.|.j.....k.
+000018c0: 7266 7404 a005 6403 7c05 9b00 9d02 a101  rft...d.|.......
+000018d0: 0100 7c00 6a06 725a 7407 a008 6404 a101  ..|.j.rZt...d...
+000018e0: 0100 712a 7407 a008 6401 a101 0100 712a  ..q*t...d.....q*
+000018f0: 7c00 6a02 7c05 1900 6a09 7d06 7c06 6405  |.j.|...j.}.|.d.
+00001900: 6b02 729c 7404 a005 6406 7c03 9b00 6407  k.r.t...d.|...d.
+00001910: 9d03 a101 0100 6408 7c00 5f0a 7c00 6a0b  ......d.|._.|.j.
+00001920: a00c a100 0100 7c03 7c01 6b03 720a 7c02  ......|.|.k.r.|.
+00001930: a00d 7c06 a101 0100 710a 740e 7c02 8301  ..|.....q.t.|...
+00001940: 5300 2909 7a75 4c6f 6f6b 7320 6174 206e  S.).zuLooks at n
+00001950: 6578 7420 756e 6173 7369 676e 6564 2066  ext unassigned f
+00001960: 7261 6d65 2061 6372 6f73 7320 7468 6520  rame across the 
+00001970: 706f 7274 7320 746f 2064 6574 6572 6d69  ports to determi
+00001980: 6e65 0a20 2020 2020 2020 2074 6865 2065  ne.        the e
+00001990: 6172 6c69 6573 7420 7469 6d65 2061 7420  arliest time at 
+000019a0: 7768 6963 6820 6561 6368 206f 6620 7468  which each of th
+000019b0: 656d 2077 6173 2072 6561 6472 5200 0000  em was readrR...
+000019c0: 7251 0000 007a 3757 6169 7469 6e67 2069  rQ...z7Waiting i
+000019d0: 6e20 6120 6c6f 6f70 2066 6f72 2066 7261  n a loop for fra
+000019e0: 6d65 2064 6174 6120 746f 2070 6f70 756c  me data to popul
+000019f0: 6174 6520 7769 7468 206b 6579 3a20 679a  ate with key: g.
+00001a00: 9999 9999 99b9 3f72 0b00 0000 7a16 456e  ......?r....z.En
+00001a10: 6420 6f66 2066 7261 6d65 7320 6174 2070  d of frames at p
+00001a20: 6f72 7420 7a21 2064 6574 6563 7465 643b  ort z! detected;
+00001a30: 2065 6e64 696e 6720 7379 6e63 6872 6f6e   ending synchron
+00001a40: 697a 6174 696f 6e54 290f 7217 0000 0072  izationT).r....r
+00001a50: 4500 0000 7214 0000 00da 046b 6579 7372  E...r......keysr
+00001a60: 3600 0000 7237 0000 0072 1b00 0000 da04  6...r7...r......
+00001a70: 7469 6d65 da05 736c 6565 7072 5700 0000  time..sleeprW...
+00001a80: 7216 0000 0072 1500 0000 723d 0000 0072  r....r....r=...r
+00001a90: 1a00 0000 da03 6d69 6e29 0772 2400 0000  ......min).r$...
+00001aa0: 720f 0000 005a 1474 696d 6573 5f6f 665f  r....Z.times_of_
+00001ab0: 6e65 7874 5f66 7261 6d65 73da 0170 5a0a  next_frames..pZ.
+00001ac0: 6e65 7874 5f69 6e64 6578 da0e 6672 616d  next_index..fram
+00001ad0: 655f 6461 7461 5f6b 6579 5a0f 6e65 7874  e_data_keyZ.next
+00001ae0: 5f66 7261 6d65 5f74 696d 6572 0c00 0000  _frame_timer....
+00001af0: 720c 0000 0072 1000 0000 da13 6561 726c  r....r......earl
+00001b00: 6965 7374 5f6e 6578 745f 6672 616d 65a3  iest_next_frame.
+00001b10: 0000 0073 2a00 0000 0003 0401 0a01 0e01  ...s*...........
+00001b20: 0e03 0e01 0401 08ff 0403 0601 0c02 0c02  ................
+00001b30: 0c02 0801 0401 0aff 0403 0601 0a02 0801  ................
+00001b40: 0c02 7a20 5379 6e63 6872 6f6e 697a 6572  ..z Synchronizer
+00001b50: 2e65 6172 6c69 6573 745f 6e65 7874 5f66  .earliest_next_f
+00001b60: 7261 6d65 6302 0000 0000 0000 0000 0000  ramec...........
+00001b70: 0007 0000 0004 0000 0043 0000 0073 4e00  .........C...sN.
+00001b80: 0000 6700 7d02 7c00 6a00 4400 5d3a 7d03  ..g.}.|.j.D.]:}.
+00001b90: 7c00 6a01 7c03 1900 7d04 7c03 9b00 6401  |.j.|...}.|...d.
+00001ba0: 7c04 9b00 9d03 7d05 7c00 6a02 7c05 1900  |.....}.|.j.|...
+00001bb0: 6a03 7d06 7c03 7c01 6b03 720a 7c02 a004  j.}.|.|.k.r.|...
+00001bc0: 7c06 a101 0100 710a 7405 7c02 8301 5300  |.....q.t.|...S.
+00001bd0: 2902 7a57 5072 6f76 6964 6573 2074 6865  ).zWProvides the
+00001be0: 206c 6174 6573 7420 6672 616d 655f 7469   latest frame_ti
+00001bf0: 6d65 206f 6620 7468 6520 6375 7272 656e  me of the curren
+00001c00: 7420 6672 616d 6573 206e 6f74 2069 6e63  t frames not inc
+00001c10: 6c75 7369 7665 206f 6620 7468 6520 7072  lusive of the pr
+00001c20: 6f76 6964 6564 2070 6f72 7472 5100 0000  ovided portrQ...
+00001c30: 2906 7217 0000 0072 4500 0000 7214 0000  ).r....rE...r...
+00001c40: 0072 5700 0000 721a 0000 00da 036d 6178  .rW...r......max
+00001c50: 2907 7224 0000 0072 0f00 0000 5a17 7469  ).r$...r....Z.ti
+00001c60: 6d65 735f 6f66 5f63 7572 7265 6e74 5f66  mes_of_current_f
+00001c70: 7261 6d65 7372 5d00 0000 5a0d 6375 7272  ramesr]...Z.curr
+00001c80: 656e 745f 696e 6465 7872 5e00 0000 5a12  ent_indexr^...Z.
+00001c90: 6375 7272 656e 745f 6672 616d 655f 7469  current_frame_ti
+00001ca0: 6d65 720c 0000 0072 0c00 0000 7210 0000  mer....r....r...
+00001cb0: 00da 146c 6174 6573 745f 6375 7272 656e  ...latest_curren
+00001cc0: 745f 6672 616d 65c3 0000 0073 1000 0000  t_frame....s....
+00001cd0: 0002 0401 0a01 0a01 0e01 0c01 0801 0c02  ................
+00001ce0: 7a21 5379 6e63 6872 6f6e 697a 6572 2e6c  z!Synchronizer.l
+00001cf0: 6174 6573 745f 6375 7272 656e 745f 6672  atest_current_fr
+00001d00: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
+00001d10: 0200 0000 0400 0000 0300 0000 732c 0000  ............s,..
+00001d20: 0087 0066 0164 0164 0284 0888 006a 0044  ...f.d.d.....j.D
+00001d30: 0083 017d 0174 01a0 0264 037c 019b 009d  ...}.t...d.|....
+00001d40: 02a1 0101 0074 037c 0183 0153 0029 047a  .....t.|...S.).z
+00001d50: 4244 6574 6572 6d69 6e65 2068 6f77 206d  BDetermine how m
+00001d60: 616e 7920 756e 6173 7369 676e 6564 2066  any unassigned f
+00001d70: 7261 6d65 7320 6172 6520 7369 7474 696e  rames are sittin
+00001d80: 6720 696e 2073 656c 662e 6461 7461 6672  g in self.datafr
+00001d90: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
+00001da0: 0200 0000 0500 0000 1300 0000 7320 0000  ............s ..
+00001db0: 0067 007c 005d 187d 0188 006a 007c 0119  .g.|.].}...j.|..
+00001dc0: 0088 006a 017c 0119 0018 0091 0271 0453  ...j.|.......q.S
+00001dd0: 0072 0c00 0000 2902 7244 0000 0072 4500  .r....).rD...rE.
+00001de0: 0000 720d 0000 0072 2d00 0000 720c 0000  ..r....r-...r...
+00001df0: 0072 1000 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00001e00: 703e d100 0000 7304 0000 0006 0202 ff7a  p>....s........z
+00001e10: 2c53 796e 6368 726f 6e69 7a65 722e 6672  ,Synchronizer.fr
+00001e20: 616d 655f 736c 6163 6b2e 3c6c 6f63 616c  ame_slack.<local
+00001e30: 733e 2e3c 6c69 7374 636f 6d70 3e7a 1353  s>.<listcomp>z.S
+00001e40: 6c61 636b 2069 6e20 6672 616d 6573 2069  lack in frames i
+00001e50: 7320 2904 7217 0000 0072 3600 0000 7256  s ).r....r6...rV
+00001e60: 0000 0072 5c00 0000 2902 7224 0000 005a  ...r\...).r$...Z
+00001e70: 0573 6c61 636b 720c 0000 0072 2d00 0000  .slackr....r-...
+00001e80: 7210 0000 00da 0b66 7261 6d65 5f73 6c61  r......frame_sla
+00001e90: 636b cf00 0000 730a 0000 0000 020a 0204  ck....s.........
+00001ea0: fe06 0410 017a 1853 796e 6368 726f 6e69  .....z.Synchroni
+00001eb0: 7a65 722e 6672 616d 655f 736c 6163 6b63  zer.frame_slackc
+00001ec0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00001ed0: 0300 0000 4300 0000 733c 0000 0074 007c  ....C...s<...t.|
+00001ee0: 006a 0183 0164 016b 0472 1e7c 006a 0164  .j...d.k.r.|.j.d
+00001ef0: 0264 0085 0219 007c 005f 0174 02a0 037c  .d.....|._.t...|
+00001f00: 006a 01a1 017d 0174 02a0 047c 01a1 017d  .j...}.t...|...}
+00001f10: 0264 037c 021b 0053 0029 044e e90a 0000  .d.|...S.).N....
+00001f20: 0069 f6ff ffff 7252 0000 0029 05da 036c  .i....rR...)...l
+00001f30: 656e 7246 0000 0072 3300 0000 da04 6469  enrF...r3.....di
+00001f40: 6666 7234 0000 0029 0372 2400 0000 5a07  ffr4...).r$...Z.
+00001f50: 6465 6c74 615f 745a 0c6d 6561 6e5f 6465  delta_tZ.mean_de
+00001f60: 6c74 615f 7472 0c00 0000 720c 0000 0072  lta_tr....r....r
+00001f70: 1000 0000 da0b 6176 6572 6167 655f 6670  ......average_fp
+00001f80: 73d8 0000 0073 0a00 0000 0001 0e01 1002  s....s..........
+00001f90: 0c01 0a02 7a18 5379 6e63 6872 6f6e 697a  ....z.Synchroniz
+00001fa0: 6572 2e61 7665 7261 6765 5f66 7073 6301  er.average_fpsc.
+00001fb0: 0000 0000 0000 0000 0000 000c 0000 0009  ................
+00001fc0: 0000 0043 0000 0073 0a02 0000 7400 a001  ...C...s....t...
+00001fd0: 6401 a101 0100 6402 7d01 7400 a001 6403  d.....d.}.t...d.
+00001fe0: a101 0100 7c00 6a02 a003 a100 9001 73fc  ....|.j.......s.
+00001ff0: 6900 7d02 6700 7d03 6900 7d04 6900 7d05  i.}.g.}.i.}.i.}.
+00002000: 7c00 6a04 4400 5d2a 7d06 7c00 a005 7c06  |.j.D.]*}.|...|.
+00002010: a101 7c04 7c06 3c00 7c00 a006 7c06 a101  ..|.|.<.|...|...
+00002020: 7c05 7c06 3c00 7c00 6a07 7c06 1900 7d07  |.|.<.|.j.|...}.
+00002030: 713a 7c00 6a04 4400 5dd0 7d06 7c00 6a07  q:|.j.D.].}.|.j.
+00002040: 7c06 1900 7d07 7c06 9b00 6404 7c07 9b00  |...}.|...d.|...
+00002050: 9d03 7d08 7c00 6a08 7c08 1900 7d09 7c09  ..}.|.j.|...}.|.
+00002060: 6a09 7d0a 7c0a 7c04 7c06 1900 6b04 72c0  j.}.|.|.|...k.r.
+00002070: 6400 7c02 7c06 3c00 7400 a00a 6405 7c06  d.|.|.<.t...d.|.
+00002080: 9b00 6406 9d03 a101 0100 716c 7c04 7c06  ..d.......ql|.|.
+00002090: 1900 7c0a 1800 7c0a 7c05 7c06 1900 1800  ..|...|.|.|.....
+000020a0: 6b00 72f4 6400 7c02 7c06 3c00 7400 a00a  k.r.d.|.|.<.t...
+000020b0: 6405 7c06 9b00 6407 9d03 a101 0100 716c  d.|...d.......ql
+000020c0: 7c00 6a08 a00b 7c08 a101 7c02 7c06 3c00  |.j...|...|.|.<.
+000020d0: 7c00 6a07 7c06 0500 1900 6408 3700 0300  |.j.|.....d.7...
+000020e0: 3c00 7c03 a00c 7c0a a101 0100 7400 a00d  <.|...|.....t...
+000020f0: 6409 7c06 9b00 640a 7c07 9b00 640b 7c0a  d.|...d.|...d.|.
+00002100: 9b00 9d06 a101 0100 716c 7400 a00d 640c  ........qlt...d.
+00002110: 740e 7c00 6a08 8301 9b00 9d02 a101 0100  t.|.j...........
+00002120: 7c00 6a0f a00c 7410 a011 7c03 a101 a101  |.j...t...|.....
+00002130: 0100 7412 7c01 7c02 8302 7c00 5f13 7c00  ..t.|.|...|._.|.
+00002140: a014 a100 0100 7c01 6408 3700 7d01 7c00  ......|.d.7.}.|.
+00002150: 6a02 a003 a100 9001 729e 7400 a001 640d  j.......r.t...d.
+00002160: a101 0100 6400 7c00 5f13 7c00 6a15 4400  ....d.|._.|.j.D.
+00002170: 5d20 7d0b 7400 a00d 640e 7c0b 9b00 9d02  ] }.t...d.|.....
+00002180: a101 0100 7c0b a016 640f a101 0100 9001  ....|...d.......
+00002190: 71a4 7c00 6a17 4400 5d22 7d0b 7400 a00d  q.|.j.D.]"}.t...
+000021a0: 6410 7c0b 9b00 9d02 a101 0100 7c0b a016  d.|.........|...
+000021b0: 7c00 6a13 a101 0100 9001 71cc 7c00 a018  |.j.......q.|...
+000021c0: a100 7c00 5f19 7118 7400 a001 6411 a101  ..|._.q.t...d...
+000021d0: 0100 6400 5300 2912 4e7a 3457 6169 7469  ..d.S.).Nz4Waiti
+000021e0: 6e67 2066 6f72 2061 6c6c 2070 6f72 7473  ng for all ports
+000021f0: 2074 6f20 6265 6769 6e20 6861 7276 6573   to begin harves
+00002200: 7469 6e67 2063 6f72 6e65 7273 2e2e 2e72  ting corners...r
+00002210: 0100 0000 7a26 4162 6f75 7420 746f 2073  ....z&About to s
+00002220: 7461 7274 2073 796e 6368 726f 6e69 7a69  tart synchronizi
+00002230: 6e67 2066 7261 6d65 732e 2e2e 7251 0000  ng frames...rQ..
+00002240: 007a 1653 6b69 7070 6564 2066 7261 6d65  .z.Skipped frame
+00002250: 2061 7420 706f 7274 207a 113a 203e 2065   at port z.: > e
+00002260: 6172 6c69 6573 745f 6e65 7874 7a1d 3a20  arliest_nextz.: 
+00002270: 6465 6c74 6120 3c20 7469 6d65 2d6c 6174  delta < time-lat
+00002280: 6573 745f 6375 7272 656e 7472 5200 0000  est_currentrR...
+00002290: 7a1a 4164 6469 6e67 2074 6f20 6c61 7965  z.Adding to laye
+000022a0: 7220 6672 6f6d 2070 6f72 7420 7a0a 2061  r from port z. a
+000022b0: 7420 696e 6465 7820 7a11 2061 6e64 2066  t index z. and f
+000022c0: 7261 6d65 2074 696d 653a 207a 1355 6e61  rame time: z.Una
+000022d0: 7373 6967 6e65 6420 4672 616d 6573 3a20  ssigned Frames: 
+000022e0: 7a37 5365 6e64 696e 6720 604e 6f6e 6560  z7Sending `None`
+000022f0: 206f 6e20 7175 6575 6520 746f 2073 6967   on queue to sig
+00002300: 6e61 6c20 656e 6420 6f66 2073 796e 6365  nal end of synce
+00002310: 6420 6672 616d 6573 2e7a 2f47 6976 696e  d frames.z/Givin
+00002320: 6720 6e6f 7469 6365 206f 6620 6e65 7720  g notice of new 
+00002330: 7379 6e63 6865 6420 6672 616d 6573 2070  synched frames p
+00002340: 6163 6b65 7420 7669 6120 7a1c 6e65 7720  acket via z.new 
+00002350: 7379 6e63 6865 6420 6672 616d 6573 2061  synched frames a
+00002360: 7661 696c 6162 6c65 7a2c 506c 6163 696e  vailablez,Placin
+00002370: 6720 6e65 7720 7379 6e63 6865 6420 6672  g new synched fr
+00002380: 616d 6573 2070 6163 6b65 7420 6f6e 2071  ames packet on q
+00002390: 7565 7565 3a20 7a25 4672 616d 6520 7379  ueue: z%Frame sy
+000023a0: 6e63 6820 776f 726b 6572 2073 7563 6365  nch worker succe
+000023b0: 7373 6675 6c6c 7920 656e 6465 6429 1a72  ssfully ended).r
+000023c0: 3600 0000 7237 0000 0072 1500 0000 7253  6...r7...r....rS
+000023d0: 0000 0072 1700 0000 725f 0000 0072 6100  ...r....r_...ra.
+000023e0: 0000 7245 0000 0072 1400 0000 7257 0000  ..rE...r....rW..
+000023f0: 00da 0777 6172 6e69 6e67 da03 706f 7072  ...warning..popr
+00002400: 1a00 0000 7256 0000 0072 6500 0000 7246  ....rV...re...rF
+00002410: 0000 0072 3300 0000 7234 0000 0072 0600  ...r3...r4...r..
+00002420: 0000 722f 0000 0072 3200 0000 7212 0000  ..r/...r2...r...
+00002430: 00da 0370 7574 7213 0000 0072 6700 0000  ...putr....rg...
+00002440: 721f 0000 0029 0c72 2400 0000 da0a 7379  r....).r$.....sy
+00002450: 6e63 5f69 6e64 6578 5a15 6375 7272 656e  nc_indexZ.curren
+00002460: 745f 6672 616d 655f 7061 636b 6574 735a  t_frame_packetsZ
+00002470: 116c 6179 6572 5f66 7261 6d65 5f74 696d  .layer_frame_tim
+00002480: 6573 5a0d 6561 726c 6965 7374 5f6e 6578  esZ.earliest_nex
+00002490: 745a 0e6c 6174 6573 745f 6375 7272 656e  tZ.latest_curren
+000024a0: 7472 0f00 0000 5a13 6375 7272 656e 745f  tr....Z.current_
+000024b0: 6672 616d 655f 696e 6465 785a 0e70 6f72  frame_indexZ.por
+000024c0: 745f 696e 6465 785f 6b65 795a 1463 7572  t_index_keyZ.cur
+000024d0: 7265 6e74 5f66 7261 6d65 5f70 6163 6b65  rent_frame_packe
+000024e0: 7472 5700 0000 7227 0000 0072 0c00 0000  trW...r'...r....
+000024f0: 720c 0000 0072 1000 0000 724a 0000 00e1  r....r....rJ....
+00002500: 0000 0073 6400 0000 0002 0a02 0402 0a01  ...sd...........
+00002510: 0c02 0402 0404 0401 0402 0a01 0e01 0e01  ................
+00002520: 0c02 0a01 0a02 0e01 0a01 0603 0c02 0801  ................
+00002530: 1402 16ff 0205 0801 0401 0aff 0605 0601  ................
+00002540: 02ff 0804 1201 0a01 0401 14ff 0604 1602  ................
+00002550: 1202 0c02 0802 0802 0c01 0a01 0604 0a01  ................
+00002560: 1001 0e02 0a01 1001 1002 0c02 7a20 5379  ............z Sy
+00002570: 6e63 6872 6f6e 697a 6572 2e73 796e 6368  nchronizer.synch
+00002580: 5f66 7261 6d65 735f 776f 726b 6572 4e29  _frames_workerN)
+00002590: 0172 0900 0000 291b da08 5f5f 6e61 6d65  .r....)...__name
+000025a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000025b0: 5f5f 7175 616c 6e61 6d65 5f5f da04 6469  __qualname__..di
+000025c0: 6374 7228 0000 00da 0462 6f6f 6c72 2c00  ctr(.....boolr,.
+000025d0: 0000 722e 0000 0072 3200 0000 da08 7072  ..r....r2.....pr
+000025e0: 6f70 6572 7479 7235 0000 0072 1e00 0000  opertyr5...r....
+000025f0: 721c 0000 0072 3c00 0000 7242 0000 0072  r....r<...rB...r
+00002600: 2200 0000 7223 0000 0072 4c00 0000 724e  "...r#...rL...rN
+00002610: 0000 0072 4f00 0000 7250 0000 0072 4900  ...rO...rP...rI.
+00002620: 0000 725f 0000 0072 6100 0000 7263 0000  ..r_...ra...rc..
+00002630: 0072 6700 0000 724a 0000 0072 0c00 0000  .rg...rJ...r....
+00002640: 720c 0000 0072 0c00 0000 7210 0000 0072  r....r....r....r
+00002650: 0800 0000 1300 0000 732c 0000 0008 0110  ........s,......
+00002660: 230e 0408 0308 0702 010a 0708 0608 0508  #...............
+00002670: 0608 0608 0608 0e08 0708 0808 0408 0408  ................
+00002680: 1408 2008 0c08 0908 0972 0800 0000 da08  .. ......r......
+00002690: 5f5f 6d61 696e 5f5f 2901 da07 4368 6172  __main__)...Char
+000026a0: 7563 6f29 01da 0e43 6861 7275 636f 5472  uco)...CharucoTr
+000026b0: 6163 6b65 7229 02da 0e52 6563 6f72 6465  acker)...Recorde
+000026c0: 6453 7472 6561 6dda 1252 6563 6f72 6465  dStream..Recorde
+000026d0: 6453 7472 6561 6d50 6f6f 6c29 01da 0753  dStreamPool)...S
+000026e0: 6573 7369 6f6e 2901 da08 5f5f 726f 6f74  ession)...__root
+000026f0: 5f5f 46da 0574 6573 7473 5a03 3231 3754  __F..testsZ.217T
+00002700: 7a15 4372 6561 7469 6e67 2053 796e 6368  z.Creating Synch
+00002710: 726f 6e69 7a65 72e9 0500 0000 2901 7225  ronizer.....).r%
+00002720: 0000 0072 5200 0000 e902 0000 00e9 0300  ...rR...........
+00002730: 0000 e904 0000 005a 0873 6573 7369 6f6e  .......Z.session
+00002740: 73e9 0b00 0000 6700 0000 0000 0021 4067  s.....g......!@g
+00002750: 0000 0000 0000 e83f 6700 0000 0000 0015  .......?g.......
+00002760: 4029 03da 0b61 7275 636f 5f73 6361 6c65  @)...aruco_scale
+00002770: da16 7371 7561 7265 5f73 697a 655f 6f76  ..square_size_ov
+00002780: 6572 6964 655f 636d da08 696e 7665 7274  eride_cm..invert
+00002790: 6564 2901 da07 6368 6172 7563 6fe9 1400  ed)...charuco...
+000027a0: 0000 7a16 4265 6769 6e6e 696e 6720 706c  ..z.Beginning pl
+000027b0: 6179 6261 636b 2061 7420 7a05 506f 7274  ayback at z.Port
+000027c0: 2072 2700 0000 7a15 506c 6179 6261 636b   r'...z.Playback
+000027d0: 2066 696e 6973 6865 6420 6174 2029 43da   finished at )C.
+000027e0: 0d70 7978 7933 642e 6c6f 6767 6572 da06  .pyxy3d.logger..
+000027f0: 7079 7879 3364 7236 0000 0072 5400 0000  pyxy3dr6...rT...
+00002800: 726c 0000 00da 076c 6f67 6769 6e67 da08  rl.....logging..
+00002810: 7365 744c 6576 656c da05 4445 4255 4772  setLevel..DEBUGr
+00002820: 5a00 0000 da07 7061 7468 6c69 6272 0200  Z.....pathlibr..
+00002830: 0000 da05 7175 6575 6572 0300 0000 da09  ....queuer......
+00002840: 7468 7265 6164 696e 6772 0400 0000 7205  threadingr....r.
+00002850: 0000 00da 0363 7632 da05 6e75 6d70 7972  .....cv2..numpyr
+00002860: 3300 0000 da1b 7079 7879 3364 2e63 616d  3.....pyxy3d.cam
+00002870: 6572 6173 2e64 6174 615f 7061 636b 6574  eras.data_packet
+00002880: 7372 0600 0000 7231 0000 0072 0800 0000  sr....r1...r....
+00002890: da1a 7079 7879 3364 2e63 616c 6962 7261  ..pyxy3d.calibra
+000028a0: 7469 6f6e 2e63 6861 7275 636f 7273 0000  tion.charucors..
+000028b0: 00da 1d70 7978 7933 642e 696d 6732 7879  ...pyxy3d.img2xy
+000028c0: 2e63 6861 7275 636f 5f74 7261 636b 6572  .charuco_tracker
+000028d0: 7274 0000 005a 2070 7978 7933 642e 7265  rt...Z pyxy3d.re
+000028e0: 636f 7264 696e 672e 7265 636f 7264 6564  cording.recorded
+000028f0: 5f73 7472 6561 6d72 7500 0000 7276 0000  _streamru...rv..
+00002900: 00da 0e70 7978 7933 642e 7365 7373 696f  ...pyxy3d.sessio
+00002910: 6e72 7700 0000 7278 0000 005a 0974 6573  nrw...rx...Z.tes
+00002920: 745f 6c69 7665 da11 7365 7373 696f 6e5f  t_live..session_
+00002930: 6469 7265 6374 6f72 79da 0773 6573 7369  directory..sessi
+00002940: 6f6e da0c 6c6f 6164 5f63 616d 6572 6173  on..load_cameras
+00002950: da0c 6c6f 6164 5f73 7472 6561 6d73 720a  ..load_streamsr.
+00002960: 0000 0072 1900 0000 720f 0000 0072 2600  ...r....r....r&.
+00002970: 0000 da09 5f73 686f 775f 6670 73da 0d5f  ...._show_fps.._
+00002980: 7368 6f77 5f63 6861 7275 636f 7237 0000  show_charucor7..
+00002990: 005a 0573 796e 6372 7217 0000 005a 1372  .Z.syncrr....Z.r
+000029a0: 6563 6f72 6469 6e67 5f64 6972 6563 746f  ecording_directo
+000029b0: 7279 7282 0000 005a 1472 6563 6f72 6465  ryr....Z.recorde
+000029c0: 645f 7374 7265 616d 5f70 6f6f 6c5a 0b70  d_stream_poolZ.p
+000029d0: 6c61 795f 7669 6465 6f73 5a0e 6e6f 7469  lay_videosZ.noti
+000029e0: 6669 6361 7469 6f6e 5f71 724c 0000 00da  fication_qrL....
+000029f0: 0c70 6572 665f 636f 756e 7465 7272 1500  .perf_counterr..
+00002a00: 0000 7253 0000 005a 1573 796e 6368 6564  ..rS...Z.synched
+00002a10: 5f66 7261 6d65 735f 6e6f 7469 6365 722f  _frames_noticer/
+00002a20: 0000 005a 0b73 796e 635f 7061 636b 6574  ...Z.sync_packet
+00002a30: da0d 6672 616d 655f 7061 636b 6574 7372  ..frame_packetsr
+00002a40: 5800 0000 da06 696d 7368 6f77 da05 6672  X.....imshow..fr
+00002a50: 616d 65da 0777 6169 744b 6579 da03 6b65  ame..waitKey..ke
+00002a60: 79da 036f 7264 da11 6465 7374 726f 7941  y..ord..destroyA
+00002a70: 6c6c 5769 6e64 6f77 7372 0c00 0000 720c  llWindowsr....r.
+00002a80: 0000 0072 0c00 0000 7210 0000 00da 083c  ...r....r......<
+00002a90: 6d6f 6475 6c65 3e01 0000 0073 8200 0000  module>....s....
+00002aa0: 0802 0c01 0802 0c02 0801 0c01 0c01 1002  ................
+00002ab0: 0801 0801 0c02 0402 0e7f 007f 0025 0a01  .............%..
+00002ac0: 0c01 0c01 1002 0c01 0802 0c04 0402 0602  ................
+00002ad0: 0c02 0801 0801 0803 1201 0601 0a02 0a01  ................
+00002ae0: 1002 0e02 0e01 0201 0200 0200 0200 0200  ................
+00002af0: 0200 0200 02ff 0603 0201 0200 0200 02ff  ................
+00002b00: 0603 0a01 0e01 0802 0602 0a01 1402 0c01  ................
+00002b10: 0801 0601 1202 0601 1802 0a02 0e01 0801  ................
+00002b20: 0802                                     ..
```

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 13 18:30:16 2023 UTC, .py size: 14586 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,691 +1,619 @@
-00000000: 550d 0d0a 0000 0000 384a 3864 fa38 0000  U.......8J8d.8..
+00000000: 6f0d 0d0a 0000 0000 4253 8b64 e634 0000  o.......BS.d.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 5002 0000 6400  .....@...sP...d.
+00000020: 0003 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
-00000040: 5a02 6400 6401 6c05 5a05 6502 a006 6505  Z.d.d.l.Z.e...e.
-00000050: 6a07 a101 0100 6400 6401 6c08 5a08 6400  j.....d.d.l.Z.d.
-00000060: 6402 6c09 6d0a 5a0a 0100 6400 6403 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0c 0100 6400 6404 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 6d0f 5a0f 0100 6400 6401 6c10 5a10 6400  m.Z...d.d.l.Z.d.
-00000090: 6401 6c11 5a12 6400 6405 6c13 6d14 5a14  d.l.Z.d.d.l.m.Z.
-000000a0: 0100 6406 5a15 4700 6407 6408 8400 6408  ..d.Z.G.d.d...d.
-000000b0: 8302 5a16 6504 6409 6b02 9002 724c 6400  ..Z.e.d.k...rLd.
-000000c0: 640a 6c17 6d18 5a18 0100 6400 640b 6c19  d.l.m.Z...d.d.l.
-000000d0: 6d1a 5a1a 0100 6400 640c 6c1b 6d1c 5a1c  m.Z...d.d.l.m.Z.
-000000e0: 6d1d 5a1d 0100 6400 640d 6c1e 6d1f 5a1f  m.Z...d.d.l.m.Z.
-000000f0: 0100 6400 6401 6c08 5a08 6400 640e 6c01  ..d.d.l.Z.d.d.l.
-00000100: 6d20 5a20 0100 640f 5a21 6521 9001 7242  m Z ..d.Z!e!..rB
-00000110: 650a 6520 6410 6411 8303 5a22 651f 6522  e.e d.d...Z"e.e"
-00000120: 8301 5a23 6523 a024 a100 0100 6523 a025  ..Z#e#.$....e#.%
-00000130: a100 0100 6523 6a26 a027 a100 4400 5d16  ....e#j&.'..D.].
-00000140: 5c02 5a28 5a29 6412 6529 5f2a 6412 6529  \.Z(Z)d.e)_*d.e)
-00000150: 5f2b 9001 7110 6502 a02c 6413 a101 0100  _+..q.e..,d.....
-00000160: 6516 6523 6a26 6414 6415 8d02 5a2d 6e60  e.e#j&d.d...Z-n`
-00000170: 6400 6416 6417 6418 6419 6705 5a2e 650a  d.d.d.d.d.g.Z.e.
-00000180: 6520 6410 641a 6411 8304 5a2f 6518 6419  e d.d.d...Z/e.d.
-00000190: 6414 641b 641c 641d 641e 6412 641f 8d07  d.d.d.d.d.d.d...
-000001a0: 5a30 651d 652e 652f 6530 6420 8d03 5a31  Z0e.e.e/e0d ..Z1
-000001b0: 6502 a02c 6413 a101 0100 6516 6531 6a26  e..,d.....e.e1j&
-000001c0: 6421 6415 8d02 5a2d 6531 a032 a100 0100  d!d...Z-e1.2....
-000001d0: 650c 8300 5a33 652d a034 6533 a101 0100  e...Z3e-.4e3....
-000001e0: 6502 a02c 6422 6508 a035 a100 9b00 9d02  e..,d"e..5......
-000001f0: a101 0100 652d 6a36 a037 a100 9002 7338  ....e-j6.7....s8
-00000200: 6533 a003 a100 5a38 652d 6a39 5a3a 653a  e3....Z8e-j9Z:e:
-00000210: 6a3b a027 a100 4400 5d24 5c02 5a28 5a3c  j;.'..D.]$\.Z(Z<
-00000220: 653c 9001 72ea 6510 a03d 6423 6528 9b00  e<..r.e..=d#e(..
-00000230: 9d02 653c 6a3e a102 0100 9001 71ea 6510  ..e<j>......q.e.
-00000240: a03f 6416 a101 5a40 6540 6541 6424 8301  .?d...Z@e@eAd$..
-00000250: 6b02 9001 72c6 6510 a042 a100 0100 9002  k...r.e..B......
-00000260: 7138 9001 71c6 6502 a02c 6425 6508 a035  q8..q.e..,d%e..5
-00000270: a100 9b00 9d02 a101 0100 6401 5300 2926  ..........d.S.)&
-00000280: e900 0000 004e 2901 da04 5061 7468 2901  .....N)...Path).
-00000290: da05 5175 6575 6529 02da 0654 6872 6561  ..Queue)...Threa
-000002a0: 64da 0545 7665 6e74 2901 da0a 5379 6e63  d..Event)...Sync
-000002b0: 5061 636b 6574 e964 0000 0063 0000 0000  Packet.d...c....
-000002c0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-000002d0: 4000 0000 73c6 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000002e0: 0264 2f65 0364 029c 0164 0364 0484 055a  .d/e.d...d.d...Z
-000002f0: 0465 0564 059c 0164 0664 0784 045a 0664  .e.d...d.d...Z.d
-00000300: 0864 0984 005a 0764 0a64 0b84 005a 0865  .d...Z.d.d...Z.e
-00000310: 0964 0c64 0d84 0083 015a 0a64 0e64 0f84  .d.d.....Z.d.d..
-00000320: 005a 0b64 1064 1184 005a 0c64 1264 1384  .Z.d.d...Z.d.d..
-00000330: 005a 0d64 1464 1584 005a 0e64 1664 1784  .Z.d.d...Z.d.d..
-00000340: 005a 0f64 1864 1984 005a 1064 1a64 1b84  .Z.d.d...Z.d.d..
-00000350: 005a 1164 1c64 1d84 005a 1264 1e64 1f84  .Z.d.d...Z.d.d..
-00000360: 005a 1364 2064 2184 005a 1464 2264 2384  .Z.d d!..Z.d"d#.
-00000370: 005a 1564 2464 2584 005a 1664 2664 2784  .Z.d$d%..Z.d&d'.
-00000380: 005a 1764 2864 2984 005a 1864 2a64 2b84  .Z.d(d)..Z.d*d+.
-00000390: 005a 1964 2c64 2d84 005a 1a64 2e53 0029  .Z.d,d-..Z.d.S.)
-000003a0: 30da 0c53 796e 6368 726f 6e69 7a65 72e9  0..Synchronizer.
-000003b0: 0600 0000 2901 da07 7374 7265 616d 7363  ....)...streamsc
-000003c0: 0300 0000 0000 0000 0000 0000 0600 0000  ................
-000003d0: 0400 0000 4300 0000 73ba 0000 007c 017c  ....C...s....|.|
-000003e0: 005f 0064 007c 005f 0167 007c 005f 0267  ._.d.|._.g.|._.g
-000003f0: 007c 005f 0369 007c 005f 0474 0583 007c  .|._.i.|._.t...|
-00000400: 005f 0664 017c 005f 0767 007c 005f 0869  ._.d.|._.g.|._.i
-00000410: 007c 005f 097c 006a 00a0 0aa1 0044 005d  .|._.|.j.....D.]
-00000420: 265c 027d 037d 047c 006a 08a0 0b7c 03a1  &\.}.}.|.j...|..
-00000430: 0101 0074 0c64 0283 017d 057c 057c 006a  ...t.d...}.|.|.j
-00000440: 097c 033c 0071 4264 017c 005f 0d7c 00a0  .|.<.qBd.|._.|..
-00000450: 0ea1 0001 007c 027c 005f 0f7c 00a0 107c  .....|.|._.|...|
-00000460: 006a 0fa1 0101 007c 027c 005f 1164 0364  .j.....|.|._.d.d
-00000470: 0484 0074 127c 006a 0883 0144 0083 017c  ...t.|.j...D...|
-00000480: 005f 137c 00a0 14a1 0001 007c 00a0 15a1  ._.|.......|....
-00000490: 0001 0064 0053 0029 054e 46e9 ffff ffff  ...d.S.).NF.....
-000004a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000004b0: 0004 0000 0053 0000 0073 1200 0000 6900  .....S...s....i.
-000004c0: 7c00 5d0a 7d01 7c01 6700 9302 7104 5300  |.].}.|.g...q.S.
-000004d0: a900 720c 0000 00a9 02da 022e 30da 0470  ..r.........0..p
-000004e0: 6f72 7472 0c00 0000 720c 0000 00fa 3f43  ortr....r.....?C
-000004f0: 3a5c 5573 6572 735c 4d61 6320 5072 6962  :\Users\Mac Prib
-00000500: 6c65 5c72 6570 6f73 5c70 7978 7933 645c  le\repos\pyxy3d\
-00000510: 7079 7879 3364 5c63 616d 6572 6173 5c73  pyxy3d\cameras\s
-00000520: 796e 6368 726f 6e69 7a65 722e 7079 da0a  ynchronizer.py..
-00000530: 3c64 6963 7463 6f6d 703e 3200 0000 7306  <dictcomp>2...s.
-00000540: 0000 0006 0002 0002 007a 2953 796e 6368  .........z)Synch
-00000550: 726f 6e69 7a65 722e 5f5f 696e 6974 5f5f  ronizer.__init__
-00000560: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00000570: 6f6d 703e 2916 720a 0000 005a 1663 7572  omp>).r....Z.cur
-00000580: 7265 6e74 5f73 796e 6368 6564 5f66 7261  rent_synched_fra
-00000590: 6d65 73da 1773 796e 635f 6e6f 7469 6365  mes..sync_notice
-000005a0: 5f73 7562 7363 7269 6265 7273 da1a 7379  _subscribers..sy
-000005b0: 6e63 6865 645f 6672 616d 6573 5f73 7562  nched_frames_sub
-000005c0: 7363 7269 6265 7273 da11 616c 6c5f 6672  scribers..all_fr
-000005d0: 616d 655f 7061 636b 6574 7372 0500 0000  ame_packetsr....
-000005e0: da0a 7374 6f70 5f65 7665 6e74 da0f 6672  ..stop_event..fr
-000005f0: 616d 6573 5f63 6f6d 706c 6574 65da 0570  ames_complete..p
-00000600: 6f72 7473 da13 6672 616d 655f 7061 636b  orts..frame_pack
-00000610: 6574 5f71 7565 7565 73da 0569 7465 6d73  et_queues..items
-00000620: da06 6170 7065 6e64 7203 0000 00da 1573  ..appendr......s
-00000630: 7562 7363 7269 6265 645f 746f 5f73 7472  ubscribed_to_str
-00000640: 6561 6d73 da14 7375 6273 6372 6962 655f  eams..subscribe_
-00000650: 746f 5f73 7472 6561 6d73 da0b 5f66 7073  to_streams.._fps
-00000660: 5f74 6172 6765 74da 0e73 6574 5f66 7073  _target..set_fps
-00000670: 5f74 6172 6765 74da 0866 7073 5f6d 6561  _target..fps_mea
-00000680: 6eda 0673 6f72 7465 64da 1564 726f 7070  n..sorted..dropp
-00000690: 6564 5f66 7261 6d65 5f68 6973 746f 7279  ed_frame_history
-000006a0: da12 696e 6974 6961 6c69 7a65 5f6c 6564  ..initialize_led
-000006b0: 6765 7273 da05 7374 6172 7429 06da 0473  gers..start)...s
-000006c0: 656c 6672 0a00 0000 da0a 6670 735f 7461  elfr......fps_ta
-000006d0: 7267 6574 720f 0000 00da 0673 7472 6561  rgetr......strea
-000006e0: 6dda 0171 720c 0000 0072 0c00 0000 7210  m..qr....r....r.
-000006f0: 0000 00da 085f 5f69 6e69 745f 5f14 0000  .....__init__...
-00000700: 0073 2e00 0000 0001 0601 0603 02ff 0404  .s..............
-00000710: 02ff 0404 0601 0801 0602 0601 0601 1201  ................
-00000720: 0c01 0801 0c02 0601 0802 0601 0c01 0603  ................
-00000730: 1602 0801 7a15 5379 6e63 6872 6f6e 697a  ....z.Synchroniz
-00000740: 6572 2e5f 5f69 6e69 745f 5f29 01da 0574  er.__init__)...t
-00000750: 7261 636b 6302 0000 0000 0000 0000 0000  rackc...........
-00000760: 0004 0000 0004 0000 0043 0000 0073 2200  .........C...s".
-00000770: 0000 7c00 6a00 a001 a100 4400 5d12 5c02  ..|.j.....D.].\.
-00000780: 7d02 7d03 7c03 a002 7c01 a101 0100 710a  }.}.|...|.....q.
-00000790: 6400 5300 a901 4e29 0372 0a00 0000 7219  d.S...N).r....r.
-000007a0: 0000 00da 0f73 6574 5f74 7261 636b 696e  .....set_trackin
-000007b0: 675f 6f6e 2904 7224 0000 0072 2900 0000  g_on).r$...r)...
-000007c0: 720f 0000 0072 2600 0000 720c 0000 0072  r....r&...r....r
-000007d0: 0c00 0000 7210 0000 00da 1773 6574 5f74  ....r......set_t
-000007e0: 7261 636b 696e 675f 6f6e 5f73 7472 6561  racking_on_strea
-000007f0: 6d73 3700 0000 7304 0000 0000 0112 017a  ms7...s........z
-00000800: 2453 796e 6368 726f 6e69 7a65 722e 7365  $Synchronizer.se
-00000810: 745f 7472 6163 6b69 6e67 5f6f 6e5f 7374  t_tracking_on_st
-00000820: 7265 616d 7363 0100 0000 0000 0000 0000  reamsc..........
-00000830: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00000840: 0000 007c 006a 0053 0072 2a00 0000 2901  ...|.j.S.r*...).
-00000850: 721d 0000 00a9 0172 2400 0000 720c 0000  r......r$...r...
-00000860: 0072 0c00 0000 7210 0000 00da 0e67 6574  .r....r......get
-00000870: 5f66 7073 5f74 6172 6765 743b 0000 0073  _fps_target;...s
-00000880: 0200 0000 0001 7a1b 5379 6e63 6872 6f6e  ......z.Synchron
-00000890: 697a 6572 2e67 6574 5f66 7073 5f74 6172  izer.get_fps_tar
-000008a0: 6765 7463 0100 0000 0000 0000 0000 0000  getc............
-000008b0: 0400 0000 0400 0000 4300 0000 7348 0000  ........C...sH..
-000008c0: 007c 006a 006a 017d 017c 01a0 02a1 0044  .|.j.j.}.|.....D
-000008d0: 005d 325c 027d 027d 037c 006a 037c 0219  .]2\.}.}.|.j.|..
-000008e0: 00a0 047c 03a1 0101 007c 006a 037c 0219  ...|.....|.j.|..
-000008f0: 0074 050b 0064 0085 0219 007c 006a 037c  .t...d.....|.j.|
-00000900: 023c 0071 1064 0053 0072 2a00 0000 2906  .<.q.d.S.r*...).
-00000910: da13 6375 7272 656e 745f 7379 6e63 5f70  ..current_sync_p
-00000920: 6163 6b65 74da 0764 726f 7070 6564 7219  acket..droppedr.
-00000930: 0000 0072 2100 0000 721a 0000 00da 1a44  ...r!...r......D
-00000940: 524f 5050 4544 5f46 5241 4d45 5f54 5241  ROPPED_FRAME_TRA
-00000950: 434b 5f57 494e 444f 5729 0472 2400 0000  CK_WINDOW).r$...
-00000960: 5a0f 6375 7272 656e 745f 6472 6f70 7065  Z.current_droppe
-00000970: 6472 0f00 0000 7230 0000 0072 0c00 0000  dr....r0...r....
-00000980: 720c 0000 0072 1000 0000 da1c 7570 6461  r....r......upda
-00000990: 7465 5f64 726f 7070 6564 5f66 7261 6d65  te_dropped_frame
-000009a0: 5f68 6973 746f 7279 3e00 0000 7308 0000  _history>...s...
-000009b0: 0000 0108 0210 0110 017a 2953 796e 6368  .........z)Synch
-000009c0: 726f 6e69 7a65 722e 7570 6461 7465 5f64  ronizer.update_d
-000009d0: 726f 7070 6564 5f66 7261 6d65 5f68 6973  ropped_frame_his
-000009e0: 746f 7279 6301 0000 0000 0000 0000 0000  toryc...........
-000009f0: 0001 0000 0003 0000 0043 0000 0073 1400  .........C...s..
-00000a00: 0000 6401 6402 8400 7c00 6a00 a001 a100  ..d.d...|.j.....
-00000a10: 4400 8301 5300 2903 7a4a 0a20 2020 2020  D...S.).zJ.     
-00000a20: 2020 2041 7665 7261 6765 7320 6472 6f70     Averages drop
-00000a30: 7065 6420 6672 616d 6520 636f 756e 7420  ped frame count 
-00000a40: 6163 726f 7373 2074 6865 206f 6273 6572  across the obser
-00000a50: 7665 6420 6869 7374 6f72 790a 2020 2020  ved history.    
-00000a60: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00000a70: 0003 0000 0006 0000 0053 0000 0073 1c00  .........S...s..
-00000a80: 0000 6900 7c00 5d14 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
-00000a90: 7400 a001 7c02 a101 9302 7104 5300 720c  t...|.....q.S.r.
-00000aa0: 0000 0029 02da 026e 70da 046d 6561 6e29  ...)...np..mean)
-00000ab0: 0372 0e00 0000 720f 0000 005a 0c64 726f  .r....r....Z.dro
-00000ac0: 705f 6869 7374 6f72 7972 0c00 0000 720c  p_historyr....r.
-00000ad0: 0000 0072 1000 0000 7211 0000 004a 0000  ...r....r....J..
-00000ae0: 0073 0600 0000 0600 0600 0200 7a2c 5379  .s..........z,Sy
-00000af0: 6e63 6872 6f6e 697a 6572 2e64 726f 7070  nchronizer.dropp
-00000b00: 6564 5f66 7073 2e3c 6c6f 6361 6c73 3e2e  ed_fps.<locals>.
-00000b10: 3c64 6963 7463 6f6d 703e 2902 7221 0000  <dictcomp>).r!..
-00000b20: 0072 1900 0000 722d 0000 0072 0c00 0000  .r....r-...r....
-00000b30: 720c 0000 0072 1000 0000 da0b 6472 6f70  r....r......drop
-00000b40: 7065 645f 6670 7345 0000 0073 0200 0000  ped_fpsE...s....
-00000b50: 0005 7a18 5379 6e63 6872 6f6e 697a 6572  ..z.Synchronizer
-00000b60: 2e64 726f 7070 6564 5f66 7073 6302 0000  .dropped_fpsc...
-00000b70: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00000b80: 0043 0000 0073 3800 0000 7c01 7c00 5f00  .C...s8...|.|._.
-00000b90: 7401 a002 6401 7c01 9b00 9d02 a101 0100  t...d.|.........
-00000ba0: 7c00 6a03 a004 a100 4400 5d12 5c02 7d02  |.j.....D.].\.}.
-00000bb0: 7d03 7c03 a005 7c01 a101 0100 7120 6400  }.|...|.....q d.
-00000bc0: 5300 2902 4e7a 2e41 7474 656d 7074 696e  S.).Nz.Attemptin
-00000bd0: 6720 746f 2063 6861 6e67 6520 7461 7267  g to change targ
-00000be0: 6574 2066 7073 2069 6e20 7374 7265 616d  et fps in stream
-00000bf0: 7320 746f 2029 0672 1d00 0000 da06 6c6f  s to ).r......lo
-00000c00: 6767 6572 da04 696e 666f 720a 0000 0072  gger..infor....r
-00000c10: 1900 0000 721e 0000 0029 0472 2400 0000  ....r....).r$...
-00000c20: da06 7461 7267 6574 720f 0000 0072 2600  ..targetr....r&.
-00000c30: 0000 720c 0000 0072 0c00 0000 7210 0000  ..r....r....r...
-00000c40: 0072 1e00 0000 4d00 0000 7308 0000 0000  .r....M...s.....
-00000c50: 0106 0110 0112 017a 1b53 796e 6368 726f  .......z.Synchro
-00000c60: 6e69 7a65 722e 7365 745f 6670 735f 7461  nizer.set_fps_ta
-00000c70: 7267 6574 6301 0000 0000 0000 0000 0000  rgetc...........
-00000c80: 0003 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
-00000c90: 0000 7c00 6a00 a001 a100 4400 5d18 5c02  ..|.j.....D.].\.
-00000ca0: 7d01 7d02 7c02 a002 7c00 6a03 7c01 1900  }.}.|...|.j.|...
-00000cb0: a101 0100 710a 6401 7c00 5f04 6400 5300  ....q.d.|._.d.S.
-00000cc0: 2902 4e54 2905 720a 0000 0072 1900 0000  ).NT).r....r....
-00000cd0: da09 7375 6273 6372 6962 6572 1800 0000  ..subscriber....
-00000ce0: 721b 0000 00a9 0372 2400 0000 720f 0000  r......r$...r...
-00000cf0: 0072 2600 0000 720c 0000 0072 0c00 0000  .r&...r....r....
-00000d00: 7210 0000 0072 1c00 0000 5300 0000 7306  r....r....S...s.
-00000d10: 0000 0000 0112 0112 017a 2153 796e 6368  .........z!Synch
-00000d20: 726f 6e69 7a65 722e 7375 6273 6372 6962  ronizer.subscrib
-00000d30: 655f 746f 5f73 7472 6561 6d73 6301 0000  e_to_streamsc...
-00000d40: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-00000d50: 0043 0000 0073 3e00 0000 7c00 6a00 a001  .C...s>...|.j...
-00000d60: a100 4400 5d28 5c02 7d01 7d02 7402 a003  ..D.](\.}.}.t...
-00000d70: 6401 7c01 9b00 9d02 a101 0100 7c02 a004  d.|.........|...
-00000d80: 7c00 6a05 7c01 1900 a101 0100 710a 6402  |.j.|.......q.d.
-00000d90: 7c00 5f06 6400 5300 2903 4e7a 2375 6e73  |._.d.S.).Nz#uns
-00000da0: 7562 7363 7269 6265 2073 796e 6368 726f  ubscribe synchro
-00000db0: 6e69 7a65 7220 6672 6f6d 2070 6f72 7420  nizer from port 
-00000dc0: 4629 0772 0a00 0000 7219 0000 0072 3600  F).r....r....r6.
-00000dd0: 0000 7237 0000 00da 0b75 6e73 7562 7363  ..r7.....unsubsc
-00000de0: 7269 6265 7218 0000 0072 1b00 0000 723a  riber....r....r:
-00000df0: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-00000e00: 0000 da16 756e 7375 6273 6372 6962 655f  ....unsubscribe_
-00000e10: 746f 5f73 7472 6561 6d73 5800 0000 7308  to_streamsX...s.
-00000e20: 0000 0000 0112 0110 0112 017a 2353 796e  ...........z#Syn
-00000e30: 6368 726f 6e69 7a65 722e 756e 7375 6273  chronizer.unsubs
-00000e40: 6372 6962 655f 746f 5f73 7472 6561 6d73  cribe_to_streams
-00000e50: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000e60: 0003 0000 0043 0000 0073 2c00 0000 7c00  .....C...s,...|.
-00000e70: 6a00 a001 a100 0100 7c00 6a02 a003 a100  j.......|.j.....
-00000e80: 0100 7c00 6a04 4400 5d0c 7d01 7c01 a003  ..|.j.D.].}.|...
-00000e90: a100 0100 711a 6400 5300 722a 0000 0029  ....q.d.S.r*...)
-00000ea0: 0572 1500 0000 da03 7365 74da 0674 6872  .r......set..thr
-00000eb0: 6561 64da 046a 6f69 6eda 0774 6872 6561  ead..join..threa
-00000ec0: 6473 2902 7224 0000 00da 0174 720c 0000  ds).r$.....tr...
-00000ed0: 0072 0c00 0000 7210 0000 00da 0473 746f  .r....r......sto
-00000ee0: 705e 0000 0073 0800 0000 0001 0a01 0a01  p^...s..........
-00000ef0: 0a01 7a11 5379 6e63 6872 6f6e 697a 6572  ..z.Synchronizer
-00000f00: 2e73 746f 7063 0100 0000 0000 0000 0000  .stopc..........
-00000f10: 0000 0100 0000 0200 0000 4300 0000 732e  ..........C...s.
-00000f20: 0000 0064 0164 0284 007c 006a 0044 0083  ...d.d...|.j.D..
-00000f30: 017c 005f 0164 0364 0284 007c 006a 0044  .|._.d.d...|.j.D
-00000f40: 0083 017c 005f 0267 007c 005f 0364 0053  ...|._.g.|._.d.S
-00000f50: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00000f60: 0002 0000 0004 0000 0053 0000 0073 1200  .........S...s..
-00000f70: 0000 6900 7c00 5d0a 7d01 7c01 6400 9302  ..i.|.].}.|.d...
-00000f80: 7104 5300 a901 7201 0000 0072 0c00 0000  q.S...r....r....
-00000f90: 720d 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000fa0: 1000 0000 7211 0000 0066 0000 0073 0600  ....r....f...s..
-00000fb0: 0000 0600 0200 0200 7a33 5379 6e63 6872  ........z3Synchr
-00000fc0: 6f6e 697a 6572 2e69 6e69 7469 616c 697a  onizer.initializ
-00000fd0: 655f 6c65 6467 6572 732e 3c6c 6f63 616c  e_ledgers.<local
-00000fe0: 733e 2e3c 6469 6374 636f 6d70 3e63 0100  s>.<dictcomp>c..
-00000ff0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001000: 0000 5300 0000 7312 0000 0069 007c 005d  ..S...s....i.|.]
-00001010: 0a7d 017c 0164 0093 0271 0453 0072 4300  .}.|.d...q.S.rC.
-00001020: 0000 720c 0000 0072 0d00 0000 720c 0000  ..r....r....r...
-00001030: 0072 0c00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00001040: 6700 0000 7306 0000 0006 0002 0002 0029  g...s..........)
-00001050: 0472 1700 0000 da10 706f 7274 5f66 7261  .r......port_fra
-00001060: 6d65 5f63 6f75 6e74 da12 706f 7274 5f63  me_count..port_c
-00001070: 7572 7265 6e74 5f66 7261 6d65 da10 6d65  urrent_frame..me
-00001080: 616e 5f66 7261 6d65 5f74 696d 6573 722d  an_frame_timesr-
-00001090: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-000010a0: 0000 7222 0000 0064 0000 0073 0600 0000  ..r"...d...s....
-000010b0: 0002 1201 1201 7a1f 5379 6e63 6872 6f6e  ......z.Synchron
-000010c0: 697a 6572 2e69 6e69 7469 616c 697a 655f  izer.initialize_
-000010d0: 6c65 6467 6572 7363 0100 0000 0000 0000  ledgersc........
-000010e0: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
-000010f0: 737e 0000 0074 00a0 0164 01a1 0101 0067  s~...t...d.....g
-00001100: 007c 005f 027c 006a 03a0 04a1 0044 005d  .|._.|.j.....D.]
-00001110: 2e5c 027d 017d 0274 057c 006a 067c 0266  .\.}.}.t.|.j.|.f
-00001120: 0164 0264 038d 037d 037c 03a0 07a1 0001  .d.d...}.|......
-00001130: 007c 006a 02a0 087c 03a1 0101 0071 1a74  .|.j...|.....q.t
-00001140: 00a0 0164 04a1 0101 0074 00a0 0164 05a1  ...d.....t...d..
-00001150: 0101 0074 057c 006a 0964 0664 0264 038d  ...t.|.j.d.d.d..
-00001160: 037c 005f 0a7c 006a 0aa0 07a1 0001 0064  .|._.|.j.......d
-00001170: 0053 0029 074e 7a2e 4162 6f75 7420 746f  .S.).Nz.About to
-00001180: 2073 7562 6d69 7420 5468 7265 6164 706f   submit Threadpo
-00001190: 6f6c 206f 6620 6672 616d 6520 4861 7276  ol of frame Harv
-000011a0: 6573 7465 7273 5429 0372 3800 0000 da04  estersT).r8.....
-000011b0: 6172 6773 da06 6461 656d 6f6e 7a1f 4672  args..daemonz.Fr
-000011c0: 616d 6520 6861 7276 6573 7465 7273 206a  ame harvesters j
-000011d0: 7573 7420 7375 626d 6974 7465 647a 1e53  ust submittedz.S
-000011e0: 7461 7274 696e 6720 6672 616d 6520 7379  tarting frame sy
-000011f0: 6e63 6872 6f6e 697a 6572 2e2e 2e72 0c00  nchronizer...r..
-00001200: 0000 290b 7236 0000 0072 3700 0000 7240  ..).r6...r7...r@
-00001210: 0000 0072 0a00 0000 7219 0000 0072 0400  ...r....r....r..
-00001220: 0000 da15 6861 7276 6573 745f 6672 616d  ....harvest_fram
-00001230: 655f 7061 636b 6574 7372 2300 0000 721a  e_packetsr#...r.
-00001240: 0000 00da 1373 796e 6368 5f66 7261 6d65  .....synch_frame
-00001250: 735f 776f 726b 6572 723e 0000 0029 0472  s_workerr>...).r
-00001260: 2400 0000 720f 0000 0072 2600 0000 7241  $...r....r&...rA
-00001270: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-00001280: 0000 7223 0000 006a 0000 0073 1400 0000  ..r#...j...s....
-00001290: 0002 0a01 0601 1201 1201 0801 0e01 0a02  ................
-000012a0: 0a01 1201 7a12 5379 6e63 6872 6f6e 697a  ....z.Synchroniz
-000012b0: 6572 2e73 7461 7274 6302 0000 0000 0000  er.startc.......
-000012c0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000012d0: 0073 1a00 0000 7400 a001 6401 a101 0100  .s....t...d.....
-000012e0: 7c00 6a02 a003 7c01 a101 0100 6400 5300  |.j...|.....d.S.
-000012f0: 2902 4e7a 3741 6464 696e 6720 7175 6575  ).Nz7Adding queu
-00001300: 6520 746f 2072 6563 6569 7665 206e 6f74  e to receive not
-00001310: 6963 6520 6f66 2073 796e 6368 6564 2066  ice of synched f
-00001320: 7261 6d65 7320 7570 6461 7465 2904 7236  rames update).r6
-00001330: 0000 0072 3700 0000 7212 0000 0072 1a00  ...r7...r....r..
-00001340: 0000 a902 7224 0000 0072 2700 0000 720c  ....r$...r'...r.
-00001350: 0000 0072 0c00 0000 7210 0000 00da 1373  ...r....r......s
-00001360: 7562 7363 7269 6265 5f74 6f5f 6e6f 7469  ubscribe_to_noti
-00001370: 6365 7800 0000 7304 0000 0000 040a 017a  cex...s........z
-00001380: 2053 796e 6368 726f 6e69 7a65 722e 7375   Synchronizer.su
-00001390: 6273 6372 6962 655f 746f 5f6e 6f74 6963  bscribe_to_notic
-000013a0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-000013b0: 0000 0300 0000 4300 0000 731a 0000 0074  ......C...s....t
-000013c0: 00a0 0164 01a1 0101 007c 006a 02a0 037c  ...d.....|.j...|
-000013d0: 01a1 0101 0064 0053 0029 024e 7a46 5265  .....d.S.).NzFRe
-000013e0: 6d6f 7669 6e67 2071 7565 7565 2074 6861  moving queue tha
-000013f0: 7420 6861 6420 6265 656e 2072 6563 6569  t had been recei
-00001400: 7669 6e67 206e 6f74 6963 6520 6f66 2073  ving notice of s
-00001410: 796e 6368 6564 2066 7261 6d65 7320 7570  ynched frames up
-00001420: 6461 7465 2904 7236 0000 0072 3700 0000  date).r6...r7...
-00001430: 7212 0000 00da 0672 656d 6f76 6572 4b00  r......removerK.
-00001440: 0000 720c 0000 0072 0c00 0000 7210 0000  ..r....r....r...
-00001450: 00da 1575 6e73 7562 7363 7269 6265 5f74  ...unsubscribe_t
-00001460: 6f5f 6e6f 7469 6365 7f00 0000 7304 0000  o_notice....s...
-00001470: 0000 040a 017a 2253 796e 6368 726f 6e69  .....z"Synchroni
-00001480: 7a65 722e 756e 7375 6273 6372 6962 655f  zer.unsubscribe_
-00001490: 746f 5f6e 6f74 6963 6563 0200 0000 0000  to_noticec......
-000014a0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000014b0: 0000 731a 0000 0074 00a0 0164 01a1 0101  ..s....t...d....
-000014c0: 007c 006a 02a0 037c 01a1 0101 0064 0053  .|.j...|.....d.S
-000014d0: 0029 024e 7a26 4164 6469 6e67 2071 7565  .).Nz&Adding que
-000014e0: 7565 2074 6f20 7265 6365 6976 6520 7379  ue to receive sy
-000014f0: 6e63 6865 6420 6672 616d 6573 2904 7236  nched frames).r6
-00001500: 0000 0072 3700 0000 7213 0000 0072 1a00  ...r7...r....r..
-00001510: 0000 724b 0000 0072 0c00 0000 720c 0000  ..rK...r....r...
-00001520: 0072 1000 0000 da19 7375 6273 6372 6962  .r......subscrib
-00001530: 655f 746f 5f73 796e 635f 7061 636b 6574  e_to_sync_packet
-00001540: 7387 0000 0073 0400 0000 0001 0a01 7a26  s....s........z&
-00001550: 5379 6e63 6872 6f6e 697a 6572 2e73 7562  Synchronizer.sub
-00001560: 7363 7269 6265 5f74 6f5f 7379 6e63 5f70  scribe_to_sync_p
-00001570: 6163 6b65 7473 6302 0000 0000 0000 0000  acketsc.........
-00001580: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00001590: 1a00 0000 7400 a001 6401 a101 0100 7c00  ....t...d.....|.
-000015a0: 6a02 a003 7c01 a101 0100 6400 5300 2902  j...|.....d.S.).
-000015b0: 4e7a 1652 656c 6561 7369 6e67 2072 6563  Nz.Releasing rec
-000015c0: 6f72 6420 7175 6575 6529 0472 3600 0000  ord queue).r6...
-000015d0: 7237 0000 0072 1300 0000 724d 0000 0072  r7...r....rM...r
-000015e0: 4b00 0000 720c 0000 0072 0c00 0000 7210  K...r....r....r.
-000015f0: 0000 00da 1572 656c 6561 7365 5f73 796e  .....release_syn
-00001600: 635f 7061 636b 6574 5f71 8b00 0000 7304  c_packet_q....s.
-00001610: 0000 0000 010a 017a 2253 796e 6368 726f  .......z"Synchro
-00001620: 6e69 7a65 722e 7265 6c65 6173 655f 7379  nizer.release_sy
-00001630: 6e63 5f70 6163 6b65 745f 7163 0200 0000  nc_packet_qc....
-00001640: 0000 0000 0000 0000 0500 0000 0800 0000  ................
-00001650: 4300 0000 73a0 0000 007c 016a 007d 0274  C...s....|.j.}.t
-00001660: 01a0 0264 017c 029b 009d 02a1 0101 007c  ...d.|.........|
-00001670: 006a 03a0 04a1 0073 8a7c 006a 057c 0219  .j.....s.|.j.|..
-00001680: 00a0 06a1 007d 037c 006a 077c 0219 007d  .....}.|.j.|...}
-00001690: 047c 047c 035f 087c 037c 006a 097c 029b  .|.|._.|.|.j.|..
-000016a0: 0064 027c 036a 089b 009d 033c 007c 006a  .d.|.j.....<.|.j
-000016b0: 077c 0205 0019 0064 0337 0003 003c 0074  .|.....d.7...<.t
-000016c0: 01a0 0a64 047c 036a 009b 0064 057c 036a  ...d.|.j...d.|.j
-000016d0: 089b 0064 067c 036a 0b9b 009d 06a1 0101  ...d.|.j........
-000016e0: 0071 1674 01a0 0264 077c 029b 0064 089d  .q.t...d.|...d..
-000016f0: 03a1 0101 0064 0053 0029 094e 7a2c 4265  .....d.S.).Nz,Be
-00001700: 6769 6e6e 696e 6720 746f 2063 6f6c 6c65  ginning to colle
-00001710: 6374 2064 6174 6120 6765 6e65 7261 7465  ct data generate
-00001720: 6420 6174 2070 6f72 7420 da01 5fe9 0100  d at port .._...
-00001730: 0000 7a1f 4672 616d 6520 6461 7461 2068  ..z.Frame data h
-00001740: 6172 7665 7374 6564 2066 726f 6d20 7265  arvested from re
-00001750: 656c 207a 0c20 7769 7468 2069 6e64 6578  el z. with index
-00001760: 207a 1320 616e 6420 6672 616d 6520 7469   z. and frame ti
-00001770: 6d65 206f 6620 7a19 4672 616d 6520 6861  me of z.Frame ha
-00001780: 7276 6573 7465 7220 666f 7220 706f 7274  rvester for port
-00001790: 207a 0a20 636f 6d70 6c65 7465 6429 0c72   z. completed).r
-000017a0: 0f00 0000 7236 0000 0072 3700 0000 7215  ....r6...r7...r.
-000017b0: 0000 00da 0669 735f 7365 7472 1800 0000  .....is_setr....
-000017c0: da03 6765 7472 4400 0000 da0b 6672 616d  ..getrD.....fram
-000017d0: 655f 696e 6465 7872 1400 0000 da05 6465  e_indexr......de
-000017e0: 6275 67da 0a66 7261 6d65 5f74 696d 6529  bug..frame_time)
-000017f0: 0572 2400 0000 7226 0000 0072 0f00 0000  .r$...r&...r....
-00001800: da0c 6672 616d 655f 7061 636b 6574 7255  ..frame_packetrU
-00001810: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-00001820: 0000 7249 0000 008f 0000 0073 1800 0000  ..rI.......s....
-00001830: 0001 0602 1002 0a01 0e01 0a01 0602 1601  ................
-00001840: 1202 0401 1aff 0604 7a22 5379 6e63 6872  ........z"Synchr
-00001850: 6f6e 697a 6572 2e68 6172 7665 7374 5f66  onizer.harvest_f
-00001860: 7261 6d65 5f70 6163 6b65 7473 6302 0000  rame_packetsc...
-00001870: 0000 0000 0000 0000 0007 0000 0006 0000  ................
-00001880: 0043 0000 0073 b800 0000 6700 7d02 7c00  .C...s....g.}.|.
-00001890: 6a00 4400 5da4 7d03 7c00 6a01 7c03 1900  j.D.].}.|.j.|...
-000018a0: 6401 1700 7d04 7c03 9b00 6402 7c04 9b00  d...}.|...d.|...
-000018b0: 9d03 7d05 7c05 7c00 6a02 a003 a100 6b07  ..}.|.|.j.....k.
-000018c0: 7266 7404 a005 6403 7c05 9b00 9d02 a101  rft...d.|.......
-000018d0: 0100 7c00 6a06 725a 7407 a008 6404 a101  ..|.j.rZt...d...
-000018e0: 0100 712a 7407 a008 6401 a101 0100 712a  ..q*t...d.....q*
-000018f0: 7c00 6a02 7c05 1900 6a09 7d06 7c06 6405  |.j.|...j.}.|.d.
-00001900: 6b02 729c 7404 a005 6406 7c03 9b00 6407  k.r.t...d.|...d.
-00001910: 9d03 a101 0100 6408 7c00 5f0a 7c00 6a0b  ......d.|._.|.j.
-00001920: a00c a100 0100 7c03 7c01 6b03 720a 7c02  ......|.|.k.r.|.
-00001930: a00d 7c06 a101 0100 710a 740e 7c02 8301  ..|.....q.t.|...
-00001940: 5300 2909 7a75 4c6f 6f6b 7320 6174 206e  S.).zuLooks at n
-00001950: 6578 7420 756e 6173 7369 676e 6564 2066  ext unassigned f
-00001960: 7261 6d65 2061 6372 6f73 7320 7468 6520  rame across the 
-00001970: 706f 7274 7320 746f 2064 6574 6572 6d69  ports to determi
-00001980: 6e65 0a20 2020 2020 2020 2074 6865 2065  ne.        the e
-00001990: 6172 6c69 6573 7420 7469 6d65 2061 7420  arliest time at 
-000019a0: 7768 6963 6820 6561 6368 206f 6620 7468  which each of th
-000019b0: 656d 2077 6173 2072 6561 6472 5200 0000  em was readrR...
-000019c0: 7251 0000 007a 3757 6169 7469 6e67 2069  rQ...z7Waiting i
-000019d0: 6e20 6120 6c6f 6f70 2066 6f72 2066 7261  n a loop for fra
-000019e0: 6d65 2064 6174 6120 746f 2070 6f70 756c  me data to popul
-000019f0: 6174 6520 7769 7468 206b 6579 3a20 679a  ate with key: g.
-00001a00: 9999 9999 99b9 3f72 0b00 0000 7a16 456e  ......?r....z.En
-00001a10: 6420 6f66 2066 7261 6d65 7320 6174 2070  d of frames at p
-00001a20: 6f72 7420 7a21 2064 6574 6563 7465 643b  ort z! detected;
-00001a30: 2065 6e64 696e 6720 7379 6e63 6872 6f6e   ending synchron
-00001a40: 697a 6174 696f 6e54 290f 7217 0000 0072  izationT).r....r
-00001a50: 4500 0000 7214 0000 00da 046b 6579 7372  E...r......keysr
-00001a60: 3600 0000 7237 0000 0072 1b00 0000 da04  6...r7...r......
-00001a70: 7469 6d65 da05 736c 6565 7072 5700 0000  time..sleeprW...
-00001a80: 7216 0000 0072 1500 0000 723d 0000 0072  r....r....r=...r
-00001a90: 1a00 0000 da03 6d69 6e29 0772 2400 0000  ......min).r$...
-00001aa0: 720f 0000 005a 1474 696d 6573 5f6f 665f  r....Z.times_of_
-00001ab0: 6e65 7874 5f66 7261 6d65 73da 0170 5a0a  next_frames..pZ.
-00001ac0: 6e65 7874 5f69 6e64 6578 da0e 6672 616d  next_index..fram
-00001ad0: 655f 6461 7461 5f6b 6579 5a0f 6e65 7874  e_data_keyZ.next
-00001ae0: 5f66 7261 6d65 5f74 696d 6572 0c00 0000  _frame_timer....
-00001af0: 720c 0000 0072 1000 0000 da13 6561 726c  r....r......earl
-00001b00: 6965 7374 5f6e 6578 745f 6672 616d 65a3  iest_next_frame.
-00001b10: 0000 0073 2a00 0000 0003 0401 0a01 0e01  ...s*...........
-00001b20: 0e03 0e01 0401 08ff 0403 0601 0c02 0c02  ................
-00001b30: 0c02 0801 0401 0aff 0403 0601 0a02 0801  ................
-00001b40: 0c02 7a20 5379 6e63 6872 6f6e 697a 6572  ..z Synchronizer
-00001b50: 2e65 6172 6c69 6573 745f 6e65 7874 5f66  .earliest_next_f
-00001b60: 7261 6d65 6302 0000 0000 0000 0000 0000  ramec...........
-00001b70: 0007 0000 0004 0000 0043 0000 0073 4e00  .........C...sN.
-00001b80: 0000 6700 7d02 7c00 6a00 4400 5d3a 7d03  ..g.}.|.j.D.]:}.
-00001b90: 7c00 6a01 7c03 1900 7d04 7c03 9b00 6401  |.j.|...}.|...d.
-00001ba0: 7c04 9b00 9d03 7d05 7c00 6a02 7c05 1900  |.....}.|.j.|...
-00001bb0: 6a03 7d06 7c03 7c01 6b03 720a 7c02 a004  j.}.|.|.k.r.|...
-00001bc0: 7c06 a101 0100 710a 7405 7c02 8301 5300  |.....q.t.|...S.
-00001bd0: 2902 7a57 5072 6f76 6964 6573 2074 6865  ).zWProvides the
-00001be0: 206c 6174 6573 7420 6672 616d 655f 7469   latest frame_ti
-00001bf0: 6d65 206f 6620 7468 6520 6375 7272 656e  me of the curren
-00001c00: 7420 6672 616d 6573 206e 6f74 2069 6e63  t frames not inc
-00001c10: 6c75 7369 7665 206f 6620 7468 6520 7072  lusive of the pr
-00001c20: 6f76 6964 6564 2070 6f72 7472 5100 0000  ovided portrQ...
-00001c30: 2906 7217 0000 0072 4500 0000 7214 0000  ).r....rE...r...
-00001c40: 0072 5700 0000 721a 0000 00da 036d 6178  .rW...r......max
-00001c50: 2907 7224 0000 0072 0f00 0000 5a17 7469  ).r$...r....Z.ti
-00001c60: 6d65 735f 6f66 5f63 7572 7265 6e74 5f66  mes_of_current_f
-00001c70: 7261 6d65 7372 5d00 0000 5a0d 6375 7272  ramesr]...Z.curr
-00001c80: 656e 745f 696e 6465 7872 5e00 0000 5a12  ent_indexr^...Z.
-00001c90: 6375 7272 656e 745f 6672 616d 655f 7469  current_frame_ti
-00001ca0: 6d65 720c 0000 0072 0c00 0000 7210 0000  mer....r....r...
-00001cb0: 00da 146c 6174 6573 745f 6375 7272 656e  ...latest_curren
-00001cc0: 745f 6672 616d 65c3 0000 0073 1000 0000  t_frame....s....
-00001cd0: 0002 0401 0a01 0a01 0e01 0c01 0801 0c02  ................
-00001ce0: 7a21 5379 6e63 6872 6f6e 697a 6572 2e6c  z!Synchronizer.l
-00001cf0: 6174 6573 745f 6375 7272 656e 745f 6672  atest_current_fr
-00001d00: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-00001d10: 0200 0000 0400 0000 0300 0000 732c 0000  ............s,..
-00001d20: 0087 0066 0164 0164 0284 0888 006a 0044  ...f.d.d.....j.D
-00001d30: 0083 017d 0174 01a0 0264 037c 019b 009d  ...}.t...d.|....
-00001d40: 02a1 0101 0074 037c 0183 0153 0029 047a  .....t.|...S.).z
-00001d50: 4244 6574 6572 6d69 6e65 2068 6f77 206d  BDetermine how m
-00001d60: 616e 7920 756e 6173 7369 676e 6564 2066  any unassigned f
-00001d70: 7261 6d65 7320 6172 6520 7369 7474 696e  rames are sittin
-00001d80: 6720 696e 2073 656c 662e 6461 7461 6672  g in self.datafr
-00001d90: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-00001da0: 0200 0000 0500 0000 1300 0000 7320 0000  ............s ..
-00001db0: 0067 007c 005d 187d 0188 006a 007c 0119  .g.|.].}...j.|..
-00001dc0: 0088 006a 017c 0119 0018 0091 0271 0453  ...j.|.......q.S
-00001dd0: 0072 0c00 0000 2902 7244 0000 0072 4500  .r....).rD...rE.
-00001de0: 0000 720d 0000 0072 2d00 0000 720c 0000  ..r....r-...r...
-00001df0: 0072 1000 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00001e00: 703e d100 0000 7304 0000 0006 0202 ff7a  p>....s........z
-00001e10: 2c53 796e 6368 726f 6e69 7a65 722e 6672  ,Synchronizer.fr
-00001e20: 616d 655f 736c 6163 6b2e 3c6c 6f63 616c  ame_slack.<local
-00001e30: 733e 2e3c 6c69 7374 636f 6d70 3e7a 1353  s>.<listcomp>z.S
-00001e40: 6c61 636b 2069 6e20 6672 616d 6573 2069  lack in frames i
-00001e50: 7320 2904 7217 0000 0072 3600 0000 7256  s ).r....r6...rV
-00001e60: 0000 0072 5c00 0000 2902 7224 0000 005a  ...r\...).r$...Z
-00001e70: 0573 6c61 636b 720c 0000 0072 2d00 0000  .slackr....r-...
-00001e80: 7210 0000 00da 0b66 7261 6d65 5f73 6c61  r......frame_sla
-00001e90: 636b cf00 0000 730a 0000 0000 020a 0204  ck....s.........
-00001ea0: fe06 0410 017a 1853 796e 6368 726f 6e69  .....z.Synchroni
-00001eb0: 7a65 722e 6672 616d 655f 736c 6163 6b63  zer.frame_slackc
-00001ec0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001ed0: 0300 0000 4300 0000 733c 0000 0074 007c  ....C...s<...t.|
-00001ee0: 006a 0183 0164 016b 0472 1e7c 006a 0164  .j...d.k.r.|.j.d
-00001ef0: 0264 0085 0219 007c 005f 0174 02a0 037c  .d.....|._.t...|
-00001f00: 006a 01a1 017d 0174 02a0 047c 01a1 017d  .j...}.t...|...}
-00001f10: 0264 037c 021b 0053 0029 044e e90a 0000  .d.|...S.).N....
-00001f20: 0069 f6ff ffff 7252 0000 0029 05da 036c  .i....rR...)...l
-00001f30: 656e 7246 0000 0072 3300 0000 da04 6469  enrF...r3.....di
-00001f40: 6666 7234 0000 0029 0372 2400 0000 5a07  ffr4...).r$...Z.
-00001f50: 6465 6c74 615f 745a 0c6d 6561 6e5f 6465  delta_tZ.mean_de
-00001f60: 6c74 615f 7472 0c00 0000 720c 0000 0072  lta_tr....r....r
-00001f70: 1000 0000 da0b 6176 6572 6167 655f 6670  ......average_fp
-00001f80: 73d8 0000 0073 0a00 0000 0001 0e01 1002  s....s..........
-00001f90: 0c01 0a02 7a18 5379 6e63 6872 6f6e 697a  ....z.Synchroniz
-00001fa0: 6572 2e61 7665 7261 6765 5f66 7073 6301  er.average_fpsc.
-00001fb0: 0000 0000 0000 0000 0000 000c 0000 0009  ................
-00001fc0: 0000 0043 0000 0073 0a02 0000 7400 a001  ...C...s....t...
-00001fd0: 6401 a101 0100 6402 7d01 7400 a001 6403  d.....d.}.t...d.
-00001fe0: a101 0100 7c00 6a02 a003 a100 9001 73fc  ....|.j.......s.
-00001ff0: 6900 7d02 6700 7d03 6900 7d04 6900 7d05  i.}.g.}.i.}.i.}.
-00002000: 7c00 6a04 4400 5d2a 7d06 7c00 a005 7c06  |.j.D.]*}.|...|.
-00002010: a101 7c04 7c06 3c00 7c00 a006 7c06 a101  ..|.|.<.|...|...
-00002020: 7c05 7c06 3c00 7c00 6a07 7c06 1900 7d07  |.|.<.|.j.|...}.
-00002030: 713a 7c00 6a04 4400 5dd0 7d06 7c00 6a07  q:|.j.D.].}.|.j.
-00002040: 7c06 1900 7d07 7c06 9b00 6404 7c07 9b00  |...}.|...d.|...
-00002050: 9d03 7d08 7c00 6a08 7c08 1900 7d09 7c09  ..}.|.j.|...}.|.
-00002060: 6a09 7d0a 7c0a 7c04 7c06 1900 6b04 72c0  j.}.|.|.|...k.r.
-00002070: 6400 7c02 7c06 3c00 7400 a00a 6405 7c06  d.|.|.<.t...d.|.
-00002080: 9b00 6406 9d03 a101 0100 716c 7c04 7c06  ..d.......ql|.|.
-00002090: 1900 7c0a 1800 7c0a 7c05 7c06 1900 1800  ..|...|.|.|.....
-000020a0: 6b00 72f4 6400 7c02 7c06 3c00 7400 a00a  k.r.d.|.|.<.t...
-000020b0: 6405 7c06 9b00 6407 9d03 a101 0100 716c  d.|...d.......ql
-000020c0: 7c00 6a08 a00b 7c08 a101 7c02 7c06 3c00  |.j...|...|.|.<.
-000020d0: 7c00 6a07 7c06 0500 1900 6408 3700 0300  |.j.|.....d.7...
-000020e0: 3c00 7c03 a00c 7c0a a101 0100 7400 a00d  <.|...|.....t...
-000020f0: 6409 7c06 9b00 640a 7c07 9b00 640b 7c0a  d.|...d.|...d.|.
-00002100: 9b00 9d06 a101 0100 716c 7400 a00d 640c  ........qlt...d.
-00002110: 740e 7c00 6a08 8301 9b00 9d02 a101 0100  t.|.j...........
-00002120: 7c00 6a0f a00c 7410 a011 7c03 a101 a101  |.j...t...|.....
-00002130: 0100 7412 7c01 7c02 8302 7c00 5f13 7c00  ..t.|.|...|._.|.
-00002140: a014 a100 0100 7c01 6408 3700 7d01 7c00  ......|.d.7.}.|.
-00002150: 6a02 a003 a100 9001 729e 7400 a001 640d  j.......r.t...d.
-00002160: a101 0100 6400 7c00 5f13 7c00 6a15 4400  ....d.|._.|.j.D.
-00002170: 5d20 7d0b 7400 a00d 640e 7c0b 9b00 9d02  ] }.t...d.|.....
-00002180: a101 0100 7c0b a016 640f a101 0100 9001  ....|...d.......
-00002190: 71a4 7c00 6a17 4400 5d22 7d0b 7400 a00d  q.|.j.D.]"}.t...
-000021a0: 6410 7c0b 9b00 9d02 a101 0100 7c0b a016  d.|.........|...
-000021b0: 7c00 6a13 a101 0100 9001 71cc 7c00 a018  |.j.......q.|...
-000021c0: a100 7c00 5f19 7118 7400 a001 6411 a101  ..|._.q.t...d...
-000021d0: 0100 6400 5300 2912 4e7a 3457 6169 7469  ..d.S.).Nz4Waiti
-000021e0: 6e67 2066 6f72 2061 6c6c 2070 6f72 7473  ng for all ports
-000021f0: 2074 6f20 6265 6769 6e20 6861 7276 6573   to begin harves
-00002200: 7469 6e67 2063 6f72 6e65 7273 2e2e 2e72  ting corners...r
-00002210: 0100 0000 7a26 4162 6f75 7420 746f 2073  ....z&About to s
-00002220: 7461 7274 2073 796e 6368 726f 6e69 7a69  tart synchronizi
-00002230: 6e67 2066 7261 6d65 732e 2e2e 7251 0000  ng frames...rQ..
-00002240: 007a 1653 6b69 7070 6564 2066 7261 6d65  .z.Skipped frame
-00002250: 2061 7420 706f 7274 207a 113a 203e 2065   at port z.: > e
-00002260: 6172 6c69 6573 745f 6e65 7874 7a1d 3a20  arliest_nextz.: 
-00002270: 6465 6c74 6120 3c20 7469 6d65 2d6c 6174  delta < time-lat
-00002280: 6573 745f 6375 7272 656e 7472 5200 0000  est_currentrR...
-00002290: 7a1a 4164 6469 6e67 2074 6f20 6c61 7965  z.Adding to laye
-000022a0: 7220 6672 6f6d 2070 6f72 7420 7a0a 2061  r from port z. a
-000022b0: 7420 696e 6465 7820 7a11 2061 6e64 2066  t index z. and f
-000022c0: 7261 6d65 2074 696d 653a 207a 1355 6e61  rame time: z.Una
-000022d0: 7373 6967 6e65 6420 4672 616d 6573 3a20  ssigned Frames: 
-000022e0: 7a37 5365 6e64 696e 6720 604e 6f6e 6560  z7Sending `None`
-000022f0: 206f 6e20 7175 6575 6520 746f 2073 6967   on queue to sig
-00002300: 6e61 6c20 656e 6420 6f66 2073 796e 6365  nal end of synce
-00002310: 6420 6672 616d 6573 2e7a 2f47 6976 696e  d frames.z/Givin
-00002320: 6720 6e6f 7469 6365 206f 6620 6e65 7720  g notice of new 
-00002330: 7379 6e63 6865 6420 6672 616d 6573 2070  synched frames p
-00002340: 6163 6b65 7420 7669 6120 7a1c 6e65 7720  acket via z.new 
-00002350: 7379 6e63 6865 6420 6672 616d 6573 2061  synched frames a
-00002360: 7661 696c 6162 6c65 7a2c 506c 6163 696e  vailablez,Placin
-00002370: 6720 6e65 7720 7379 6e63 6865 6420 6672  g new synched fr
-00002380: 616d 6573 2070 6163 6b65 7420 6f6e 2071  ames packet on q
-00002390: 7565 7565 3a20 7a25 4672 616d 6520 7379  ueue: z%Frame sy
-000023a0: 6e63 6820 776f 726b 6572 2073 7563 6365  nch worker succe
-000023b0: 7373 6675 6c6c 7920 656e 6465 6429 1a72  ssfully ended).r
-000023c0: 3600 0000 7237 0000 0072 1500 0000 7253  6...r7...r....rS
-000023d0: 0000 0072 1700 0000 725f 0000 0072 6100  ...r....r_...ra.
-000023e0: 0000 7245 0000 0072 1400 0000 7257 0000  ..rE...r....rW..
-000023f0: 00da 0777 6172 6e69 6e67 da03 706f 7072  ...warning..popr
-00002400: 1a00 0000 7256 0000 0072 6500 0000 7246  ....rV...re...rF
-00002410: 0000 0072 3300 0000 7234 0000 0072 0600  ...r3...r4...r..
-00002420: 0000 722f 0000 0072 3200 0000 7212 0000  ..r/...r2...r...
-00002430: 00da 0370 7574 7213 0000 0072 6700 0000  ...putr....rg...
-00002440: 721f 0000 0029 0c72 2400 0000 da0a 7379  r....).r$.....sy
-00002450: 6e63 5f69 6e64 6578 5a15 6375 7272 656e  nc_indexZ.curren
-00002460: 745f 6672 616d 655f 7061 636b 6574 735a  t_frame_packetsZ
-00002470: 116c 6179 6572 5f66 7261 6d65 5f74 696d  .layer_frame_tim
-00002480: 6573 5a0d 6561 726c 6965 7374 5f6e 6578  esZ.earliest_nex
-00002490: 745a 0e6c 6174 6573 745f 6375 7272 656e  tZ.latest_curren
-000024a0: 7472 0f00 0000 5a13 6375 7272 656e 745f  tr....Z.current_
-000024b0: 6672 616d 655f 696e 6465 785a 0e70 6f72  frame_indexZ.por
-000024c0: 745f 696e 6465 785f 6b65 795a 1463 7572  t_index_keyZ.cur
-000024d0: 7265 6e74 5f66 7261 6d65 5f70 6163 6b65  rent_frame_packe
-000024e0: 7472 5700 0000 7227 0000 0072 0c00 0000  trW...r'...r....
-000024f0: 720c 0000 0072 1000 0000 724a 0000 00e1  r....r....rJ....
-00002500: 0000 0073 6400 0000 0002 0a02 0402 0a01  ...sd...........
-00002510: 0c02 0402 0404 0401 0402 0a01 0e01 0e01  ................
-00002520: 0c02 0a01 0a02 0e01 0a01 0603 0c02 0801  ................
-00002530: 1402 16ff 0205 0801 0401 0aff 0605 0601  ................
-00002540: 02ff 0804 1201 0a01 0401 14ff 0604 1602  ................
-00002550: 1202 0c02 0802 0802 0c01 0a01 0604 0a01  ................
-00002560: 1001 0e02 0a01 1001 1002 0c02 7a20 5379  ............z Sy
-00002570: 6e63 6872 6f6e 697a 6572 2e73 796e 6368  nchronizer.synch
-00002580: 5f66 7261 6d65 735f 776f 726b 6572 4e29  _frames_workerN)
-00002590: 0172 0900 0000 291b da08 5f5f 6e61 6d65  .r....)...__name
-000025a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000025b0: 5f5f 7175 616c 6e61 6d65 5f5f da04 6469  __qualname__..di
-000025c0: 6374 7228 0000 00da 0462 6f6f 6c72 2c00  ctr(.....boolr,.
-000025d0: 0000 722e 0000 0072 3200 0000 da08 7072  ..r....r2.....pr
-000025e0: 6f70 6572 7479 7235 0000 0072 1e00 0000  opertyr5...r....
-000025f0: 721c 0000 0072 3c00 0000 7242 0000 0072  r....r<...rB...r
-00002600: 2200 0000 7223 0000 0072 4c00 0000 724e  "...r#...rL...rN
-00002610: 0000 0072 4f00 0000 7250 0000 0072 4900  ...rO...rP...rI.
-00002620: 0000 725f 0000 0072 6100 0000 7263 0000  ..r_...ra...rc..
-00002630: 0072 6700 0000 724a 0000 0072 0c00 0000  .rg...rJ...r....
-00002640: 720c 0000 0072 0c00 0000 7210 0000 0072  r....r....r....r
-00002650: 0800 0000 1300 0000 732c 0000 0008 0110  ........s,......
-00002660: 230e 0408 0308 0702 010a 0708 0608 0508  #...............
-00002670: 0608 0608 0608 0e08 0708 0808 0408 0408  ................
-00002680: 1408 2008 0c08 0908 0972 0800 0000 da08  .. ......r......
-00002690: 5f5f 6d61 696e 5f5f 2901 da07 4368 6172  __main__)...Char
-000026a0: 7563 6f29 01da 0e43 6861 7275 636f 5472  uco)...CharucoTr
-000026b0: 6163 6b65 7229 02da 0e52 6563 6f72 6465  acker)...Recorde
-000026c0: 6453 7472 6561 6dda 1252 6563 6f72 6465  dStream..Recorde
-000026d0: 6453 7472 6561 6d50 6f6f 6c29 01da 0753  dStreamPool)...S
-000026e0: 6573 7369 6f6e 2901 da08 5f5f 726f 6f74  ession)...__root
-000026f0: 5f5f 46da 0574 6573 7473 5a03 3231 3754  __F..testsZ.217T
-00002700: 7a15 4372 6561 7469 6e67 2053 796e 6368  z.Creating Synch
-00002710: 726f 6e69 7a65 72e9 0500 0000 2901 7225  ronizer.....).r%
-00002720: 0000 0072 5200 0000 e902 0000 00e9 0300  ...rR...........
-00002730: 0000 e904 0000 005a 0873 6573 7369 6f6e  .......Z.session
-00002740: 73e9 0b00 0000 6700 0000 0000 0021 4067  s.....g......!@g
-00002750: 0000 0000 0000 e83f 6700 0000 0000 0015  .......?g.......
-00002760: 4029 03da 0b61 7275 636f 5f73 6361 6c65  @)...aruco_scale
-00002770: da16 7371 7561 7265 5f73 697a 655f 6f76  ..square_size_ov
-00002780: 6572 6964 655f 636d da08 696e 7665 7274  eride_cm..invert
-00002790: 6564 2901 da07 6368 6172 7563 6fe9 1400  ed)...charuco...
-000027a0: 0000 7a16 4265 6769 6e6e 696e 6720 706c  ..z.Beginning pl
-000027b0: 6179 6261 636b 2061 7420 7a05 506f 7274  ayback at z.Port
-000027c0: 2072 2700 0000 7a15 506c 6179 6261 636b   r'...z.Playback
-000027d0: 2066 696e 6973 6865 6420 6174 2029 43da   finished at )C.
-000027e0: 0d70 7978 7933 642e 6c6f 6767 6572 da06  .pyxy3d.logger..
-000027f0: 7079 7879 3364 7236 0000 0072 5400 0000  pyxy3dr6...rT...
-00002800: 726c 0000 00da 076c 6f67 6769 6e67 da08  rl.....logging..
-00002810: 7365 744c 6576 656c da05 4445 4255 4772  setLevel..DEBUGr
-00002820: 5a00 0000 da07 7061 7468 6c69 6272 0200  Z.....pathlibr..
-00002830: 0000 da05 7175 6575 6572 0300 0000 da09  ....queuer......
-00002840: 7468 7265 6164 696e 6772 0400 0000 7205  threadingr....r.
-00002850: 0000 00da 0363 7632 da05 6e75 6d70 7972  .....cv2..numpyr
-00002860: 3300 0000 da1b 7079 7879 3364 2e63 616d  3.....pyxy3d.cam
-00002870: 6572 6173 2e64 6174 615f 7061 636b 6574  eras.data_packet
-00002880: 7372 0600 0000 7231 0000 0072 0800 0000  sr....r1...r....
-00002890: da1a 7079 7879 3364 2e63 616c 6962 7261  ..pyxy3d.calibra
-000028a0: 7469 6f6e 2e63 6861 7275 636f 7273 0000  tion.charucors..
-000028b0: 00da 1d70 7978 7933 642e 696d 6732 7879  ...pyxy3d.img2xy
-000028c0: 2e63 6861 7275 636f 5f74 7261 636b 6572  .charuco_tracker
-000028d0: 7274 0000 005a 2070 7978 7933 642e 7265  rt...Z pyxy3d.re
-000028e0: 636f 7264 696e 672e 7265 636f 7264 6564  cording.recorded
-000028f0: 5f73 7472 6561 6d72 7500 0000 7276 0000  _streamru...rv..
-00002900: 00da 0e70 7978 7933 642e 7365 7373 696f  ...pyxy3d.sessio
-00002910: 6e72 7700 0000 7278 0000 005a 0974 6573  nrw...rx...Z.tes
-00002920: 745f 6c69 7665 da11 7365 7373 696f 6e5f  t_live..session_
-00002930: 6469 7265 6374 6f72 79da 0773 6573 7369  directory..sessi
-00002940: 6f6e da0c 6c6f 6164 5f63 616d 6572 6173  on..load_cameras
-00002950: da0c 6c6f 6164 5f73 7472 6561 6d73 720a  ..load_streamsr.
-00002960: 0000 0072 1900 0000 720f 0000 0072 2600  ...r....r....r&.
-00002970: 0000 da09 5f73 686f 775f 6670 73da 0d5f  ...._show_fps.._
-00002980: 7368 6f77 5f63 6861 7275 636f 7237 0000  show_charucor7..
-00002990: 005a 0573 796e 6372 7217 0000 005a 1372  .Z.syncrr....Z.r
-000029a0: 6563 6f72 6469 6e67 5f64 6972 6563 746f  ecording_directo
-000029b0: 7279 7282 0000 005a 1472 6563 6f72 6465  ryr....Z.recorde
-000029c0: 645f 7374 7265 616d 5f70 6f6f 6c5a 0b70  d_stream_poolZ.p
-000029d0: 6c61 795f 7669 6465 6f73 5a0e 6e6f 7469  lay_videosZ.noti
-000029e0: 6669 6361 7469 6f6e 5f71 724c 0000 00da  fication_qrL....
-000029f0: 0c70 6572 665f 636f 756e 7465 7272 1500  .perf_counterr..
-00002a00: 0000 7253 0000 005a 1573 796e 6368 6564  ..rS...Z.synched
-00002a10: 5f66 7261 6d65 735f 6e6f 7469 6365 722f  _frames_noticer/
-00002a20: 0000 005a 0b73 796e 635f 7061 636b 6574  ...Z.sync_packet
-00002a30: da0d 6672 616d 655f 7061 636b 6574 7372  ..frame_packetsr
-00002a40: 5800 0000 da06 696d 7368 6f77 da05 6672  X.....imshow..fr
-00002a50: 616d 65da 0777 6169 744b 6579 da03 6b65  ame..waitKey..ke
-00002a60: 79da 036f 7264 da11 6465 7374 726f 7941  y..ord..destroyA
-00002a70: 6c6c 5769 6e64 6f77 7372 0c00 0000 720c  llWindowsr....r.
-00002a80: 0000 0072 0c00 0000 7210 0000 00da 083c  ...r....r......<
-00002a90: 6d6f 6475 6c65 3e01 0000 0073 8200 0000  module>....s....
-00002aa0: 0802 0c01 0802 0c02 0801 0c01 0c01 1002  ................
-00002ab0: 0801 0801 0c02 0402 0e7f 007f 0025 0a01  .............%..
-00002ac0: 0c01 0c01 1002 0c01 0802 0c04 0402 0602  ................
-00002ad0: 0c02 0801 0801 0803 1201 0601 0a02 0a01  ................
-00002ae0: 1002 0e02 0e01 0201 0200 0200 0200 0200  ................
-00002af0: 0200 0200 02ff 0603 0201 0200 0200 02ff  ................
-00002b00: 0603 0a01 0e01 0802 0602 0a01 1402 0c01  ................
-00002b10: 0801 0601 1202 0601 1802 0a02 0e01 0801  ................
-00002b20: 0802                                     ..
+00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
+00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
+00000060: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
+00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6401 6c0e  m.Z.m.Z...d.d.l.
+00000080: 5a0e 6400 6401 6c0f 5a10 6400 6405 6c11  Z.d.d.l.Z.d.d.l.
+00000090: 6d12 5a12 0100 6406 5a13 4700 6407 6408  m.Z...d.Z.G.d.d.
+000000a0: 8400 6408 8302 5a14 6401 5300 2909 e900  ..d...Z.d.S.)...
+000000b0: 0000 004e 2901 da04 5061 7468 2901 da05  ...N)...Path)...
+000000c0: 5175 6575 6529 02da 0654 6872 6561 64da  Queue)...Thread.
+000000d0: 0545 7665 6e74 2901 da0a 5379 6e63 5061  .Event)...SyncPa
+000000e0: 636b 6574 e964 0000 0063 0000 0000 0000  cket.d...c......
+000000f0: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000100: 0000 73be 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000110: 2d64 0265 0366 0264 0364 0484 055a 0464  -d.e.f.d.d...Z.d
+00000120: 0565 0566 0264 0664 0784 045a 0664 0864  .e.f.d.d...Z.d.d
+00000130: 0984 005a 0765 0864 0a64 0b84 0083 015a  ...Z.e.d.d.....Z
+00000140: 0964 0c64 0d84 005a 0a64 0e64 0f84 005a  .d.d...Z.d.d...Z
+00000150: 0b64 1064 1184 005a 0c64 1264 1384 005a  .d.d...Z.d.d...Z
+00000160: 0d64 1464 1584 005a 0e64 1664 1784 005a  .d.d...Z.d.d...Z
+00000170: 0f64 1864 1984 005a 1064 1a64 1b84 005a  .d.d...Z.d.d...Z
+00000180: 1164 1c64 1d84 005a 1264 1e64 1f84 005a  .d.d...Z.d.d...Z
+00000190: 1364 2064 2184 005a 1464 2264 2384 005a  .d d!..Z.d"d#..Z
+000001a0: 1564 2464 2584 005a 1664 2664 2784 005a  .d$d%..Z.d&d'..Z
+000001b0: 1764 2864 2984 005a 1864 2a64 2b84 005a  .d(d)..Z.d*d+..Z
+000001c0: 1964 2c53 0029 2eda 0c53 796e 6368 726f  .d,S.)...Synchro
+000001d0: 6e69 7a65 72e9 0600 0000 da07 7374 7265  nizer.......stre
+000001e0: 616d 7363 0300 0000 0000 0000 0000 0000  amsc............
+000001f0: 0600 0000 0400 0000 4300 0000 73b2 0000  ........C...s...
+00000200: 007c 017c 005f 0064 007c 005f 0167 007c  .|.|._.d.|._.g.|
+00000210: 005f 0267 007c 005f 0369 007c 005f 0474  ._.g.|._.i.|._.t
+00000220: 0583 007c 005f 0664 017c 005f 0767 007c  ...|._.d.|._.g.|
+00000230: 005f 0869 007c 005f 097c 006a 00a0 0aa1  ._.i.|._.|.j....
+00000240: 0044 005d 135c 027d 037d 047c 006a 08a0  .D.].\.}.}.|.j..
+00000250: 0b7c 03a1 0101 0074 0c64 0283 017d 057c  .|.....t.d...}.|
+00000260: 057c 006a 097c 033c 0071 2164 017c 005f  .|.j.|.<.q!d.|._
+00000270: 0d7c 00a0 0ea1 0001 007c 00a0 0f7c 02a1  .|.......|...|..
+00000280: 0101 007c 027c 005f 1064 0364 0484 0074  ...|.|._.d.d...t
+00000290: 117c 006a 0883 0144 0083 017c 005f 127c  .|.j...D...|._.|
+000002a0: 00a0 13a1 0001 007c 00a0 14a1 0001 0064  .......|.......d
+000002b0: 0053 0029 054e 46e9 ffff ffff 6301 0000  .S.).NF.....c...
+000002c0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000002d0: 0053 0000 0073 1200 0000 6900 7c00 5d05  .S...s....i.|.].
+000002e0: 7d01 7c01 6700 9302 7102 5300 a900 720c  }.|.g...q.S...r.
+000002f0: 0000 00a9 02da 022e 30da 0470 6f72 7472  ........0..portr
+00000300: 0c00 0000 720c 0000 00fa 3f43 3a5c 5573  ....r.....?C:\Us
+00000310: 6572 735c 4d61 6320 5072 6962 6c65 5c72  ers\Mac Prible\r
+00000320: 6570 6f73 5c70 7978 7933 645c 7079 7879  epos\pyxy3d\pyxy
+00000330: 3364 5c63 616d 6572 6173 5c73 796e 6368  3d\cameras\synch
+00000340: 726f 6e69 7a65 722e 7079 da0a 3c64 6963  ronizer.py..<dic
+00000350: 7463 6f6d 703e 3100 0000 f302 0000 0012  tcomp>1.........
+00000360: 007a 2953 796e 6368 726f 6e69 7a65 722e  .z)Synchronizer.
+00000370: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+00000380: 3e2e 3c64 6963 7463 6f6d 703e 2915 720a  >.<dictcomp>).r.
+00000390: 0000 005a 1663 7572 7265 6e74 5f73 796e  ...Z.current_syn
+000003a0: 6368 6564 5f66 7261 6d65 73da 1773 796e  ched_frames..syn
+000003b0: 635f 6e6f 7469 6365 5f73 7562 7363 7269  c_notice_subscri
+000003c0: 6265 7273 da1a 7379 6e63 6865 645f 6672  bers..synched_fr
+000003d0: 616d 6573 5f73 7562 7363 7269 6265 7273  ames_subscribers
+000003e0: da11 616c 6c5f 6672 616d 655f 7061 636b  ..all_frame_pack
+000003f0: 6574 7372 0500 0000 da0a 7374 6f70 5f65  etsr......stop_e
+00000400: 7665 6e74 da0f 6672 616d 6573 5f63 6f6d  vent..frames_com
+00000410: 706c 6574 65da 0570 6f72 7473 da13 6672  plete..ports..fr
+00000420: 616d 655f 7061 636b 6574 5f71 7565 7565  ame_packet_queue
+00000430: 73da 0569 7465 6d73 da06 6170 7065 6e64  s..items..append
+00000440: 7203 0000 00da 1573 7562 7363 7269 6265  r......subscribe
+00000450: 645f 746f 5f73 7472 6561 6d73 da14 7375  d_to_streams..su
+00000460: 6273 6372 6962 655f 746f 5f73 7472 6561  bscribe_to_strea
+00000470: 6d73 da0e 7365 745f 7374 7265 616d 5f66  ms..set_stream_f
+00000480: 7073 da08 6670 735f 6d65 616e da06 736f  ps..fps_mean..so
+00000490: 7274 6564 da15 6472 6f70 7065 645f 6672  rted..dropped_fr
+000004a0: 616d 655f 6869 7374 6f72 79da 1269 6e69  ame_history..ini
+000004b0: 7469 616c 697a 655f 6c65 6467 6572 73da  tialize_ledgers.
+000004c0: 0573 7461 7274 2906 da04 7365 6c66 720a  .start)...selfr.
+000004d0: 0000 00da 0a66 7073 5f74 6172 6765 7472  .....fps_targetr
+000004e0: 0f00 0000 da06 7374 7265 616d da01 7172  ......stream..qr
+000004f0: 0c00 0000 720c 0000 0072 1000 0000 da08  ....r....r......
+00000500: 5f5f 696e 6974 5f5f 1400 0000 732c 0000  __init__....s,..
+00000510: 0006 0106 0102 0304 ff02 0404 ff06 0408  ................
+00000520: 0106 0106 0206 0112 010c 0108 010c 0106  ................
+00000530: 0208 010a 0206 0116 0308 020c 017a 1553  .............z.S
+00000540: 796e 6368 726f 6e69 7a65 722e 5f5f 696e  ynchronizer.__in
+00000550: 6974 5f5f da05 7472 6163 6b63 0200 0000  it__..trackc....
+00000560: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000570: 4300 0000 7322 0000 007c 006a 00a0 01a1  C...s"...|.j....
+00000580: 0044 005d 095c 027d 027d 037c 03a0 027c  .D.].\.}.}.|...|
+00000590: 01a1 0101 0071 0564 0053 00a9 014e 2903  .....q.d.S...N).
+000005a0: 720a 0000 0072 1a00 0000 da0f 7365 745f  r....r......set_
+000005b0: 7472 6163 6b69 6e67 5f6f 6e29 0472 2400  tracking_on).r$.
+000005c0: 0000 7229 0000 0072 0f00 0000 7226 0000  ..r)...r....r&..
+000005d0: 0072 0c00 0000 720c 0000 0072 1000 0000  .r....r....r....
+000005e0: da17 7365 745f 7472 6163 6b69 6e67 5f6f  ..set_tracking_o
+000005f0: 6e5f 7374 7265 616d 7336 0000 0073 0600  n_streams6...s..
+00000600: 0000 1201 0c01 04ff 7a24 5379 6e63 6872  ........z$Synchr
+00000610: 6f6e 697a 6572 2e73 6574 5f74 7261 636b  onizer.set_track
+00000620: 696e 675f 6f6e 5f73 7472 6561 6d73 6301  ing_on_streamsc.
+00000630: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00000640: 0000 0043 0000 0073 4800 0000 7c00 6a00  ...C...sH...|.j.
+00000650: 6a01 7d01 7c01 a002 a100 4400 5d19 5c02  j.}.|.....D.].\.
+00000660: 7d02 7d03 7c00 6a03 7c02 1900 a004 7c03  }.}.|.j.|.....|.
+00000670: a101 0100 7c00 6a03 7c02 1900 7405 0b00  ....|.j.|...t...
+00000680: 6400 8502 1900 7c00 6a03 7c02 3c00 7108  d.....|.j.|.<.q.
+00000690: 6400 5300 722a 0000 0029 06da 1363 7572  d.S.r*...)...cur
+000006a0: 7265 6e74 5f73 796e 635f 7061 636b 6574  rent_sync_packet
+000006b0: da07 6472 6f70 7065 6472 1a00 0000 7221  ..droppedr....r!
+000006c0: 0000 0072 1b00 0000 da1a 4452 4f50 5045  ...r......DROPPE
+000006d0: 445f 4652 414d 455f 5452 4143 4b5f 5749  D_FRAME_TRACK_WI
+000006e0: 4e44 4f57 2904 7224 0000 005a 0f63 7572  NDOW).r$...Z.cur
+000006f0: 7265 6e74 5f64 726f 7070 6564 720f 0000  rent_droppedr...
+00000700: 0072 2e00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000710: 7210 0000 00da 1c75 7064 6174 655f 6472  r......update_dr
+00000720: 6f70 7065 645f 6672 616d 655f 6869 7374  opped_frame_hist
+00000730: 6f72 793a 0000 0073 0a00 0000 0801 1002  ory:...s........
+00000740: 1001 1c01 04fe 7a29 5379 6e63 6872 6f6e  ......z)Synchron
+00000750: 697a 6572 2e75 7064 6174 655f 6472 6f70  izer.update_drop
+00000760: 7065 645f 6672 616d 655f 6869 7374 6f72  ped_frame_histor
+00000770: 7963 0100 0000 0000 0000 0000 0000 0100  yc..............
+00000780: 0000 0300 0000 4300 0000 7314 0000 0064  ......C...s....d
+00000790: 0164 0284 007c 006a 00a0 01a1 0044 0083  .d...|.j.....D..
+000007a0: 0153 0029 037a 4a0a 2020 2020 2020 2020  .S.).zJ.        
+000007b0: 4176 6572 6167 6573 2064 726f 7070 6564  Averages dropped
+000007c0: 2066 7261 6d65 2063 6f75 6e74 2061 6372   frame count acr
+000007d0: 6f73 7320 7468 6520 6f62 7365 7276 6564  oss the observed
+000007e0: 2068 6973 746f 7279 0a20 2020 2020 2020   history.       
+000007f0: 2063 0100 0000 0000 0000 0000 0000 0300   c..............
+00000800: 0000 0600 0000 5300 0000 731c 0000 0069  ......S...s....i
+00000810: 007c 005d 0a5c 027d 017d 027c 0174 00a0  .|.].\.}.}.|.t..
+00000820: 017c 02a1 0193 0271 0253 0072 0c00 0000  .|.....q.S.r....
+00000830: 2902 da02 6e70 da04 6d65 616e 2903 720e  )...np..mean).r.
+00000840: 0000 0072 0f00 0000 5a0c 6472 6f70 5f68  ...r....Z.drop_h
+00000850: 6973 746f 7279 720c 0000 0072 0c00 0000  istoryr....r....
+00000860: 7210 0000 0072 1100 0000 4600 0000 7302  r....r....F...s.
+00000870: 0000 001c 007a 2c53 796e 6368 726f 6e69  .....z,Synchroni
+00000880: 7a65 722e 6472 6f70 7065 645f 6670 732e  zer.dropped_fps.
+00000890: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+000008a0: 6d70 3e29 0272 2100 0000 721a 0000 00a9  mp>).r!...r.....
+000008b0: 0172 2400 0000 720c 0000 0072 0c00 0000  .r$...r....r....
+000008c0: 7210 0000 00da 0b64 726f 7070 6564 5f66  r......dropped_f
+000008d0: 7073 4100 0000 7302 0000 0014 057a 1853  psA...s......z.S
+000008e0: 796e 6368 726f 6e69 7a65 722e 6472 6f70  ynchronizer.drop
+000008f0: 7065 645f 6670 7363 0200 0000 0000 0000  ped_fpsc........
+00000900: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00000910: 7338 0000 007c 017c 005f 0074 01a0 0264  s8...|.|._.t...d
+00000920: 017c 019b 009d 02a1 0101 007c 006a 03a0  .|.........|.j..
+00000930: 04a1 0044 005d 095c 027d 027d 037c 03a0  ...D.].\.}.}.|..
+00000940: 057c 01a1 0101 0071 1064 0053 0029 024e  .|.....q.d.S.).N
+00000950: 7a2e 4174 7465 6d70 7469 6e67 2074 6f20  z.Attempting to 
+00000960: 6368 616e 6765 2074 6172 6765 7420 6670  change target fp
+00000970: 7320 696e 2073 7472 6561 6d73 2074 6f20  s in streams to 
+00000980: 2906 7225 0000 00da 066c 6f67 6765 72da  ).r%.....logger.
+00000990: 0469 6e66 6f72 0a00 0000 721a 0000 00da  .infor....r.....
+000009a0: 0e73 6574 5f66 7073 5f74 6172 6765 7429  .set_fps_target)
+000009b0: 0472 2400 0000 7225 0000 0072 0f00 0000  .r$...r%...r....
+000009c0: 7226 0000 0072 0c00 0000 720c 0000 0072  r&...r....r....r
+000009d0: 1000 0000 721e 0000 0049 0000 0073 0a00  ....r....I...s..
+000009e0: 0000 0601 1001 1201 0c01 04ff 7a1b 5379  ............z.Sy
+000009f0: 6e63 6872 6f6e 697a 6572 2e73 6574 5f73  nchronizer.set_s
+00000a00: 7472 6561 6d5f 6670 7363 0100 0000 0000  tream_fpsc......
+00000a10: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
+00000a20: 0000 f33e 0000 007c 006a 00a0 01a1 0044  ...>...|.j.....D
+00000a30: 005d 145c 027d 017d 0274 02a0 0364 017c  .].\.}.}.t...d.|
+00000a40: 019b 009d 02a1 0101 007c 02a0 047c 006a  .........|...|.j
+00000a50: 057c 0119 00a1 0101 0071 0564 027c 005f  .|.......q.d.|._
+00000a60: 0664 0053 0029 034e 7a2d 5375 6273 6372  .d.S.).Nz-Subscr
+00000a70: 6962 696e 6720 7379 6e63 6872 6f6e 697a  ibing synchroniz
+00000a80: 6572 2074 6f20 7374 7265 616d 2066 726f  er to stream fro
+00000a90: 6d20 706f 7274 2054 2907 720a 0000 0072  m port T).r....r
+00000aa0: 1a00 0000 7235 0000 0072 3600 0000 da09  ....r5...r6.....
+00000ab0: 7375 6273 6372 6962 6572 1900 0000 721c  subscriber....r.
+00000ac0: 0000 00a9 0372 2400 0000 720f 0000 0072  .....r$...r....r
+00000ad0: 2600 0000 720c 0000 0072 0c00 0000 7210  &...r....r....r.
+00000ae0: 0000 0072 1d00 0000 4f00 0000 f308 0000  ...r....O.......
+00000af0: 0012 0110 0112 010a 017a 2153 796e 6368  .........z!Synch
+00000b00: 726f 6e69 7a65 722e 7375 6273 6372 6962  ronizer.subscrib
+00000b10: 655f 746f 5f73 7472 6561 6d73 6301 0000  e_to_streamsc...
+00000b20: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000b30: 0043 0000 0072 3800 0000 2903 4e7a 2375  .C...r8...).Nz#u
+00000b40: 6e73 7562 7363 7269 6265 2073 796e 6368  nsubscribe synch
+00000b50: 726f 6e69 7a65 7220 6672 6f6d 2070 6f72  ronizer from por
+00000b60: 7420 4629 0772 0a00 0000 721a 0000 0072  t F).r....r....r
+00000b70: 3500 0000 7236 0000 00da 0b75 6e73 7562  5...r6.....unsub
+00000b80: 7363 7269 6265 7219 0000 0072 1c00 0000  scriber....r....
+00000b90: 723a 0000 0072 0c00 0000 720c 0000 0072  r:...r....r....r
+00000ba0: 1000 0000 da18 756e 7375 6273 6372 6962  ......unsubscrib
+00000bb0: 655f 6672 6f6d 5f73 7472 6561 6d73 5500  e_from_streamsU.
+00000bc0: 0000 723b 0000 007a 2553 796e 6368 726f  ..r;...z%Synchro
+00000bd0: 6e69 7a65 722e 756e 7375 6273 6372 6962  nizer.unsubscrib
+00000be0: 655f 6672 6f6d 5f73 7472 6561 6d73 6301  e_from_streamsc.
+00000bf0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00000c00: 0000 0043 0000 0073 2c00 0000 7c00 6a00  ...C...s,...|.j.
+00000c10: a001 a100 0100 7c00 6a02 a003 a100 0100  ......|.j.......
+00000c20: 7c00 6a04 4400 5d06 7d01 7c01 a003 a100  |.j.D.].}.|.....
+00000c30: 0100 710d 6400 5300 722a 0000 0029 0572  ..q.d.S.r*...).r
+00000c40: 1600 0000 da03 7365 74da 0674 6872 6561  ......set..threa
+00000c50: 64da 046a 6f69 6eda 0774 6872 6561 6473  d..join..threads
+00000c60: 2902 7224 0000 00da 0174 720c 0000 0072  ).r$.....tr....r
+00000c70: 0c00 0000 7210 0000 00da 0473 746f 705b  ....r......stop[
+00000c80: 0000 0073 0a00 0000 0a01 0a01 0a01 0a01  ...s............
+00000c90: 04ff 7a11 5379 6e63 6872 6f6e 697a 6572  ..z.Synchronizer
+00000ca0: 2e73 746f 7063 0100 0000 0000 0000 0000  .stopc..........
+00000cb0: 0000 0100 0000 0200 0000 4300 0000 732e  ..........C...s.
+00000cc0: 0000 0064 0164 0284 007c 006a 0044 0083  ...d.d...|.j.D..
+00000cd0: 017c 005f 0164 0364 0284 007c 006a 0044  .|._.d.d...|.j.D
+00000ce0: 0083 017c 005f 0267 007c 005f 0364 0053  ...|._.g.|._.d.S
+00000cf0: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000d00: 0002 0000 0004 0000 0053 0000 00f3 1200  .........S......
+00000d10: 0000 6900 7c00 5d05 7d01 7c01 6400 9302  ..i.|.].}.|.d...
+00000d20: 7102 5300 a901 7201 0000 0072 0c00 0000  q.S...r....r....
+00000d30: 720d 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000d40: 1000 0000 7211 0000 0063 0000 0072 1200  ....r....c...r..
+00000d50: 0000 7a33 5379 6e63 6872 6f6e 697a 6572  ..z3Synchronizer
+00000d60: 2e69 6e69 7469 616c 697a 655f 6c65 6467  .initialize_ledg
+00000d70: 6572 732e 3c6c 6f63 616c 733e 2e3c 6469  ers.<locals>.<di
+00000d80: 6374 636f 6d70 3e63 0100 0000 0000 0000  ctcomp>c........
+00000d90: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00000da0: 7244 0000 0072 4500 0000 720c 0000 0072  rD...rE...r....r
+00000db0: 0d00 0000 720c 0000 0072 0c00 0000 7210  ....r....r....r.
+00000dc0: 0000 0072 1100 0000 6400 0000 7212 0000  ...r....d...r...
+00000dd0: 0029 0472 1800 0000 da10 706f 7274 5f66  .).r......port_f
+00000de0: 7261 6d65 5f63 6f75 6e74 da12 706f 7274  rame_count..port
+00000df0: 5f63 7572 7265 6e74 5f66 7261 6d65 da10  _current_frame..
+00000e00: 6d65 616e 5f66 7261 6d65 5f74 696d 6573  mean_frame_times
+00000e10: 7233 0000 0072 0c00 0000 720c 0000 0072  r3...r....r....r
+00000e20: 1000 0000 7222 0000 0061 0000 0073 0600  ....r"...a...s..
+00000e30: 0000 1202 1201 0a01 7a1f 5379 6e63 6872  ........z.Synchr
+00000e40: 6f6e 697a 6572 2e69 6e69 7469 616c 697a  onizer.initializ
+00000e50: 655f 6c65 6467 6572 7363 0100 0000 0000  e_ledgersc......
+00000e60: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
+00000e70: 0000 737e 0000 0074 00a0 0164 01a1 0101  ..s~...t...d....
+00000e80: 0067 007c 005f 027c 006a 03a0 04a1 0044  .g.|._.|.j.....D
+00000e90: 005d 175c 027d 017d 0274 057c 006a 067c  .].\.}.}.t.|.j.|
+00000ea0: 0266 0164 0264 038d 037d 037c 03a0 07a1  .f.d.d...}.|....
+00000eb0: 0001 007c 006a 02a0 087c 03a1 0101 0071  ...|.j...|.....q
+00000ec0: 0d74 00a0 0164 04a1 0101 0074 00a0 0164  .t...d.....t...d
+00000ed0: 05a1 0101 0074 057c 006a 0964 0664 0264  .....t.|.j.d.d.d
+00000ee0: 038d 037c 005f 0a7c 006a 0aa0 07a1 0001  ...|._.|.j......
+00000ef0: 0064 0053 0029 074e 7a2e 4162 6f75 7420  .d.S.).Nz.About 
+00000f00: 746f 2073 7562 6d69 7420 5468 7265 6164  to submit Thread
+00000f10: 706f 6f6c 206f 6620 6672 616d 6520 4861  pool of frame Ha
+00000f20: 7276 6573 7465 7273 5429 03da 0674 6172  rvestersT)...tar
+00000f30: 6765 74da 0461 7267 73da 0664 6165 6d6f  get..args..daemo
+00000f40: 6e7a 1f46 7261 6d65 2068 6172 7665 7374  nz.Frame harvest
+00000f50: 6572 7320 6a75 7374 2073 7562 6d69 7474  ers just submitt
+00000f60: 6564 7a1e 5374 6172 7469 6e67 2066 7261  edz.Starting fra
+00000f70: 6d65 2073 796e 6368 726f 6e69 7a65 722e  me synchronizer.
+00000f80: 2e2e 720c 0000 0029 0b72 3500 0000 7236  ..r....).r5...r6
+00000f90: 0000 0072 4100 0000 720a 0000 0072 1a00  ...rA...r....r..
+00000fa0: 0000 7204 0000 00da 1568 6172 7665 7374  ..r......harvest
+00000fb0: 5f66 7261 6d65 5f70 6163 6b65 7473 7223  _frame_packetsr#
+00000fc0: 0000 0072 1b00 0000 da13 7379 6e63 685f  ...r......synch_
+00000fd0: 6672 616d 6573 5f77 6f72 6b65 7272 3f00  frames_workerr?.
+00000fe0: 0000 2904 7224 0000 0072 0f00 0000 7226  ..).r$...r....r&
+00000ff0: 0000 0072 4200 0000 720c 0000 0072 0c00  ...rB...r....r..
+00001000: 0000 7210 0000 0072 2300 0000 6700 0000  ..r....r#...g...
+00001010: 7314 0000 000a 0206 0112 0112 0108 010e  s...............
+00001020: 010a 010a 0212 010e 017a 1253 796e 6368  .........z.Synch
+00001030: 726f 6e69 7a65 722e 7374 6172 7463 0200  ronizer.startc..
+00001040: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001050: 0000 4300 0000 f31a 0000 0074 00a0 0164  ..C........t...d
+00001060: 01a1 0101 007c 006a 02a0 037c 01a1 0101  .....|.j...|....
+00001070: 0064 0053 0029 024e 7a37 4164 6469 6e67  .d.S.).Nz7Adding
+00001080: 2071 7565 7565 2074 6f20 7265 6365 6976   queue to receiv
+00001090: 6520 6e6f 7469 6365 206f 6620 7379 6e63  e notice of sync
+000010a0: 6865 6420 6672 616d 6573 2075 7064 6174  hed frames updat
+000010b0: 6529 0472 3500 0000 7236 0000 0072 1300  e).r5...r6...r..
+000010c0: 0000 721b 0000 00a9 0272 2400 0000 7227  ..r......r$...r'
+000010d0: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
+000010e0: 0000 da13 7375 6273 6372 6962 655f 746f  ....subscribe_to
+000010f0: 5f6e 6f74 6963 6575 0000 00f3 0400 0000  _noticeu........
+00001100: 0a04 1001 7a20 5379 6e63 6872 6f6e 697a  ....z Synchroniz
+00001110: 6572 2e73 7562 7363 7269 6265 5f74 6f5f  er.subscribe_to_
+00001120: 6e6f 7469 6365 6302 0000 0000 0000 0000  noticec.........
+00001130: 0000 0002 0000 0003 0000 0043 0000 0072  ...........C...r
+00001140: 4e00 0000 2902 4e7a 4652 656d 6f76 696e  N...).NzFRemovin
+00001150: 6720 7175 6575 6520 7468 6174 2068 6164  g queue that had
+00001160: 2062 6565 6e20 7265 6365 6976 696e 6720   been receiving 
+00001170: 6e6f 7469 6365 206f 6620 7379 6e63 6865  notice of synche
+00001180: 6420 6672 616d 6573 2075 7064 6174 6529  d frames update)
+00001190: 0472 3500 0000 7236 0000 0072 1300 0000  .r5...r6...r....
+000011a0: da06 7265 6d6f 7665 724f 0000 0072 0c00  ..removerO...r..
+000011b0: 0000 720c 0000 0072 1000 0000 da15 756e  ..r....r......un
+000011c0: 7375 6273 6372 6962 655f 746f 5f6e 6f74  subscribe_to_not
+000011d0: 6963 657c 0000 0072 5100 0000 7a22 5379  ice|...rQ...z"Sy
+000011e0: 6e63 6872 6f6e 697a 6572 2e75 6e73 7562  nchronizer.unsub
+000011f0: 7363 7269 6265 5f74 6f5f 6e6f 7469 6365  scribe_to_notice
+00001200: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001210: 0003 0000 0043 0000 0072 4e00 0000 2902  .....C...rN...).
+00001220: 4e7a 2641 6464 696e 6720 7175 6575 6520  Nz&Adding queue 
+00001230: 746f 2072 6563 6569 7665 2073 796e 6368  to receive synch
+00001240: 6564 2066 7261 6d65 7329 0472 3500 0000  ed frames).r5...
+00001250: 7236 0000 0072 1400 0000 721b 0000 0072  r6...r....r....r
+00001260: 4f00 0000 720c 0000 0072 0c00 0000 7210  O...r....r....r.
+00001270: 0000 00da 1973 7562 7363 7269 6265 5f74  .....subscribe_t
+00001280: 6f5f 7379 6e63 5f70 6163 6b65 7473 8400  o_sync_packets..
+00001290: 0000 f304 0000 000a 0110 017a 2653 796e  ...........z&Syn
+000012a0: 6368 726f 6e69 7a65 722e 7375 6273 6372  chronizer.subscr
+000012b0: 6962 655f 746f 5f73 796e 635f 7061 636b  ibe_to_sync_pack
+000012c0: 6574 7363 0200 0000 0000 0000 0000 0000  etsc............
+000012d0: 0200 0000 0300 0000 4300 0000 724e 0000  ........C...rN..
+000012e0: 0029 024e 7a16 5265 6c65 6173 696e 6720  .).Nz.Releasing 
+000012f0: 7265 636f 7264 2071 7565 7565 2904 7235  record queue).r5
+00001300: 0000 0072 3600 0000 7214 0000 0072 5200  ...r6...r....rR.
+00001310: 0000 724f 0000 0072 0c00 0000 720c 0000  ..rO...r....r...
+00001320: 0072 1000 0000 da15 7265 6c65 6173 655f  .r......release_
+00001330: 7379 6e63 5f70 6163 6b65 745f 7188 0000  sync_packet_q...
+00001340: 0072 5500 0000 7a22 5379 6e63 6872 6f6e  .rU...z"Synchron
+00001350: 697a 6572 2e72 656c 6561 7365 5f73 796e  izer.release_syn
+00001360: 635f 7061 636b 6574 5f71 6302 0000 0000  c_packet_qc.....
+00001370: 0000 0000 0000 0005 0000 0008 0000 0043  ...............C
+00001380: 0000 0073 a800 0000 7c01 6a00 7d02 7401  ...s....|.j.}.t.
+00001390: a002 6401 7c02 9b00 9d02 a101 0100 7c00  ..d.|.........|.
+000013a0: 6a03 a004 a100 7349 7c00 6a05 7c02 1900  j.....sI|.j.|...
+000013b0: a006 a100 7d03 7c00 6a07 7c02 1900 7d04  ....}.|.j.|...}.
+000013c0: 7c04 7c03 5f08 7c03 7c00 6a09 7c02 9b00  |.|._.|.|.j.|...
+000013d0: 6402 7c03 6a08 9b00 9d03 3c00 7c00 6a07  d.|.j.....<.|.j.
+000013e0: 7c02 0500 1900 6403 3700 0300 3c00 7401  |.....d.7...<.t.
+000013f0: a00a 6404 7c03 6a00 9b00 6405 7c03 6a08  ..d.|.j...d.|.j.
+00001400: 9b00 6406 7c03 6a0b 9b00 9d06 a101 0100  ..d.|.j.........
+00001410: 7c00 6a03 a004 a100 7210 7401 a002 6407  |.j.....r.t...d.
+00001420: 7c02 9b00 6408 9d03 a101 0100 6400 5300  |...d.......d.S.
+00001430: 2909 4e7a 2c42 6567 696e 6e69 6e67 2074  ).Nz,Beginning t
+00001440: 6f20 636f 6c6c 6563 7420 6461 7461 2067  o collect data g
+00001450: 656e 6572 6174 6564 2061 7420 706f 7274  enerated at port
+00001460: 20da 015f e901 0000 007a 1f46 7261 6d65   .._.....z.Frame
+00001470: 2064 6174 6120 6861 7276 6573 7465 6420   data harvested 
+00001480: 6672 6f6d 2072 6565 6c20 7a0c 2077 6974  from reel z. wit
+00001490: 6820 696e 6465 7820 7a13 2061 6e64 2066  h index z. and f
+000014a0: 7261 6d65 2074 696d 6520 6f66 207a 1946  rame time of z.F
+000014b0: 7261 6d65 2068 6172 7665 7374 6572 2066  rame harvester f
+000014c0: 6f72 2070 6f72 7420 7a0a 2063 6f6d 706c  or port z. compl
+000014d0: 6574 6564 290c 720f 0000 0072 3500 0000  eted).r....r5...
+000014e0: 7236 0000 0072 1600 0000 da06 6973 5f73  r6...r......is_s
+000014f0: 6574 7219 0000 00da 0367 6574 7246 0000  etr......getrF..
+00001500: 00da 0b66 7261 6d65 5f69 6e64 6578 7215  ...frame_indexr.
+00001510: 0000 00da 0564 6562 7567 da0a 6672 616d  .....debug..fram
+00001520: 655f 7469 6d65 2905 7224 0000 0072 2600  e_time).r$...r&.
+00001530: 0000 720f 0000 00da 0c66 7261 6d65 5f70  ..r......frame_p
+00001540: 6163 6b65 7472 5b00 0000 720c 0000 0072  acketr[...r....r
+00001550: 0c00 0000 7210 0000 0072 4c00 0000 8c00  ....r....rL.....
+00001560: 0000 731a 0000 0006 0110 020a 020e 010a  ..s.............
+00001570: 0106 0116 0212 0104 021a 0104 ff0a f816  ................
+00001580: 0c7a 2253 796e 6368 726f 6e69 7a65 722e  .z"Synchronizer.
+00001590: 6861 7276 6573 745f 6672 616d 655f 7061  harvest_frame_pa
+000015a0: 636b 6574 7363 0200 0000 0000 0000 0000  cketsc..........
+000015b0: 0000 0700 0000 0600 0000 4300 0000 73e2  ..........C...s.
+000015c0: 0000 0067 007d 027c 006a 0044 005d 677d  ...g.}.|.j.D.]g}
+000015d0: 037c 006a 017c 0319 0064 0117 007d 047c  .|.j.|...d...}.|
+000015e0: 039b 0064 027c 049b 009d 037d 057c 057c  ...d.|.....}.|.|
+000015f0: 006a 02a0 03a1 0076 0172 4874 04a0 0564  .j.....v.rHt...d
+00001600: 037c 059b 009d 02a1 0101 007c 006a 0672  .|.........|.j.r
+00001610: 2d74 07a0 0864 04a1 0101 006e 1474 0974  -t...d.....n.t.t
+00001620: 07a0 07a1 0083 0164 0516 0064 066b 0272  .......d...d.k.r
+00001630: 3c74 04a0 0a64 07a1 0101 0074 07a0 0864  <t...d.....t...d
+00001640: 01a1 0101 007c 057c 006a 02a0 03a1 0076  .....|.|.j.....v
+00001650: 0173 1c7c 006a 027c 0519 006a 0b7d 067c  .s.|.j.|...j.}.|
+00001660: 0664 086b 0272 6374 04a0 0a64 097c 039b  .d.k.rct...d.|..
+00001670: 0064 0a9d 03a1 0101 0064 0b7c 005f 0c7c  .d.......d.|._.|
+00001680: 006a 0da0 0ea1 0001 007c 037c 016b 0372  .j.......|.|.k.r
+00001690: 6c7c 02a0 0f7c 06a1 0101 0071 0574 107c  l|...|.....q.t.|
+000016a0: 0283 0153 0029 0c7a 754c 6f6f 6b73 2061  ...S.).zuLooks a
+000016b0: 7420 6e65 7874 2075 6e61 7373 6967 6e65  t next unassigne
+000016c0: 6420 6672 616d 6520 6163 726f 7373 2074  d frame across t
+000016d0: 6865 2070 6f72 7473 2074 6f20 6465 7465  he ports to dete
+000016e0: 726d 696e 650a 2020 2020 2020 2020 7468  rmine.        th
+000016f0: 6520 6561 726c 6965 7374 2074 696d 6520  e earliest time 
+00001700: 6174 2077 6869 6368 2065 6163 6820 6f66  at which each of
+00001710: 2074 6865 6d20 7761 7320 7265 6164 7258   them was readrX
+00001720: 0000 0072 5700 0000 7a37 5761 6974 696e  ...rW...z7Waitin
+00001730: 6720 696e 2061 206c 6f6f 7020 666f 7220  g in a loop for 
+00001740: 6672 616d 6520 6461 7461 2074 6f20 706f  frame data to po
+00001750: 7075 6c61 7465 2077 6974 6820 6b65 793a  pulate with key:
+00001760: 2067 9a99 9999 9999 b93f e90a 0000 0072   g.......?.....r
+00001770: 0100 0000 7a3e 5379 6e63 6872 6f6e 697a  ....z>Synchroniz
+00001780: 6572 206e 6f74 2073 7562 7363 7269 6265  er not subscribe
+00001790: 6420 746f 2061 6e79 2073 7472 6561 6d73  d to any streams
+000017a0: 2061 6e64 2062 7573 7920 7761 6974 696e   and busy waitin
+000017b0: 672e 2e2e 720b 0000 007a 1645 6e64 206f  g...r....z.End o
+000017c0: 6620 6672 616d 6573 2061 7420 706f 7274  f frames at port
+000017d0: 207a 2120 6465 7465 6374 6564 3b20 656e   z! detected; en
+000017e0: 6469 6e67 2073 796e 6368 726f 6e69 7a61  ding synchroniza
+000017f0: 7469 6f6e 5429 1172 1800 0000 7247 0000  tionT).r....rG..
+00001800: 0072 1500 0000 da04 6b65 7973 7235 0000  .r......keysr5..
+00001810: 0072 5c00 0000 721c 0000 00da 0474 696d  .r\...r......tim
+00001820: 65da 0573 6c65 6570 da03 696e 7472 3600  e..sleep..intr6.
+00001830: 0000 725d 0000 0072 1700 0000 7216 0000  ..r]...r....r...
+00001840: 0072 3e00 0000 721b 0000 00da 036d 696e  .r>...r......min
+00001850: 2907 7224 0000 0072 0f00 0000 5a14 7469  ).r$...r....Z.ti
+00001860: 6d65 735f 6f66 5f6e 6578 745f 6672 616d  mes_of_next_fram
+00001870: 6573 da01 705a 0a6e 6578 745f 696e 6465  es..pZ.next_inde
+00001880: 78da 0e66 7261 6d65 5f64 6174 615f 6b65  x..frame_data_ke
+00001890: 795a 0f6e 6578 745f 6672 616d 655f 7469  yZ.next_frame_ti
+000018a0: 6d65 720c 0000 0072 0c00 0000 7210 0000  mer....r....r...
+000018b0: 00da 1365 6172 6c69 6573 745f 6e65 7874  ...earliest_next
+000018c0: 5f66 7261 6d65 a000 0000 7332 0000 0004  _frame....s2....
+000018d0: 030a 010e 010e 010e 0304 0108 0104 ff06  ................
+000018e0: 030c 0114 030a 010a 010e f60c 0c08 0204  ................
+000018f0: 010a 0104 ff06 040a 0108 020a 0102 8008  ................
+00001900: 027a 2053 796e 6368 726f 6e69 7a65 722e  .z Synchronizer.
+00001910: 6561 726c 6965 7374 5f6e 6578 745f 6672  earliest_next_fr
+00001920: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
+00001930: 0700 0000 0400 0000 4300 0000 734e 0000  ........C...sN..
+00001940: 0067 007d 027c 006a 0044 005d 1d7d 037c  .g.}.|.j.D.].}.|
+00001950: 006a 017c 0319 007d 047c 039b 0064 017c  .j.|...}.|...d.|
+00001960: 049b 009d 037d 057c 006a 027c 0519 006a  .....}.|.j.|...j
+00001970: 037d 067c 037c 016b 0372 227c 02a0 047c  .}.|.|.k.r"|...|
+00001980: 06a1 0101 0071 0574 057c 0283 0153 0029  .....q.t.|...S.)
+00001990: 027a 5750 726f 7669 6465 7320 7468 6520  .zWProvides the 
+000019a0: 6c61 7465 7374 2066 7261 6d65 5f74 696d  latest frame_tim
+000019b0: 6520 6f66 2074 6865 2063 7572 7265 6e74  e of the current
+000019c0: 2066 7261 6d65 7320 6e6f 7420 696e 636c   frames not incl
+000019d0: 7573 6976 6520 6f66 2074 6865 2070 726f  usive of the pro
+000019e0: 7669 6465 6420 706f 7274 7257 0000 0029  vided portrW...)
+000019f0: 0672 1800 0000 7247 0000 0072 1500 0000  .r....rG...r....
+00001a00: 725d 0000 0072 1b00 0000 da03 6d61 7829  r]...r......max)
+00001a10: 0772 2400 0000 720f 0000 005a 1774 696d  .r$...r....Z.tim
+00001a20: 6573 5f6f 665f 6375 7272 656e 745f 6672  es_of_current_fr
+00001a30: 616d 6573 7265 0000 00da 0d63 7572 7265  amesre.....curre
+00001a40: 6e74 5f69 6e64 6578 7266 0000 005a 1263  nt_indexrf...Z.c
+00001a50: 7572 7265 6e74 5f66 7261 6d65 5f74 696d  urrent_frame_tim
+00001a60: 6572 0c00 0000 720c 0000 0072 1000 0000  er....r....r....
+00001a70: da14 6c61 7465 7374 5f63 7572 7265 6e74  ..latest_current
+00001a80: 5f66 7261 6d65 c400 0000 7312 0000 0004  _frame....s.....
+00001a90: 020a 010a 010e 010c 0108 010a 0102 8008  ................
+00001aa0: 027a 2153 796e 6368 726f 6e69 7a65 722e  .z!Synchronizer.
+00001ab0: 6c61 7465 7374 5f63 7572 7265 6e74 5f66  latest_current_f
+00001ac0: 7261 6d65 6301 0000 0000 0000 0000 0000  ramec...........
+00001ad0: 0002 0000 0004 0000 0003 0000 0073 2c00  .............s,.
+00001ae0: 0000 8700 6601 6401 6402 8408 8800 6a00  ....f.d.d.....j.
+00001af0: 4400 8301 7d01 7401 a002 6403 7c01 9b00  D...}.t...d.|...
+00001b00: 9d02 a101 0100 7403 7c01 8301 5300 2904  ......t.|...S.).
+00001b10: 7a42 4465 7465 726d 696e 6520 686f 7720  zBDetermine how 
+00001b20: 6d61 6e79 2075 6e61 7373 6967 6e65 6420  many unassigned 
+00001b30: 6672 616d 6573 2061 7265 2073 6974 7469  frames are sitti
+00001b40: 6e67 2069 6e20 7365 6c66 2e64 6174 6166  ng in self.dataf
+00001b50: 7261 6d65 6301 0000 0000 0000 0000 0000  ramec...........
+00001b60: 0002 0000 0005 0000 0013 0000 0073 2000  .............s .
+00001b70: 0000 6700 7c00 5d0c 7d01 8800 6a00 7c01  ..g.|.].}...j.|.
+00001b80: 1900 8800 6a01 7c01 1900 1800 9102 7102  ....j.|.......q.
+00001b90: 5300 720c 0000 0029 0272 4600 0000 7247  S.r....).rF...rG
+00001ba0: 0000 0072 0d00 0000 7233 0000 0072 0c00  ...r....r3...r..
+00001bb0: 0000 7210 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00001bc0: 6d70 3ed2 0000 0073 0800 0000 0600 0202  mp>....s........
+00001bd0: 12ff 06ff 7a2c 5379 6e63 6872 6f6e 697a  ....z,Synchroniz
+00001be0: 6572 2e66 7261 6d65 5f73 6c61 636b 2e3c  er.frame_slack.<
+00001bf0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001c00: 703e 7a13 536c 6163 6b20 696e 2066 7261  p>z.Slack in fra
+00001c10: 6d65 7320 6973 2029 0472 1800 0000 7235  mes is ).r....r5
+00001c20: 0000 0072 5c00 0000 7264 0000 0029 0272  ...r\...rd...).r
+00001c30: 2400 0000 5a05 736c 6163 6b72 0c00 0000  $...Z.slackr....
+00001c40: 7233 0000 0072 1000 0000 da0b 6672 616d  r3...r......fram
+00001c50: 655f 736c 6163 6bd0 0000 0073 0a00 0000  e_slack....s....
+00001c60: 0a02 0402 06fe 1004 0801 7a18 5379 6e63  ..........z.Sync
+00001c70: 6872 6f6e 697a 6572 2e66 7261 6d65 5f73  hronizer.frame_s
+00001c80: 6c61 636b 6301 0000 0000 0000 0000 0000  lackc...........
+00001c90: 0003 0000 0003 0000 0043 0000 0073 3c00  .........C...s<.
+00001ca0: 0000 7400 7c00 6a01 8301 6401 6b04 720f  ..t.|.j...d.k.r.
+00001cb0: 7c00 6a01 6402 6400 8502 1900 7c00 5f01  |.j.d.d.....|._.
+00001cc0: 7402 a003 7c00 6a01 a101 7d01 7402 a004  t...|.j...}.t...
+00001cd0: 7c01 a101 7d02 6403 7c02 1b00 5300 2904  |...}.d.|...S.).
+00001ce0: 4e72 5f00 0000 69f6 ffff ff72 5800 0000  Nr_...i....rX...
+00001cf0: 2905 da03 6c65 6e72 4800 0000 7231 0000  )...lenrH...r1..
+00001d00: 00da 0464 6966 6672 3200 0000 2903 7224  ...diffr2...).r$
+00001d10: 0000 005a 0764 656c 7461 5f74 5a0c 6d65  ...Z.delta_tZ.me
+00001d20: 616e 5f64 656c 7461 5f74 720c 0000 0072  an_delta_tr....r
+00001d30: 0c00 0000 7210 0000 00da 0b61 7665 7261  ....r......avera
+00001d40: 6765 5f66 7073 d900 0000 730a 0000 000e  ge_fps....s.....
+00001d50: 0110 010c 020a 0108 027a 1853 796e 6368  .........z.Synch
+00001d60: 726f 6e69 7a65 722e 6176 6572 6167 655f  ronizer.average_
+00001d70: 6670 7363 0100 0000 0000 0000 0000 0000  fpsc............
+00001d80: 0c00 0000 0900 0000 4300 0000 7394 0200  ........C...s...
+00001d90: 0074 00a0 0164 01a1 0101 0064 027d 0174  .t...d.....d.}.t
+00001da0: 00a0 0164 03a1 0101 007c 006a 02a0 03a1  ...d.....|.j....
+00001db0: 0090 0173 4369 007d 0267 007d 0369 007d  ...sCi.}.g.}.i.}
+00001dc0: 0469 007d 057c 006a 0444 005d 157d 067c  .i.}.|.j.D.].}.|
+00001dd0: 00a0 057c 06a1 017c 047c 063c 007c 00a0  ...|...|.|.<.|..
+00001de0: 067c 06a1 017c 057c 063c 007c 006a 077c  .|...|.|.<.|.j.|
+00001df0: 0619 007d 0771 1d7c 006a 0444 005d 687d  ...}.q.|.j.D.]h}
+00001e00: 067c 006a 077c 0619 007d 077c 069b 0064  .|.j.|...}.|...d
+00001e10: 047c 079b 009d 037d 087c 006a 087c 0819  .|.....}.|.j.|..
+00001e20: 007d 097c 096a 097d 0a7c 0a7c 047c 0619  .}.|.j.}.|.|.|..
+00001e30: 006b 0472 6064 007c 027c 063c 0074 00a0  .k.r`d.|.|.<.t..
+00001e40: 0a64 057c 069b 0064 069d 03a1 0101 0071  .d.|...d.......q
+00001e50: 367c 047c 0619 007c 0a18 007c 0a7c 057c  6|.|...|...|.|.|
+00001e60: 0619 0018 006b 0072 7a64 007c 027c 063c  .....k.rzd.|.|.<
+00001e70: 0074 00a0 0a64 057c 069b 0064 079d 03a1  .t...d.|...d....
+00001e80: 0101 0071 367c 006a 08a0 0b7c 08a1 017c  ...q6|.j...|...|
+00001e90: 027c 063c 007c 006a 077c 0605 0019 0064  .|.<.|.j.|.....d
+00001ea0: 0837 0003 003c 007c 03a0 0c7c 0aa1 0101  .7...<.|...|....
+00001eb0: 0074 00a0 0d64 097c 069b 0064 0a7c 079b  .t...d.|...d.|..
+00001ec0: 0064 0b7c 0a9b 009d 06a1 0101 0071 3674  .d.|.........q6t
+00001ed0: 00a0 0d64 0c74 0e7c 006a 0883 019b 009d  ...d.t.|.j......
+00001ee0: 02a1 0101 007c 006a 0fa0 0c74 10a0 117c  .....|.j...t...|
+00001ef0: 03a1 01a1 0101 0074 127c 017c 0283 027c  .......t.|.|...|
+00001f00: 005f 137c 00a0 14a1 0001 007c 0164 0837  ._.|.......|.d.7
+00001f10: 007d 017c 006a 02a0 03a1 0072 ce74 00a0  .}.|.j.....r.t..
+00001f20: 0164 0da1 0101 0064 007c 005f 137c 006a  .d.....d.|._.|.j
+00001f30: 1544 005d 0f7d 0b74 00a0 0164 0e7c 019b  .D.].}.t...d.|..
+00001f40: 009d 02a1 0101 007c 0ba0 1664 0fa1 0101  .......|...d....
+00001f50: 0071 d17c 006a 1744 005d 547d 0b7c 0ba0  .q.|.j.D.]T}.|..
+00001f60: 167c 006a 13a1 0101 007c 006a 1364 0075  .|.j.....|.j.d.u
+00001f70: 0190 0172 1b74 00a0 0d64 107c 006a 136a  ...r.t...d.|.j.j
+00001f80: 189b 0064 119d 03a1 0101 0074 00a0 0d64  ...d.......t...d
+00001f90: 127c 006a 136a 199b 009d 02a1 0101 007c  .|.j.j.........|
+00001fa0: 006a 136a 1964 1316 0064 026b 0290 0172  .j.j.d...d.k...r
+00001fb0: 1a74 00a0 0164 127c 006a 136a 199b 009d  .t...d.|.j.j....
+00001fc0: 02a1 0101 0071 e474 00a0 0164 14a1 0101  .....q.t...d....
+00001fd0: 007c 006a 1aa0 1ba1 0044 005d 125c 027d  .|.j.....D.].\.}
+00001fe0: 067d 0b74 00a0 0164 157c 0ba0 1ca1 009b  .}.t...d.|......
+00001ff0: 0064 167c 069b 009d 04a1 0101 0090 0171  .d.|...........q
+00002000: 2571 e47c 00a0 1da1 007c 005f 1e7c 006a  %q.|.....|._.|.j
+00002010: 02a0 03a1 0072 1274 00a0 0164 17a1 0101  .....r.t...d....
+00002020: 0064 0053 0029 184e 7a34 5761 6974 696e  .d.S.).Nz4Waitin
+00002030: 6720 666f 7220 616c 6c20 706f 7274 7320  g for all ports 
+00002040: 746f 2062 6567 696e 2068 6172 7665 7374  to begin harvest
+00002050: 696e 6720 636f 726e 6572 732e 2e2e 7201  ing corners...r.
+00002060: 0000 007a 2641 626f 7574 2074 6f20 7374  ...z&About to st
+00002070: 6172 7420 7379 6e63 6872 6f6e 697a 696e  art synchronizin
+00002080: 6720 6672 616d 6573 2e2e 2e72 5700 0000  g frames...rW...
+00002090: 7a16 536b 6970 7065 6420 6672 616d 6520  z.Skipped frame 
+000020a0: 6174 2070 6f72 7420 7a11 3a20 3e20 6561  at port z.: > ea
+000020b0: 726c 6965 7374 5f6e 6578 747a 1d3a 2064  rliest_nextz.: d
+000020c0: 656c 7461 203c 2074 696d 652d 6c61 7465  elta < time-late
+000020d0: 7374 5f63 7572 7265 6e74 7258 0000 007a  st_currentrX...z
+000020e0: 1a41 6464 696e 6720 746f 206c 6179 6572  .Adding to layer
+000020f0: 2066 726f 6d20 706f 7274 207a 0a20 6174   from port z. at
+00002100: 2069 6e64 6578 207a 1120 616e 6420 6672   index z. and fr
+00002110: 616d 6520 7469 6d65 3a20 7a13 556e 6173  ame time: z.Unas
+00002120: 7369 676e 6564 2046 7261 6d65 733a 207a  signed Frames: z
+00002130: 3753 656e 6469 6e67 2060 4e6f 6e65 6020  7Sending `None` 
+00002140: 6f6e 2071 7565 7565 2074 6f20 7369 676e  on queue to sign
+00002150: 616c 2065 6e64 206f 6620 7379 6e63 6564  al end of synced
+00002160: 2066 7261 6d65 732e 7a42 4769 7669 6e67   frames.zBGiving
+00002170: 206e 6f74 6963 6520 6f66 206e 6577 2073   notice of new s
+00002180: 796e 6368 6564 2066 7261 6d65 7320 7061  ynched frames pa
+00002190: 636b 6574 2076 6961 2071 7565 7565 3b20  cket via queue; 
+000021a0: 7379 6e63 2069 6e64 6578 3a20 7a1c 6e65  sync index: z.ne
+000021b0: 7720 7379 6e63 6865 6420 6672 616d 6573  w synched frames
+000021c0: 2061 7661 696c 6162 6c65 7a30 506c 6163   availablez0Plac
+000021d0: 696e 6720 6e65 7720 7379 6e63 6865 6420  ing new synched 
+000021e0: 6672 616d 6573 2070 6163 6b65 7420 6f6e  frames packet on
+000021f0: 2071 7565 7565 2077 6974 6820 7a07 2066   queue with z. f
+00002200: 7261 6d65 737a 2650 6c61 6369 6e67 206e  ramesz&Placing n
+00002210: 6577 2073 796e 6368 6564 2066 7261 6d65  ew synched frame
+00002220: 7320 7769 7468 2069 6e64 6578 2072 0700  s with index r..
+00002230: 0000 7a3f 7369 676e 616c 696e 6720 656e  ..z?signaling en
+00002240: 6420 6f66 2066 7261 6d65 7320 7769 7468  d of frames with
+00002250: 2060 4e6f 6e65 6020 7061 636b 6574 206f   `None` packet o
+00002260: 6e20 7375 6273 6372 6962 6572 2071 7565  n subscriber que
+00002270: 7565 2e7a 0a43 7572 7265 6e74 6c79 207a  ue.z.Currently z
+00002280: 2420 6672 616d 6520 7061 636b 6574 7320  $ frame packets 
+00002290: 756e 7072 6f63 6573 7365 6420 666f 7220  unprocessed for 
+000022a0: 706f 7274 207a 2546 7261 6d65 2073 796e  port z%Frame syn
+000022b0: 6368 2077 6f72 6b65 7220 7375 6363 6573  ch worker succes
+000022c0: 7366 756c 6c79 2065 6e64 6564 291f 7235  sfully ended).r5
+000022d0: 0000 0072 3600 0000 7216 0000 0072 5900  ...r6...r....rY.
+000022e0: 0000 7218 0000 0072 6700 0000 726a 0000  ..r....rg...rj..
+000022f0: 0072 4700 0000 7215 0000 0072 5d00 0000  .rG...r....r]...
+00002300: da07 7761 726e 696e 67da 0370 6f70 721b  ..warning..popr.
+00002310: 0000 0072 5c00 0000 726d 0000 0072 4800  ...r\...rm...rH.
+00002320: 0000 7231 0000 0072 3200 0000 7206 0000  ..r1...r2...r...
+00002330: 0072 2d00 0000 7230 0000 0072 1300 0000  .r-...r0...r....
+00002340: da03 7075 7472 1400 0000 da12 6672 616d  ..putr......fram
+00002350: 655f 7061 636b 6574 5f63 6f75 6e74 da0a  e_packet_count..
+00002360: 7379 6e63 5f69 6e64 6578 7219 0000 0072  sync_indexr....r
+00002370: 1a00 0000 da05 7173 697a 6572 6f00 0000  ......qsizero...
+00002380: 721f 0000 0029 0c72 2400 0000 7274 0000  r....).r$...rt..
+00002390: 005a 1563 7572 7265 6e74 5f66 7261 6d65  .Z.current_frame
+000023a0: 5f70 6163 6b65 7473 5a11 6c61 7965 725f  _packetsZ.layer_
+000023b0: 6672 616d 655f 7469 6d65 735a 0d65 6172  frame_timesZ.ear
+000023c0: 6c69 6573 745f 6e65 7874 5a0e 6c61 7465  liest_nextZ.late
+000023d0: 7374 5f63 7572 7265 6e74 720f 0000 005a  st_currentr....Z
+000023e0: 1363 7572 7265 6e74 5f66 7261 6d65 5f69  .current_frame_i
+000023f0: 6e64 6578 5a0e 706f 7274 5f69 6e64 6578  ndexZ.port_index
+00002400: 5f6b 6579 5a14 6375 7272 656e 745f 6672  _keyZ.current_fr
+00002410: 616d 655f 7061 636b 6574 725d 0000 0072  ame_packetr]...r
+00002420: 2700 0000 720c 0000 0072 0c00 0000 7210  '...r....r....r.
+00002430: 0000 0072 4d00 0000 e200 0000 7378 0000  ...rM.......sx..
+00002440: 000a 0204 020a 020c 0104 0204 0204 0404  ................
+00002450: 010a 020e 010e 010c 010a 020a 010e 020a  ................
+00002460: 0106 010c 0308 0214 0116 0202 ff08 0504  ................
+00002470: 010a 0106 ff06 0502 0108 ff12 040a 0104  ................
+00002480: 0114 0106 ff16 0412 020c 0208 0208 020a  ................
+00002490: 020a 0106 010a 0410 010c 010a 020c 010c  ................
+000024a0: 0116 0114 0112 0314 0102 800a 0212 011e  ................
+000024b0: 0102 ff0a 030a ad0e 557a 2053 796e 6368  ........Uz Synch
+000024c0: 726f 6e69 7a65 722e 7379 6e63 685f 6672  ronizer.synch_fr
+000024d0: 616d 6573 5f77 6f72 6b65 724e 2901 7209  ames_workerN).r.
+000024e0: 0000 0029 1ada 085f 5f6e 616d 655f 5fda  ...)...__name__.
+000024f0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00002500: 7561 6c6e 616d 655f 5fda 0464 6963 7472  ualname__..dictr
+00002510: 2800 0000 da04 626f 6f6c 722c 0000 0072  (.....boolr,...r
+00002520: 3000 0000 da08 7072 6f70 6572 7479 7234  0.....propertyr4
+00002530: 0000 0072 1e00 0000 721d 0000 0072 3d00  ...r....r....r=.
+00002540: 0000 7243 0000 0072 2200 0000 7223 0000  ..rC...r"...r#..
+00002550: 0072 5000 0000 7253 0000 0072 5400 0000  .rP...rS...rT...
+00002560: 7256 0000 0072 4c00 0000 7267 0000 0072  rV...rL...rg...r
+00002570: 6a00 0000 726c 0000 0072 6f00 0000 724d  j...rl...ro...rM
+00002580: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
+00002590: 0000 7210 0000 0072 0800 0000 1300 0000  ..r....r........
+000025a0: 732c 0000 0008 0010 010e 2208 0402 070a  s,........".....
+000025b0: 0108 0708 0608 0608 0608 0608 0608 0e08  ................
+000025c0: 0708 0808 0408 0408 1408 2408 0c08 090c  ..........$.....
+000025d0: 0972 0800 0000 2915 da0d 7079 7879 3364  .r....)...pyxy3d
+000025e0: 2e6c 6f67 6765 72da 0670 7978 7933 6472  .logger..pyxy3dr
+000025f0: 3500 0000 725a 0000 0072 7600 0000 da07  5...rZ...rv.....
+00002600: 6c6f 6767 696e 6772 6100 0000 da07 7061  loggingra.....pa
+00002610: 7468 6c69 6272 0200 0000 da05 7175 6575  thlibr......queu
+00002620: 6572 0300 0000 da09 7468 7265 6164 696e  er......threadin
+00002630: 6772 0400 0000 7205 0000 00da 0363 7632  gr....r......cv2
+00002640: da05 6e75 6d70 7972 3100 0000 da10 7079  ..numpyr1.....py
+00002650: 7879 3364 2e69 6e74 6572 6661 6365 7206  xy3d.interfacer.
+00002660: 0000 0072 2f00 0000 7208 0000 0072 0c00  ...r/...r....r..
+00002670: 0000 720c 0000 0072 0c00 0000 7210 0000  ..r....r....r...
+00002680: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00002690: 1800 0000 0800 0c02 0801 0804 0c01 0c01  ................
+000026a0: 1001 0802 0801 0c01 0402 1202            ............
```

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/camera.py` & `pyxy3d-0.0.22/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.0.22/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.0.22/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.0.22/pyxy3d/cameras/live_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.0.22/pyxy3d/cameras/synchronizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self.fps_target = fps_target
         logger.info(f"Attempting to change target fps in streams to {fps_target}")
         for port, stream in self.streams.items():
             stream.set_fps_target(fps_target)
 
     def subscribe_to_streams(self):
         for port, stream in self.streams.items():
+            logger.info(f"Subscribing synchronizer to stream from port {port}")
             stream.subscribe(self.frame_packet_queues[port])
         self.subscribed_to_streams = True
 
     def unsubscribe_from_streams(self):
         for port, stream in self.streams.items():
             logger.info(f"unsubscribe synchronizer from port {port}")
             stream.unsubscribe(self.frame_packet_queues[port])
@@ -291,15 +292,15 @@
             if self.stop_event.is_set():
                 logger.info("Sending `None` on queue to signal end of synced frames.")
                 self.current_sync_packet = None
 
             # notify other processes that the new frames are ready for processing
             # only for tasks that can risk missing frames (i.e. only for gui purposes)
             for q in self.sync_notice_subscribers:
-                logger.debug(f"Giving notice of new synched frames packet via queue")
+                logger.debug(f"Giving notice of new synched frames packet via queue; sync index: {sync_index}")
                 q.put("new synched frames available")
 
             for q in self.synched_frames_subscribers:
                 q.put(self.current_sync_packet)
                 if self.current_sync_packet is not None:
                     logger.debug(f"Placing new synched frames packet on queue with {self.current_sync_packet.frame_packet_count} frames")
                     logger.debug(f"Placing new synched frames with index {self.current_sync_packet.sync_index}")
@@ -312,71 +313,7 @@
                     for port, q in self.frame_packet_queues.items():
                         logger.info(f"Currently {q.qsize()} frame packets unprocessed for port {port}")
                     
             self.fps_mean = self.average_fps()
 
         logger.info("Frame synch worker successfully ended")
 
-
-if __name__ == "__main__":
-    from pyxy3d.calibration.charuco import Charuco
-    from pyxy3d.trackers.charuco_tracker import CharucoTracker
-    from pyxy3d.recording.recorded_stream import RecordedStream, RecordedStreamPool
-
-    from pyxy3d.session.session import Session
-    import time
-
-    from pyxy3d import __root__
-    
-
-    # test_live = True
-    test_live = False
-
-    if test_live:
-
-        session_directory = Path(__root__, "tests", "217")
-        # config = Path(session_directory, "config.toml")
-        session = Session(session_directory)
-        # session.load_cameras()
-        session.load_stream_tools()
-        # session.adjust_resolutions()
-
-        for port, stream in session.streams.items():
-            stream._show_fps = True
-            stream._show_charuco = True
-
-        logger.info("Creating Synchronizer")
-        syncr = Synchronizer(session.streams, fps_target=5)
-    else:
-        ports = [0, 1, 2, 3, 4]
-        # ports = [0,1]
-        recording_directory = Path(__root__, "tests","sessions", "217")
-        tracker = Charuco(
-                4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
-            )
-        recorded_stream_pool = RecordedStreamPool(
-            ports, recording_directory, charuco=tracker
-        )
-        logger.info("Creating Synchronizer")
-        syncr = Synchronizer(recorded_stream_pool.streams, fps_target=20)
-        recorded_stream_pool.play_videos()
-
-    notification_q = Queue()
-
-    syncr.subscribe_to_notice(notification_q)
-    logger.info(f"Beginning playback at {time.perf_counter()}")
-
-    while not syncr.stop_event.is_set():
-        synched_frames_notice = notification_q.get()
-        sync_packet = syncr.current_sync_packet
-        for port, frame_packet in sync_packet.frame_packets.items():
-
-            if frame_packet:
-                cv2.imshow(f"Port {port}", frame_packet.frame)
-
-        key = cv2.waitKey(1)
-
-        if key == ord("q"):
-            cv2.destroyAllWindows()
-            break
-
-    logger.info(f"Playback finished at {time.perf_counter()}")
```

### Comparing `pyxy3d-0.0.21/pyxy3d/configurator.py` & `pyxy3d-0.0.22/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/export.py` & `pyxy3d-0.0.22/pyxy3d/export.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 17:07:44 2023 UTC, .py size: 7438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e050 8764 0e1d 0000  o........P.d....
+00000000: 6f0d 0d0a 0000 0000 8150 8b64 231d 0000  o........P.d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6401 6c07 5a07 6400 6401 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 5a08 6400 6402 6c09 6d0a 5a0a 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6403 6c0b 6d0c 5a0c 0100 6400 6404 6c0d  d.l.m.Z...d.d.l.
@@ -197,160 +197,160 @@
 00000c40: 7265 6e74 2077 6964 6765 7420 746f 2063  rent widget to c
 00000c50: 6f6e 6669 6720 7465 6d70 6f72 6172 696c  onfig temporaril
 00000c60: 79fa 1252 656d 6f76 6520 7374 6572 656f  y..Remove stereo
 00000c70: 6672 616d 65fa 1643 7265 6174 6520 6e65  frame..Create ne
 00000c80: 7720 7374 6572 656f 6672 616d 6529 0972  w stereoframe).r
 00000c90: 2200 0000 7223 0000 0072 2c00 0000 7235  "...r#...r,...r5
 00000ca0: 0000 00da 0c72 656d 6f76 6557 6964 6765  .....removeWidge
-00000cb0: 7472 3800 0000 da0d 6672 616d 655f 6275  tr8.....frame_bu
-00000cc0: 696c 6465 72da 1d75 6e73 7562 7363 7269  ilder..unsubscri
-00000cd0: 6265 5f66 726f 6d5f 7379 6e63 6872 6f6e  be_from_synchron
-00000ce0: 697a 6572 da16 6c61 756e 6368 5f6e 6577  izer..launch_new
-00000cf0: 5f73 7465 7265 6f66 7261 6d65 7234 0000  _stereoframer4..
-00000d00: 0072 3100 0000 7231 0000 0072 3200 0000  .r1...r1...r2...
-00000d10: 723d 0000 0077 0000 0073 1000 0000 0a01  r=...w...s......
-00000d20: 0c01 0a02 0c01 0c01 0401 0a02 0c01 7a25  ..............z%
-00000d30: 4361 6c69 6272 6174 696f 6e57 6964 6765  CalibrationWidge
-00000d40: 742e 7265 6672 6573 685f 7374 6572 656f  t.refresh_stereo
-00000d50: 6672 616d 6563 0100 0000 0000 0000 0000  framec..........
-00000d60: 0000 0200 0000 0300 0000 4300 0000 735a  ..........C...sZ
-00000d70: 0000 0074 00a0 0164 01a1 0101 007c 00a0  ...t...d.....|..
-00000d80: 027c 006a 03a1 0101 007c 006a 04a0 05a1  .|.j.....|.j....
-00000d90: 0001 007c 006a 066a 07a0 08a1 0001 007c  ...|.j.j.......|
-00000da0: 00a0 097c 006a 06a1 0101 007c 0060 067c  ...|.j.....|.`.|
-00000db0: 006a 036a 0aa0 0ba1 007d 017c 006a 036a  .j.j.....}.|.j.j
-00000dc0: 0aa0 0c7c 01a1 0101 0064 0053 0029 024e  ...|.....d.S.).N
-00000dd0: 7a2d 4d6f 7669 6e67 2062 6163 6b20 746f  z-Moving back to
-00000de0: 2063 616d 6572 6120 636f 6e66 6967 2066   camera config f
-00000df0: 726f 6d20 7374 6572 656f 6672 616d 6529  rom stereoframe)
-00000e00: 0d72 2200 0000 7223 0000 0072 2c00 0000  .r"...r#...r,...
-00000e10: 7235 0000 0072 1b00 0000 5a12 7061 7573  r5...r....Z.paus
-00000e20: 655f 7379 6e63 6872 6f6e 697a 6572 7238  e_synchronizerr8
-00000e30: 0000 0072 4300 0000 7244 0000 0072 4200  ...rC...rD...rB.
-00000e40: 0000 5a0b 6361 6d65 7261 5f74 6162 735a  ..Z.camera_tabsZ
-00000e50: 0c63 7572 7265 6e74 496e 6465 785a 1461  .currentIndexZ.a
-00000e60: 6374 6976 6174 655f 6375 7272 656e 745f  ctivate_current_
-00000e70: 7461 6229 0272 2e00 0000 5a0b 6163 7469  tab).r....Z.acti
-00000e80: 7665 5f70 6f72 7472 3100 0000 7231 0000  ve_portr1...r1..
-00000e90: 0072 3200 0000 723b 0000 0084 0000 0073  .r2...r;.......s
-00000ea0: 1000 0000 0a01 0c01 0a01 0c02 0c01 0401  ................
-00000eb0: 0c02 1201 7a2e 4361 6c69 6272 6174 696f  ....z.Calibratio
-00000ec0: 6e57 6964 6765 742e 6261 636b 5f74 6f5f  nWidget.back_to_
-00000ed0: 6361 6d65 7261 5f63 6f6e 6669 675f 7769  camera_config_wi
-00000ee0: 7a61 7264 6301 0000 0000 0000 0000 0000  zardc...........
-00000ef0: 0001 0000 0003 0000 0043 0000 0073 5e00  .........C...s^.
-00000f00: 0000 7400 a001 6401 a101 0100 7402 7c00  ..t...d.....t.|.
-00000f10: 6a03 8301 7c00 5f04 7400 a001 6402 a101  j...|._.t...d...
-00000f20: 0100 7c00 a005 7c00 6a04 a101 0100 7400  ..|...|.j.....t.
-00000f30: a001 6403 a101 0100 7c00 a006 7c00 6a04  ..d.....|...|.j.
-00000f40: a101 0100 7c00 6a04 6a07 6a08 6a09 a00a  ....|.j.j.j.j...
-00000f50: 7c00 6a0b a101 0100 7c00 600c 6400 5300  |.j.....|.`.d.S.
-00000f60: 2904 4e7a 1e43 7265 6174 696e 6720 4361  ).Nz.Creating Ca
-00000f70: 7074 7572 6520 566f 6c75 6d65 2077 6964  pture Volume wid
-00000f80: 6765 747a 2b41 6464 696e 6720 6361 7074  getz+Adding capt
-00000f90: 7572 6520 766f 6c75 6d65 2077 6964 6765  ure volume widge
-00000fa0: 7420 746f 206d 6169 6e20 5769 7a61 7264  t to main Wizard
-00000fb0: 7a2a 5365 7420 6375 7272 656e 7420 696e  z*Set current in
-00000fc0: 6465 7820 746f 2063 6170 7475 7265 2076  dex to capture v
-00000fd0: 6f6c 756d 6520 7769 6467 6574 290d 7222  olume widget).r"
-00000fe0: 0000 0072 2300 0000 7218 0000 0072 1b00  ...r#...r....r..
-00000ff0: 0000 da0e 6361 7074 7572 655f 766f 6c75  ....capture_volu
-00001000: 6d65 722b 0000 0072 2c00 0000 7225 0000  mer+...r,...r%..
-00001010: 0072 3a00 0000 7226 0000 0072 2700 0000  .r:...r&...r'...
-00001020: da14 6261 636b 5f74 6f5f 7374 6572 656f  ..back_to_stereo
-00001030: 5f66 7261 6d65 5a09 7174 5f6c 6f67 6765  _frameZ.qt_logge
-00001040: 7272 3400 0000 7231 0000 0072 3100 0000  rr4...r1...r1...
-00001050: 7232 0000 0072 3c00 0000 9000 0000 7314  r2...r<.......s.
-00001060: 0000 000a 010c 010a 010c 010a 010c 010c  ................
-00001070: 0104 0104 ff08 047a 2843 616c 6962 7261  .......z(Calibra
-00001080: 7469 6f6e 5769 6467 6574 2e6e 6578 745f  tionWidget.next_
-00001090: 746f 5f63 6170 7475 7265 5f76 6f6c 756d  to_capture_volum
-000010a0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-000010b0: 0000 0300 0000 4300 0000 7376 0000 0074  ......C...sv...t
-000010c0: 00a0 0164 01a1 0101 007c 00a0 027c 006a  ...d.....|...|.j
-000010d0: 03a1 0101 0074 00a0 0164 02a1 0101 007c  .....t...d.....|
-000010e0: 00a0 047c 006a 05a1 0101 0074 00a0 0164  ...|.j.....t...d
-000010f0: 03a1 0101 007c 00a0 047c 006a 06a1 0101  .....|...|.j....
-00001100: 007c 0060 067c 006a 056a 07a0 08a1 0001  .|.`.|.j.j......
-00001110: 007c 0060 0574 00a0 0164 04a1 0101 007c  .|.`.t...d.....|
-00001120: 00a0 09a1 0001 007c 006a 0aa0 0ba1 0001  .......|.j......
-00001130: 0064 0053 0029 054e 723f 0000 0072 4000  .d.S.).Nr?...r@.
-00001140: 0000 7a15 5265 6d6f 7665 2063 6170 7475  ..z.Remove captu
-00001150: 7265 2076 6f6c 756d 6572 4100 0000 290c  re volumerA...).
-00001160: 7222 0000 0072 2300 0000 722c 0000 0072  r"...r#...r,...r
-00001170: 3500 0000 7242 0000 0072 3800 0000 7246  5...rB...r8...rF
-00001180: 0000 0072 4300 0000 7244 0000 0072 4500  ...rC...rD...rE.
-00001190: 0000 721b 0000 005a 1475 6e70 6175 7365  ..r....Z.unpause
-000011a0: 5f73 796e 6368 726f 6e69 7a65 7272 3400  _synchronizerr4.
-000011b0: 0000 7231 0000 0072 3100 0000 7232 0000  ..r1...r1...r2..
-000011c0: 0072 4700 0000 9e00 0000 7318 0000 000a  .rG.......s.....
-000011d0: 010c 010a 020c 010a 010c 0104 010c 0104  ................
-000011e0: 010a 0208 010e 017a 2643 616c 6962 7261  .......z&Calibra
-000011f0: 7469 6f6e 5769 6467 6574 2e62 6163 6b5f  tionWidget.back_
-00001200: 746f 5f73 7465 7265 6f5f 6672 616d 6529  to_stereo_frame)
-00001210: 10da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001220: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001230: 616d 655f 5f72 0500 0000 5a11 6361 6d65  ame__r....Z.came
-00001240: 7261 735f 636f 6e6e 6563 7465 6472 0f00  ras_connectedr..
-00001250: 0000 721d 0000 0072 2d00 0000 7228 0000  ..r....r-...r(..
-00001260: 0072 3700 0000 723e 0000 0072 3d00 0000  .r7...r>...r=...
-00001270: 723b 0000 0072 3c00 0000 7247 0000 00da  r;...r<...rG....
-00001280: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7231  .__classcell__r1
-00001290: 0000 0072 3100 0000 722f 0000 0072 3200  ...r1...r/...r2.
-000012a0: 0000 721a 0000 0025 0000 0073 1600 0000  ..r....%...s....
-000012b0: 0800 0601 1202 081a 0807 0815 0804 0815  ................
-000012c0: 080d 080c 100e 721a 0000 0072 2000 0000  ......r....r ...
-000012d0: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-000012e0: 0003 0000 0043 0000 0073 4200 0000 7400  .....C...sB...t.
-000012f0: 7c00 8301 7d01 7401 7c01 8301 7d02 7c02  |...}.t.|...}.|.
-00001300: a002 7403 6a04 a101 0100 7405 7406 6a07  ..t.j.....t.t.j.
-00001310: 8301 7d03 7408 7c02 8301 7d04 7c04 a009  ..}.t.|...}.|...
-00001320: a100 0100 7c03 a00a a100 0100 6400 5300  ....|.......d.S.
-00001330: 7233 0000 0029 0b72 1900 0000 720f 0000  r3...).r....r...
-00001340: 0072 2900 0000 7210 0000 0072 3900 0000  .r)...r....r9...
-00001350: 7209 0000 00da 0373 7973 da04 6172 6776  r......sys..argv
-00001360: 721a 0000 005a 0473 686f 77da 0465 7865  r....Z.show..exe
-00001370: 6329 0572 2000 0000 7221 0000 0072 1b00  c).r ...r!...r..
-00001380: 0000 5a03 6170 705a 0677 696e 646f 7772  ..Z.appZ.windowr
-00001390: 3100 0000 7231 0000 0072 3200 0000 da23  1...r1...r2....#
-000013a0: 6c61 756e 6368 5f65 7874 7269 6e73 6963  launch_extrinsic
-000013b0: 5f63 616c 6962 7261 7469 6f6e 5f77 6964  _calibration_wid
-000013c0: 6765 74af 0000 0073 0e00 0000 0801 0801  get....s........
-000013d0: 0c01 0a02 0801 0801 0c01 724f 0000 0029  ..........rO...)
-000013e0: 2fda 0d70 7978 7933 642e 6c6f 6767 6572  /..pyxy3d.logger
-000013f0: da06 7079 7879 3364 7222 0000 00da 0367  ..pyxy3dr".....g
-00001400: 6574 7248 0000 00da 026f 7372 4c00 0000  etrH.....osrL...
-00001410: 5a06 7368 7574 696c da04 7469 6d65 da07  Z.shutil..time..
-00001420: 7061 7468 6c69 6272 0200 0000 da09 7468  pathlibr......th
-00001430: 7265 6164 696e 6772 0300 0000 5a0c 5079  readingr....Z.Py
-00001440: 5174 362e 5174 436f 7265 7204 0000 0072  Qt6.QtCorer....r
-00001450: 0500 0000 5a0b 5079 5174 362e 5174 4775  ....Z.PyQt6.QtGu
-00001460: 6972 0600 0000 7207 0000 00da 0f50 7951  ir....r......PyQ
-00001470: 7436 2e51 7457 6964 6765 7473 7208 0000  t6.QtWidgetsr...
-00001480: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00001490: 720c 0000 0072 0d00 0000 720e 0000 005a  r....r....r....Z
-000014a0: 1670 7978 7933 642e 7365 7373 696f 6e2e  .pyxy3d.session.
-000014b0: 7365 7373 696f 6e72 0f00 0000 7210 0000  sessionr....r...
-000014c0: 005a 1970 7978 7933 642e 6775 692e 6368  .Z.pyxy3d.gui.ch
-000014d0: 6172 7563 6f5f 7769 6467 6574 7211 0000  aruco_widgetr...
-000014e0: 005a 3570 7978 7933 642e 6775 692e 6361  .Z5pyxy3d.gui.ca
-000014f0: 6d65 7261 5f63 6f6e 6669 672e 696e 7472  mera_config.intr
-00001500: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
-00001510: 6e5f 7769 6467 6574 7212 0000 0072 1300  n_widgetr....r..
-00001520: 0000 7214 0000 005a 1f70 7978 7933 642e  ..r....Z.pyxy3d.
-00001530: 7472 6163 6b65 7273 2e63 6861 7275 636f  trackers.charuco
-00001540: 5f74 7261 636b 6572 7215 0000 005a 2770  _trackerr....Z'p
-00001550: 7978 7933 642e 6775 692e 6578 7472 696e  yxy3d.gui.extrin
-00001560: 7369 635f 6361 6c69 6272 6174 696f 6e5f  sic_calibration_
-00001570: 7769 6467 6574 7216 0000 0072 1700 0000  widgetr....r....
-00001580: 5a36 7079 7879 3364 2e67 7569 2e76 697a  Z6pyxy3d.gui.viz
-00001590: 7561 6c69 7a65 2e63 616c 6962 7261 7469  ualize.calibrati
-000015a0: 6f6e 2e63 6170 7475 7265 5f76 6f6c 756d  on.capture_volum
-000015b0: 655f 7769 6467 6574 7218 0000 005a 1370  e_widgetr....Z.p
-000015c0: 7978 7933 642e 636f 6e66 6967 7572 6174  yxy3d.configurat
-000015d0: 6f72 7219 0000 0072 1a00 0000 724f 0000  orr....r....rO..
-000015e0: 0072 3100 0000 7231 0000 0072 3100 0000  .r1...r1...r1...
-000015f0: 7232 0000 00da 083c 6d6f 6475 6c65 3e01  r2.....<module>.
-00001600: 0000 0073 2c00 0000 0800 0c02 0802 0801  ...s,...........
-00001610: 0801 0801 0c01 0c01 1001 1001 2401 100a  ............$...
-00001620: 0c01 0c01 1001 0c01 1002 0c04 0c01 1003  ................
-00001630: 007f 120b                                ....
+00000cb0: 7472 3800 0000 da14 7061 6972 6564 5f66  tr8.....paired_f
+00000cc0: 7261 6d65 5f62 7569 6c64 6572 da1d 756e  rame_builder..un
+00000cd0: 7375 6273 6372 6962 655f 6672 6f6d 5f73  subscribe_from_s
+00000ce0: 796e 6368 726f 6e69 7a65 72da 166c 6175  ynchronizer..lau
+00000cf0: 6e63 685f 6e65 775f 7374 6572 656f 6672  nch_new_stereofr
+00000d00: 616d 6572 3400 0000 7231 0000 0072 3100  amer4...r1...r1.
+00000d10: 0000 7232 0000 0072 3d00 0000 7700 0000  ..r2...r=...w...
+00000d20: 7310 0000 000a 010c 010a 020c 010c 0104  s...............
+00000d30: 010a 020c 017a 2543 616c 6962 7261 7469  .....z%Calibrati
+00000d40: 6f6e 5769 6467 6574 2e72 6566 7265 7368  onWidget.refresh
+00000d50: 5f73 7465 7265 6f66 7261 6d65 6301 0000  _stereoframec...
+00000d60: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00000d70: 0043 0000 0073 5a00 0000 7400 a001 6401  .C...sZ...t...d.
+00000d80: a101 0100 7c00 a002 7c00 6a03 a101 0100  ....|...|.j.....
+00000d90: 7c00 6a04 a005 a100 0100 7c00 6a06 6a07  |.j.......|.j.j.
+00000da0: a008 a100 0100 7c00 a009 7c00 6a06 a101  ......|...|.j...
+00000db0: 0100 7c00 6006 7c00 6a03 6a0a a00b a100  ..|.`.|.j.j.....
+00000dc0: 7d01 7c00 6a03 6a0a a00c 7c01 a101 0100  }.|.j.j...|.....
+00000dd0: 6400 5300 2902 4e7a 2d4d 6f76 696e 6720  d.S.).Nz-Moving 
+00000de0: 6261 636b 2074 6f20 6361 6d65 7261 2063  back to camera c
+00000df0: 6f6e 6669 6720 6672 6f6d 2073 7465 7265  onfig from stere
+00000e00: 6f66 7261 6d65 290d 7222 0000 0072 2300  oframe).r"...r#.
+00000e10: 0000 722c 0000 0072 3500 0000 721b 0000  ..r,...r5...r...
+00000e20: 005a 1270 6175 7365 5f73 796e 6368 726f  .Z.pause_synchro
+00000e30: 6e69 7a65 7272 3800 0000 7243 0000 0072  nizerr8...rC...r
+00000e40: 4400 0000 7242 0000 005a 0b63 616d 6572  D...rB...Z.camer
+00000e50: 615f 7461 6273 5a0c 6375 7272 656e 7449  a_tabsZ.currentI
+00000e60: 6e64 6578 5a14 6163 7469 7661 7465 5f63  ndexZ.activate_c
+00000e70: 7572 7265 6e74 5f74 6162 2902 722e 0000  urrent_tab).r...
+00000e80: 005a 0b61 6374 6976 655f 706f 7274 7231  .Z.active_portr1
+00000e90: 0000 0072 3100 0000 7232 0000 0072 3b00  ...r1...r2...r;.
+00000ea0: 0000 8400 0000 7310 0000 000a 010c 010a  ......s.........
+00000eb0: 010c 020c 0104 010c 0212 017a 2e43 616c  ...........z.Cal
+00000ec0: 6962 7261 7469 6f6e 5769 6467 6574 2e62  ibrationWidget.b
+00000ed0: 6163 6b5f 746f 5f63 616d 6572 615f 636f  ack_to_camera_co
+00000ee0: 6e66 6967 5f77 697a 6172 6463 0100 0000  nfig_wizardc....
+00000ef0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000f00: 4300 0000 735e 0000 0074 00a0 0164 01a1  C...s^...t...d..
+00000f10: 0101 0074 027c 006a 0383 017c 005f 0474  ...t.|.j...|._.t
+00000f20: 00a0 0164 02a1 0101 007c 00a0 057c 006a  ...d.....|...|.j
+00000f30: 04a1 0101 0074 00a0 0164 03a1 0101 007c  .....t...d.....|
+00000f40: 00a0 067c 006a 04a1 0101 007c 006a 046a  ...|.j.....|.j.j
+00000f50: 076a 086a 09a0 0a7c 006a 0ba1 0101 007c  .j.j...|.j.....|
+00000f60: 0060 0c64 0053 0029 044e 7a1e 4372 6561  .`.d.S.).Nz.Crea
+00000f70: 7469 6e67 2043 6170 7475 7265 2056 6f6c  ting Capture Vol
+00000f80: 756d 6520 7769 6467 6574 7a2b 4164 6469  ume widgetz+Addi
+00000f90: 6e67 2063 6170 7475 7265 2076 6f6c 756d  ng capture volum
+00000fa0: 6520 7769 6467 6574 2074 6f20 6d61 696e  e widget to main
+00000fb0: 2057 697a 6172 647a 2a53 6574 2063 7572   Wizardz*Set cur
+00000fc0: 7265 6e74 2069 6e64 6578 2074 6f20 6361  rent index to ca
+00000fd0: 7074 7572 6520 766f 6c75 6d65 2077 6964  pture volume wid
+00000fe0: 6765 7429 0d72 2200 0000 7223 0000 0072  get).r"...r#...r
+00000ff0: 1800 0000 721b 0000 00da 0e63 6170 7475  ....r......captu
+00001000: 7265 5f76 6f6c 756d 6572 2b00 0000 722c  re_volumer+...r,
+00001010: 0000 0072 2500 0000 723a 0000 0072 2600  ...r%...r:...r&.
+00001020: 0000 7227 0000 00da 1462 6163 6b5f 746f  ..r'.....back_to
+00001030: 5f73 7465 7265 6f5f 6672 616d 655a 0971  _stereo_frameZ.q
+00001040: 745f 6c6f 6767 6572 7234 0000 0072 3100  t_loggerr4...r1.
+00001050: 0000 7231 0000 0072 3200 0000 723c 0000  ..r1...r2...r<..
+00001060: 0090 0000 0073 1400 0000 0a01 0c01 0a01  .....s..........
+00001070: 0c01 0a01 0c01 0c01 0401 04ff 0804 7a28  ..............z(
+00001080: 4361 6c69 6272 6174 696f 6e57 6964 6765  CalibrationWidge
+00001090: 742e 6e65 7874 5f74 6f5f 6361 7074 7572  t.next_to_captur
+000010a0: 655f 766f 6c75 6d65 6301 0000 0000 0000  e_volumec.......
+000010b0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000010c0: 0073 7600 0000 7400 a001 6401 a101 0100  .sv...t...d.....
+000010d0: 7c00 a002 7c00 6a03 a101 0100 7400 a001  |...|.j.....t...
+000010e0: 6402 a101 0100 7c00 a004 7c00 6a05 a101  d.....|...|.j...
+000010f0: 0100 7400 a001 6403 a101 0100 7c00 a004  ..t...d.....|...
+00001100: 7c00 6a06 a101 0100 7c00 6006 7c00 6a05  |.j.....|.`.|.j.
+00001110: 6a07 a008 a100 0100 7c00 6005 7400 a001  j.......|.`.t...
+00001120: 6404 a101 0100 7c00 a009 a100 0100 7c00  d.....|.......|.
+00001130: 6a0a a00b a100 0100 6400 5300 2905 4e72  j.......d.S.).Nr
+00001140: 3f00 0000 7240 0000 007a 1552 656d 6f76  ?...r@...z.Remov
+00001150: 6520 6361 7074 7572 6520 766f 6c75 6d65  e capture volume
+00001160: 7241 0000 0029 0c72 2200 0000 7223 0000  rA...).r"...r#..
+00001170: 0072 2c00 0000 7235 0000 0072 4200 0000  .r,...r5...rB...
+00001180: 7238 0000 0072 4600 0000 7243 0000 0072  r8...rF...rC...r
+00001190: 4400 0000 7245 0000 0072 1b00 0000 5a14  D...rE...r....Z.
+000011a0: 756e 7061 7573 655f 7379 6e63 6872 6f6e  unpause_synchron
+000011b0: 697a 6572 7234 0000 0072 3100 0000 7231  izerr4...r1...r1
+000011c0: 0000 0072 3200 0000 7247 0000 009e 0000  ...r2...rG......
+000011d0: 0073 1800 0000 0a01 0c01 0a02 0c01 0a01  .s..............
+000011e0: 0c01 0401 0c01 0401 0a02 0801 0e01 7a26  ..............z&
+000011f0: 4361 6c69 6272 6174 696f 6e57 6964 6765  CalibrationWidge
+00001200: 742e 6261 636b 5f74 6f5f 7374 6572 656f  t.back_to_stereo
+00001210: 5f66 7261 6d65 2910 da08 5f5f 6e61 6d65  _frame)...__name
+00001220: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00001230: 5f5f 7175 616c 6e61 6d65 5f5f 7205 0000  __qualname__r...
+00001240: 005a 1163 616d 6572 6173 5f63 6f6e 6e65  .Z.cameras_conne
+00001250: 6374 6564 720f 0000 0072 1d00 0000 722d  ctedr....r....r-
+00001260: 0000 0072 2800 0000 7237 0000 0072 3e00  ...r(...r7...r>.
+00001270: 0000 723d 0000 0072 3b00 0000 723c 0000  ..r=...r;...r<..
+00001280: 0072 4700 0000 da0d 5f5f 636c 6173 7363  .rG.....__classc
+00001290: 656c 6c5f 5f72 3100 0000 7231 0000 0072  ell__r1...r1...r
+000012a0: 2f00 0000 7232 0000 0072 1a00 0000 2500  /...r2...r....%.
+000012b0: 0000 7316 0000 0008 0006 0112 0208 1a08  ..s.............
+000012c0: 0708 1508 0408 1508 0d08 0c10 0e72 1a00  .............r..
+000012d0: 0000 7220 0000 0063 0100 0000 0000 0000  ..r ...c........
+000012e0: 0000 0000 0500 0000 0300 0000 4300 0000  ............C...
+000012f0: 7342 0000 0074 007c 0083 017d 0174 017c  sB...t.|...}.t.|
+00001300: 0183 017d 027c 02a0 0274 036a 04a1 0101  ...}.|...t.j....
+00001310: 0074 0574 066a 0783 017d 0374 087c 0283  .t.t.j...}.t.|..
+00001320: 017d 047c 04a0 09a1 0001 007c 03a0 0aa1  .}.|.......|....
+00001330: 0001 0064 0053 0072 3300 0000 290b 7219  ...d.S.r3...).r.
+00001340: 0000 0072 0f00 0000 7229 0000 0072 1000  ...r....r)...r..
+00001350: 0000 7239 0000 0072 0900 0000 da03 7379  ..r9...r......sy
+00001360: 73da 0461 7267 7672 1a00 0000 5a04 7368  s..argvr....Z.sh
+00001370: 6f77 da04 6578 6563 2905 7220 0000 0072  ow..exec).r ...r
+00001380: 2100 0000 721b 0000 005a 0361 7070 5a06  !...r....Z.appZ.
+00001390: 7769 6e64 6f77 7231 0000 0072 3100 0000  windowr1...r1...
+000013a0: 7232 0000 00da 236c 6175 6e63 685f 6578  r2....#launch_ex
+000013b0: 7472 696e 7369 635f 6361 6c69 6272 6174  trinsic_calibrat
+000013c0: 696f 6e5f 7769 6467 6574 af00 0000 730e  ion_widget....s.
+000013d0: 0000 0008 0108 010c 010a 0208 0108 010c  ................
+000013e0: 0172 4f00 0000 292f da0d 7079 7879 3364  .rO...)/..pyxy3d
+000013f0: 2e6c 6f67 6765 72da 0670 7978 7933 6472  .logger..pyxy3dr
+00001400: 2200 0000 da03 6765 7472 4800 0000 da02  ".....getrH.....
+00001410: 6f73 724c 0000 005a 0673 6875 7469 6cda  osrL...Z.shutil.
+00001420: 0474 696d 65da 0770 6174 686c 6962 7202  .time..pathlibr.
+00001430: 0000 00da 0974 6872 6561 6469 6e67 7203  .....threadingr.
+00001440: 0000 005a 0c50 7951 7436 2e51 7443 6f72  ...Z.PyQt6.QtCor
+00001450: 6572 0400 0000 7205 0000 005a 0b50 7951  er....r....Z.PyQ
+00001460: 7436 2e51 7447 7569 7206 0000 0072 0700  t6.QtGuir....r..
+00001470: 0000 da0f 5079 5174 362e 5174 5769 6467  ....PyQt6.QtWidg
+00001480: 6574 7372 0800 0000 7209 0000 0072 0a00  etsr....r....r..
+00001490: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000014a0: 0072 0e00 0000 5a16 7079 7879 3364 2e73  .r....Z.pyxy3d.s
+000014b0: 6573 7369 6f6e 2e73 6573 7369 6f6e 720f  ession.sessionr.
+000014c0: 0000 0072 1000 0000 5a19 7079 7879 3364  ...r....Z.pyxy3d
+000014d0: 2e67 7569 2e63 6861 7275 636f 5f77 6964  .gui.charuco_wid
+000014e0: 6765 7472 1100 0000 5a35 7079 7879 3364  getr....Z5pyxy3d
+000014f0: 2e67 7569 2e63 616d 6572 615f 636f 6e66  .gui.camera_conf
+00001500: 6967 2e69 6e74 7269 6e73 6963 5f63 616c  ig.intrinsic_cal
+00001510: 6962 7261 7469 6f6e 5f77 6964 6765 7472  ibration_widgetr
+00001520: 1200 0000 7213 0000 0072 1400 0000 5a1f  ....r....r....Z.
+00001530: 7079 7879 3364 2e74 7261 636b 6572 732e  pyxy3d.trackers.
+00001540: 6368 6172 7563 6f5f 7472 6163 6b65 7272  charuco_trackerr
+00001550: 1500 0000 5a27 7079 7879 3364 2e67 7569  ....Z'pyxy3d.gui
+00001560: 2e65 7874 7269 6e73 6963 5f63 616c 6962  .extrinsic_calib
+00001570: 7261 7469 6f6e 5f77 6964 6765 7472 1600  ration_widgetr..
+00001580: 0000 7217 0000 005a 3670 7978 7933 642e  ..r....Z6pyxy3d.
+00001590: 6775 692e 7669 7a75 616c 697a 652e 6361  gui.vizualize.ca
+000015a0: 6c69 6272 6174 696f 6e2e 6361 7074 7572  libration.captur
+000015b0: 655f 766f 6c75 6d65 5f77 6964 6765 7472  e_volume_widgetr
+000015c0: 1800 0000 5a13 7079 7879 3364 2e63 6f6e  ....Z.pyxy3d.con
+000015d0: 6669 6775 7261 746f 7272 1900 0000 721a  figuratorr....r.
+000015e0: 0000 0072 4f00 0000 7231 0000 0072 3100  ...rO...r1...r1.
+000015f0: 0000 7231 0000 0072 3200 0000 da08 3c6d  ..r1...r2.....<m
+00001600: 6f64 756c 653e 0100 0000 732c 0000 0008  odule>....s,....
+00001610: 000c 0208 0208 0108 0108 010c 010c 0110  ................
+00001620: 0110 0124 0110 0a0c 010c 0110 010c 0110  ...$............
+00001630: 020c 040c 0110 0300 7f12 0b              ...........
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 16:49:05 2023 UTC, .py size: 10279 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 814c 8764 2728 0000  o........L.d'(..
+00000000: 6f0d 0d0a 0000 0000 8850 8b64 302a 0000  o........P.d0*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 bc01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6400 6401 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
 00000070: 6404 6c0c 6d0d 5a0d 0100 6400 6401 6c0e  d.l.m.Z...d.d.l.
@@ -77,431 +77,459 @@
 000004c0: 0664 0784 005a 0a64 0864 0984 005a 0b64  .d...Z.d.d...Z.d
 000004d0: 0a64 0b84 005a 0c64 0c64 0d84 005a 0d64  .d...Z.d.d...Z.d
 000004e0: 0e64 0f84 005a 0e64 1064 1184 005a 0f64  .d...Z.d.d...Z.d
 000004f0: 1264 1384 005a 1064 1464 1584 005a 1187  .d...Z.d.d...Z..
 00000500: 0004 005a 1253 0029 16da 1a45 7874 7269  ...Z.S.)...Extri
 00000510: 6e73 6963 4361 6c69 6272 6174 696f 6e57  nsicCalibrationW
 00000520: 6964 6765 74da 0773 6573 7369 6f6e 6302  idget..sessionc.
-00000530: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000540: 0000 0003 0000 0073 9000 0000 7400 7401  .......s....t.t.
+00000530: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000540: 0000 0003 0000 0073 ae00 0000 7400 7401  .......s....t.t.
 00000550: 7c00 8302 a002 a100 0100 7c01 7c00 5f03  |.........|.|._.
-00000560: 7c00 6a03 6a04 7c00 5f04 7c00 a005 a100  |.j.j.|._.|.....
-00000570: 0100 7406 8300 7c00 5f07 7c00 6a07 a008  ..t...|._.|.j...
-00000580: 7c00 6a04 6a09 a101 0100 7406 8300 7c00  |.j.j.....t...|.
-00000590: 5f0a 7c00 6a0a a008 7c00 6a0b 6a0c a101  _.|.j...|.j.j...
-000005a0: 0100 740d 8300 7c00 5f0e 740f 6a10 7c00  ..t...|._.t.j.|.
-000005b0: 5f11 7412 7c00 6a11 6a13 8301 7c00 5f14  _.t.|.j.j...|._.
-000005c0: 7c00 a015 a100 0100 7c00 a016 a100 0100  |.......|.......
-000005d0: 7c00 a017 a100 0100 6400 5300 a901 4e29  |.......d.S...N)
-000005e0: 18da 0573 7570 6572 722a 0000 00da 085f  ...superr*....._
-000005f0: 5f69 6e69 745f 5f72 2b00 0000 da0c 7379  _init__r+.....sy
-00000600: 6e63 6872 6f6e 697a 6572 da18 6372 6561  nchronizer..crea
-00000610: 7465 5f73 7465 7265 6f66 7261 6d65 5f74  te_stereoframe_t
-00000620: 6f6f 6c73 720f 0000 00da 0f66 7261 6d65  oolsr......frame
-00000630: 5f72 6174 655f 7370 696e da08 7365 7456  _rate_spin..setV
-00000640: 616c 7565 da0a 6670 735f 7461 7267 6574  alue..fps_target
-00000650: da10 626f 6172 645f 636f 756e 745f 7370  ..board_count_sp
-00000660: 696e da0d 6672 616d 655f 6275 696c 6465  in..frame_builde
-00000670: 72da 1262 6f61 7264 5f63 6f75 6e74 5f74  r..board_count_t
-00000680: 6172 6765 7472 1700 0000 da14 7374 6572  argetr......ster
-00000690: 656f 5f66 7261 6d65 5f64 6973 706c 6179  eo_frame_display
-000006a0: 7221 0000 0072 2700 0000 da0f 706f 7373  r!...r'.....poss
-000006b0: 6962 6c65 5f61 6374 696f 6e72 1800 0000  ible_actionr....
-000006c0: da05 7661 6c75 65da 1563 616c 6962 7261  ..value..calibra
-000006d0: 7465 5f63 6f6c 6c65 6374 5f62 746e da0d  te_collect_btn..
-000006e0: 706c 6163 655f 7769 6467 6574 73da 0f63  place_widgets..c
-000006f0: 6f6e 6e65 6374 5f77 6964 6765 7473 da16  onnect_widgets..
-00000700: 7570 6461 7465 5f62 746e 5f65 6c69 6769  update_btn_eligi
-00000710: 6269 6c69 7479 2902 da04 7365 6c66 722b  bility)...selfr+
-00000720: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
-00000730: 7228 0000 0072 2900 0000 722e 0000 0035  r(...r)...r....5
-00000740: 0000 0073 1c00 0000 0e02 0601 0a01 0802  ...s............
-00000750: 0802 1001 0801 1001 0802 0802 0e01 0802  ................
-00000760: 0801 0c02 7a23 4578 7472 696e 7369 6343  ....z#ExtrinsicC
-00000770: 616c 6962 7261 7469 6f6e 5769 6467 6574  alibrationWidget
-00000780: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000790: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000007a0: 0000 732a 0000 007c 006a 00a0 01a1 0072  ..s*...|.j.....r
-000007b0: 0d7c 006a 02a0 0364 01a1 0101 0064 0053  .|.j...d.....d.S
-000007c0: 007c 006a 02a0 0364 02a1 0101 0064 0053  .|.j...d.....d.S
-000007d0: 0029 034e 5446 2904 722b 0000 00da 2169  .).NTF).r+....!i
-000007e0: 735f 6578 7472 696e 7369 635f 6361 6c69  s_extrinsic_cali
-000007f0: 6272 6174 696f 6e5f 656c 6967 6962 6c65  bration_eligible
-00000800: 723a 0000 00da 0a73 6574 456e 6162 6c65  r:.....setEnable
-00000810: 64a9 0172 3e00 0000 7228 0000 0072 2800  d..r>...r(...r(.
-00000820: 0000 7229 0000 0072 3d00 0000 4c00 0000  ..r)...r=...L...
-00000830: 7306 0000 000a 0110 0110 027a 3145 7874  s..........z1Ext
-00000840: 7269 6e73 6963 4361 6c69 6272 6174 696f  rinsicCalibratio
-00000850: 6e57 6964 6765 742e 7570 6461 7465 5f62  nWidget.update_b
-00000860: 746e 5f65 6c69 6769 6269 6c69 7479 6301  tn_eligibilityc.
-00000870: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000880: 0000 0043 0000 0073 2a00 0000 7400 7c00  ...C...s*...t.|.
-00000890: 6a01 6401 6402 8d02 7c00 5f02 7403 7c00  j.d.d...|._.t.|.
-000008a0: 6a02 8301 7c00 5f04 7c00 6a04 a005 a100  j...|._.|.j.....
-000008b0: 0100 6400 5300 2903 4ee9 1e00 0000 2901  ..d.S.).N.....).
-000008c0: 7236 0000 0029 0672 1c00 0000 722f 0000  r6...).r....r/..
-000008d0: 0072 3500 0000 da12 5061 6972 6564 4672  .r5.....PairedFr
-000008e0: 616d 6545 6d69 7474 6572 da0d 6672 616d  ameEmitter..fram
-000008f0: 655f 656d 6974 7465 72da 0573 7461 7274  e_emitter..start
-00000900: 7243 0000 0072 2800 0000 7228 0000 0072  rC...r(...r(...r
-00000910: 2900 0000 7230 0000 0053 0000 0073 0600  )...r0...S...s..
-00000920: 0000 1002 0c01 0e01 7a33 4578 7472 696e  ........z3Extrin
-00000930: 7369 6343 616c 6962 7261 7469 6f6e 5769  sicCalibrationWi
-00000940: 6467 6574 2e63 7265 6174 655f 7374 6572  dget.create_ster
-00000950: 656f 6672 616d 655f 746f 6f6c 7363 0100  eoframe_toolsc..
-00000960: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00000970: 0000 4300 0000 73ca 0000 007c 00a0 0074  ..C...s....|...t
-00000980: 0183 00a1 0101 0074 0264 0183 017c 005f  .......t.d...|._
-00000990: 037c 006a 03a0 0074 0483 00a1 0101 007c  .|.j...t.......|
-000009a0: 006a 03a0 05a1 00a0 0674 0764 0283 01a1  .j.......t.d....
-000009b0: 0101 007c 006a 03a0 05a1 00a0 067c 006a  ...|.j.......|.j
-000009c0: 08a1 0101 007c 006a 03a0 05a1 00a0 0674  .....|.j.......t
-000009d0: 0764 0383 01a1 0101 007c 006a 03a0 05a1  .d.......|.j....
-000009e0: 00a0 067c 006a 09a1 0101 007c 00a0 05a1  ...|.j.....|....
-000009f0: 00a0 067c 006a 03a1 0101 0074 0a83 007c  ...|.j.....t...|
-00000a00: 005f 0b7c 006a 0ba0 0c74 0d6a 0e6a 0fa1  ._.|.j...t.j.j..
-00000a10: 0101 007c 00a0 05a1 00a0 067c 006a 0ba1  ...|.......|.j..
-00000a20: 0101 007c 006a 0ba0 107c 006a 11a1 0101  ...|.j...|.j....
-00000a30: 007c 00a0 05a1 00a0 067c 006a 12a1 0101  .|.......|.j....
-00000a40: 0064 0053 0029 044e 5a08 5365 7474 696e  .d.S.).NZ.Settin
-00000a50: 6773 7a0b 4672 616d 6520 5261 7465 3a7a  gsz.Frame Rate:z
-00000a60: 1354 6172 6765 7420 426f 6172 6420 436f  .Target Board Co
-00000a70: 756e 743a 2913 da09 7365 744c 6179 6f75  unt:)...setLayou
-00000a80: 7472 1a00 0000 7214 0000 005a 0e73 6574  tr....r....Z.set
-00000a90: 7469 6e67 735f 6772 6f75 7072 1600 0000  tings_groupr....
-00000aa0: da06 6c61 796f 7574 da09 6164 6457 6964  ..layout..addWid
-00000ab0: 6765 7472 1700 0000 7231 0000 0072 3400  getr....r1...r4.
-00000ac0: 0000 7210 0000 005a 0b73 6372 6f6c 6c5f  ..r....Z.scroll_
-00000ad0: 6172 6561 5a1a 7365 7456 6572 7469 6361  areaZ.setVertica
-00000ae0: 6c53 6372 6f6c 6c42 6172 506f 6c69 6379  lScrollBarPolicy
-00000af0: 7206 0000 005a 0f53 6372 6f6c 6c42 6172  r....Z.ScrollBar
-00000b00: 506f 6c69 6379 5a11 5363 726f 6c6c 4261  PolicyZ.ScrollBa
-00000b10: 7241 6c77 6179 734f 6eda 0973 6574 5769  rAlwaysOn..setWi
-00000b20: 6467 6574 7237 0000 0072 3a00 0000 7243  dgetr7...r:...rC
-00000b30: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00000b40: 0000 723b 0000 0059 0000 0073 1a00 0000  ..r;...Y...s....
-00000b50: 0c01 0a02 0e01 1401 1201 1401 1201 1002  ................
-00000b60: 0804 1001 1002 0e02 1402 7a28 4578 7472  ..........z(Extr
-00000b70: 696e 7369 6343 616c 6962 7261 7469 6f6e  insicCalibration
-00000b80: 5769 6467 6574 2e70 6c61 6365 5f77 6964  Widget.place_wid
-00000b90: 6765 7473 6301 0000 0000 0000 0000 0000  getsc...........
-00000ba0: 0001 0000 0003 0000 0043 0000 0073 6600  .........C...sf.
-00000bb0: 0000 7c00 6a00 6a01 a002 7c00 6a03 a101  ..|.j.j...|.j...
-00000bc0: 0100 7c00 6a04 6a05 a002 7c00 6a06 a101  ..|.j.j...|.j...
-00000bd0: 0100 7c00 6a04 6a07 a002 7c00 6a08 a101  ..|.j.j...|.j...
-00000be0: 0100 7c00 6a09 6a0a a002 7c00 6a0b 6a0c  ..|.j.j...|.j.j.
-00000bf0: a101 0100 7c00 6a0d 6a0a a002 7c00 6a0e  ....|.j.j...|.j.
-00000c00: a101 0100 7c00 6a04 6a0f a002 7c00 6a10  ....|.j.j...|.j.
-00000c10: a101 0100 6400 5300 722c 0000 0029 1172  ....d.S.r,...).r
-00000c20: 3a00 0000 da07 636c 6963 6b65 64da 0763  :.....clicked..c
-00000c30: 6f6e 6e65 6374 da1a 6f6e 5f63 616c 6962  onnect..on_calib
-00000c40: 7261 7465 5f63 6f6c 6c65 6374 5f63 6c69  rate_collect_cli
-00000c50: 636b 7246 0000 00da 0e49 6d61 6765 4272  ckrF.....ImageBr
-00000c60: 6f61 6463 6173 74da 0f49 6d61 6765 5570  oadcast..ImageUp
-00000c70: 6461 7465 536c 6f74 da1c 706f 7373 6962  dateSlot..possib
-00000c80: 6c65 5f74 6f5f 696e 6974 6961 6c69 7a65  le_to_initialize
-00000c90: 5f61 7272 6179 da12 656e 6162 6c65 5f63  _array..enable_c
-00000ca0: 616c 6962 7261 7469 6f6e 7231 0000 00da  alibrationr1....
-00000cb0: 0c76 616c 7565 4368 616e 6765 6472 2f00  .valueChangedr/.
-00000cc0: 0000 da0e 7365 745f 7374 7265 616d 5f66  ....set_stream_f
-00000cd0: 7073 7234 0000 00da 1975 7064 6174 655f  psr4.....update_
-00000ce0: 626f 6172 645f 636f 756e 745f 7461 7267  board_count_targ
-00000cf0: 6574 da1a 6361 6c69 6272 6174 696f 6e5f  et..calibration_
-00000d00: 6461 7461 5f63 6f6c 6c65 6374 6564 da14  data_collected..
-00000d10: 696e 6974 6961 7465 5f63 616c 6962 7261  initiate_calibra
-00000d20: 7469 6f6e 7243 0000 0072 2800 0000 7228  tionrC...r(...r(
-00000d30: 0000 0072 2900 0000 723c 0000 0072 0000  ...r)...r<...r..
-00000d40: 0073 0c00 0000 1002 1001 1001 1201 1001  .s..............
-00000d50: 1401 7a2a 4578 7472 696e 7369 6343 616c  ..z*ExtrinsicCal
-00000d60: 6962 7261 7469 6f6e 5769 6467 6574 2e63  ibrationWidget.c
-00000d70: 6f6e 6e65 6374 5f77 6964 6765 7473 6302  onnect_widgetsc.
-00000d80: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000d90: 0000 0043 0000 0073 0c00 0000 7c01 7c00  ...C...s....|.|.
-00000da0: 6a00 5f01 6400 5300 722c 0000 0029 0272  j._.d.S.r,...).r
-00000db0: 3500 0000 7236 0000 0029 0272 3e00 0000  5...r6...).r>...
-00000dc0: da06 7461 7267 6574 7228 0000 0072 2800  ..targetr(...r(.
-00000dd0: 0000 7229 0000 0072 5500 0000 7b00 0000  ..r)...rU...{...
-00000de0: 7302 0000 000c 017a 3445 7874 7269 6e73  s......z4Extrins
-00000df0: 6963 4361 6c69 6272 6174 696f 6e57 6964  icCalibrationWid
-00000e00: 6765 742e 7570 6461 7465 5f62 6f61 7264  get.update_board
-00000e10: 5f63 6f75 6e74 5f74 6172 6765 7463 0100  _count_targetc..
-00000e20: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000e30: 0000 4300 0000 73e6 0000 007c 006a 0074  ..C...s....|.j.t
-00000e40: 016a 026b 0272 3c74 03a0 0464 01a1 0101  .j.k.r<t...d....
-00000e50: 007c 006a 056a 06a0 07a1 0001 0074 087c  .|.j.j.......t.|
-00000e60: 006a 096a 0a64 0264 0383 037d 017c 006a  .j.j.d.d...}.|.j
-00000e70: 096a 0b7c 0164 0464 058d 0201 0074 016a  .j.|.d.d.....t.j
-00000e80: 0c7c 005f 007c 006a 0da0 0e7c 006a 006a  .|._.|.j...|.j.j
-00000e90: 0fa1 0101 007c 006a 0da0 1064 04a1 0101  .....|.j...d....
-00000ea0: 007c 006a 116a 12a0 1064 06a1 0101 0064  .|.j.j...d.....d
-00000eb0: 0053 007c 006a 0074 016a 0c6b 0272 5a74  .S.|.j.t.j.k.rZt
-00000ec0: 03a0 0464 07a1 0101 007c 006a 13a0 14a1  ...d.....|.j....
-00000ed0: 0001 0074 016a 027c 005f 007c 006a 0da0  ...t.j.|._.|.j..
-00000ee0: 0e7c 006a 006a 0fa1 0101 0064 0053 007c  .|.j.j.....d.S.|
-00000ef0: 006a 0074 016a 156b 0272 7174 03a0 0464  .j.t.j.k.rqt...d
-00000f00: 08a1 0101 007c 006a 056a 06a0 16a1 0001  .....|.j.j......
-00000f10: 007c 00a0 17a1 0001 0064 0053 0064 0053  .|.......d.S.d.S
-00000f20: 0029 094e 7a21 4265 6769 6e20 636f 6c6c  .).Nz!Begin coll
-00000f30: 6563 7469 6e67 2063 616c 6962 7261 7469  ecting calibrati
-00000f40: 6f6e 2064 6174 61da 0b63 616c 6962 7261  on data..calibra
-00000f50: 7469 6f6e da09 6578 7472 696e 7369 6354  tion..extrinsicT
-00000f60: 2901 da13 7374 6f72 655f 706f 696e 745f  )...store_point_
-00000f70: 6869 7374 6f72 7946 7a23 5465 726d 696e  historyFz#Termin
-00000f80: 6174 696e 6720 6375 7272 656e 7420 6461  ating current da
-00000f90: 7461 2063 6f6c 6c65 6374 696f 6e7a 3750  ta collectionz7P
-00000fa0: 7265 6d61 7475 7265 6c79 2065 6e64 2064  rematurely end d
-00000fb0: 6174 6120 636f 6c6c 6563 7469 6f6e 2074  ata collection t
-00000fc0: 6f20 696e 6974 6961 7465 2063 616c 6962  o initiate calib
-00000fd0: 7261 7469 6f6e 2918 7238 0000 0072 2100  ration).r8...r!.
-00000fe0: 0000 7227 0000 00da 066c 6f67 6765 72da  ..r'.....logger.
-00000ff0: 0469 6e66 6f72 3500 0000 5a0c 7374 6f72  .infor5...Z.stor
-00001000: 655f 706f 696e 7473 da03 7365 7472 0200  e_points..setr..
-00001010: 0000 722b 0000 00da 0470 6174 68da 0f73  ..r+.....path..s
-00001020: 7461 7274 5f72 6563 6f72 6469 6e67 7222  tart_recordingr"
-00001030: 0000 0072 3a00 0000 da07 7365 7454 6578  ...r:.....setTex
-00001040: 7472 3900 0000 7242 0000 00da 0e6e 6176  tr9...rB.....nav
-00001050: 6967 6174 696f 6e5f 6261 72da 0862 6163  igation_bar..bac
-00001060: 6b5f 6274 6eda 0974 6572 6d69 6e61 7465  k_btn..terminate
-00001070: da04 656d 6974 7223 0000 00da 0563 6c65  ..emitr#.....cle
-00001080: 6172 7257 0000 0029 0272 3e00 0000 5a1a  arrW...).r>...Z.
-00001090: 6578 7472 696e 7369 635f 6361 6c69 6272  extrinsic_calibr
-000010a0: 6174 696f 6e5f 7061 7468 7228 0000 0072  ation_pathr(...r
-000010b0: 2800 0000 7229 0000 0072 4e00 0000 7e00  (...r)...rN...~.
-000010c0: 0000 7326 0000 000c 010a 010c 0210 0110  ..s&............
-000010d0: 0108 0110 010c 0112 010c 020a 010a 0108  ................
-000010e0: 0314 010c 020a 010c 010c 0104 fd7a 3545  .............z5E
-000010f0: 7874 7269 6e73 6963 4361 6c69 6272 6174  xtrinsicCalibrat
-00001100: 696f 6e57 6964 6765 742e 6f6e 5f63 616c  ionWidget.on_cal
-00001110: 6962 7261 7465 5f63 6f6c 6c65 6374 5f63  ibrate_collect_c
-00001120: 6c69 636b 6301 0000 0000 0000 0000 0000  lickc...........
-00001130: 0001 0000 0003 0000 0043 0000 0073 2800  .........C...s(.
-00001140: 0000 7400 6a01 7c00 5f02 7c00 6a03 a004  ..t.j.|._.|.j...
-00001150: 7c00 6a02 6a05 a101 0100 7c00 6a03 a006  |.j.j.....|.j...
-00001160: 6401 a101 0100 6400 5300 2902 4e54 2907  d.....d.S.).NT).
-00001170: 7221 0000 0072 2300 0000 7238 0000 0072  r!...r#...r8...r
-00001180: 3a00 0000 7261 0000 0072 3900 0000 7242  :...ra...r9...rB
-00001190: 0000 0072 4300 0000 7228 0000 0072 2800  ...rC...r(...r(.
-000011a0: 0000 7229 0000 0072 5200 0000 9900 0000  ..r)...rR.......
-000011b0: 7306 0000 0008 0110 0110 017a 2d45 7874  s..........z-Ext
-000011c0: 7269 6e73 6963 4361 6c69 6272 6174 696f  rinsicCalibratio
-000011d0: 6e57 6964 6765 742e 656e 6162 6c65 5f63  nWidget.enable_c
-000011e0: 616c 6962 7261 7469 6f6e 6302 0000 0000  alibrationc.....
-000011f0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00001200: 0000 0073 2c00 0000 7c00 6a00 a001 7c00  ...s,...|.j...|.
-00001210: 6a00 a002 a100 a101 0100 7403 a004 7c01  j.........t...|.
-00001220: a101 7d02 7c00 6a00 a005 7c02 a101 0100  ..}.|.j...|.....
-00001230: 6400 5300 722c 0000 0029 0672 3700 0000  d.S.r,...).r7...
-00001240: da06 7265 7369 7a65 5a08 7369 7a65 4869  ..resizeZ.sizeHi
-00001250: 6e74 720a 0000 00da 0966 726f 6d49 6d61  ntr......fromIma
-00001260: 6765 da09 7365 7450 6978 6d61 7029 0372  ge..setPixmap).r
-00001270: 3e00 0000 5a07 715f 696d 6167 655a 0771  >...Z.q_imageZ.q
-00001280: 7069 786d 6170 7228 0000 0072 2800 0000  pixmapr(...r(...
-00001290: 7229 0000 0072 5000 0000 9f00 0000 7306  r)...rP.......s.
-000012a0: 0000 0012 010a 0210 017a 2a45 7874 7269  .........z*Extri
-000012b0: 6e73 6963 4361 6c69 6272 6174 696f 6e57  nsicCalibrationW
-000012c0: 6964 6765 742e 496d 6167 6555 7064 6174  idget.ImageUpdat
-000012d0: 6553 6c6f 7463 0100 0000 0000 0000 0000  eSlotc..........
-000012e0: 0000 0200 0000 0500 0000 0300 0000 732a  ..............s*
-000012f0: 0000 0087 0066 0164 0164 0284 087d 0174  .....f.d.d...}.t
-00001300: 007c 0164 0364 0464 058d 0388 005f 0188  .|.d.d.d....._..
-00001310: 006a 01a0 02a1 0001 0064 0053 0029 064e  .j.......d.S.).N
-00001320: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001330: 0003 0000 0013 0000 0073 a400 0000 8800  .........s......
-00001340: 6a00 a001 a100 0100 7402 a003 6401 a101  j.......t...d...
-00001350: 0100 8800 6a04 a005 6402 a101 0100 8800  ....j...d.......
-00001360: 6a04 a006 6403 a101 0100 7402 a003 6404  j...d.....t...d.
-00001370: a101 0100 8800 6a07 a008 a100 0100 7402  ......j.......t.
-00001380: a003 6405 a101 0100 7402 a003 6406 a101  ..d.....t...d...
-00001390: 0100 8800 6a07 a009 a100 0100 8800 6a07  ....j.........j.
-000013a0: a00a a100 0100 740b 6a0c 8800 5f0d 8800  ......t.j..._...
-000013b0: 6a04 a005 8800 6a0d 6a0e a101 0100 8800  j.....j.j.......
-000013c0: 6a04 a006 6407 a101 0100 8800 6a0f a001  j...d.......j...
-000013d0: a100 0100 7402 a003 6408 a101 0100 6400  ....t...d.....d.
-000013e0: 5300 2909 4e7a 3042 6567 696e 6e69 6e67  S.).Nz0Beginning
-000013f0: 2077 696e 642d 646f 776e 2070 726f 6365   wind-down proce
-00001400: 7373 2070 7269 6f72 2074 6f20 6361 6c69  ss prior to cali
-00001410: 6272 6174 696f 6e7a 112d 2d2d 6361 6c69  brationz.---cali
-00001420: 6272 6174 696e 672d 2d2d 467a 1453 746f  brating---Fz.Sto
-00001430: 7020 7265 636f 7264 696e 6720 7669 6465  p recording vide
-00001440: 6f7a 1142 6567 696e 2063 616c 6962 7261  oz.Begin calibra
-00001450: 7469 6f6e 7a12 5061 7573 6520 7379 6e63  tionz.Pause sync
-00001460: 6872 6f6e 697a 6572 547a 2343 616c 6962  hronizerTz#Calib
-00001470: 7261 7469 6f6e 2043 6f6d 706c 6574 6520  ration Complete 
-00001480: 7369 676e 616c 2073 656e 742e 2e2e 2910  signal sent...).
-00001490: da15 6361 6c69 6272 6174 696f 6e5f 696e  ..calibration_in
-000014a0: 6974 6961 7465 6472 6500 0000 725c 0000  itiatedre...r\..
-000014b0: 0072 5d00 0000 723a 0000 0072 6100 0000  .r]...r:...ra...
-000014c0: 7242 0000 0072 2b00 0000 da0e 7374 6f70  rB...r+.....stop
-000014d0: 5f72 6563 6f72 6469 6e67 da12 7061 7573  _recording..paus
-000014e0: 655f 7379 6e63 6872 6f6e 697a 6572 da13  e_synchronizer..
-000014f0: 6573 7469 6d61 7465 5f65 7874 7269 6e73  estimate_extrins
-00001500: 6963 7372 2100 0000 7227 0000 0072 3800  icsr!...r'...r8.
-00001510: 0000 7239 0000 00da 1463 616c 6962 7261  ..r9.....calibra
-00001520: 7469 6f6e 5f63 6f6d 706c 6574 6572 2800  tion_completer(.
-00001530: 0000 7243 0000 0072 2800 0000 7229 0000  ..rC...r(...r)..
-00001540: 00da 0677 6f72 6b65 72a8 0000 0073 1e00  ...worker....s..
-00001550: 0000 0a01 0a01 0c01 0c01 0a03 0a01 0a01  ................
-00001560: 0a01 0a01 0a01 0802 1001 0c01 0a01 0e01  ................
-00001570: 7a3f 4578 7472 696e 7369 6343 616c 6962  z?ExtrinsicCalib
-00001580: 7261 7469 6f6e 5769 6467 6574 2e69 6e69  rationWidget.ini
-00001590: 7469 6174 655f 6361 6c69 6272 6174 696f  tiate_calibratio
-000015a0: 6e2e 3c6c 6f63 616c 733e 2e77 6f72 6b65  n.<locals>.worke
-000015b0: 7272 2800 0000 5429 0372 5800 0000 da04  rr(...T).rX.....
-000015c0: 6172 6773 da06 6461 656d 6f6e 2903 7203  args..daemon).r.
-000015d0: 0000 005a 1769 6e69 745f 6361 6c69 6272  ...Z.init_calibr
-000015e0: 6174 696f 6e5f 7468 7265 6164 7247 0000  ation_threadrG..
-000015f0: 0029 0272 3e00 0000 726f 0000 0072 2800  .).r>...ro...r(.
-00001600: 0000 7243 0000 0072 2900 0000 7257 0000  ..rC...r)...rW..
-00001610: 00a7 0000 0073 0600 0000 0c01 1014 0e01  .....s..........
-00001620: 7a2f 4578 7472 696e 7369 6343 616c 6962  z/ExtrinsicCalib
-00001630: 7261 7469 6f6e 5769 6467 6574 2e69 6e69  rationWidget.ini
-00001640: 7469 6174 655f 6361 6c69 6272 6174 696f  tiate_calibratio
-00001650: 6e29 1372 2400 0000 7225 0000 0072 2600  n).r$...r%...r&.
-00001660: 0000 7207 0000 0072 6e00 0000 726a 0000  ..r....rn...rj..
-00001670: 0072 6400 0000 721b 0000 0072 2e00 0000  .rd...r....r....
-00001680: 723d 0000 0072 3000 0000 723b 0000 0072  r=...r0...r;...r
-00001690: 3c00 0000 7255 0000 0072 4e00 0000 7252  <...rU...rN...rR
-000016a0: 0000 0072 5000 0000 7257 0000 00da 0d5f  ...rP...rW....._
-000016b0: 5f63 6c61 7373 6365 6c6c 5f5f 7228 0000  _classcell__r(..
-000016c0: 0072 2800 0000 723f 0000 0072 2900 0000  .r(...r?...r)...
-000016d0: 722a 0000 0030 0000 0073 1c00 0000 0800  r*...0...s......
-000016e0: 0601 0601 0601 1202 0817 0807 0806 0819  ................
-000016f0: 0809 0803 081b 0806 1008 722a 0000 0063  ..........r*...c
-00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001710: 0400 0000 0000 0000 733e 0000 0065 005a  ........s>...e.Z
-00001720: 0164 005a 0265 0365 0483 015a 0565 0383  .d.Z.e.e...Z.e..
-00001730: 005a 0665 0383 005a 0764 0165 0866 0287  .Z.e...Z.d.e.f..
-00001740: 0066 0164 0264 0384 0c5a 0964 0464 0584  .f.d.d...Z.d.d..
-00001750: 005a 0a87 0004 005a 0b53 0029 0672 4500  .Z.....Z.S.).rE.
-00001760: 0000 da14 7061 6972 6564 5f66 7261 6d65  ....paired_frame
-00001770: 5f62 7569 6c64 6572 6302 0000 0000 0000  _builderc.......
-00001780: 0000 0000 0002 0000 0003 0000 0003 0000  ................
-00001790: 0073 3000 0000 7400 7401 7c00 8302 a002  .s0...t.t.|.....
-000017a0: a100 0100 7c01 7c00 5f03 7404 a005 6401  ....|.|._.t...d.
-000017b0: a101 0100 7406 8300 7c00 5f07 6402 7c00  ....t...|._.d.|.
-000017c0: 5f08 6400 5300 2903 4e7a 1749 6e69 7469  _.d.S.).Nz.Initi
-000017d0: 6174 6564 2066 7261 6d65 2065 6d69 7474  ated frame emitt
-000017e0: 6572 4629 0972 2d00 0000 7245 0000 0072  erF).r-...rE...r
-000017f0: 2e00 0000 7273 0000 0072 5c00 0000 725d  ....rs...r\...r]
-00001800: 0000 0072 0400 0000 da0f 6b65 6570 5f63  ...r......keep_c
-00001810: 6f6c 6c65 6374 696e 67da 1363 6f6c 6c65  ollecting..colle
-00001820: 6374 696f 6e5f 636f 6d70 6c65 7465 2902  ction_complete).
-00001830: 723e 0000 0072 7300 0000 723f 0000 0072  r>...rs...r?...r
-00001840: 2800 0000 7229 0000 0072 2e00 0000 c400  (...r)...r......
-00001850: 0000 730a 0000 000e 0206 010a 0108 010a  ..s.............
-00001860: 017a 1b50 6169 7265 6446 7261 6d65 456d  .z.PairedFrameEm
-00001870: 6974 7465 722e 5f5f 696e 6974 5f5f 6301  itter.__init__c.
-00001880: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00001890: 0000 0043 0000 0073 b400 0000 7c00 6a00  ...C...s....|.j.
-000018a0: a001 a100 0100 6401 7c00 5f02 6401 7d01  ......d.|._.d.}.
-000018b0: 7c00 6a00 a003 a100 7253 7404 7c00 6a05  |.j.....rSt.|.j.
-000018c0: 6a06 8301 6402 6b02 7227 7c00 6a02 7327  j...d.k.r'|.j.s'
-000018d0: 7407 a008 6403 a101 0100 6404 7c00 5f02  t...d.....d.|._.
-000018e0: 7c00 6a09 a00a a100 0100 7c01 733b 7c00  |.j.......|.s;|.
-000018f0: 6a05 a00b 740c a101 723b 7407 a008 6405  j...t...r;t...d.
-00001900: a101 0100 6404 7d01 7c00 6a0b a00a a100  ....d.}.|.j.....
-00001910: 0100 7c00 6a05 a00d a100 7d02 7c02 6400  ..|.j.....}.|.d.
-00001920: 7501 724e 740e 7c02 8301 7d03 7c00 6a0f  u.rNt.|...}.|.j.
-00001930: a00a 7c03 a101 0100 7c00 6a00 a003 a100  ..|.....|.j.....
-00001940: 730f 7407 a008 6406 a101 0100 6400 5300  s.t...d.....d.S.
-00001950: 2907 4e46 7201 0000 007a 3453 6967 6e61  ).NFr....z4Signa
-00001960: 6c6c 696e 6720 7468 6174 2063 616c 6962  lling that calib
-00001970: 7261 7469 6f6e 2064 6174 6120 6973 2066  ration data is f
-00001980: 756c 6c79 2063 6f6c 6c65 6374 6564 2e54  ully collected.T
-00001990: 7a4a 5369 676e 616c 696e 6720 7468 6174  zJSignaling that
-000019a0: 2069 7420 6973 2070 6f73 7369 626c 6520   it is possible 
-000019b0: 746f 2069 6e69 7469 616c 697a 6520 6172  to initialize ar
-000019c0: 7261 7920 6261 7365 6420 6f6e 2063 6f6c  ray based on col
-000019d0: 6c65 6374 6564 2064 6174 612e 7a27 5374  lected data.z'St
-000019e0: 6572 656f 6672 616d 6520 656d 6974 7465  ereoframe emitte
-000019f0: 7220 7275 6e20 7468 7265 6164 2065 6e64  r run thread end
-00001a00: 6564 2e2e 2e29 1072 7400 0000 725e 0000  ed...).rt...r^..
-00001a10: 0072 7500 0000 da06 6973 5f73 6574 da03  .ru.....is_set..
-00001a20: 6c65 6e72 7300 0000 5a0b 7374 6572 656f  lenrs...Z.stereo
-00001a30: 5f6c 6973 7472 5c00 0000 725d 0000 0072  _listr\...r]...r
-00001a40: 5600 0000 7265 0000 0072 5100 0000 da21  V...re...rQ....!
-00001a50: 4d49 4e5f 5448 5245 5348 4f4c 445f 464f  MIN_THRESHOLD_FO
-00001a60: 525f 4541 524c 595f 4341 4c49 4252 4154  R_EARLY_CALIBRAT
-00001a70: 455a 1067 6574 5f73 7465 7265 6f5f 6672  EZ.get_stereo_fr
-00001a80: 616d 65da 0d63 7632 5f74 6f5f 716c 6162  ame..cv2_to_qlab
-00001a90: 656c 724f 0000 0029 0472 3e00 0000 5a16  elrO...).r>...Z.
-00001aa0: 706f 7373 6962 6c65 5f74 6f5f 696e 6974  possible_to_init
-00001ab0: 6961 6c69 7a65 5a0c 7374 6572 656f 5f66  ializeZ.stereo_f
-00001ac0: 7261 6d65 da05 696d 6167 6572 2800 0000  rame..imager(...
-00001ad0: 7228 0000 0072 2900 0000 da03 7275 6ecc  r(...r).....run.
-00001ae0: 0000 0073 2600 0000 0a02 0601 0402 0a02  ...s&...........
-00001af0: 1604 0a01 0601 0a01 0404 0c02 0a01 0401  ................
-00001b00: 0a01 0a02 0802 0801 0c01 0aea 0e18 7a16  ..............z.
-00001b10: 5061 6972 6564 4672 616d 6545 6d69 7474  PairedFrameEmitt
-00001b20: 6572 2e72 756e 290c 7224 0000 0072 2500  er.run).r$...r%.
-00001b30: 0000 7226 0000 0072 0700 0000 7209 0000  ..r&...r....r...
-00001b40: 0072 4f00 0000 7256 0000 0072 5100 0000  .rO...rV...rQ...
-00001b50: 721c 0000 0072 2e00 0000 727b 0000 0072  r....r....r{...r
-00001b60: 7200 0000 7228 0000 0072 2800 0000 723f  r...r(...r(...r?
-00001b70: 0000 0072 2900 0000 7245 0000 00bf 0000  ...r)...rE......
-00001b80: 0073 0c00 0000 0800 0801 0601 0601 1202  .s..............
-00001b90: 1008 7245 0000 0063 0100 0000 0000 0000  ..rE...c........
-00001ba0: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-00001bb0: 7332 0000 0074 00a0 017c 0074 006a 02a1  s2...t...|.t.j..
-00001bc0: 027d 0174 037c 016a 047c 016a 0564 0119  .}.t.|.j.|.j.d..
-00001bd0: 007c 016a 0564 0219 0074 036a 066a 0783  .|.j.d...t.j.j..
-00001be0: 047d 027c 0253 0029 034e e901 0000 0072  .}.|.S.).N.....r
-00001bf0: 0100 0000 2908 da03 6376 32da 0863 7674  ....)...cv2..cvt
-00001c00: 436f 6c6f 72da 0d43 4f4c 4f52 5f42 4752  Color..COLOR_BGR
-00001c10: 3252 4742 7209 0000 00da 0464 6174 61da  2RGBr......data.
-00001c20: 0573 6861 7065 da06 466f 726d 6174 da0d  .shape..Format..
-00001c30: 466f 726d 6174 5f52 4742 3838 3829 03da  Format_RGB888)..
-00001c40: 0566 7261 6d65 727a 0000 00da 0871 745f  .framerz.....qt_
-00001c50: 6672 616d 6572 2800 0000 7228 0000 0072  framer(...r(...r
-00001c60: 2900 0000 7279 0000 00f4 0000 0073 1000  )...ry.......s..
-00001c70: 0000 0e01 0202 0401 0801 0801 0601 04fc  ................
-00001c80: 0406 7279 0000 00da 085f 5f6d 6169 6e5f  ..ry.....__main_
-00001c90: 5f29 01da 0c43 6f6e 6669 6775 7261 746f  _)...Configurato
-00001ca0: 7229 01da 0e43 6861 7275 636f 5472 6163  r)...CharucoTrac
-00001cb0: 6b65 72da 0364 6576 5a0f 7361 6d70 6c65  ker..devZ.sample
-00001cc0: 5f73 6573 7369 6f6e 735a 0332 3537 2901  _sessionsZ.257).
-00001cd0: da07 7472 6163 6b65 7229 45da 0d70 7978  ..tracker)E..pyx
-00001ce0: 7933 642e 6c6f 6767 6572 da06 7079 7879  y3d.logger..pyxy
-00001cf0: 3364 725c 0000 00da 0367 6574 7224 0000  3dr\.....getr$..
-00001d00: 00da 0373 7973 da07 7061 7468 6c69 6272  ...sys..pathlibr
-00001d10: 0200 0000 da09 7468 7265 6164 696e 6772  ......threadingr
-00001d20: 0300 0000 7204 0000 00da 0474 696d 65da  ....r......time.
-00001d30: 0465 6e75 6d72 0500 0000 727d 0000 00da  .enumr....r}....
-00001d40: 0c50 7951 7436 2e51 7443 6f72 6572 0600  .PyQt6.QtCorer..
-00001d50: 0000 7207 0000 0072 0800 0000 da0b 5079  ..r....r......Py
-00001d60: 5174 362e 5174 4775 6972 0900 0000 720a  Qt6.QtGuir....r.
-00001d70: 0000 0072 0b00 0000 da0f 5079 5174 362e  ...r......PyQt6.
-00001d80: 5174 5769 6467 6574 7372 0c00 0000 720d  QtWidgetsr....r.
-00001d90: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
-00001da0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001db0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001dc0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00001dd0: 1a00 0000 da16 7079 7879 3364 2e73 6573  ......pyxy3d.ses
-00001de0: 7369 6f6e 2e73 6573 7369 6f6e 721b 0000  sion.sessionr...
-00001df0: 005a 2e70 7978 7933 642e 6775 692e 6672  .Z.pyxy3d.gui.fr
-00001e00: 616d 655f 6275 696c 6465 7273 2e70 6169  ame_builders.pai
-00001e10: 7265 645f 6672 616d 655f 6275 696c 6465  red_frame_builde
-00001e20: 7272 1c00 0000 da1b 7079 7879 3364 2e63  rr......pyxy3d.c
-00001e30: 616d 6572 6173 2e73 796e 6368 726f 6e69  ameras.synchroni
-00001e40: 7a65 7272 1d00 0000 721e 0000 00da 1a70  zerr....r......p
-00001e50: 7978 7933 642e 6775 692e 6e61 7669 6761  yxy3d.gui.naviga
-00001e60: 7469 6f6e 5f62 6172 7372 1f00 0000 7278  tion_barsr....rx
-00001e70: 0000 0072 2100 0000 722a 0000 0072 4500  ...r!...r*...rE.
-00001e80: 0000 7279 0000 00da 1370 7978 7933 642e  ..ry.....pyxy3d.
-00001e90: 636f 6e66 6967 7572 6174 6f72 7287 0000  configuratorr...
-00001ea0: 00da 1f70 7978 7933 642e 7472 6163 6b65  ...pyxy3d.tracke
-00001eb0: 7273 2e63 6861 7275 636f 5f74 7261 636b  rs.charuco_track
-00001ec0: 6572 7288 0000 00da 0461 7267 76da 0341  err......argv..A
-00001ed0: 7070 da0c 7365 7373 696f 6e5f 7061 7468  pp..session_path
-00001ee0: da0c 636f 6e66 6967 7572 6174 6f72 722b  ..configuratorr+
-00001ef0: 0000 00da 0763 6861 7275 636f 728a 0000  .....charucor...
-00001f00: 00da 116c 6f61 645f 7374 7265 616d 5f74  ...load_stream_t
-00001f10: 6f6f 6c73 5a0d 7374 6572 656f 5f64 6961  oolsZ.stereo_dia
-00001f20: 6c6f 67da 0473 686f 77da 0465 7869 74da  log..show..exit.
-00001f30: 0465 7865 6372 2800 0000 7228 0000 0072  .execr(...r(...r
-00001f40: 2800 0000 7229 0000 00da 083c 6d6f 6475  (...r).....<modu
-00001f50: 6c65 3e01 0000 0073 4600 0000 0801 0c01  le>....sF.......
-00001f60: 0802 0c01 1001 0801 0c01 0802 1401 1401  ................
-00001f70: 4401 0c13 0c01 0c01 0c01 0c01 0403 1003  D...............
-00001f80: 1005 007f 1010 0835 080c 0c01 0c01 0a02  .......5........
-00001f90: 0e02 0801 0802 0a02 0c01 0803 0801 1202  ................
-00001fa0: 04ee                                     ..
+00000560: 7c00 6a03 6a04 7c00 5f04 7405 7c00 6a04  |.j.j.|._.t.|.j.
+00000570: 6401 6402 8d02 7c00 5f06 7407 7c00 6a06  d.d...|._.t.|.j.
+00000580: 8301 7c00 5f08 7c00 6a08 a009 a100 0100  ..|._.|.j.......
+00000590: 740a 8300 7c00 5f0b 7c00 6a0b a00c 7c00  t...|._.|.j...|.
+000005a0: 6a04 6a0d a101 0100 740a 8300 7c00 5f0e  j.j.....t...|._.
+000005b0: 7c00 6a0e a00c 7c00 6a06 6a0f a101 0100  |.j...|.j.j.....
+000005c0: 7410 8300 7c00 5f11 7412 6a13 7c00 5f14  t...|._.t.j.|._.
+000005d0: 7415 7c00 6a14 6a16 8301 7c00 5f17 7c00  t.|.j.j...|._.|.
+000005e0: a018 a100 0100 7c00 a019 a100 0100 7c00  ......|.......|.
+000005f0: a01a a100 0100 6400 5300 2903 4ee9 1e00  ......d.S.).N...
+00000600: 0000 2901 da12 626f 6172 645f 636f 756e  ..)...board_coun
+00000610: 745f 7461 7267 6574 291b da05 7375 7065  t_target)...supe
+00000620: 7272 2a00 0000 da08 5f5f 696e 6974 5f5f  rr*.....__init__
+00000630: 722b 0000 00da 0c73 796e 6368 726f 6e69  r+.....synchroni
+00000640: 7a65 7272 1c00 0000 da14 7061 6972 6564  zerr......paired
+00000650: 5f66 7261 6d65 5f62 7569 6c64 6572 da12  _frame_builder..
+00000660: 5061 6972 6564 4672 616d 6545 6d69 7474  PairedFrameEmitt
+00000670: 6572 da14 7061 6972 6564 5f66 7261 6d65  er..paired_frame
+00000680: 5f65 6d69 7474 6572 da05 7374 6172 7472  _emitter..startr
+00000690: 0f00 0000 da0f 6672 616d 655f 7261 7465  ......frame_rate
+000006a0: 5f73 7069 6eda 0873 6574 5661 6c75 65da  _spin..setValue.
+000006b0: 0a66 7073 5f74 6172 6765 74da 1062 6f61  .fps_target..boa
+000006c0: 7264 5f63 6f75 6e74 5f73 7069 6e72 2d00  rd_count_spinr-.
+000006d0: 0000 7217 0000 00da 1473 7465 7265 6f5f  ..r......stereo_
+000006e0: 6672 616d 655f 6469 7370 6c61 7972 2100  frame_displayr!.
+000006f0: 0000 7227 0000 00da 0f70 6f73 7369 626c  ..r'.....possibl
+00000700: 655f 6163 7469 6f6e 7218 0000 00da 0576  e_actionr......v
+00000710: 616c 7565 da15 6361 6c69 6272 6174 655f  alue..calibrate_
+00000720: 636f 6c6c 6563 745f 6274 6eda 0d70 6c61  collect_btn..pla
+00000730: 6365 5f77 6964 6765 7473 da0f 636f 6e6e  ce_widgets..conn
+00000740: 6563 745f 7769 6467 6574 73da 1675 7064  ect_widgets..upd
+00000750: 6174 655f 6274 6e5f 656c 6967 6962 696c  ate_btn_eligibil
+00000760: 6974 7929 02da 0473 656c 6672 2b00 0000  ity)...selfr+...
+00000770: a901 da09 5f5f 636c 6173 735f 5f72 2800  ....__class__r(.
+00000780: 0000 7229 0000 0072 2f00 0000 3500 0000  ..r)...r/...5...
+00000790: 7320 0000 000e 0206 010a 0110 020c 010a  s ..............
+000007a0: 0108 0210 0108 0110 0108 0208 020e 0108  ................
+000007b0: 0208 010c 027a 2345 7874 7269 6e73 6963  .....z#Extrinsic
+000007c0: 4361 6c69 6272 6174 696f 6e57 6964 6765  CalibrationWidge
+000007d0: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
+000007e0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+000007f0: 0000 0073 2e00 0000 7400 a001 6401 a101  ...s....t...d...
+00000800: 0100 7c00 6a02 a003 a100 0100 7400 a001  ..|.j.......t...
+00000810: 6402 a101 0100 7c00 6a04 6a05 a006 a100  d.....|.j.j.....
+00000820: 0100 6403 5300 2904 611c 0100 000a 2020  ..d.S.).a.....  
+00000830: 2020 2020 2020 5468 6572 6520 6d61 7920        There may 
+00000840: 6265 2073 6f6d 6520 6c69 6e67 6572 696e  be some lingerin
+00000850: 6720 7468 7265 6164 7320 7275 6e6e 696e  g threads runnin
+00000860: 6720 7768 656e 2074 6865 2065 7874 7269  g when the extri
+00000870: 6e73 6963 2063 616c 6962 7261 746f 7220  nsic calibrator 
+00000880: 6c6f 7365 7320 666f 6375 730a 2020 2020  loses focus.    
+00000890: 2020 2020 5468 6973 206d 6179 2062 6520      This may be 
+000008a0: 6361 7573 696e 6720 7079 7468 6f6e 2074  causing python t
+000008b0: 6f20 6f76 6572 6c6f 6164 2061 6e64 2070  o overload and p
+000008c0: 7971 7420 746f 2073 6567 6661 756c 7420  yqt to segfault 
+000008d0: 6475 7269 6e67 2074 6865 2063 616c 6962  during the calib
+000008e0: 7261 7469 6f6e 2070 726f 6365 7373 0a20  ration process. 
+000008f0: 2020 2020 2020 2069 6620 4927 7665 206d         if I've m
+00000900: 6f76 6564 2066 726f 6d20 7468 6520 6578  oved from the ex
+00000910: 7472 696e 7369 6320 6361 6c69 6272 6174  trinsic calibrat
+00000920: 696f 6e20 7769 6467 6574 2074 6f20 6120  ion widget to a 
+00000930: 6469 6666 6572 656e 7420 6f6e 652e 2e2e  different one...
+00000940: 0a20 2020 2020 2020 207a 3155 6e73 7562  .        z1Unsub
+00000950: 7363 7269 6265 2070 6169 7265 6420 6672  scribe paired fr
+00000960: 616d 6520 6275 696c 6465 7220 6672 6f6d  ame builder from
+00000970: 2073 796e 6320 6e6f 7469 6365 7a35 7369   sync noticez5si
+00000980: 676e 616c 2070 6169 7265 6420 6672 616d  gnal paired fram
+00000990: 6520 656d 6974 7465 7220 746f 2073 746f  e emitter to sto
+000009a0: 7020 636f 6c6c 6563 7469 6e67 2066 7261  p collecting fra
+000009b0: 6d65 734e 2907 da06 6c6f 6767 6572 da04  mesN)...logger..
+000009c0: 696e 666f 7231 0000 00da 1d75 6e73 7562  infor1.....unsub
+000009d0: 7363 7269 6265 5f66 726f 6d5f 7379 6e63  scribe_from_sync
+000009e0: 6872 6f6e 697a 6572 7233 0000 00da 0f6b  hronizerr3.....k
+000009f0: 6565 705f 636f 6c6c 6563 7469 6e67 da05  eep_collecting..
+00000a00: 636c 6561 72a9 0172 4000 0000 7228 0000  clear..r@...r(..
+00000a10: 0072 2800 0000 7229 0000 00da 1073 6875  .r(...r).....shu
+00000a20: 7464 6f77 6e5f 7468 7265 6164 734e 0000  tdown_threadsN..
+00000a30: 0073 0800 0000 0a06 0a01 0a01 1001 7a2b  .s............z+
+00000a40: 4578 7472 696e 7369 6343 616c 6962 7261  ExtrinsicCalibra
+00000a50: 7469 6f6e 5769 6467 6574 2e73 6875 7464  tionWidget.shutd
+00000a60: 6f77 6e5f 7468 7265 6164 7363 0100 0000  own_threadsc....
+00000a70: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000a80: 4300 0000 732a 0000 007c 006a 00a0 01a1  C...s*...|.j....
+00000a90: 0072 0d7c 006a 02a0 0364 01a1 0101 0064  .r.|.j...d.....d
+00000aa0: 0053 007c 006a 02a0 0364 02a1 0101 0064  .S.|.j...d.....d
+00000ab0: 0053 0029 034e 5446 2904 722b 0000 00da  .S.).NTF).r+....
+00000ac0: 2169 735f 6578 7472 696e 7369 635f 6361  !is_extrinsic_ca
+00000ad0: 6c69 6272 6174 696f 6e5f 656c 6967 6962  libration_eligib
+00000ae0: 6c65 723c 0000 00da 0a73 6574 456e 6162  ler<.....setEnab
+00000af0: 6c65 6472 4800 0000 7228 0000 0072 2800  ledrH...r(...r(.
+00000b00: 0000 7229 0000 0072 3f00 0000 5900 0000  ..r)...r?...Y...
+00000b10: 7306 0000 000a 0110 0110 027a 3145 7874  s..........z1Ext
+00000b20: 7269 6e73 6963 4361 6c69 6272 6174 696f  rinsicCalibratio
+00000b30: 6e57 6964 6765 742e 7570 6461 7465 5f62  nWidget.update_b
+00000b40: 746e 5f65 6c69 6769 6269 6c69 7479 6301  tn_eligibilityc.
+00000b50: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000b60: 0000 0043 0000 0073 ca00 0000 7c00 a000  ...C...s....|...
+00000b70: 7401 8300 a101 0100 7402 6401 8301 7c00  t.......t.d...|.
+00000b80: 5f03 7c00 6a03 a000 7404 8300 a101 0100  _.|.j...t.......
+00000b90: 7c00 6a03 a005 a100 a006 7407 6402 8301  |.j.......t.d...
+00000ba0: a101 0100 7c00 6a03 a005 a100 a006 7c00  ....|.j.......|.
+00000bb0: 6a08 a101 0100 7c00 6a03 a005 a100 a006  j.....|.j.......
+00000bc0: 7407 6403 8301 a101 0100 7c00 6a03 a005  t.d.......|.j...
+00000bd0: a100 a006 7c00 6a09 a101 0100 7c00 a005  ....|.j.....|...
+00000be0: a100 a006 7c00 6a03 a101 0100 740a 8300  ....|.j.....t...
+00000bf0: 7c00 5f0b 7c00 6a0b a00c 740d 6a0e 6a0f  |._.|.j...t.j.j.
+00000c00: a101 0100 7c00 a005 a100 a006 7c00 6a0b  ....|.......|.j.
+00000c10: a101 0100 7c00 6a0b a010 7c00 6a11 a101  ....|.j...|.j...
+00000c20: 0100 7c00 a005 a100 a006 7c00 6a12 a101  ..|.......|.j...
+00000c30: 0100 6400 5300 2904 4e5a 0853 6574 7469  ..d.S.).NZ.Setti
+00000c40: 6e67 737a 0b46 7261 6d65 2052 6174 653a  ngsz.Frame Rate:
+00000c50: 7a13 5461 7267 6574 2042 6f61 7264 2043  z.Target Board C
+00000c60: 6f75 6e74 3a29 13da 0973 6574 4c61 796f  ount:)...setLayo
+00000c70: 7574 721a 0000 0072 1400 0000 5a0e 7365  utr....r....Z.se
+00000c80: 7474 696e 6773 5f67 726f 7570 7216 0000  ttings_groupr...
+00000c90: 00da 066c 6179 6f75 74da 0961 6464 5769  ...layout..addWi
+00000ca0: 6467 6574 7217 0000 0072 3500 0000 7238  dgetr....r5...r8
+00000cb0: 0000 0072 1000 0000 5a0b 7363 726f 6c6c  ...r....Z.scroll
+00000cc0: 5f61 7265 615a 1a73 6574 5665 7274 6963  _areaZ.setVertic
+00000cd0: 616c 5363 726f 6c6c 4261 7250 6f6c 6963  alScrollBarPolic
+00000ce0: 7972 0600 0000 5a0f 5363 726f 6c6c 4261  yr....Z.ScrollBa
+00000cf0: 7250 6f6c 6963 795a 1153 6372 6f6c 6c42  rPolicyZ.ScrollB
+00000d00: 6172 416c 7761 7973 4f6e da09 7365 7457  arAlwaysOn..setW
+00000d10: 6964 6765 7472 3900 0000 723c 0000 0072  idgetr9...r<...r
+00000d20: 4800 0000 7228 0000 0072 2800 0000 7229  H...r(...r(...r)
+00000d30: 0000 0072 3d00 0000 6000 0000 731a 0000  ...r=...`...s...
+00000d40: 000c 010a 020e 0114 0112 0114 0112 0110  ................
+00000d50: 0208 0410 0110 020e 0214 027a 2845 7874  ...........z(Ext
+00000d60: 7269 6e73 6963 4361 6c69 6272 6174 696f  rinsicCalibratio
+00000d70: 6e57 6964 6765 742e 706c 6163 655f 7769  nWidget.place_wi
+00000d80: 6467 6574 7363 0100 0000 0000 0000 0000  dgetsc..........
+00000d90: 0000 0100 0000 0300 0000 4300 0000 7366  ..........C...sf
+00000da0: 0000 007c 006a 006a 01a0 027c 006a 03a1  ...|.j.j...|.j..
+00000db0: 0101 007c 006a 046a 05a0 027c 006a 06a1  ...|.j.j...|.j..
+00000dc0: 0101 007c 006a 046a 07a0 027c 006a 08a1  ...|.j.j...|.j..
+00000dd0: 0101 007c 006a 096a 0aa0 027c 006a 0b6a  ...|.j.j...|.j.j
+00000de0: 0ca1 0101 007c 006a 0d6a 0aa0 027c 006a  .....|.j.j...|.j
+00000df0: 0ea1 0101 007c 006a 046a 0fa0 027c 006a  .....|.j.j...|.j
+00000e00: 10a1 0101 0064 0053 00a9 014e 2911 723c  .....d.S...N).r<
+00000e10: 0000 00da 0763 6c69 636b 6564 da07 636f  .....clicked..co
+00000e20: 6e6e 6563 74da 1a6f 6e5f 6361 6c69 6272  nnect..on_calibr
+00000e30: 6174 655f 636f 6c6c 6563 745f 636c 6963  ate_collect_clic
+00000e40: 6b72 3300 0000 da0e 496d 6167 6542 726f  kr3.....ImageBro
+00000e50: 6164 6361 7374 da0f 496d 6167 6555 7064  adcast..ImageUpd
+00000e60: 6174 6553 6c6f 74da 1c70 6f73 7369 626c  ateSlot..possibl
+00000e70: 655f 746f 5f69 6e69 7469 616c 697a 655f  e_to_initialize_
+00000e80: 6172 7261 79da 1265 6e61 626c 655f 6361  array..enable_ca
+00000e90: 6c69 6272 6174 696f 6e72 3500 0000 da0c  librationr5.....
+00000ea0: 7661 6c75 6543 6861 6e67 6564 7230 0000  valueChangedr0..
+00000eb0: 00da 0e73 6574 5f73 7472 6561 6d5f 6670  ...set_stream_fp
+00000ec0: 7372 3800 0000 da19 7570 6461 7465 5f62  sr8.....update_b
+00000ed0: 6f61 7264 5f63 6f75 6e74 5f74 6172 6765  oard_count_targe
+00000ee0: 74da 1a63 616c 6962 7261 7469 6f6e 5f64  t..calibration_d
+00000ef0: 6174 615f 636f 6c6c 6563 7465 64da 1469  ata_collected..i
+00000f00: 6e69 7469 6174 655f 6361 6c69 6272 6174  nitiate_calibrat
+00000f10: 696f 6e72 4800 0000 7228 0000 0072 2800  ionrH...r(...r(.
+00000f20: 0000 7229 0000 0072 3e00 0000 7900 0000  ..r)...r>...y...
+00000f30: 730c 0000 0010 0210 0110 0112 0110 0114  s...............
+00000f40: 017a 2a45 7874 7269 6e73 6963 4361 6c69  .z*ExtrinsicCali
+00000f50: 6272 6174 696f 6e57 6964 6765 742e 636f  brationWidget.co
+00000f60: 6e6e 6563 745f 7769 6467 6574 7363 0200  nnect_widgetsc..
+00000f70: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000f80: 0000 4300 0000 730c 0000 007c 017c 006a  ..C...s....|.|.j
+00000f90: 005f 0164 0053 0072 5000 0000 2902 7231  ._.d.S.rP...).r1
+00000fa0: 0000 0072 2d00 0000 2902 7240 0000 00da  ...r-...).r@....
+00000fb0: 0674 6172 6765 7472 2800 0000 7228 0000  .targetr(...r(..
+00000fc0: 0072 2900 0000 725a 0000 0082 0000 0073  .r)...rZ.......s
+00000fd0: 0200 0000 0c01 7a34 4578 7472 696e 7369  ......z4Extrinsi
+00000fe0: 6343 616c 6962 7261 7469 6f6e 5769 6467  cCalibrationWidg
+00000ff0: 6574 2e75 7064 6174 655f 626f 6172 645f  et.update_board_
+00001000: 636f 756e 745f 7461 7267 6574 6301 0000  count_targetc...
+00001010: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00001020: 0043 0000 0073 e600 0000 7c00 6a00 7401  .C...s....|.j.t.
+00001030: 6a02 6b02 723c 7403 a004 6401 a101 0100  j.k.r<t...d.....
+00001040: 7c00 6a05 6a06 a007 a100 0100 7408 7c00  |.j.j.......t.|.
+00001050: 6a09 6a0a 6402 6403 8303 7d01 7c00 6a09  j.j.d.d...}.|.j.
+00001060: 6a0b 7c01 6404 6405 8d02 0100 7401 6a0c  j.|.d.d.....t.j.
+00001070: 7c00 5f00 7c00 6a0d a00e 7c00 6a00 6a0f  |._.|.j...|.j.j.
+00001080: a101 0100 7c00 6a0d a010 6404 a101 0100  ....|.j...d.....
+00001090: 7c00 6a11 6a12 a010 6406 a101 0100 6400  |.j.j...d.....d.
+000010a0: 5300 7c00 6a00 7401 6a0c 6b02 725a 7403  S.|.j.t.j.k.rZt.
+000010b0: a004 6407 a101 0100 7c00 6a13 a014 a100  ..d.....|.j.....
+000010c0: 0100 7401 6a02 7c00 5f00 7c00 6a0d a00e  ..t.j.|._.|.j...
+000010d0: 7c00 6a00 6a0f a101 0100 6400 5300 7c00  |.j.j.....d.S.|.
+000010e0: 6a00 7401 6a15 6b02 7271 7403 a004 6408  j.t.j.k.rqt...d.
+000010f0: a101 0100 7c00 6a05 6a06 a016 a100 0100  ....|.j.j.......
+00001100: 7c00 a017 a100 0100 6400 5300 6400 5300  |.......d.S.d.S.
+00001110: 2909 4e7a 2142 6567 696e 2063 6f6c 6c65  ).Nz!Begin colle
+00001120: 6374 696e 6720 6361 6c69 6272 6174 696f  cting calibratio
+00001130: 6e20 6461 7461 da0b 6361 6c69 6272 6174  n data..calibrat
+00001140: 696f 6eda 0965 7874 7269 6e73 6963 5429  ion..extrinsicT)
+00001150: 01da 1373 746f 7265 5f70 6f69 6e74 5f68  ...store_point_h
+00001160: 6973 746f 7279 467a 2354 6572 6d69 6e61  istoryFz#Termina
+00001170: 7469 6e67 2063 7572 7265 6e74 2064 6174  ting current dat
+00001180: 6120 636f 6c6c 6563 7469 6f6e 7a37 5072  a collectionz7Pr
+00001190: 656d 6174 7572 656c 7920 656e 6420 6461  ematurely end da
+000011a0: 7461 2063 6f6c 6c65 6374 696f 6e20 746f  ta collection to
+000011b0: 2069 6e69 7469 6174 6520 6361 6c69 6272   initiate calibr
+000011c0: 6174 696f 6e29 1872 3a00 0000 7221 0000  ation).r:...r!..
+000011d0: 0072 2700 0000 7243 0000 0072 4400 0000  .r'...rC...rD...
+000011e0: 7231 0000 005a 0c73 746f 7265 5f70 6f69  r1...Z.store_poi
+000011f0: 6e74 73da 0373 6574 7202 0000 0072 2b00  nts..setr....r+.
+00001200: 0000 da04 7061 7468 da0f 7374 6172 745f  ....path..start_
+00001210: 7265 636f 7264 696e 6772 2200 0000 723c  recordingr"...r<
+00001220: 0000 00da 0773 6574 5465 7874 723b 0000  .....setTextr;..
+00001230: 0072 4b00 0000 da0e 6e61 7669 6761 7469  .rK.....navigati
+00001240: 6f6e 5f62 6172 da08 6261 636b 5f62 746e  on_bar..back_btn
+00001250: da09 7465 726d 696e 6174 65da 0465 6d69  ..terminate..emi
+00001260: 7472 2300 0000 7247 0000 0072 5c00 0000  tr#...rG...r\...
+00001270: 2902 7240 0000 005a 1a65 7874 7269 6e73  ).r@...Z.extrins
+00001280: 6963 5f63 616c 6962 7261 7469 6f6e 5f70  ic_calibration_p
+00001290: 6174 6872 2800 0000 7228 0000 0072 2900  athr(...r(...r).
+000012a0: 0000 7253 0000 0085 0000 0073 2600 0000  ..rS.......s&...
+000012b0: 0c01 0a01 0c02 1001 1001 0801 1001 0c01  ................
+000012c0: 1201 0c02 0a01 0a01 0801 1401 0c02 0a01  ................
+000012d0: 0c01 0c01 04fd 7a35 4578 7472 696e 7369  ......z5Extrinsi
+000012e0: 6343 616c 6962 7261 7469 6f6e 5769 6467  cCalibrationWidg
+000012f0: 6574 2e6f 6e5f 6361 6c69 6272 6174 655f  et.on_calibrate_
+00001300: 636f 6c6c 6563 745f 636c 6963 6b63 0100  collect_clickc..
+00001310: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00001320: 0000 4300 0000 7328 0000 0074 006a 017c  ..C...s(...t.j.|
+00001330: 005f 027c 006a 03a0 047c 006a 026a 05a1  ._.|.j...|.j.j..
+00001340: 0101 007c 006a 03a0 0664 01a1 0101 0064  ...|.j...d.....d
+00001350: 0053 0029 024e 5429 0772 2100 0000 7223  .S.).NT).r!...r#
+00001360: 0000 0072 3a00 0000 723c 0000 0072 6400  ...r:...r<...rd.
+00001370: 0000 723b 0000 0072 4b00 0000 7248 0000  ..r;...rK...rH..
+00001380: 0072 2800 0000 7228 0000 0072 2900 0000  .r(...r(...r)...
+00001390: 7257 0000 009e 0000 0073 0600 0000 0801  rW.......s......
+000013a0: 1001 1001 7a2d 4578 7472 696e 7369 6343  ....z-ExtrinsicC
+000013b0: 616c 6962 7261 7469 6f6e 5769 6467 6574  alibrationWidget
+000013c0: 2e65 6e61 626c 655f 6361 6c69 6272 6174  .enable_calibrat
+000013d0: 696f 6e63 0200 0000 0000 0000 0000 0000  ionc............
+000013e0: 0300 0000 0400 0000 4300 0000 732c 0000  ........C...s,..
+000013f0: 007c 006a 00a0 017c 006a 00a0 02a1 00a1  .|.j...|.j......
+00001400: 0101 0074 03a0 047c 01a1 017d 027c 006a  ...t...|...}.|.j
+00001410: 00a0 057c 02a1 0101 0064 0053 0072 5000  ...|.....d.S.rP.
+00001420: 0000 2906 7239 0000 00da 0672 6573 697a  ..).r9.....resiz
+00001430: 655a 0873 697a 6548 696e 7472 0a00 0000  eZ.sizeHintr....
+00001440: da09 6672 6f6d 496d 6167 65da 0973 6574  ..fromImage..set
+00001450: 5069 786d 6170 2903 7240 0000 005a 0771  Pixmap).r@...Z.q
+00001460: 5f69 6d61 6765 5a07 7170 6978 6d61 7072  _imageZ.qpixmapr
+00001470: 2800 0000 7228 0000 0072 2900 0000 7255  (...r(...r)...rU
+00001480: 0000 00a4 0000 0073 0600 0000 1201 0a02  .......s........
+00001490: 1001 7a2a 4578 7472 696e 7369 6343 616c  ..z*ExtrinsicCal
+000014a0: 6962 7261 7469 6f6e 5769 6467 6574 2e49  ibrationWidget.I
+000014b0: 6d61 6765 5570 6461 7465 536c 6f74 6301  mageUpdateSlotc.
+000014c0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+000014d0: 0000 0003 0000 0073 2a00 0000 8700 6601  .......s*.....f.
+000014e0: 6401 6402 8408 7d01 7400 7c01 6403 6404  d.d...}.t.|.d.d.
+000014f0: 6405 8d03 8800 5f01 8800 6a01 a002 a100  d....._...j.....
+00001500: 0100 6400 5300 2906 4e63 0000 0000 0000  ..d.S.).Nc......
+00001510: 0000 0000 0000 0000 0000 0300 0000 1300  ................
+00001520: 0000 73a4 0000 0088 006a 00a0 01a1 0001  ..s......j......
+00001530: 0074 02a0 0364 01a1 0101 0088 006a 04a0  .t...d.......j..
+00001540: 0564 02a1 0101 0088 006a 04a0 0664 03a1  .d.......j...d..
+00001550: 0101 0074 02a0 0364 04a1 0101 0088 006a  ...t...d.......j
+00001560: 07a0 08a1 0001 0074 02a0 0364 05a1 0101  .......t...d....
+00001570: 0074 02a0 0364 06a1 0101 0088 006a 07a0  .t...d.......j..
+00001580: 09a1 0001 0088 006a 07a0 0aa1 0001 0074  .......j.......t
+00001590: 0b6a 0c88 005f 0d88 006a 04a0 0588 006a  .j..._...j.....j
+000015a0: 0d6a 0ea1 0101 0088 006a 04a0 0664 07a1  .j.......j...d..
+000015b0: 0101 0088 006a 0fa0 01a1 0001 0074 02a0  .....j.......t..
+000015c0: 0364 08a1 0101 0064 0053 0029 094e 7a30  .d.....d.S.).Nz0
+000015d0: 4265 6769 6e6e 696e 6720 7769 6e64 2d64  Beginning wind-d
+000015e0: 6f77 6e20 7072 6f63 6573 7320 7072 696f  own process prio
+000015f0: 7220 746f 2063 616c 6962 7261 7469 6f6e  r to calibration
+00001600: 7a11 2d2d 2d63 616c 6962 7261 7469 6e67  z.---calibrating
+00001610: 2d2d 2d46 7a14 5374 6f70 2072 6563 6f72  ---Fz.Stop recor
+00001620: 6469 6e67 2076 6964 656f 7a11 4265 6769  ding videoz.Begi
+00001630: 6e20 6361 6c69 6272 6174 696f 6e7a 1250  n calibrationz.P
+00001640: 6175 7365 2073 796e 6368 726f 6e69 7a65  ause synchronize
+00001650: 7254 7a23 4361 6c69 6272 6174 696f 6e20  rTz#Calibration 
+00001660: 436f 6d70 6c65 7465 2073 6967 6e61 6c20  Complete signal 
+00001670: 7365 6e74 2e2e 2e29 10da 1563 616c 6962  sent...)...calib
+00001680: 7261 7469 6f6e 5f69 6e69 7469 6174 6564  ration_initiated
+00001690: 7268 0000 0072 4300 0000 7244 0000 0072  rh...rC...rD...r
+000016a0: 3c00 0000 7264 0000 0072 4b00 0000 722b  <...rd...rK...r+
+000016b0: 0000 00da 0e73 746f 705f 7265 636f 7264  .....stop_record
+000016c0: 696e 67da 1270 6175 7365 5f73 796e 6368  ing..pause_synch
+000016d0: 726f 6e69 7a65 72da 1365 7374 696d 6174  ronizer..estimat
+000016e0: 655f 6578 7472 696e 7369 6373 7221 0000  e_extrinsicsr!..
+000016f0: 0072 2700 0000 723a 0000 0072 3b00 0000  .r'...r:...r;...
+00001700: da14 6361 6c69 6272 6174 696f 6e5f 636f  ..calibration_co
+00001710: 6d70 6c65 7465 7228 0000 0072 4800 0000  mpleter(...rH...
+00001720: 7228 0000 0072 2900 0000 da06 776f 726b  r(...r).....work
+00001730: 6572 ad00 0000 731e 0000 000a 010a 010c  er....s.........
+00001740: 010c 010a 030a 010a 010a 010a 010a 0108  ................
+00001750: 0210 010c 010a 010e 017a 3f45 7874 7269  .........z?Extri
+00001760: 6e73 6963 4361 6c69 6272 6174 696f 6e57  nsicCalibrationW
+00001770: 6964 6765 742e 696e 6974 6961 7465 5f63  idget.initiate_c
+00001780: 616c 6962 7261 7469 6f6e 2e3c 6c6f 6361  alibration.<loca
+00001790: 6c73 3e2e 776f 726b 6572 7228 0000 0054  ls>.workerr(...T
+000017a0: 2903 725d 0000 00da 0461 7267 73da 0664  ).r].....args..d
+000017b0: 6165 6d6f 6e29 0372 0300 0000 5a17 696e  aemon).r....Z.in
+000017c0: 6974 5f63 616c 6962 7261 7469 6f6e 5f74  it_calibration_t
+000017d0: 6872 6561 6472 3400 0000 2902 7240 0000  hreadr4...).r@..
+000017e0: 0072 7100 0000 7228 0000 0072 4800 0000  .rq...r(...rH...
+000017f0: 7229 0000 0072 5c00 0000 ac00 0000 7306  r)...r\.......s.
+00001800: 0000 000c 0110 140e 017a 2f45 7874 7269  .........z/Extri
+00001810: 6e73 6963 4361 6c69 6272 6174 696f 6e57  nsicCalibrationW
+00001820: 6964 6765 742e 696e 6974 6961 7465 5f63  idget.initiate_c
+00001830: 616c 6962 7261 7469 6f6e 2913 7224 0000  alibration).r$..
+00001840: 0072 2500 0000 7226 0000 0072 0700 0000  .r%...r&...r....
+00001850: 7270 0000 0072 6c00 0000 7267 0000 0072  rp...rl...rg...r
+00001860: 1b00 0000 722f 0000 0072 4900 0000 723f  ....r/...rI...r?
+00001870: 0000 0072 3d00 0000 723e 0000 0072 5a00  ...r=...r>...rZ.
+00001880: 0000 7253 0000 0072 5700 0000 7255 0000  ..rS...rW...rU..
+00001890: 0072 5c00 0000 da0d 5f5f 636c 6173 7363  .r\.....__classc
+000018a0: 656c 6c5f 5f72 2800 0000 7228 0000 0072  ell__r(...r(...r
+000018b0: 4100 0000 7229 0000 0072 2a00 0000 3000  A...r)...r*...0.
+000018c0: 0000 731c 0000 0008 0006 0106 0106 0112  ..s.............
+000018d0: 0208 1908 0b08 0708 1908 0908 0308 1908  ................
+000018e0: 0610 0872 2a00 0000 6300 0000 0000 0000  ...r*...c.......
+000018f0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00001900: 0073 3e00 0000 6500 5a01 6400 5a02 6503  .s>...e.Z.d.Z.e.
+00001910: 6504 8301 5a05 6503 8300 5a06 6503 8300  e...Z.e...Z.e...
+00001920: 5a07 6401 6508 6602 8700 6601 6402 6403  Z.d.e.f...f.d.d.
+00001930: 840c 5a09 6404 6405 8400 5a0a 8700 0400  ..Z.d.d...Z.....
+00001940: 5a0b 5300 2906 7232 0000 0072 3100 0000  Z.S.).r2...r1...
+00001950: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001960: 0003 0000 0003 0000 0073 3000 0000 7400  .........s0...t.
+00001970: 7401 7c00 8302 a002 a100 0100 7c01 7c00  t.|.........|.|.
+00001980: 5f03 7404 a005 6401 a101 0100 7406 8300  _.t...d.....t...
+00001990: 7c00 5f07 6402 7c00 5f08 6400 5300 2903  |._.d.|._.d.S.).
+000019a0: 4e7a 1749 6e69 7469 6174 6564 2066 7261  Nz.Initiated fra
+000019b0: 6d65 2065 6d69 7474 6572 4629 0972 2e00  me emitterF).r..
+000019c0: 0000 7232 0000 0072 2f00 0000 7231 0000  ..r2...r/...r1..
+000019d0: 0072 4300 0000 7244 0000 0072 0400 0000  .rC...rD...r....
+000019e0: 7246 0000 00da 1363 6f6c 6c65 6374 696f  rF.....collectio
+000019f0: 6e5f 636f 6d70 6c65 7465 2902 7240 0000  n_complete).r@..
+00001a00: 0072 3100 0000 7241 0000 0072 2800 0000  .r1...rA...r(...
+00001a10: 7229 0000 0072 2f00 0000 c900 0000 730a  r)...r/.......s.
+00001a20: 0000 000e 0206 010a 0108 010a 017a 1b50  .............z.P
+00001a30: 6169 7265 6446 7261 6d65 456d 6974 7465  airedFrameEmitte
+00001a40: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
+00001a50: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+00001a60: 0000 0073 b400 0000 7c00 6a00 a001 a100  ...s....|.j.....
+00001a70: 0100 6401 7c00 5f02 6401 7d01 7c00 6a00  ..d.|._.d.}.|.j.
+00001a80: a003 a100 7253 7404 7c00 6a05 6a06 8301  ....rSt.|.j.j...
+00001a90: 6402 6b02 7227 7c00 6a02 7327 7407 a008  d.k.r'|.j.s't...
+00001aa0: 6403 a101 0100 6404 7c00 5f02 7c00 6a09  d.....d.|._.|.j.
+00001ab0: a00a a100 0100 7c01 733b 7c00 6a05 a00b  ......|.s;|.j...
+00001ac0: 740c a101 723b 7407 a008 6405 a101 0100  t...r;t...d.....
+00001ad0: 6404 7d01 7c00 6a0b a00a a100 0100 7c00  d.}.|.j.......|.
+00001ae0: 6a05 a00d a100 7d02 7c02 6400 7501 724e  j.....}.|.d.u.rN
+00001af0: 740e 7c02 8301 7d03 7c00 6a0f a00a 7c03  t.|...}.|.j...|.
+00001b00: a101 0100 7c00 6a00 a003 a100 730f 7407  ....|.j.....s.t.
+00001b10: a008 6406 a101 0100 6400 5300 2907 4e46  ..d.....d.S.).NF
+00001b20: 7201 0000 007a 3453 6967 6e61 6c6c 696e  r....z4Signallin
+00001b30: 6720 7468 6174 2063 616c 6962 7261 7469  g that calibrati
+00001b40: 6f6e 2064 6174 6120 6973 2066 756c 6c79  on data is fully
+00001b50: 2063 6f6c 6c65 6374 6564 2e54 7a4a 5369   collected.TzJSi
+00001b60: 676e 616c 696e 6720 7468 6174 2069 7420  gnaling that it 
+00001b70: 6973 2070 6f73 7369 626c 6520 746f 2069  is possible to i
+00001b80: 6e69 7469 616c 697a 6520 6172 7261 7920  nitialize array 
+00001b90: 6261 7365 6420 6f6e 2063 6f6c 6c65 6374  based on collect
+00001ba0: 6564 2064 6174 612e 7a27 5374 6572 656f  ed data.z'Stereo
+00001bb0: 6672 616d 6520 656d 6974 7465 7220 7275  frame emitter ru
+00001bc0: 6e20 7468 7265 6164 2065 6e64 6564 2e2e  n thread ended..
+00001bd0: 2e29 1072 4600 0000 7261 0000 0072 7500  .).rF...ra...ru.
+00001be0: 0000 da06 6973 5f73 6574 da03 6c65 6e72  ....is_set..lenr
+00001bf0: 3100 0000 5a0b 7374 6572 656f 5f6c 6973  1...Z.stereo_lis
+00001c00: 7472 4300 0000 7244 0000 0072 5b00 0000  trC...rD...r[...
+00001c10: 7268 0000 0072 5600 0000 da21 4d49 4e5f  rh...rV....!MIN_
+00001c20: 5448 5245 5348 4f4c 445f 464f 525f 4541  THRESHOLD_FOR_EA
+00001c30: 524c 595f 4341 4c49 4252 4154 455a 1067  RLY_CALIBRATEZ.g
+00001c40: 6574 5f73 7465 7265 6f5f 6672 616d 65da  et_stereo_frame.
+00001c50: 0d63 7632 5f74 6f5f 716c 6162 656c 7254  .cv2_to_qlabelrT
+00001c60: 0000 0029 0472 4000 0000 5a16 706f 7373  ...).r@...Z.poss
+00001c70: 6962 6c65 5f74 6f5f 696e 6974 6961 6c69  ible_to_initiali
+00001c80: 7a65 5a0c 7374 6572 656f 5f66 7261 6d65  zeZ.stereo_frame
+00001c90: da05 696d 6167 6572 2800 0000 7228 0000  ..imager(...r(..
+00001ca0: 0072 2900 0000 da03 7275 6ed1 0000 0073  .r).....run....s
+00001cb0: 2600 0000 0a02 0601 0402 0a02 1604 0a01  &...............
+00001cc0: 0601 0a01 0404 0c02 0a01 0401 0a01 0a02  ................
+00001cd0: 0802 0801 0c01 0aea 0e18 7a16 5061 6972  ..........z.Pair
+00001ce0: 6564 4672 616d 6545 6d69 7474 6572 2e72  edFrameEmitter.r
+00001cf0: 756e 290c 7224 0000 0072 2500 0000 7226  un).r$...r%...r&
+00001d00: 0000 0072 0700 0000 7209 0000 0072 5400  ...r....r....rT.
+00001d10: 0000 725b 0000 0072 5600 0000 721c 0000  ..r[...rV...r...
+00001d20: 0072 2f00 0000 727b 0000 0072 7400 0000  .r/...r{...rt...
+00001d30: 7228 0000 0072 2800 0000 7241 0000 0072  r(...r(...rA...r
+00001d40: 2900 0000 7232 0000 00c4 0000 0073 0c00  )...r2.......s..
+00001d50: 0000 0800 0801 0601 0601 1202 1008 7232  ..............r2
+00001d60: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001d70: 0300 0000 0500 0000 4300 0000 7332 0000  ........C...s2..
+00001d80: 0074 00a0 017c 0074 006a 02a1 027d 0174  .t...|.t.j...}.t
+00001d90: 037c 016a 047c 016a 0564 0119 007c 016a  .|.j.|.j.d...|.j
+00001da0: 0564 0219 0074 036a 066a 0783 047d 027c  .d...t.j.j...}.|
+00001db0: 0253 0029 034e e901 0000 0072 0100 0000  .S.).N.....r....
+00001dc0: 2908 da03 6376 32da 0863 7674 436f 6c6f  )...cv2..cvtColo
+00001dd0: 72da 0d43 4f4c 4f52 5f42 4752 3252 4742  r..COLOR_BGR2RGB
+00001de0: 7209 0000 00da 0464 6174 61da 0573 6861  r......data..sha
+00001df0: 7065 da06 466f 726d 6174 da0d 466f 726d  pe..Format..Form
+00001e00: 6174 5f52 4742 3838 3829 03da 0566 7261  at_RGB888)...fra
+00001e10: 6d65 727a 0000 00da 0871 745f 6672 616d  merz.....qt_fram
+00001e20: 6572 2800 0000 7228 0000 0072 2900 0000  er(...r(...r)...
+00001e30: 7279 0000 00f9 0000 0073 1000 0000 0e01  ry.......s......
+00001e40: 0202 0401 0801 0801 0601 04fc 0406 7279  ..............ry
+00001e50: 0000 00da 085f 5f6d 6169 6e5f 5f29 01da  .....__main__)..
+00001e60: 0c43 6f6e 6669 6775 7261 746f 7229 01da  .Configurator)..
+00001e70: 0e43 6861 7275 636f 5472 6163 6b65 72da  .CharucoTracker.
+00001e80: 0364 6576 5a0f 7361 6d70 6c65 5f73 6573  .devZ.sample_ses
+00001e90: 7369 6f6e 735a 0332 3537 2901 da07 7472  sionsZ.257)...tr
+00001ea0: 6163 6b65 7229 45da 0d70 7978 7933 642e  acker)E..pyxy3d.
+00001eb0: 6c6f 6767 6572 da06 7079 7879 3364 7243  logger..pyxy3drC
+00001ec0: 0000 00da 0367 6574 7224 0000 00da 0373  .....getr$.....s
+00001ed0: 7973 da07 7061 7468 6c69 6272 0200 0000  ys..pathlibr....
+00001ee0: da09 7468 7265 6164 696e 6772 0300 0000  ..threadingr....
+00001ef0: 7204 0000 00da 0474 696d 65da 0465 6e75  r......time..enu
+00001f00: 6d72 0500 0000 727d 0000 00da 0c50 7951  mr....r}.....PyQ
+00001f10: 7436 2e51 7443 6f72 6572 0600 0000 7207  t6.QtCorer....r.
+00001f20: 0000 0072 0800 0000 da0b 5079 5174 362e  ...r......PyQt6.
+00001f30: 5174 4775 6972 0900 0000 720a 0000 0072  QtGuir....r....r
+00001f40: 0b00 0000 da0f 5079 5174 362e 5174 5769  ......PyQt6.QtWi
+00001f50: 6467 6574 7372 0c00 0000 720d 0000 0072  dgetsr....r....r
+00001f60: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00001f70: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00001f80: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001f90: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00001fa0: da16 7079 7879 3364 2e73 6573 7369 6f6e  ..pyxy3d.session
+00001fb0: 2e73 6573 7369 6f6e 721b 0000 005a 2e70  .sessionr....Z.p
+00001fc0: 7978 7933 642e 6775 692e 6672 616d 655f  yxy3d.gui.frame_
+00001fd0: 6275 696c 6465 7273 2e70 6169 7265 645f  builders.paired_
+00001fe0: 6672 616d 655f 6275 696c 6465 7272 1c00  frame_builderr..
+00001ff0: 0000 da1b 7079 7879 3364 2e63 616d 6572  ....pyxy3d.camer
+00002000: 6173 2e73 796e 6368 726f 6e69 7a65 7272  as.synchronizerr
+00002010: 1d00 0000 721e 0000 00da 1a70 7978 7933  ....r......pyxy3
+00002020: 642e 6775 692e 6e61 7669 6761 7469 6f6e  d.gui.navigation
+00002030: 5f62 6172 7372 1f00 0000 7278 0000 0072  _barsr....rx...r
+00002040: 2100 0000 722a 0000 0072 3200 0000 7279  !...r*...r2...ry
+00002050: 0000 00da 1370 7978 7933 642e 636f 6e66  .....pyxy3d.conf
+00002060: 6967 7572 6174 6f72 7287 0000 00da 1f70  iguratorr......p
+00002070: 7978 7933 642e 7472 6163 6b65 7273 2e63  yxy3d.trackers.c
+00002080: 6861 7275 636f 5f74 7261 636b 6572 7288  haruco_trackerr.
+00002090: 0000 00da 0461 7267 76da 0341 7070 da0c  .....argv..App..
+000020a0: 7365 7373 696f 6e5f 7061 7468 da0c 636f  session_path..co
+000020b0: 6e66 6967 7572 6174 6f72 722b 0000 00da  nfiguratorr+....
+000020c0: 0763 6861 7275 636f 728a 0000 00da 116c  .charucor......l
+000020d0: 6f61 645f 7374 7265 616d 5f74 6f6f 6c73  oad_stream_tools
+000020e0: 5a0d 7374 6572 656f 5f64 6961 6c6f 67da  Z.stereo_dialog.
+000020f0: 0473 686f 77da 0465 7869 74da 0465 7865  .show..exit..exe
+00002100: 6372 2800 0000 7228 0000 0072 2800 0000  cr(...r(...r(...
+00002110: 7229 0000 00da 083c 6d6f 6475 6c65 3e01  r).....<module>.
+00002120: 0000 0073 4600 0000 0801 0c01 0802 0c01  ...sF...........
+00002130: 1001 0801 0c01 0802 1401 1401 4401 0c13  ............D...
+00002140: 0c01 0c01 0c01 0c01 0403 1003 1005 007f  ................
+00002150: 1015 0835 080c 0c01 0c01 0a02 0e02 0801  ...5............
+00002160: 0802 0a02 0c01 0803 0801 1202 04ee       ..............
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 16:49:05 2023 UTC, .py size: 14273 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 814c 8764 c137 0000  o........L.d.7..
+00000000: 6f0d 0d0a 0000 0000 0556 8b64 af3e 0000  o........V.d.>..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 9201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c00 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: 6a02 a003 6504 a101 5a02 6400 6402 6c05  j...e...Z.d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6501  m.Z.m.Z.m.Z...e.
 00000060: 6a02 a003 6504 a101 5a02 6400 6403 6c09  j...e...Z.d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000080: 0100 6400 6401 6c0d 5a0d 6400 6405 6c05  ..d.d.l.Z.d.d.l.
 00000090: 6d0e 5a0e 6d06 5a06 6d07 5a07 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
@@ -19,620 +19,714 @@
 00000120: 640c 6c27 6d28 5a28 0100 6400 640d 6c29  d.l'm(Z(..d.d.l)
 00000130: 6d2a 5a2a 0100 6400 640e 6c2b 6d2c 5a2c  m*Z*..d.d.l+m,Z,
 00000140: 0100 6400 640f 6c2d 6d2e 5a2e 0100 6400  ..d.d.l-m.Z...d.
 00000150: 6410 6c2f 6d30 5a30 0100 6400 6411 6c31  d.l/m0Z0..d.d.l1
 00000160: 6d32 5a32 0100 6400 6412 6c33 6d34 5a34  m2Z2..d.d.l3m4Z4
 00000170: 0100 4700 6413 6414 8400 6414 6517 8303  ..G.d.d...d.e...
 00000180: 5a35 4700 6415 6416 8400 6416 6506 8303  Z5G.d.d...d.e...
-00000190: 5a36 6417 6418 8400 5a37 6504 6419 6b02  Z6d.d...Z7e.d.k.
-000001a0: 72bf 6537 8300 0100 6401 5300 6401 5300  r.e7....d.S.d.S.
-000001b0: 291a e900 0000 004e 2903 da0b 514d 6169  )......N)...QMai
-000001c0: 6e57 696e 646f 77da 0e51 5374 6163 6b65  nWindow..QStacke
-000001d0: 644c 6179 6f75 74da 0b51 4669 6c65 4469  dLayout..QFileDi
-000001e0: 616c 6f67 2901 da04 5061 7468 2901 da06  alog)...Path)...
-000001f0: 5468 7265 6164 2909 da0c 5141 7070 6c69  Thread)...QAppli
-00000200: 6361 7469 6f6e 7202 0000 0072 0300 0000  cationr....r....
-00000210: da07 5157 6964 6765 74da 0b51 446f 636b  ..QWidget..QDock
-00000220: 5769 6467 6574 da0b 5156 426f 784c 6179  Widget..QVBoxLay
-00000230: 6f75 74da 0551 4d65 6e75 da08 514d 656e  out..QMenu..QMen
-00000240: 7542 6172 da0a 5154 6162 5769 6467 6574  uBar..QTabWidget
-00000250: 2901 da04 456e 756d 2904 da05 5149 636f  )...Enum)...QIco
-00000260: 6eda 0751 4163 7469 6f6e da0c 514b 6579  n..QAction..QKey
-00000270: 5365 7175 656e 6365 da09 5153 686f 7274  Sequence..QShort
-00000280: 6375 7429 01da 0251 7429 03da 085f 5f72  cut)...Qt)...__r
-00000290: 6f6f 745f 5fda 115f 5f73 6574 7469 6e67  oot__..__setting
-000002a0: 735f 7061 7468 5f5f da0c 5f5f 7573 6572  s_path__..__user
-000002b0: 5f64 6972 5f5f 2902 da07 5365 7373 696f  _dir__)...Sessio
-000002c0: 6eda 0b53 6573 7369 6f6e 4d6f 6465 2901  n..SessionMode).
-000002d0: da09 4c6f 6757 6964 6765 7429 01da 0c43  ..LogWidget)...C
-000002e0: 6f6e 6669 6775 7261 746f 7229 01da 1143  onfigurator)...C
-000002f0: 616c 6962 7261 7469 6f6e 5769 6467 6574  alibrationWidget
-00000300: 2901 da0d 4368 6172 7563 6f57 6964 6765  )...CharucoWidge
-00000310: 7429 01da 1a49 6e74 7269 6e73 6963 4361  t)...IntrinsicCa
-00000320: 6c69 6272 6174 696f 6e57 6964 6765 7429  librationWidget)
-00000330: 01da 1c43 616c 6962 7261 7465 4361 7074  ...CalibrateCapt
-00000340: 7572 6556 6f6c 756d 6557 6964 6765 7429  ureVolumeWidget)
-00000350: 01da 0f52 6563 6f72 6469 6e67 5769 6467  ...RecordingWidg
-00000360: 6574 2901 da14 506f 7374 5072 6f63 6573  et)...PostProces
-00000370: 7369 6e67 5769 6467 6574 6300 0000 0000  singWidgetc.....
-00000380: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00000390: 0000 0073 2000 0000 6500 5a01 6400 5a02  ...s ...e.Z.d.Z.
-000003a0: 6401 5a03 6402 5a04 6403 5a05 6404 5a06  d.Z.d.Z.d.Z.d.Z.
-000003b0: 6405 5a07 6406 5300 2907 da08 5461 6249  d.Z.d.S.)...TabI
-000003c0: 6e64 6578 7201 0000 00e9 0100 0000 e902  ndexr...........
-000003d0: 0000 00e9 0300 0000 e904 0000 004e 2908  .............N).
-000003e0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000003f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000400: 6d65 5f5f da07 4368 6172 7563 6fda 0743  me__..Charuco..C
-00000410: 616d 6572 6173 da0d 4361 7074 7572 6556  ameras..CaptureV
-00000420: 6f6c 756d 65da 0952 6563 6f72 6469 6e67  olume..Recording
-00000430: da0a 5072 6f63 6573 7369 6e67 a900 722e  ..Processing..r.
-00000440: 0000 0072 2e00 0000 fa3a 433a 5c55 7365  ...r.....:C:\Use
-00000450: 7273 5c4d 6163 2050 7269 626c 655c 7265  rs\Mac Prible\re
-00000460: 706f 735c 7079 7879 3364 5c70 7978 7933  pos\pyxy3d\pyxy3
-00000470: 645c 6775 695c 6d61 696e 5f77 6964 6765  d\gui\main_widge
-00000480: 742e 7079 7221 0000 0029 0000 0073 0c00  t.pyr!...)...s..
-00000490: 0000 0800 0401 0401 0401 0401 0801 7221  ..............r!
-000004a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000004b0: 0000 0000 0300 0000 0000 0000 73a8 0000  ............s...
-000004c0: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
-000004d0: 0284 085a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
-000004e0: 0684 005a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
-000004f0: 0a84 005a 0764 0b65 0866 0264 0c64 0d84  ...Z.d.e.f.d.d..
-00000500: 045a 0964 0e64 0f84 005a 0a64 1064 1184  .Z.d.d...Z.d.d..
-00000510: 005a 0b64 1264 1384 005a 0c64 1464 1584  .Z.d.d...Z.d.d..
-00000520: 005a 0d64 1664 1784 005a 0e64 1864 1984  .Z.d.d...Z.d.d..
-00000530: 005a 0f64 1a65 0866 0264 1b64 1c84 045a  .Z.d.e.f.d.d...Z
-00000540: 1064 1d64 1e84 005a 1164 1f64 2084 005a  .d.d...Z.d.d ..Z
-00000550: 1264 2164 2284 005a 1364 2364 2484 005a  .d!d"..Z.d#d$..Z
-00000560: 1487 0004 005a 1553 0029 25da 0a4d 6169  .....Z.S.)%..Mai
-00000570: 6e57 696e 646f 7763 0100 0000 0000 0000  nWindowc........
-00000580: 0000 0000 0200 0000 0700 0000 0300 0000  ................
-00000590: 73aa 0100 0074 0074 017c 0083 02a0 02a1  s....t.t.|......
-000005a0: 0001 0074 03a0 0474 05a1 017c 005f 067c  ...t...t...|._.|
-000005b0: 00a0 0764 01a1 0101 007c 00a0 0874 0974  ...d.....|...t.t
-000005c0: 0a74 0b74 0c64 0283 0283 0183 01a1 0101  .t.t.d..........
-000005d0: 007c 00a0 0d64 0364 03a1 0201 007c 00a0  .|...d.d.....|..
-000005e0: 0ea1 007c 005f 0f7c 006a 0fa0 1064 04a1  ...|._.|.j...d..
-000005f0: 017c 005f 1174 1264 057c 0083 027c 005f  .|._.t.d.|...|._
-00000600: 137c 006a 136a 14a0 157c 006a 16a1 0101  .|.j.j...|.j....
-00000610: 007c 006a 11a0 177c 006a 13a1 0101 0074  .|.j...|.j.....t
-00000620: 1864 067c 0083 027c 005f 1974 1a7c 006a  .d.|...|._.t.|.j
-00000630: 0664 0719 0083 0144 005d 077d 017c 00a0  .d.....D.].}.|..
-00000640: 1b7c 01a1 0101 0071 527c 006a 11a0 107c  .|.....qR|.j...|
-00000650: 006a 19a1 0101 0074 1264 087c 0083 027c  .j.....t.d.|...|
-00000660: 005f 1c7c 006a 11a0 177c 006a 1ca1 0101  ._.|.j...|.j....
-00000670: 007c 006a 0fa0 1064 09a1 017c 005f 1d74  .|.j...d...|._.t
-00000680: 1264 0a7c 0083 027c 005f 1e7c 006a 1da0  .d.|...|._.|.j..
-00000690: 177c 006a 1ea1 0101 007c 006a 1ea0 1f64  .|.j.....|.j...d
-000006a0: 0ba1 0101 0074 1264 0c7c 0083 027c 005f  .....t.d.|...|._
-000006b0: 207c 006a 1da0 177c 006a 20a1 0101 007c   |.j...|.j ....|
-000006c0: 006a 20a0 1f64 0ba1 0101 007c 00a0 21a1  .j ..d.....|..!.
-000006d0: 0001 0074 2283 007c 005f 237c 00a0 247c  ...t"..|._#|..$|
-000006e0: 006a 23a1 0101 0074 2564 0d7c 0083 027c  .j#....t%d.|...|
-000006f0: 005f 267c 006a 26a0 2774 256a 286a 29a1  ._&|.j&.'t%j(j).
-00000700: 0101 007c 006a 26a0 2a74 2b6a 2c6a 2da1  ...|.j&.*t+j,j-.
-00000710: 0101 0074 2e83 007c 005f 2f7c 006a 26a0  ...t...|._/|.j&.
-00000720: 307c 006a 2fa1 0101 007c 00a0 3174 2b6a  0|.j/....|..1t+j
-00000730: 2c6a 2d7c 006a 26a1 0201 0064 0053 0029  ,j-|.j&....d.S.)
-00000740: 0e4e 5a06 5079 5859 3344 7a1e 7079 7879  .NZ.PyXY3Dz.pyxy
-00000750: 3364 2f67 7569 2f69 636f 6e73 2f70 7978  3d/gui/icons/pyx
-00000760: 795f 6c6f 676f 2e73 7667 69f4 0100 00da  y_logo.svgi.....
-00000770: 0446 696c 657a 104e 6577 2f4f 7065 6e20  .Filez.New/Open 
-00000780: 5072 6f6a 6563 747a 1252 6563 656e 7420  Projectz.Recent 
-00000790: 5072 6f6a 6563 7473 2e2e 2eda 0f72 6563  Projects.....rec
-000007a0: 656e 745f 7072 6f6a 6563 7473 5a04 4578  ent_projectsZ.Ex
-000007b0: 6974 722a 0000 007a 0f43 6f6e 6e65 6374  itr*...z.Connect
-000007c0: 2043 616d 6572 6173 467a 1244 6973 636f   CamerasFz.Disco
-000007d0: 6e6e 6563 7420 4361 6d65 7261 735a 034c  nnect CamerasZ.L
-000007e0: 6f67 2932 da05 7375 7065 7272 3000 0000  og)2..superr0...
-000007f0: da08 5f5f 696e 6974 5f5f da04 746f 6d6c  ..__init__..toml
-00000800: da04 6c6f 6164 7215 0000 00da 0c61 7070  ..loadr......app
-00000810: 5f73 6574 7469 6e67 73da 0e73 6574 5769  _settings..setWi
-00000820: 6e64 6f77 5469 746c 65da 0d73 6574 5769  ndowTitle..setWi
-00000830: 6e64 6f77 4963 6f6e 720f 0000 00da 0373  ndowIconr......s
-00000840: 7472 7205 0000 0072 1400 0000 da0e 7365  trr....r......se
-00000850: 744d 696e 696d 756d 5369 7a65 5a07 6d65  tMinimumSizeZ.me
-00000860: 6e75 4261 72da 046d 656e 75da 0761 6464  nuBar..menu..add
-00000870: 4d65 6e75 5a09 6669 6c65 5f6d 656e 7572  MenuZ.file_menur
-00000880: 1000 0000 5a13 6f70 656e 5f70 726f 6a65  ....Z.open_proje
-00000890: 6374 5f61 6374 696f 6eda 0974 7269 6767  ct_action..trigg
-000008a0: 6572 6564 da07 636f 6e6e 6563 74da 1963  ered..connect..c
-000008b0: 7265 6174 655f 6e65 775f 7072 6f6a 6563  reate_new_projec
-000008c0: 745f 666f 6c64 6572 da09 6164 6441 6374  t_folder..addAct
-000008d0: 696f 6e72 0b00 0000 da1b 6f70 656e 5f72  ionr......open_r
-000008e0: 6563 656e 745f 7072 6f6a 6563 745f 7375  ecent_project_su
-000008f0: 626d 656e 75da 0872 6576 6572 7365 64da  bmenu..reversed.
-00000900: 1561 6464 5f74 6f5f 7265 6365 6e74 5f70  .add_to_recent_p
-00000910: 726f 6a65 6374 da12 6578 6974 5f70 7978  roject..exit_pyx
-00000920: 7933 645f 6163 7469 6f6e 5a0c 6361 6d65  y3d_actionZ.came
-00000930: 7261 735f 6d65 6e75 da16 636f 6e6e 6563  ras_menu..connec
-00000940: 745f 6361 6d65 7261 735f 6163 7469 6f6e  t_cameras_action
-00000950: da0a 7365 7445 6e61 626c 6564 da19 6469  ..setEnabled..di
-00000960: 7363 6f6e 6e65 6374 5f63 616d 6572 6173  sconnect_cameras
-00000970: 5f61 6374 696f 6eda 1463 6f6e 6e65 6374  _action..connect
-00000980: 5f6d 656e 755f 6163 7469 6f6e 7372 0d00  _menu_actionsr..
-00000990: 0000 da0a 7461 625f 7769 6467 6574 da10  ....tab_widget..
-000009a0: 7365 7443 656e 7472 616c 5769 6467 6574  setCentralWidget
-000009b0: 7209 0000 005a 0d64 6f63 6b65 645f 6c6f  r....Z.docked_lo
-000009c0: 6767 6572 5a0b 7365 7446 6561 7475 7265  ggerZ.setFeature
-000009d0: 735a 1144 6f63 6b57 6964 6765 7446 6561  sZ.DockWidgetFea
-000009e0: 7475 7265 5a11 446f 636b 5769 6467 6574  tureZ.DockWidget
-000009f0: 4d6f 7661 626c 655a 0f73 6574 416c 6c6f  MovableZ.setAllo
-00000a00: 7765 6441 7265 6173 7213 0000 00da 0e44  wedAreasr......D
-00000a10: 6f63 6b57 6964 6765 7441 7265 61da 1442  ockWidgetArea..B
-00000a20: 6f74 746f 6d44 6f63 6b57 6964 6765 7441  ottomDockWidgetA
-00000a30: 7265 6172 1900 0000 5a0a 6c6f 675f 7769  rear....Z.log_wi
-00000a40: 6467 6574 da09 7365 7457 6964 6765 74da  dget..setWidget.
-00000a50: 0d61 6464 446f 636b 5769 6467 6574 2902  .addDockWidget).
-00000a60: da04 7365 6c66 da0c 7072 6f6a 6563 745f  ..self..project_
-00000a70: 7061 7468 a901 da09 5f5f 636c 6173 735f  path....__class_
-00000a80: 5f72 2e00 0000 722f 0000 0072 3400 0000  _r....r/...r4...
-00000a90: 3200 0000 7340 0000 000e 010c 020a 0218  2...s@..........
-00000aa0: 010c 010a 030e 010c 0310 010e 010c 0312  ................
-00000ab0: 030c 010e 020c 020e 010e 020c 010e 010c  ................
-00000ac0: 010c 020e 010c 0108 0208 030c 010c 0310  ................
-00000ad0: 0110 0108 010e 0116 027a 134d 6169 6e57  .........z.MainW
-00000ae0: 696e 646f 772e 5f5f 696e 6974 5f5f 6301  indow.__init__c.
-00000af0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000b00: 0000 0043 0000 0073 3800 0000 7c00 6a00  ...C...s8...|.j.
-00000b10: 6a01 a002 7c00 6a03 a101 0100 7c00 6a04  j...|.j.....|.j.
-00000b20: 6a01 a002 7405 a006 a100 6a07 a101 0100  j...t.....j.....
-00000b30: 7c00 6a08 6a01 a002 7c00 6a09 a101 0100  |.j.j...|.j.....
-00000b40: 6400 5300 a901 4e29 0a72 4600 0000 723e  d.S...N).rF...r>
-00000b50: 0000 0072 3f00 0000 da11 6c6f 6164 5f73  ...r?.....load_s
-00000b60: 7472 6561 6d5f 746f 6f6c 7372 4500 0000  tream_toolsrE...
-00000b70: 7207 0000 00da 0869 6e73 7461 6e63 65da  r......instance.
-00000b80: 0471 7569 7472 4800 0000 da12 6469 7363  .quitrH.....disc
-00000b90: 6f6e 6e65 6374 5f63 616d 6572 6173 a901  onnect_cameras..
-00000ba0: 7250 0000 0072 2e00 0000 722e 0000 0072  rP...r....r....r
-00000bb0: 2f00 0000 7249 0000 006a 0000 0073 0600  /...rI...j...s..
-00000bc0: 0000 1001 1401 1401 7a1f 4d61 696e 5769  ........z.MainWi
-00000bd0: 6e64 6f77 2e63 6f6e 6e65 6374 5f6d 656e  ndow.connect_men
-00000be0: 755f 6163 7469 6f6e 7363 0100 0000 0000  u_actionsc......
-00000bf0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00000c00: 0000 73b4 0000 007c 006a 00a0 017c 006a  ..s....|.j...|.j
-00000c10: 02a1 0101 007c 006a 00a0 0374 046a 056a  .....|.j...t.j.j
-00000c20: 0664 01a1 0201 007c 006a 00a0 0374 046a  .d.....|.j...t.j
-00000c30: 076a 0664 02a1 0201 007c 006a 00a0 0374  .j.d.....|.j...t
-00000c40: 046a 086a 0664 02a1 0201 007c 006a 00a0  .j.j.d.....|.j..
-00000c50: 0374 046a 096a 0664 02a1 0201 007c 006a  .t.j.j.d.....|.j
-00000c60: 00a0 0374 046a 0a6a 0664 01a1 0201 0074  ...t.j.j.d.....t
-00000c70: 0b83 007c 005f 0c74 0b83 007c 005f 0d74  ...|._.t...|._.t
-00000c80: 0b83 007c 005f 0e7c 006a 0fa0 1074 116a  ...|._.|.j...t.j
-00000c90: 05a1 0101 007c 006a 0fa0 12a1 0001 007c  .....|.j.......|
-00000ca0: 006a 13a0 1464 02a1 0101 007c 006a 15a0  .j...d.....|.j..
-00000cb0: 1464 01a1 0101 0064 0053 0029 034e 5446  .d.....d.S.).NTF
-00000cc0: 2916 724a 0000 00da 1073 6574 4375 7272  ).rJ.....setCurr
-00000cd0: 656e 7457 6964 6765 74da 0e63 6861 7275  entWidget..charu
-00000ce0: 636f 5f77 6964 6765 74da 0d73 6574 5461  co_widget..setTa
-00000cf0: 6245 6e61 626c 6564 7221 0000 0072 2900  bEnabledr!...r).
-00000d00: 0000 da05 7661 6c75 6572 2a00 0000 722b  ....valuer*...r+
-00000d10: 0000 0072 2c00 0000 722d 0000 0072 0800  ...r,...r-...r..
-00000d20: 0000 da0d 6361 6d65 7261 5f77 6964 6765  ....camera_widge
-00000d30: 74da 1f63 616c 6962 7261 7465 5f63 6170  t..calibrate_cap
-00000d40: 7475 7265 5f76 6f6c 756d 655f 7769 6467  ture_volume_widg
-00000d50: 6574 da10 7265 636f 7264 696e 675f 7769  et..recording_wi
-00000d60: 6467 6574 da07 7365 7373 696f 6eda 0873  dget..session..s
-00000d70: 6574 5f6d 6f64 6572 1800 0000 7258 0000  et_moder....rX..
-00000d80: 0072 4800 0000 7247 0000 0072 4600 0000  .rH...rG...rF...
-00000d90: 7259 0000 0072 2e00 0000 722e 0000 0072  rY...r....r....r
-00000da0: 2f00 0000 7258 0000 006f 0000 0073 1a00  /...rX...o...s..
-00000db0: 0000 0e01 1201 1201 1201 1201 1201 0802  ................
-00000dc0: 0801 0801 0e02 0a01 0c01 1001 7a1d 4d61  ............z.Ma
-00000dd0: 696e 5769 6e64 6f77 2e64 6973 636f 6e6e  inWindow.disconn
-00000de0: 6563 745f 6361 6d65 7261 7363 0100 0000  ect_camerasc....
-00000df0: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-00000e00: 4300 0000 733a 0000 007c 006a 00a0 0164  C...s:...|.j...d
-00000e10: 01a1 0101 007c 006a 02a0 0164 02a1 0101  .....|.j...d....
-00000e20: 0074 037c 006a 046a 0564 0364 0264 048d  .t.|.j.j.d.d.d..
-00000e30: 037c 005f 067c 006a 06a0 07a1 0001 0064  .|._.|.j.......d
-00000e40: 0053 0029 054e 4654 722e 0000 0029 03da  .S.).NFTr....)..
-00000e50: 0674 6172 6765 74da 0461 7267 73da 0664  .target..args..d
-00000e60: 6165 6d6f 6e29 0872 4600 0000 7247 0000  aemon).rF...rG..
-00000e70: 0072 4800 0000 7206 0000 0072 6100 0000  .rH...r....ra...
-00000e80: 7255 0000 00da 0674 6872 6561 64da 0573  rU.....thread..s
-00000e90: 7461 7274 7259 0000 0072 2e00 0000 722e  tartrY...r....r.
-00000ea0: 0000 0072 2f00 0000 7255 0000 0082 0000  ...r/...rU......
-00000eb0: 0073 0c00 0000 0c01 0c01 0201 0a01 08ff  .s..............
-00000ec0: 0e03 7a1c 4d61 696e 5769 6e64 6f77 2e6c  ..z.MainWindow.l
-00000ed0: 6f61 645f 7374 7265 616d 5f74 6f6f 6c73  oad_stream_tools
-00000ee0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000ef0: 0004 0000 0043 0000 0073 1601 0000 7400  .....C...s....t.
-00000f00: a001 6401 7c01 9b00 9d02 a101 0100 7c01  ..d.|.........|.
-00000f10: 0400 7402 6a03 6a04 6b02 721e 0100 7400  ..t.j.j.k.r...t.
-00000f20: a001 6402 a101 0100 7c00 6a05 a006 7407  ..d.....|.j...t.
-00000f30: 6a03 a101 0100 6400 5300 0400 7402 6a08  j.....d.S...t.j.
-00000f40: 6a04 6b02 7233 0100 7400 a001 6403 a101  j.k.r3..t...d...
-00000f50: 0100 7c00 6a05 a006 7407 6a09 a101 0100  ..|.j...t.j.....
-00000f60: 6400 5300 0400 7402 6a0a 6a04 6b02 725c  d.S...t.j.j.k.r\
-00000f70: 0100 7400 a001 6404 a101 0100 7c00 6a05  ..t...d.....|.j.
-00000f80: a00b a100 7250 7400 a001 6405 a101 0100  ....rPt...d.....
-00000f90: 7c00 6a0c a00d a100 0100 6400 5300 7400  |.j.......d.S.t.
-00000fa0: a001 6406 a101 0100 7c00 6a0c a00e a100  ..d.....|.j.....
-00000fb0: 0100 6400 5300 0400 7402 6a0f 6a04 6b02  ..d.S...t.j.j.k.
-00000fc0: 7271 0100 7400 a001 6407 a101 0100 7c00  rq..t...d.....|.
-00000fd0: 6a05 a006 7407 6a0f a101 0100 6400 5300  j...t.j.....d.S.
-00000fe0: 7402 6a10 6a04 6b02 7289 7400 a001 6408  t.j.j.k.r.t...d.
-00000ff0: a101 0100 7c00 6a05 a006 7407 6a11 a101  ....|.j...t.j...
-00001000: 0100 7c00 6a12 a013 a100 0100 6400 5300  ..|.j.......d.S.
-00001010: 6400 5300 2909 4e7a 1d53 7769 7463 6869  d.S.).Nz.Switchi
-00001020: 6e67 206d 6169 6e20 7769 6e64 6f77 2074  ng main window t
-00001030: 6f20 7461 6220 7a19 4163 7469 7661 7469  o tab z.Activati
-00001040: 6e67 2043 6861 7275 636f 2057 6964 6765  ng Charuco Widge
-00001050: 747a 1e41 6374 6976 6174 696e 6720 4361  tz.Activating Ca
-00001060: 6d65 7261 2053 6574 7570 2057 6964 6765  mera Setup Widge
-00001070: 747a 2a41 6374 6976 6174 696e 6720 4361  tz*Activating Ca
-00001080: 6c69 6272 6174 6520 4361 7074 7572 6520  librate Capture 
-00001090: 566f 6c75 6d65 2057 6964 6765 747a 5353  Volume WidgetzSS
-000010a0: 6573 7369 6f6e 2069 7320 656c 6967 6962  ession is eligib
-000010b0: 6c65 2066 6f72 2073 6574 7469 6e67 206f  le for setting o
-000010c0: 6620 6f72 6967 696e 2e2e 2e61 6374 6976  f origin...activ
-000010d0: 6174 696e 6720 6361 7074 7572 6520 766f  ating capture vo
-000010e0: 6c75 6d65 206f 7269 6769 6e20 7769 6467  lume origin widg
-000010f0: 6574 7a57 5365 7373 696f 6e20 6973 206e  etzWSession is n
-00001100: 6f74 2065 6c69 6769 626c 6520 666f 7220  ot eligible for 
-00001110: 7365 7474 696e 6720 6f66 206f 7269 6769  setting of origi
-00001120: 6e2e 2e2e 6163 7469 7661 7469 6e67 2065  n...activating e
-00001130: 7874 7269 6e73 6963 2063 616c 6962 7261  xtrinsic calibra
-00001140: 7469 6f6e 2077 6964 6765 747a 1741 6374  tion widgetz.Act
-00001150: 6976 6174 6520 5265 636f 7264 696e 6720  ivate Recording 
-00001160: 4d6f 6465 7a18 4163 7469 7661 7465 2050  Modez.Activate P
-00001170: 726f 6365 7373 696e 6720 4d6f 6465 2914  rocessing Mode).
-00001180: da06 6c6f 6767 6572 da04 696e 666f 7221  ..logger..infor!
-00001190: 0000 0072 2900 0000 725d 0000 0072 6100  ...r)...r]...ra.
-000011a0: 0000 7262 0000 0072 1800 0000 722a 0000  ..rb...r....r*..
-000011b0: 00da 1449 6e74 7269 6e73 6963 4361 6c69  ...IntrinsicCali
-000011c0: 6272 6174 696f 6e72 2b00 0000 da1a 6973  brationr+.....is
-000011d0: 5f63 6170 7475 7265 5f76 6f6c 756d 655f  _capture_volume_
-000011e0: 656c 6967 6962 6c65 725f 0000 005a 1e61  eligibler_...Z.a
-000011f0: 6374 6976 6174 655f 6361 7074 7572 655f  ctivate_capture_
-00001200: 766f 6c75 6d65 5f77 6964 6765 745a 2561  volume_widgetZ%a
-00001210: 6374 6976 6174 655f 6578 7472 696e 7369  ctivate_extrinsi
-00001220: 635f 6361 6c69 6272 6174 696f 6e5f 7769  c_calibration_wi
-00001230: 6467 6574 722c 0000 0072 2d00 0000 da0e  dgetr,...r-.....
-00001240: 506f 7374 5072 6f63 6573 7369 6e67 da11  PostProcessing..
-00001250: 7072 6f63 6573 7369 6e67 5f77 6964 6765  processing_widge
-00001260: 745a 1875 7064 6174 655f 7265 636f 7264  tZ.update_record
-00001270: 696e 675f 666f 6c64 6572 7329 0272 5000  ing_folders).rP.
-00001280: 0000 da05 696e 6465 7872 2e00 0000 722e  ....indexr....r.
-00001290: 0000 0072 2f00 0000 da0e 6f6e 5f74 6162  ...r/.....on_tab
-000012a0: 5f63 6861 6e67 6564 8a00 0000 732e 0000  _changed....s...
-000012b0: 0010 0102 010e 010a 0112 010e 010a 0112  ................
-000012c0: 010e 010a 010a 020a 010e 010a 020e 010e  ................
-000012d0: 020a 0112 010a 010a 010e 010e 0204 fc7a  ...............z
-000012e0: 194d 6169 6e57 696e 646f 772e 6f6e 5f74  .MainWindow.on_t
-000012f0: 6162 5f63 6861 6e67 6564 da0e 7061 7468  ab_changed..path
-00001300: 5f74 6f5f 666f 6c64 6572 6302 0000 0000  _to_folderc.....
-00001310: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00001320: 0000 0073 f000 0000 7400 7c01 8301 7d02  ...s....t.|...}.
-00001330: 7401 7c02 8301 7c00 5f02 7403 a004 6401  t.|...|._.t...d.
-00001340: 7c02 9b00 9d02 a101 0100 7405 7c00 6a02  |.........t.|.j.
-00001350: 8301 7c00 5f06 7407 7c00 6a06 8301 7c00  ..|._.t.|.j...|.
-00001360: 5f08 7409 8300 7c00 5f0a 7409 8300 7c00  _.t...|._.t...|.
-00001370: 5f0b 7409 8300 7c00 5f0c 7409 8300 7c00  _.t...|._.t...|.
-00001380: 5f0d 7c00 6a0e a00f 7c00 6a08 6402 a102  _.|.j...|.j.d...
-00001390: 0100 7c00 6a0e a00f 7c00 6a0a 6403 a102  ..|.j...|.j.d...
-000013a0: 0100 7c00 6a0e a00f 7c00 6a0d 6404 a102  ..|.j...|.j.d...
-000013b0: 0100 7c00 6a0e a00f 7c00 6a0b 6405 a102  ..|.j...|.j.d...
-000013c0: 0100 7c00 6a0e a00f 7c00 6a0c 6406 a102  ..|.j...|.j.d...
-000013d0: 0100 7c00 6a0e 6a10 a011 7c00 6a12 a101  ..|.j.j...|.j...
-000013e0: 0100 7c00 6a13 a014 6407 a101 0100 7c00  ..|.j...d.....|.
-000013f0: a015 a100 0100 7c00 6a0e a016 a100 7d03  ......|.j.....}.
-00001400: 7c00 6a0e a017 7c03 a101 0100 7c00 a018  |.j...|.....|...
-00001410: a100 0100 6400 5300 2908 4e7a 2d4c 6175  ....d.S.).Nz-Lau
-00001420: 6e63 6869 6e67 2073 6573 7369 6f6e 2077  nching session w
-00001430: 6974 6820 636f 6e66 6967 2066 696c 6520  ith config file 
-00001440: 7374 6f72 6564 2069 6e20 7229 0000 0072  stored in r)...r
-00001450: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
-00001460: 0000 0054 2919 7205 0000 0072 1a00 0000  ...T).r....r....
-00001470: da06 636f 6e66 6967 7268 0000 0072 6900  ..configrh...ri.
-00001480: 0000 7217 0000 0072 6100 0000 721c 0000  ..r....ra...r...
-00001490: 0072 5b00 0000 7208 0000 0072 5e00 0000  .r[...r....r^...
-000014a0: 7260 0000 0072 6d00 0000 725f 0000 0072  r`...rm...r_...r
-000014b0: 4a00 0000 da06 6164 6454 6162 da0e 6375  J.....addTab..cu
-000014c0: 7272 656e 7443 6861 6e67 6564 723f 0000  rrentChangedr?..
-000014d0: 0072 6f00 0000 7246 0000 0072 4700 0000  .ro...rF...rG...
-000014e0: da0b 7570 6461 7465 5f74 6162 73da 0c63  ..update_tabs..c
-000014f0: 7572 7265 6e74 496e 6465 78da 0f73 6574  urrentIndex..set
-00001500: 4375 7272 656e 7449 6e64 6578 da17 636f  CurrentIndex..co
-00001510: 6e6e 6563 745f 7365 7373 696f 6e5f 7369  nnect_session_si
-00001520: 676e 616c 7329 0472 5000 0000 7270 0000  gnals).rP...rp..
-00001530: 00da 0c73 6573 7369 6f6e 5f70 6174 685a  ...session_pathZ
-00001540: 096f 6c64 5f69 6e64 6578 722e 0000 0072  .old_indexr....r
-00001550: 2e00 0000 722f 0000 00da 0e6c 6175 6e63  ....r/.....launc
-00001560: 685f 7365 7373 696f 6ea6 0000 0073 2800  h_session....s(.
-00001570: 0000 0801 0a01 1001 0c01 0c03 0803 0801  ................
-00001580: 0801 0801 1002 1001 1001 1001 1001 1003  ................
-00001590: 0c03 0804 0a03 0c02 0c01 7a19 4d61 696e  ..........z.Main
-000015a0: 5769 6e64 6f77 2e6c 6175 6e63 685f 7365  Window.launch_se
-000015b0: 7373 696f 6e63 0100 0000 0000 0000 0000  ssionc..........
-000015c0: 0000 0100 0000 0400 0000 4300 0000 7308  ..........C...s.
-000015d0: 0100 007c 006a 00a0 0174 026a 036a 0464  ...|.j...t.j.j.d
-000015e0: 01a1 0201 007c 006a 056a 0672 4a74 077c  .....|.j.j.rJt.|
-000015f0: 006a 0883 0174 096b 0372 187c 00a0 0aa1  .j...t.k.r.|....
-00001600: 0001 0074 077c 006a 0b83 0174 0c6b 0372  ...t.|.j...t.k.r
-00001610: 237c 00a0 0da1 0001 0074 077c 006a 0e83  #|.......t.|.j..
-00001620: 0174 0f6b 0372 2e7c 00a0 10a1 0001 007c  .t.k.r.|.......|
-00001630: 006a 00a0 0174 026a 116a 0464 01a1 0201  .j...t.j.j.d....
-00001640: 007c 006a 00a0 0174 026a 126a 0464 01a1  .|.j...t.j.j.d..
-00001650: 0201 007c 006a 00a0 0174 026a 136a 0464  ...|.j...t.j.j.d
-00001660: 01a1 0201 006e 1b7c 006a 00a0 0174 026a  .....n.|.j...t.j
-00001670: 116a 0464 02a1 0201 007c 006a 00a0 0174  .j.d.....|.j...t
-00001680: 026a 126a 0464 02a1 0201 007c 006a 00a0  .j.j.d.....|.j..
-00001690: 0174 026a 136a 0464 02a1 0201 007c 006a  .t.j.j.d.....|.j
-000016a0: 05a0 14a1 0072 797c 00a0 15a1 0001 007c  .....ry|.......|
-000016b0: 006a 00a0 0174 026a 166a 0464 01a1 0201  .j...t.j.j.d....
-000016c0: 0064 0353 007c 006a 00a0 0174 026a 166a  .d.S.|.j...t.j.j
-000016d0: 0464 02a1 0201 0064 0353 0029 0461 0b01  .d.....d.S.).a..
-000016e0: 0000 0a20 2020 2020 2020 2054 6162 2075  ...        Tab u
-000016f0: 7064 6174 6573 206f 6363 7572 2070 7269  pdates occur pri
-00001700: 6d61 7269 6c79 2061 7420 3220 7469 6d65  marily at 2 time
-00001710: 733a 0a20 2020 2020 2020 2031 2e20 7570  s:.        1. up
-00001720: 6f6e 206d 6169 6e20 7769 6e64 6f77 2069  on main window i
-00001730: 6e69 7469 6174 696f 6e20 7768 656e 206f  nitiation when o
-00001740: 6666 6c69 6e65 2063 6170 6163 6974 6965  ffline capacitie
-00001750: 7320 0a20 2020 2020 2020 2028 6361 7074  s .        (capt
-00001760: 7572 6520 766f 6c75 6d65 2061 6e64 2070  ure volume and p
-00001770: 6f73 742d 7072 6f63 6573 7369 6e67 2920  ost-processing) 
-00001780: 6d61 7920 6265 2061 7661 696c 6162 6c65  may be available
-00001790: 2e0a 0a20 2020 2020 2020 2032 2e20 7570  ...        2. up
-000017a0: 6f6e 206c 6f61 6469 6e67 206f 6620 7374  on loading of st
-000017b0: 7265 616d 2074 6f6f 6c73 2077 6865 6e20  ream tools when 
-000017c0: 6361 6d65 7261 732f 7265 636f 7264 696e  cameras/recordin
-000017d0: 6720 776f 756c 6420 6265 2061 7661 696c  g would be avail
-000017e0: 6162 6c65 0a20 2020 2020 2020 2054 464e  able.        TFN
-000017f0: 2917 724a 0000 0072 5c00 0000 7221 0000  ).rJ...r\...r!..
-00001800: 0072 2900 0000 725d 0000 0072 6100 0000  .r)...r]...ra...
-00001810: da13 7374 7265 616d 5f74 6f6f 6c73 5f6c  ..stream_tools_l
-00001820: 6f61 6465 64da 0474 7970 6572 5e00 0000  oaded..typer^...
-00001830: 721d 0000 00da 126c 6f61 645f 6361 6d65  r......load_came
-00001840: 7261 5f77 6964 6765 7472 6000 0000 721f  ra_widgetr`...r.
-00001850: 0000 00da 156c 6f61 645f 7265 636f 7264  .....load_record
-00001860: 696e 675f 7769 6467 6574 725f 0000 0072  ing_widgetr_...r
-00001870: 1e00 0000 da1a 6c6f 6164 5f63 6170 7475  ......load_captu
-00001880: 7265 5f76 6f6c 756d 655f 7769 6467 6574  re_volume_widget
-00001890: 722a 0000 0072 2c00 0000 722b 0000 00da  r*...r,...r+....
-000018a0: 1b69 735f 706f 7374 5f70 726f 6365 7373  .is_post_process
-000018b0: 696e 675f 656c 6967 6962 6c65 da1b 6c6f  ing_eligible..lo
-000018c0: 6164 5f70 6f73 745f 7072 6f63 6573 7369  ad_post_processi
-000018d0: 6e67 5f77 6964 6765 7472 2d00 0000 7259  ng_widgetr-...rY
-000018e0: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
-000018f0: 0000 7274 0000 00cb 0000 0073 2400 0000  ..rt.......s$...
-00001900: 120a 0803 0e02 0801 0e02 0801 0e02 0801  ................
-00001910: 1202 1201 1401 1205 1201 1201 0a03 0801  ................
-00001920: 1601 1602 7a16 4d61 696e 5769 6e64 6f77  ....z.MainWindow
-00001930: 2e75 7064 6174 655f 7461 6273 6301 0000  .update_tabsc...
-00001940: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00001950: 0043 0000 0073 2400 0000 7c00 6a00 6a01  .C...s$...|.j.j.
-00001960: a002 7c00 6a03 a101 0100 7c00 6a00 6a04  ..|.j.....|.j.j.
-00001970: a002 7c00 6a05 a101 0100 6401 5300 2902  ..|.j.....d.S.).
-00001980: 7a90 0a20 2020 2020 2020 2041 6674 6572  z..        After
-00001990: 206c 6175 6e63 6869 6e67 2061 2073 6573   launching a ses
-000019a0: 7369 6f6e 2c20 636f 6e6e 6563 7420 7369  sion, connect si
-000019b0: 676e 616c 7320 616e 6420 736c 6f74 732e  gnals and slots.
-000019c0: 0a20 2020 2020 2020 204d 7563 6820 6f66  .        Much of
-000019d0: 2074 6865 7365 2077 696c 6c20 6265 2066   these will be f
-000019e0: 726f 6d20 7468 6520 4755 4920 746f 2074  rom the GUI to t
-000019f0: 6865 2073 6573 7369 6f6e 2061 6e64 2076  he session and v
-00001a00: 6963 652d 7665 7273 610a 2020 2020 2020  ice-versa.      
-00001a10: 2020 4e29 0672 6100 0000 da15 756e 6c6f    N).ra.....unlo
-00001a20: 636b 5f70 6f73 7470 726f 6365 7373 696e  ck_postprocessin
-00001a30: 6772 3f00 0000 7280 0000 00da 1a73 7472  gr?...r......str
-00001a40: 6561 6d5f 746f 6f6c 735f 6c6f 6164 6564  eam_tools_loaded
-00001a50: 5f73 6967 6e61 6c72 7400 0000 7259 0000  _signalrt...rY..
-00001a60: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00001a70: 7277 0000 00f7 0000 0073 0400 0000 1005  rw.......s......
-00001a80: 1401 7a22 4d61 696e 5769 6e64 6f77 2e63  ..z"MainWindow.c
-00001a90: 6f6e 6e65 6374 5f73 6573 7369 6f6e 5f73  onnect_session_s
-00001aa0: 6967 6e61 6c73 6301 0000 0000 0000 0000  ignalsc.........
-00001ab0: 0000 0002 0000 0005 0000 0043 0000 00f3  ...........C....
-00001ac0: 4600 0000 7c00 6a00 a001 7402 6a03 6a04  F...|.j...t.j.j.
-00001ad0: a101 0100 7c00 6a05 a006 a100 0100 7407  ....|.j.......t.
-00001ae0: 7c00 6a08 8301 7d01 7c00 6a00 a009 7402  |.j...}.|.j...t.
-00001af0: 6a03 6a04 7c01 7402 6a03 6a0a a103 0100  j.j.|.t.j.j.....
-00001b00: 7c01 7c00 5f05 6400 5300 7254 0000 0029  |.|._.d.S.rT...)
-00001b10: 0b72 4a00 0000 da09 7265 6d6f 7665 5461  .rJ.....removeTa
-00001b20: 6272 2100 0000 722c 0000 0072 5d00 0000  br!...r,...r]...
-00001b30: 7260 0000 00da 0b64 656c 6574 654c 6174  r`.....deleteLat
-00001b40: 6572 721f 0000 0072 6100 0000 da09 696e  err....ra.....in
-00001b50: 7365 7274 5461 62da 046e 616d 6529 0272  sertTab..name).r
-00001b60: 5000 0000 5a14 6e65 775f 7265 636f 7264  P...Z.new_record
-00001b70: 696e 675f 7769 6467 6574 722e 0000 0072  ing_widgetr....r
-00001b80: 2e00 0000 722f 0000 0072 7d00 0000 ff00  ....r/...r}.....
-00001b90: 0000 730e 0000 0010 020a 010a 0106 010e  ..s.............
-00001ba0: 0104 ff0a 037a 204d 6169 6e57 696e 646f  .....z MainWindo
-00001bb0: 772e 6c6f 6164 5f72 6563 6f72 6469 6e67  w.load_recording
-00001bc0: 5f77 6964 6765 7463 0100 0000 0000 0000  _widgetc........
-00001bd0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-00001be0: 7283 0000 0072 5400 0000 290b 724a 0000  r....rT...).rJ..
-00001bf0: 0072 8400 0000 7221 0000 0072 2d00 0000  .r....r!...r-...
-00001c00: 725d 0000 0072 6d00 0000 7285 0000 0072  r]...rm...r....r
-00001c10: 2000 0000 7261 0000 0072 8600 0000 7287   ...ra...r....r.
-00001c20: 0000 0029 0272 5000 0000 5a15 6e65 775f  ...).rP...Z.new_
-00001c30: 7072 6f63 6573 7369 6e67 5f77 6964 6765  processing_widge
-00001c40: 7472 2e00 0000 722e 0000 0072 2f00 0000  tr....r....r/...
-00001c50: 7280 0000 0009 0100 00f3 0e00 0000 1001  r...............
-00001c60: 0a01 0a01 0601 0e01 04ff 0a03 7a26 4d61  ............z&Ma
-00001c70: 696e 5769 6e64 6f77 2e6c 6f61 645f 706f  inWindow.load_po
-00001c80: 7374 5f70 726f 6365 7373 696e 675f 7769  st_processing_wi
-00001c90: 6467 6574 6301 0000 0000 0000 0000 0000  dgetc...........
-00001ca0: 0002 0000 0005 0000 0043 0000 0072 8300  .........C...r..
-00001cb0: 0000 7254 0000 0029 0b72 4a00 0000 7284  ..rT...).rJ...r.
-00001cc0: 0000 0072 2100 0000 722b 0000 0072 5d00  ...r!...r+...r].
-00001cd0: 0000 725f 0000 0072 8500 0000 721e 0000  ..r_...r....r...
-00001ce0: 0072 6100 0000 7286 0000 0072 8700 0000  .ra...r....r....
-00001cf0: 2902 7250 0000 005a 196e 6577 5f63 6170  ).rP...Z.new_cap
-00001d00: 7475 7265 5f76 6f6c 756d 655f 7769 6467  ture_volume_widg
-00001d10: 6574 722e 0000 0072 2e00 0000 722f 0000  etr....r....r/..
-00001d20: 0072 7e00 0000 1201 0000 7312 0000 0010  .r~.......s.....
-00001d30: 010a 010a 0106 0106 0102 0106 0104 fd0a  ................
-00001d40: 057a 254d 6169 6e57 696e 646f 772e 6c6f  .z%MainWindow.lo
-00001d50: 6164 5f63 6170 7475 7265 5f76 6f6c 756d  ad_capture_volum
-00001d60: 655f 7769 6467 6574 6301 0000 0000 0000  e_widgetc.......
-00001d70: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-00001d80: 0072 8300 0000 7254 0000 0029 0b72 4a00  .r....rT...).rJ.
-00001d90: 0000 7284 0000 0072 2100 0000 722a 0000  ..r....r!...r*..
-00001da0: 0072 5d00 0000 725e 0000 0072 8500 0000  .r]...r^...r....
-00001db0: 721d 0000 0072 6100 0000 7286 0000 0072  r....ra...r....r
-00001dc0: 8700 0000 2902 7250 0000 005a 116e 6577  ....).rP...Z.new
-00001dd0: 5f63 616d 6572 615f 7769 6467 6574 722e  _camera_widgetr.
-00001de0: 0000 0072 2e00 0000 722f 0000 0072 7c00  ...r....r/...r|.
-00001df0: 0000 1d01 0000 7288 0000 007a 1d4d 6169  ......r....z.Mai
-00001e00: 6e57 696e 646f 772e 6c6f 6164 5f63 616d  nWindow.load_cam
-00001e10: 6572 615f 7769 6467 6574 7251 0000 0063  era_widgetrQ...c
-00001e20: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00001e30: 0300 0000 4300 0000 7328 0000 0074 007c  ....C...s(...t.|
-00001e40: 017c 0083 027d 027c 026a 01a0 027c 006a  .|...}.|.j...|.j
-00001e50: 03a1 0101 007c 006a 04a0 057c 02a1 0101  .....|.j...|....
-00001e60: 0064 0053 0072 5400 0000 2906 7210 0000  .d.S.rT...).r...
-00001e70: 0072 3e00 0000 723f 0000 00da 136f 7065  .r>...r?.....ope
-00001e80: 6e5f 7265 6365 6e74 5f70 726f 6a65 6374  n_recent_project
-00001e90: 7242 0000 0072 4100 0000 2903 7250 0000  rB...rA...).rP..
-00001ea0: 0072 5100 0000 5a15 7265 6365 6e74 5f70  .rQ...Z.recent_p
-00001eb0: 726f 6a65 6374 5f61 6374 696f 6e72 2e00  roject_actionr..
-00001ec0: 0000 722e 0000 0072 2f00 0000 7244 0000  ..r....r/...rD..
-00001ed0: 0029 0100 0073 0600 0000 0a01 0e01 1001  .)...s..........
-00001ee0: 7a20 4d61 696e 5769 6e64 6f77 2e61 6464  z MainWindow.add
-00001ef0: 5f74 6f5f 7265 6365 6e74 5f70 726f 6a65  _to_recent_proje
-00001f00: 6374 6301 0000 0000 0000 0000 0000 0003  ctc.............
-00001f10: 0000 0004 0000 0043 0000 0073 2e00 0000  .......C...s....
-00001f20: 7c00 a000 a100 7d01 7c01 a001 a100 7d02  |.....}.|.....}.
-00001f30: 7402 a003 6401 7c02 9b00 9d02 a101 0100  t...d.|.........
-00001f40: 7c00 a004 7c02 a101 0100 6400 5300 2902  |...|.....d.S.).
-00001f50: 4e7a 214f 7065 6e69 6e67 2072 6563 656e  Nz!Opening recen
-00001f60: 7420 7365 7373 696f 6e20 7374 6f72 6564  t session stored
-00001f70: 2061 7420 2905 da06 7365 6e64 6572 da04   at )...sender..
-00001f80: 7465 7874 7268 0000 0072 6900 0000 7279  textrh...ri...ry
-00001f90: 0000 0029 0372 5000 0000 da06 6163 7469  ...).rP.....acti
-00001fa0: 6f6e 7251 0000 0072 2e00 0000 722e 0000  onrQ...r....r...
-00001fb0: 0072 2f00 0000 7289 0000 002e 0100 0073  .r/...r........s
-00001fc0: 0800 0000 0801 0801 1001 0e01 7a1e 4d61  ............z.Ma
-00001fd0: 696e 5769 6e64 6f77 2e6f 7065 6e5f 7265  inWindow.open_re
-00001fe0: 6365 6e74 5f70 726f 6a65 6374 6301 0000  cent_projectc...
-00001ff0: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00002000: 0043 0000 0073 5c00 0000 7400 7c00 6a01  .C...s\...t.|.j.
-00002010: 6401 1900 8301 7d01 7402 8300 7d02 7c02  d.....}.t...}.|.
-00002020: 6a03 6400 6402 7404 7c01 8301 7402 6a05  j.d.d.t.|...t.j.
-00002030: 6a06 6403 8d04 7d03 7c03 722c 7407 a008  j.d...}.|.r,t...
-00002040: 6404 7c03 6602 a101 0100 7c00 a009 7c03  d.|.f.....|...|.
-00002050: a101 0100 7c00 a00a 7c03 a101 0100 6400  ....|...|.....d.
-00002060: 5300 6400 5300 2905 4eda 136c 6173 745f  S.d.S.).N..last_
-00002070: 7072 6f6a 6563 745f 7061 7265 6e74 7a2d  project_parentz-
-00002080: 4f70 656e 2050 7265 7669 6f75 7320 6f72  Open Previous or
-00002090: 2043 7265 6174 6520 4e65 7720 5072 6f6a   Create New Proj
-000020a0: 6563 7420 4469 7265 6374 6f72 7929 04da  ect Directory)..
-000020b0: 0670 6172 656e 74da 0763 6170 7469 6f6e  .parent..caption
-000020c0: da09 6469 7265 6374 6f72 79da 076f 7074  ..directory..opt
-000020d0: 696f 6e73 7a19 4372 6561 7469 6e67 206e  ionsz.Creating n
-000020e0: 6577 2070 726f 6a65 6374 2069 6e20 3a29  ew project in :)
-000020f0: 0b72 0500 0000 7237 0000 0072 0400 0000  .r....r7...r....
-00002100: 5a14 6765 7445 7869 7374 696e 6744 6972  Z.getExistingDir
-00002110: 6563 746f 7279 723a 0000 00da 064f 7074  ectoryr:.....Opt
-00002120: 696f 6e5a 0c53 686f 7744 6972 734f 6e6c  ionZ.ShowDirsOnl
-00002130: 7972 6800 0000 7269 0000 00da 1561 6464  yrh...ri.....add
-00002140: 5f70 726f 6a65 6374 5f74 6f5f 7265 6365  _project_to_rece
-00002150: 6e74 7279 0000 0029 0472 5000 0000 5a0e  ntry...).rP...Z.
-00002160: 6465 6661 756c 745f 666f 6c64 6572 5a06  default_folderZ.
-00002170: 6469 616c 6f67 7270 0000 0072 2e00 0000  dialogrp...r....
-00002180: 722e 0000 0072 2f00 0000 7240 0000 0034  r....r/...r@...4
-00002190: 0100 0073 1a00 0000 0e01 0601 0401 0201  ...s............
-000021a0: 0201 0601 0601 06fc 0407 0e01 0a01 0e01  ................
-000021b0: 04fd 7a24 4d61 696e 5769 6e64 6f77 2e63  ..z$MainWindow.c
-000021c0: 7265 6174 655f 6e65 775f 7072 6f6a 6563  reate_new_projec
-000021d0: 745f 666f 6c64 6572 6302 0000 0000 0000  t_folderc.......
-000021e0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000021f0: 0073 5400 0000 7400 7c01 8301 7c00 6a01  .sT...t.|...|.j.
-00002200: 6401 1900 7600 720b 6400 5300 7c00 6a01  d...v.r.d.S.|.j.
-00002210: 6401 1900 a002 7400 7c01 8301 a101 0100  d.....t.|.......
-00002220: 7400 7403 7c01 8301 6a04 8301 7c00 6a01  t.t.|...j...|.j.
-00002230: 6402 3c00 7c00 a005 a100 0100 7c00 a006  d.<.|.......|...
-00002240: 7c01 a101 0100 6400 5300 2903 4e72 3200  |.....d.S.).Nr2.
-00002250: 0000 728d 0000 0029 0772 3a00 0000 7237  ..r....).r:...r7
-00002260: 0000 00da 0661 7070 656e 6472 0500 0000  .....appendr....
-00002270: 728e 0000 00da 1375 7064 6174 655f 6170  r......update_ap
-00002280: 705f 7365 7474 696e 6773 7244 0000 0029  p_settingsrD...)
-00002290: 0272 5000 0000 5a0b 666f 6c64 6572 5f70  .rP...Z.folder_p
-000022a0: 6174 6872 2e00 0000 722e 0000 0072 2f00  athr....r....r/.
-000022b0: 0000 7293 0000 0043 0100 0073 0c00 0000  ..r....C...s....
-000022c0: 1201 0401 1402 1401 0801 0e01 7a20 4d61  ............z Ma
-000022d0: 696e 5769 6e64 6f77 2e61 6464 5f70 726f  inWindow.add_pro
-000022e0: 6a65 6374 5f74 6f5f 7265 6365 6e74 6301  ject_to_recentc.
-000022f0: 0000 0000 0000 0000 0000 0002 0000 0008  ................
-00002300: 0000 0043 0000 0073 3e00 0000 7400 7401  ...C...s>...t.t.
-00002310: 6401 8302 8f10 7d01 7402 a003 7c00 6a04  d.....}.t...|.j.
-00002320: 7c01 a102 0100 5700 6400 0400 0400 8303  |.....W.d.......
-00002330: 0100 6400 5300 3100 7318 7701 0100 0100  ..d.S.1.s.w.....
-00002340: 0100 5900 0100 6400 5300 2902 4eda 0177  ..Y...d.S.).N..w
-00002350: 2905 da04 6f70 656e 7215 0000 0072 3500  )...openr....r5.
-00002360: 0000 da04 6475 6d70 7237 0000 0029 0272  ....dumpr7...).r
-00002370: 5000 0000 da01 6672 2e00 0000 722e 0000  P.....fr....r...
-00002380: 0072 2f00 0000 7295 0000 004c 0100 0073  .r/...r....L...s
-00002390: 0600 0000 0c01 1001 22ff 7a1e 4d61 696e  ........".z.Main
-000023a0: 5769 6e64 6f77 2e75 7064 6174 655f 6170  Window.update_ap
-000023b0: 705f 7365 7474 696e 6773 2916 7226 0000  p_settings).r&..
-000023c0: 0072 2700 0000 7228 0000 0072 3400 0000  .r'...r(...r4...
-000023d0: 7249 0000 0072 5800 0000 7255 0000 0072  rI...rX...rU...r
-000023e0: 6f00 0000 723a 0000 0072 7900 0000 7274  o...r:...ry...rt
-000023f0: 0000 0072 7700 0000 727d 0000 0072 8000  ...rw...r}...r..
-00002400: 0000 727e 0000 0072 7c00 0000 7244 0000  ..r~...r|...rD..
-00002410: 0072 8900 0000 7240 0000 0072 9300 0000  .r....r@...r....
-00002420: 7295 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-00002430: 6c6c 5f5f 722e 0000 0072 2e00 0000 7252  ll__r....r....rR
-00002440: 0000 0072 2f00 0000 7230 0000 0031 0000  ...r/...r0...1..
-00002450: 0073 2400 0000 0800 0c01 0838 0805 0813  .s$........8....
-00002460: 0808 0e1c 0825 082c 0808 080a 0809 080b  .....%.,........
-00002470: 0e0c 0805 0806 080f 1009 7230 0000 0063  ..........r0...c
-00002480: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00002490: 0200 0000 4300 0000 7324 0000 0074 0074  ....C...s$...t.t
-000024a0: 016a 0283 017d 0074 0383 007d 017c 01a0  .j...}.t...}.|..
-000024b0: 04a1 0001 007c 00a0 05a1 0001 0064 0053  .....|.......d.S
-000024c0: 0072 5400 0000 2906 7207 0000 00da 0373  .rT...).r......s
-000024d0: 7973 da04 6172 6776 7230 0000 00da 0473  ys..argvr0.....s
-000024e0: 686f 77da 0465 7865 6329 02da 0361 7070  how..exec)...app
-000024f0: da06 7769 6e64 6f77 722e 0000 0072 2e00  ..windowr....r..
-00002500: 0000 722f 0000 00da 0b6c 6175 6e63 685f  ..r/.....launch_
-00002510: 6d61 696e 5101 0000 7308 0000 000a 0106  mainQ...s.......
-00002520: 0108 010c 0272 a100 0000 da08 5f5f 6d61  .....r......__ma
-00002530: 696e 5f5f 2938 da0d 7079 7879 3364 2e6c  in__)8..pyxy3d.l
-00002540: 6f67 6765 72da 0670 7978 7933 6472 6800  ogger..pyxy3drh.
-00002550: 0000 da03 6765 7472 2600 0000 da0f 5079  ....getr&.....Py
-00002560: 5174 362e 5174 5769 6467 6574 7372 0200  Qt6.QtWidgetsr..
-00002570: 0000 7203 0000 0072 0400 0000 da07 7061  ..r....r......pa
-00002580: 7468 6c69 6272 0500 0000 da09 7468 7265  thlibr......thre
-00002590: 6164 696e 6772 0600 0000 729b 0000 0072  adingr....r....r
-000025a0: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-000025b0: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
-000025c0: 0000 7235 0000 00da 0465 6e75 6d72 0e00  ..r5.....enumr..
-000025d0: 0000 5a0b 5079 5174 362e 5174 4775 6972  ..Z.PyQt6.QtGuir
-000025e0: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
-000025f0: 0000 00da 0c50 7951 7436 2e51 7443 6f72  .....PyQt6.QtCor
-00002600: 6572 1300 0000 7214 0000 0072 1500 0000  er....r....r....
-00002610: 7216 0000 00da 1670 7978 7933 642e 7365  r......pyxy3d.se
-00002620: 7373 696f 6e2e 7365 7373 696f 6e72 1700  ssion.sessionr..
-00002630: 0000 7218 0000 005a 1570 7978 7933 642e  ..r....Z.pyxy3d.
-00002640: 6775 692e 6c6f 675f 7769 6467 6574 7219  gui.log_widgetr.
-00002650: 0000 00da 1370 7978 7933 642e 636f 6e66  .....pyxy3d.conf
-00002660: 6967 7572 6174 6f72 721a 0000 00da 1d70  iguratorr......p
-00002670: 7978 7933 642e 6775 692e 6361 6c69 6272  yxy3d.gui.calibr
-00002680: 6174 696f 6e5f 7769 6467 6574 721b 0000  ation_widgetr...
-00002690: 00da 1970 7978 7933 642e 6775 692e 6368  ...pyxy3d.gui.ch
-000026a0: 6172 7563 6f5f 7769 6467 6574 721c 0000  aruco_widgetr...
-000026b0: 00da 3570 7978 7933 642e 6775 692e 6361  ..5pyxy3d.gui.ca
-000026c0: 6d65 7261 5f63 6f6e 6669 672e 696e 7472  mera_config.intr
-000026d0: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
-000026e0: 6e5f 7769 6467 6574 721d 0000 005a 2a70  n_widgetr....Z*p
-000026f0: 7978 7933 642e 6775 692e 6361 6c69 6272  yxy3d.gui.calibr
-00002700: 6174 655f 6361 7074 7572 655f 766f 6c75  ate_capture_volu
-00002710: 6d65 5f77 6964 6765 7472 1e00 0000 da1b  me_widgetr......
-00002720: 7079 7879 3364 2e67 7569 2e72 6563 6f72  pyxy3d.gui.recor
-00002730: 6469 6e67 5f77 6964 6765 7472 1f00 0000  ding_widgetr....
-00002740: 5a21 7079 7879 3364 2e67 7569 2e70 6f73  Z!pyxy3d.gui.pos
-00002750: 745f 7072 6f63 6573 7369 6e67 5f77 6964  t_processing_wid
-00002760: 6765 7472 2000 0000 7221 0000 0072 3000  getr ...r!...r0.
-00002770: 0000 72a1 0000 0072 2e00 0000 722e 0000  ..r....r....r...
-00002780: 0072 2e00 0000 722f 0000 00da 083c 6d6f  .r....r/.....<mo
-00002790: 6475 6c65 3e01 0000 0073 3e00 0000 0800  dule>....s>.....
-000027a0: 0801 0c02 1402 0c02 0c01 0c01 0801 2c01  ..............,.
-000027b0: 080b 0c01 1801 0c01 1401 1001 0c01 0c01  ................
-000027c0: 0c01 0c01 0c01 0c03 0c01 0c01 1003 1008  ................
-000027d0: 007f 007f 0822 0808 0a01 04ff            ....."......
+00000190: 5a36 4700 6417 6418 8400 6418 6514 8303  Z6G.d.d...d.e...
+000001a0: 5a37 6419 641a 8400 5a38 6504 641b 6b02  Z7d.d...Z8e.d.k.
+000001b0: 72c7 6538 8300 0100 6401 5300 6401 5300  r.e8....d.S.d.S.
+000001c0: 291c e900 0000 004e 2903 da0b 514d 6169  )......N)...QMai
+000001d0: 6e57 696e 646f 77da 0e51 5374 6163 6b65  nWindow..QStacke
+000001e0: 644c 6179 6f75 74da 0b51 4669 6c65 4469  dLayout..QFileDi
+000001f0: 616c 6f67 2901 da04 5061 7468 2901 da06  alog)...Path)...
+00000200: 5468 7265 6164 2909 da0c 5141 7070 6c69  Thread)...QAppli
+00000210: 6361 7469 6f6e 7202 0000 0072 0300 0000  cationr....r....
+00000220: da07 5157 6964 6765 74da 0b51 446f 636b  ..QWidget..QDock
+00000230: 5769 6467 6574 da0b 5156 426f 784c 6179  Widget..QVBoxLay
+00000240: 6f75 74da 0551 4d65 6e75 da08 514d 656e  out..QMenu..QMen
+00000250: 7542 6172 da0a 5154 6162 5769 6467 6574  uBar..QTabWidget
+00000260: 2901 da04 456e 756d 2904 da05 5149 636f  )...Enum)...QIco
+00000270: 6eda 0751 4163 7469 6f6e da0c 514b 6579  n..QAction..QKey
+00000280: 5365 7175 656e 6365 da09 5153 686f 7274  Sequence..QShort
+00000290: 6375 7429 01da 0251 7429 03da 085f 5f72  cut)...Qt)...__r
+000002a0: 6f6f 745f 5fda 115f 5f73 6574 7469 6e67  oot__..__setting
+000002b0: 735f 7061 7468 5f5f da0c 5f5f 7573 6572  s_path__..__user
+000002c0: 5f64 6972 5f5f 2902 da07 5365 7373 696f  _dir__)...Sessio
+000002d0: 6eda 0b53 6573 7369 6f6e 4d6f 6465 2901  n..SessionMode).
+000002e0: da09 4c6f 6757 6964 6765 7429 01da 0c43  ..LogWidget)...C
+000002f0: 6f6e 6669 6775 7261 746f 7229 01da 1143  onfigurator)...C
+00000300: 616c 6962 7261 7469 6f6e 5769 6467 6574  alibrationWidget
+00000310: 2901 da0d 4368 6172 7563 6f57 6964 6765  )...CharucoWidge
+00000320: 7429 01da 1a49 6e74 7269 6e73 6963 4361  t)...IntrinsicCa
+00000330: 6c69 6272 6174 696f 6e57 6964 6765 7429  librationWidget)
+00000340: 01da 1c43 616c 6962 7261 7465 4361 7074  ...CalibrateCapt
+00000350: 7572 6556 6f6c 756d 6557 6964 6765 7429  ureVolumeWidget)
+00000360: 01da 0f52 6563 6f72 6469 6e67 5769 6467  ...RecordingWidg
+00000370: 6574 2901 da14 506f 7374 5072 6f63 6573  et)...PostProces
+00000380: 7369 6e67 5769 6467 6574 6300 0000 0000  singWidgetc.....
+00000390: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000003a0: 0000 0073 2000 0000 6500 5a01 6400 5a02  ...s ...e.Z.d.Z.
+000003b0: 6401 5a03 6402 5a04 6403 5a05 6404 5a06  d.Z.d.Z.d.Z.d.Z.
+000003c0: 6405 5a07 6406 5300 2907 da08 5461 6249  d.Z.d.S.)...TabI
+000003d0: 6e64 6578 7201 0000 00e9 0100 0000 e902  ndexr...........
+000003e0: 0000 00e9 0300 0000 e904 0000 004e 2908  .............N).
+000003f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000400: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000410: 6d65 5f5f da07 4368 6172 7563 6fda 0743  me__..Charuco..C
+00000420: 616d 6572 6173 da0d 4361 7074 7572 6556  ameras..CaptureV
+00000430: 6f6c 756d 65da 0952 6563 6f72 6469 6e67  olume..Recording
+00000440: da0a 5072 6f63 6573 7369 6e67 a900 722e  ..Processing..r.
+00000450: 0000 0072 2e00 0000 fa3a 433a 5c55 7365  ...r.....:C:\Use
+00000460: 7273 5c4d 6163 2050 7269 626c 655c 7265  rs\Mac Prible\re
+00000470: 706f 735c 7079 7879 3364 5c70 7978 7933  pos\pyxy3d\pyxy3
+00000480: 645c 6775 695c 6d61 696e 5f77 6964 6765  d\gui\main_widge
+00000490: 742e 7079 7221 0000 0029 0000 0073 0c00  t.pyr!...)...s..
+000004a0: 0000 0800 0401 0401 0401 0401 0801 7221  ..............r!
+000004b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000004c0: 0000 0000 0300 0000 0000 0000 73b0 0000  ............s...
+000004d0: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+000004e0: 0284 085a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
+000004f0: 0684 005a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
+00000500: 0a84 005a 0764 0b64 0c84 005a 0864 0d65  ...Z.d.d...Z.d.e
+00000510: 0966 0264 0e64 0f84 045a 0a64 1064 1184  .f.d.d...Z.d.d..
+00000520: 005a 0b64 1264 1384 005a 0c64 1464 1584  .Z.d.d...Z.d.d..
+00000530: 005a 0d64 1664 1784 005a 0e64 1864 1984  .Z.d.d...Z.d.d..
+00000540: 005a 0f64 1a64 1b84 005a 1064 1c65 0966  .Z.d.d...Z.d.e.f
+00000550: 0264 1d64 1e84 045a 1164 1f64 2084 005a  .d.d...Z.d.d ..Z
+00000560: 1264 2164 2284 005a 1364 2364 2484 005a  .d!d"..Z.d#d$..Z
+00000570: 1464 2564 2684 005a 1587 0004 005a 1653  .d%d&..Z.....Z.S
+00000580: 0029 27da 0a4d 6169 6e57 696e 646f 7763  .)'..MainWindowc
+00000590: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000005a0: 0700 0000 0300 0000 73aa 0100 0074 0074  ........s....t.t
+000005b0: 017c 0083 02a0 02a1 0001 0074 03a0 0474  .|.........t...t
+000005c0: 05a1 017c 005f 067c 00a0 0764 01a1 0101  ...|._.|...d....
+000005d0: 007c 00a0 0874 0974 0a74 0b74 0c64 0283  .|...t.t.t.t.d..
+000005e0: 0283 0183 01a1 0101 007c 00a0 0d64 0364  .........|...d.d
+000005f0: 03a1 0201 007c 00a0 0ea1 007c 005f 0f7c  .....|.....|._.|
+00000600: 006a 0fa0 1064 04a1 017c 005f 1174 1264  .j...d...|._.t.d
+00000610: 057c 0083 027c 005f 137c 006a 136a 14a0  .|...|._.|.j.j..
+00000620: 157c 006a 16a1 0101 007c 006a 11a0 177c  .|.j.....|.j...|
+00000630: 006a 13a1 0101 0074 1864 067c 0083 027c  .j.....t.d.|...|
+00000640: 005f 1974 1a7c 006a 0664 0719 0083 0144  ._.t.|.j.d.....D
+00000650: 005d 077d 017c 00a0 1b7c 01a1 0101 0071  .].}.|...|.....q
+00000660: 527c 006a 11a0 107c 006a 19a1 0101 0074  R|.j...|.j.....t
+00000670: 1264 087c 0083 027c 005f 1c7c 006a 11a0  .d.|...|._.|.j..
+00000680: 177c 006a 1ca1 0101 007c 006a 0fa0 1064  .|.j.....|.j...d
+00000690: 09a1 017c 005f 1d74 1264 0a7c 0083 027c  ...|._.t.d.|...|
+000006a0: 005f 1e7c 006a 1da0 177c 006a 1ea1 0101  ._.|.j...|.j....
+000006b0: 007c 006a 1ea0 1f64 0ba1 0101 0074 1264  .|.j...d.....t.d
+000006c0: 0c7c 0083 027c 005f 207c 006a 1da0 177c  .|...|._ |.j...|
+000006d0: 006a 20a1 0101 007c 006a 20a0 1f64 0ba1  .j ....|.j ..d..
+000006e0: 0101 007c 00a0 21a1 0001 0074 2283 007c  ...|..!....t"..|
+000006f0: 005f 237c 00a0 247c 006a 23a1 0101 0074  ._#|..$|.j#....t
+00000700: 2564 0d7c 0083 027c 005f 267c 006a 26a0  %d.|...|._&|.j&.
+00000710: 2774 256a 286a 29a1 0101 007c 006a 26a0  't%j(j)....|.j&.
+00000720: 2a74 2b6a 2c6a 2da1 0101 0074 2e83 007c  *t+j,j-....t...|
+00000730: 005f 2f7c 006a 26a0 307c 006a 2fa1 0101  ._/|.j&.0|.j/...
+00000740: 007c 00a0 3174 2b6a 2c6a 2d7c 006a 26a1  .|..1t+j,j-|.j&.
+00000750: 0201 0064 0053 0029 0e4e 5a06 5079 7879  ...d.S.).NZ.Pyxy
+00000760: 3344 7a1e 7079 7879 3364 2f67 7569 2f69  3Dz.pyxy3d/gui/i
+00000770: 636f 6e73 2f70 7978 795f 6c6f 676f 2e73  cons/pyxy_logo.s
+00000780: 7667 69f4 0100 00da 0446 696c 657a 104e  vgi......Filez.N
+00000790: 6577 2f4f 7065 6e20 5072 6f6a 6563 747a  ew/Open Projectz
+000007a0: 1252 6563 656e 7420 5072 6f6a 6563 7473  .Recent Projects
+000007b0: 2e2e 2eda 0f72 6563 656e 745f 7072 6f6a  .....recent_proj
+000007c0: 6563 7473 5a04 4578 6974 722a 0000 007a  ectsZ.Exitr*...z
+000007d0: 0f43 6f6e 6e65 6374 2043 616d 6572 6173  .Connect Cameras
+000007e0: 467a 1244 6973 636f 6e6e 6563 7420 4361  Fz.Disconnect Ca
+000007f0: 6d65 7261 735a 034c 6f67 2932 da05 7375  merasZ.Log)2..su
+00000800: 7065 7272 3000 0000 da08 5f5f 696e 6974  perr0.....__init
+00000810: 5f5f da04 746f 6d6c da04 6c6f 6164 7215  __..toml..loadr.
+00000820: 0000 00da 0c61 7070 5f73 6574 7469 6e67  .....app_setting
+00000830: 73da 0e73 6574 5769 6e64 6f77 5469 746c  s..setWindowTitl
+00000840: 65da 0d73 6574 5769 6e64 6f77 4963 6f6e  e..setWindowIcon
+00000850: 720f 0000 00da 0373 7472 7205 0000 0072  r......strr....r
+00000860: 1400 0000 da0e 7365 744d 696e 696d 756d  ......setMinimum
+00000870: 5369 7a65 5a07 6d65 6e75 4261 72da 046d  SizeZ.menuBar..m
+00000880: 656e 75da 0761 6464 4d65 6e75 5a09 6669  enu..addMenuZ.fi
+00000890: 6c65 5f6d 656e 7572 1000 0000 5a13 6f70  le_menur....Z.op
+000008a0: 656e 5f70 726f 6a65 6374 5f61 6374 696f  en_project_actio
+000008b0: 6eda 0974 7269 6767 6572 6564 da07 636f  n..triggered..co
+000008c0: 6e6e 6563 74da 1963 7265 6174 655f 6e65  nnect..create_ne
+000008d0: 775f 7072 6f6a 6563 745f 666f 6c64 6572  w_project_folder
+000008e0: da09 6164 6441 6374 696f 6e72 0b00 0000  ..addActionr....
+000008f0: da1b 6f70 656e 5f72 6563 656e 745f 7072  ..open_recent_pr
+00000900: 6f6a 6563 745f 7375 626d 656e 75da 0872  oject_submenu..r
+00000910: 6576 6572 7365 64da 1561 6464 5f74 6f5f  eversed..add_to_
+00000920: 7265 6365 6e74 5f70 726f 6a65 6374 da12  recent_project..
+00000930: 6578 6974 5f70 7978 7933 645f 6163 7469  exit_pyxy3d_acti
+00000940: 6f6e 5a0c 6361 6d65 7261 735f 6d65 6e75  onZ.cameras_menu
+00000950: da16 636f 6e6e 6563 745f 6361 6d65 7261  ..connect_camera
+00000960: 735f 6163 7469 6f6e da0a 7365 7445 6e61  s_action..setEna
+00000970: 626c 6564 da19 6469 7363 6f6e 6e65 6374  bled..disconnect
+00000980: 5f63 616d 6572 6173 5f61 6374 696f 6eda  _cameras_action.
+00000990: 1463 6f6e 6e65 6374 5f6d 656e 755f 6163  .connect_menu_ac
+000009a0: 7469 6f6e 7372 0d00 0000 da0a 7461 625f  tionsr......tab_
+000009b0: 7769 6467 6574 da10 7365 7443 656e 7472  widget..setCentr
+000009c0: 616c 5769 6467 6574 7209 0000 005a 0d64  alWidgetr....Z.d
+000009d0: 6f63 6b65 645f 6c6f 6767 6572 5a0b 7365  ocked_loggerZ.se
+000009e0: 7446 6561 7475 7265 735a 1144 6f63 6b57  tFeaturesZ.DockW
+000009f0: 6964 6765 7446 6561 7475 7265 5a11 446f  idgetFeatureZ.Do
+00000a00: 636b 5769 6467 6574 4d6f 7661 626c 655a  ckWidgetMovableZ
+00000a10: 0f73 6574 416c 6c6f 7765 6441 7265 6173  .setAllowedAreas
+00000a20: 7213 0000 00da 0e44 6f63 6b57 6964 6765  r......DockWidge
+00000a30: 7441 7265 61da 1442 6f74 746f 6d44 6f63  tArea..BottomDoc
+00000a40: 6b57 6964 6765 7441 7265 6172 1900 0000  kWidgetArear....
+00000a50: 5a0a 6c6f 675f 7769 6467 6574 da09 7365  Z.log_widget..se
+00000a60: 7457 6964 6765 74da 0d61 6464 446f 636b  tWidget..addDock
+00000a70: 5769 6467 6574 2902 da04 7365 6c66 da0c  Widget)...self..
+00000a80: 7072 6f6a 6563 745f 7061 7468 a901 da09  project_path....
+00000a90: 5f5f 636c 6173 735f 5f72 2e00 0000 722f  __class__r....r/
+00000aa0: 0000 0072 3400 0000 3200 0000 7340 0000  ...r4...2...s@..
+00000ab0: 000e 010c 020a 0218 010c 010a 030e 010c  ................
+00000ac0: 0310 010e 010c 0312 030c 010e 020c 020e  ................
+00000ad0: 010e 020c 010e 010c 010c 020e 010c 0108  ................
+00000ae0: 0208 030c 020c 0310 0110 0108 010e 0116  ................
+00000af0: 027a 134d 6169 6e57 696e 646f 772e 5f5f  .z.MainWindow.__
+00000b00: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000b10: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000b20: 3800 0000 7c00 6a00 6a01 a002 7c00 6a03  8...|.j.j...|.j.
+00000b30: a101 0100 7c00 6a04 6a01 a002 7405 a006  ....|.j.j...t...
+00000b40: a100 6a07 a101 0100 7c00 6a08 6a01 a002  ..j.....|.j.j...
+00000b50: 7c00 6a09 a101 0100 6400 5300 a901 4e29  |.j.....d.S...N)
+00000b60: 0a72 4600 0000 723e 0000 0072 3f00 0000  .rF...r>...r?...
+00000b70: da11 6c6f 6164 5f73 7472 6561 6d5f 746f  ..load_stream_to
+00000b80: 6f6c 7372 4500 0000 7207 0000 00da 0869  olsrE...r......i
+00000b90: 6e73 7461 6e63 65da 0471 7569 7472 4800  nstance..quitrH.
+00000ba0: 0000 da12 6469 7363 6f6e 6e65 6374 5f63  ....disconnect_c
+00000bb0: 616d 6572 6173 a901 7250 0000 0072 2e00  ameras..rP...r..
+00000bc0: 0000 722e 0000 0072 2f00 0000 7249 0000  ..r....r/...rI..
+00000bd0: 006b 0000 0073 0600 0000 1001 1401 1401  .k...s..........
+00000be0: 7a1f 4d61 696e 5769 6e64 6f77 2e63 6f6e  z.MainWindow.con
+00000bf0: 6e65 6374 5f6d 656e 755f 6163 7469 6f6e  nect_menu_action
+00000c00: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+00000c10: 0000 0400 0000 4300 0000 73b4 0000 007c  ......C...s....|
+00000c20: 006a 00a0 017c 006a 02a1 0101 007c 006a  .j...|.j.....|.j
+00000c30: 00a0 0374 046a 056a 0664 01a1 0201 007c  ...t.j.j.d.....|
+00000c40: 006a 00a0 0374 046a 076a 0664 02a1 0201  .j...t.j.j.d....
+00000c50: 007c 006a 00a0 0374 046a 086a 0664 02a1  .|.j...t.j.j.d..
+00000c60: 0201 007c 006a 00a0 0374 046a 096a 0664  ...|.j...t.j.j.d
+00000c70: 02a1 0201 007c 006a 00a0 0374 046a 0a6a  .....|.j...t.j.j
+00000c80: 0664 01a1 0201 0074 0b83 007c 005f 0c74  .d.....t...|._.t
+00000c90: 0b83 007c 005f 0d74 0b83 007c 005f 0e7c  ...|._.t...|._.|
+00000ca0: 006a 0fa0 1074 116a 05a1 0101 007c 006a  .j...t.j.....|.j
+00000cb0: 0fa0 12a1 0001 007c 006a 13a0 1464 02a1  .......|.j...d..
+00000cc0: 0101 007c 006a 15a0 1464 01a1 0101 0064  ...|.j...d.....d
+00000cd0: 0053 0029 034e 5446 2916 724a 0000 00da  .S.).NTF).rJ....
+00000ce0: 1073 6574 4375 7272 656e 7457 6964 6765  .setCurrentWidge
+00000cf0: 74da 0e63 6861 7275 636f 5f77 6964 6765  t..charuco_widge
+00000d00: 74da 0d73 6574 5461 6245 6e61 626c 6564  t..setTabEnabled
+00000d10: 7221 0000 0072 2900 0000 da05 7661 6c75  r!...r).....valu
+00000d20: 6572 2a00 0000 722b 0000 0072 2c00 0000  er*...r+...r,...
+00000d30: 722d 0000 0072 0800 0000 da0d 6361 6d65  r-...r......came
+00000d40: 7261 5f77 6964 6765 74da 1f63 616c 6962  ra_widget..calib
+00000d50: 7261 7465 5f63 6170 7475 7265 5f76 6f6c  rate_capture_vol
+00000d60: 756d 655f 7769 6467 6574 da10 7265 636f  ume_widget..reco
+00000d70: 7264 696e 675f 7769 6467 6574 da07 7365  rding_widget..se
+00000d80: 7373 696f 6eda 0873 6574 5f6d 6f64 6572  ssion..set_moder
+00000d90: 1800 0000 7258 0000 0072 4800 0000 7247  ....rX...rH...rG
+00000da0: 0000 0072 4600 0000 7259 0000 0072 2e00  ...rF...rY...r..
+00000db0: 0000 722e 0000 0072 2f00 0000 7258 0000  ..r....r/...rX..
+00000dc0: 0070 0000 0073 1a00 0000 0e01 1201 1201  .p...s..........
+00000dd0: 1201 1201 1201 0802 0801 0801 0e02 0a01  ................
+00000de0: 0c01 1001 7a1d 4d61 696e 5769 6e64 6f77  ....z.MainWindow
+00000df0: 2e64 6973 636f 6e6e 6563 745f 6361 6d65  .disconnect_came
+00000e00: 7261 7363 0100 0000 0000 0000 0000 0000  rasc............
+00000e10: 0100 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
+00000e20: 0074 00a0 0164 01a1 0101 007c 006a 02a0  .t...d.....|.j..
+00000e30: 03a1 0001 007c 006a 02a0 04a1 0001 0064  .....|.j.......d
+00000e40: 0053 0029 024e 7a55 5061 7573 696e 6720  .S.).NzUPausing 
+00000e50: 616c 6c20 6672 616d 6520 7265 6164 696e  all frame readin
+00000e60: 6720 6174 206c 6f61 6420 6f66 2073 7472  g at load of str
+00000e70: 6561 6d20 746f 6f6c 733b 2073 686f 756c  eam tools; shoul
+00000e80: 6420 6265 206f 6e20 6368 6172 7563 6f20  d be on charuco 
+00000e90: 7461 6220 7269 6768 7420 6e6f 7729 05da  tab right now)..
+00000ea0: 066c 6f67 6765 72da 0469 6e66 6f72 6100  .logger..infora.
+00000eb0: 0000 da19 7061 7573 655f 616c 6c5f 6d6f  ....pause_all_mo
+00000ec0: 6e6f 6361 6c69 6272 6174 6f72 73da 1270  nocalibrators..p
+00000ed0: 6175 7365 5f73 796e 6368 726f 6e69 7a65  ause_synchronize
+00000ee0: 7272 5900 0000 722e 0000 0072 2e00 0000  rrY...r....r....
+00000ef0: 722f 0000 00da 1770 6175 7365 5f61 6c6c  r/.....pause_all
+00000f00: 5f66 7261 6d65 5f72 6561 6469 6e67 8100  _frame_reading..
+00000f10: 0000 7306 0000 000a 010a 010e 017a 224d  ..s..........z"M
+00000f20: 6169 6e57 696e 646f 772e 7061 7573 655f  ainWindow.pause_
+00000f30: 616c 6c5f 6672 616d 655f 7265 6164 696e  all_frame_readin
+00000f40: 6763 0100 0000 0000 0000 0000 0000 0100  gc..............
+00000f50: 0000 0500 0000 4300 0000 734a 0000 007c  ......C...sJ...|
+00000f60: 006a 00a0 0164 01a1 0101 007c 006a 02a0  .j...d.....|.j..
+00000f70: 0164 02a1 0101 007c 006a 036a 04a0 057c  .d.....|.j.j...|
+00000f80: 006a 06a1 0101 0074 077c 006a 036a 0864  .j.....t.|.j.j.d
+00000f90: 0364 0264 048d 037c 005f 097c 006a 09a0  .d.d...|._.|.j..
+00000fa0: 0aa1 0001 0064 0053 0029 054e 4654 722e  .....d.S.).NFTr.
+00000fb0: 0000 0029 03da 0674 6172 6765 74da 0461  ...)...target..a
+00000fc0: 7267 73da 0664 6165 6d6f 6e29 0b72 4600  rgs..daemon).rF.
+00000fd0: 0000 7247 0000 0072 4800 0000 7261 0000  ..rG...rH...ra..
+00000fe0: 00da 1a73 7472 6561 6d5f 746f 6f6c 735f  ...stream_tools_
+00000ff0: 6c6f 6164 6564 5f73 6967 6e61 6c72 3f00  loaded_signalr?.
+00001000: 0000 7267 0000 0072 0600 0000 7255 0000  ..rg...r....rU..
+00001010: 00da 0674 6872 6561 64da 0573 7461 7274  ...thread..start
+00001020: 7259 0000 0072 2e00 0000 722e 0000 0072  rY...r....r....r
+00001030: 2f00 0000 7255 0000 0086 0000 0073 0e00  /...rU.......s..
+00001040: 0000 0c01 0c01 1001 0201 0a01 08ff 0e03  ................
+00001050: 7a1c 4d61 696e 5769 6e64 6f77 2e6c 6f61  z.MainWindow.loa
+00001060: 645f 7374 7265 616d 5f74 6f6f 6c73 6302  d_stream_toolsc.
+00001070: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00001080: 0000 0043 0000 0073 4401 0000 7400 a001  ...C...sD...t...
+00001090: 6401 7c01 9b00 9d02 a101 0100 7c01 0400  d.|.........|...
+000010a0: 7402 6a03 6a04 6b02 721e 0100 7400 a001  t.j.j.k.r...t...
+000010b0: 6402 a101 0100 7c00 6a05 a006 7407 6a03  d.....|.j...t.j.
+000010c0: a101 0100 6400 5300 0400 7402 6a08 6a04  ....d.S...t.j.j.
+000010d0: 6b02 7233 0100 7400 a001 6403 a101 0100  k.r3..t...d.....
+000010e0: 7c00 6a05 a006 7407 6a09 a101 0100 6400  |.j...t.j.....d.
+000010f0: 5300 0400 7402 6a0a 6a04 6b02 725c 0100  S...t.j.j.k.r\..
+00001100: 7400 a001 6404 a101 0100 7c00 6a05 a00b  t...d.....|.j...
+00001110: a100 7250 7400 a001 6405 a101 0100 7c00  ..rPt...d.....|.
+00001120: 6a0c a00d a100 0100 6400 5300 7400 a001  j.......d.S.t...
+00001130: 6406 a101 0100 7c00 6a0c a00e a100 0100  d.....|.j.......
+00001140: 6400 5300 0400 7402 6a0f 6a04 6b02 7288  d.S...t.j.j.k.r.
+00001150: 0100 7400 a001 6407 a101 0100 7a0d 7400  ..t...d.....z.t.
+00001160: a001 6408 a101 0100 7c00 6a0c 6a10 a011  ..d.....|.j.j...
+00001170: a100 0100 5700 6e09 0100 0100 0100 7400  ....W.n.......t.
+00001180: a001 6409 a101 0100 5900 7c00 6a05 a006  ..d.....Y.|.j...
+00001190: 7407 6a0f a101 0100 6400 5300 7402 6a12  t.j.....d.S.t.j.
+000011a0: 6a04 6b02 72a0 7400 a001 640a a101 0100  j.k.r.t...d.....
+000011b0: 7c00 6a05 a006 7407 6a13 a101 0100 7c00  |.j...t.j.....|.
+000011c0: 6a14 a015 a100 0100 6400 5300 6400 5300  j.......d.S.d.S.
+000011d0: 290b 4e7a 1d53 7769 7463 6869 6e67 206d  ).Nz.Switching m
+000011e0: 6169 6e20 7769 6e64 6f77 2074 6f20 7461  ain window to ta
+000011f0: 6220 7a19 4163 7469 7661 7469 6e67 2043  b z.Activating C
+00001200: 6861 7275 636f 2057 6964 6765 747a 1e41  haruco Widgetz.A
+00001210: 6374 6976 6174 696e 6720 4361 6d65 7261  ctivating Camera
+00001220: 2053 6574 7570 2057 6964 6765 747a 2a41   Setup Widgetz*A
+00001230: 6374 6976 6174 696e 6720 4361 6c69 6272  ctivating Calibr
+00001240: 6174 6520 4361 7074 7572 6520 566f 6c75  ate Capture Volu
+00001250: 6d65 2057 6964 6765 747a 5353 6573 7369  me WidgetzSSessi
+00001260: 6f6e 2069 7320 656c 6967 6962 6c65 2066  on is eligible f
+00001270: 6f72 2073 6574 7469 6e67 206f 6620 6f72  or setting of or
+00001280: 6967 696e 2e2e 2e61 6374 6976 6174 696e  igin...activatin
+00001290: 6720 6361 7074 7572 6520 766f 6c75 6d65  g capture volume
+000012a0: 206f 7269 6769 6e20 7769 6467 6574 7a57   origin widgetzW
+000012b0: 5365 7373 696f 6e20 6973 206e 6f74 2065  Session is not e
+000012c0: 6c69 6769 626c 6520 666f 7220 7365 7474  ligible for sett
+000012d0: 696e 6720 6f66 206f 7269 6769 6e2e 2e2e  ing of origin...
+000012e0: 6163 7469 7661 7469 6e67 2065 7874 7269  activating extri
+000012f0: 6e73 6963 2063 616c 6962 7261 7469 6f6e  nsic calibration
+00001300: 2077 6964 6765 747a 1741 6374 6976 6174   widgetz.Activat
+00001310: 6520 5265 636f 7264 696e 6720 4d6f 6465  e Recording Mode
+00001320: 7a38 4174 7465 6d70 7469 6e67 2074 6f20  z8Attempting to 
+00001330: 7370 696e 2064 6f77 6e20 7468 6520 6578  spin down the ex
+00001340: 7472 696e 7369 6320 6361 6c69 6272 6174  trinsic calibrat
+00001350: 696f 6e20 7769 6467 6574 7a32 4e6f 2065  ion widgetz2No e
+00001360: 7874 7269 6e73 6963 2063 616c 6962 7261  xtrinsic calibra
+00001370: 7469 6f6e 2063 616c 6962 7261 7469 6f6e  tion calibration
+00001380: 2077 6964 6765 7420 6578 6973 7473 7a18   widget existsz.
+00001390: 4163 7469 7661 7465 2050 726f 6365 7373  Activate Process
+000013a0: 696e 6720 4d6f 6465 2916 7263 0000 0072  ing Mode).rc...r
+000013b0: 6400 0000 7221 0000 0072 2900 0000 725d  d...r!...r)...r]
+000013c0: 0000 0072 6100 0000 7262 0000 0072 1800  ...ra...rb...r..
+000013d0: 0000 722a 0000 00da 1449 6e74 7269 6e73  ..r*.....Intrins
+000013e0: 6963 4361 6c69 6272 6174 696f 6e72 2b00  icCalibrationr+.
+000013f0: 0000 da1a 6973 5f63 6170 7475 7265 5f76  ....is_capture_v
+00001400: 6f6c 756d 655f 656c 6967 6962 6c65 725f  olume_eligibler_
+00001410: 0000 005a 1e61 6374 6976 6174 655f 6361  ...Z.activate_ca
+00001420: 7074 7572 655f 766f 6c75 6d65 5f77 6964  pture_volume_wid
+00001430: 6765 745a 2561 6374 6976 6174 655f 6578  getZ%activate_ex
+00001440: 7472 696e 7369 635f 6361 6c69 6272 6174  trinsic_calibrat
+00001450: 696f 6e5f 7769 6467 6574 722c 0000 00da  ion_widgetr,....
+00001460: 1c65 7874 7269 6e73 6963 5f63 616c 6962  .extrinsic_calib
+00001470: 7261 7469 6f6e 5f77 6964 6765 74da 1073  ration_widget..s
+00001480: 6875 7464 6f77 6e5f 7468 7265 6164 7372  hutdown_threadsr
+00001490: 2d00 0000 da0e 506f 7374 5072 6f63 6573  -.....PostProces
+000014a0: 7369 6e67 da11 7072 6f63 6573 7369 6e67  sing..processing
+000014b0: 5f77 6964 6765 745a 1875 7064 6174 655f  _widgetZ.update_
+000014c0: 7265 636f 7264 696e 675f 666f 6c64 6572  recording_folder
+000014d0: 73a9 0272 5000 0000 da05 696e 6465 7872  s..rP.....indexr
+000014e0: 2e00 0000 722e 0000 0072 2f00 0000 da0e  ....r....r/.....
+000014f0: 6f6e 5f74 6162 5f63 6861 6e67 6564 9100  on_tab_changed..
+00001500: 0000 7338 0000 0010 0102 010e 010a 0112  ..s8............
+00001510: 020e 010a 0112 020e 010a 010a 020a 010e  ................
+00001520: 010a 020e 010e 020a 0102 020a 0110 0106  ................
+00001530: 010c 0112 020a 010a 010e 020e 0204 fb7a  ...............z
+00001540: 194d 6169 6e57 696e 646f 772e 6f6e 5f74  .MainWindow.on_t
+00001550: 6162 5f63 6861 6e67 6564 da0e 7061 7468  ab_changed..path
+00001560: 5f74 6f5f 666f 6c64 6572 6302 0000 0000  _to_folderc.....
+00001570: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+00001580: 0000 0073 f000 0000 7400 7c01 8301 7d02  ...s....t.|...}.
+00001590: 7401 7c02 8301 7c00 5f02 7403 a004 6401  t.|...|._.t...d.
+000015a0: 7c02 9b00 9d02 a101 0100 7405 7c00 6a02  |.........t.|.j.
+000015b0: 8301 7c00 5f06 7407 7c00 6a06 8301 7c00  ..|._.t.|.j...|.
+000015c0: 5f08 7409 8300 7c00 5f0a 7409 8300 7c00  _.t...|._.t...|.
+000015d0: 5f0b 7409 8300 7c00 5f0c 7409 8300 7c00  _.t...|._.t...|.
+000015e0: 5f0d 7c00 6a0e a00f 7c00 6a08 6402 a102  _.|.j...|.j.d...
+000015f0: 0100 7c00 6a0e a00f 7c00 6a0a 6403 a102  ..|.j...|.j.d...
+00001600: 0100 7c00 6a0e a00f 7c00 6a0d 6404 a102  ..|.j...|.j.d...
+00001610: 0100 7c00 6a0e a00f 7c00 6a0b 6405 a102  ..|.j...|.j.d...
+00001620: 0100 7c00 6a0e a00f 7c00 6a0c 6406 a102  ..|.j...|.j.d...
+00001630: 0100 7c00 6a0e 6a10 a011 7c00 6a12 a101  ..|.j.j...|.j...
+00001640: 0100 7c00 6a13 a014 6407 a101 0100 7c00  ..|.j...d.....|.
+00001650: a015 a100 0100 7c00 6a0e a016 a100 7d03  ......|.j.....}.
+00001660: 7c00 6a0e a017 7c03 a101 0100 7c00 a018  |.j...|.....|...
+00001670: a100 0100 6400 5300 2908 4e7a 2d4c 6175  ....d.S.).Nz-Lau
+00001680: 6e63 6869 6e67 2073 6573 7369 6f6e 2077  nching session w
+00001690: 6974 6820 636f 6e66 6967 2066 696c 6520  ith config file 
+000016a0: 7374 6f72 6564 2069 6e20 7229 0000 0072  stored in r)...r
+000016b0: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
+000016c0: 0000 0054 2919 7205 0000 0072 1a00 0000  ...T).r....r....
+000016d0: da06 636f 6e66 6967 7263 0000 0072 6400  ..configrc...rd.
+000016e0: 0000 7217 0000 0072 6100 0000 721c 0000  ..r....ra...r...
+000016f0: 0072 5b00 0000 7208 0000 0072 5e00 0000  .r[...r....r^...
+00001700: 7260 0000 0072 7300 0000 725f 0000 0072  r`...rs...r_...r
+00001710: 4a00 0000 da06 6164 6454 6162 da0e 6375  J.....addTab..cu
+00001720: 7272 656e 7443 6861 6e67 6564 723f 0000  rrentChangedr?..
+00001730: 0072 7600 0000 7246 0000 0072 4700 0000  .rv...rF...rG...
+00001740: da0b 7570 6461 7465 5f74 6162 73da 0c63  ..update_tabs..c
+00001750: 7572 7265 6e74 496e 6465 78da 0f73 6574  urrentIndex..set
+00001760: 4375 7272 656e 7449 6e64 6578 da17 636f  CurrentIndex..co
+00001770: 6e6e 6563 745f 7365 7373 696f 6e5f 7369  nnect_session_si
+00001780: 676e 616c 7329 0472 5000 0000 7277 0000  gnals).rP...rw..
+00001790: 00da 0c73 6573 7369 6f6e 5f70 6174 685a  ...session_pathZ
+000017a0: 096f 6c64 5f69 6e64 6578 722e 0000 0072  .old_indexr....r
+000017b0: 2e00 0000 722f 0000 00da 0e6c 6175 6e63  ....r/.....launc
+000017c0: 685f 7365 7373 696f 6eb7 0000 0073 2800  h_session....s(.
+000017d0: 0000 0801 0a01 1001 0c01 0c03 0803 0801  ................
+000017e0: 0801 0801 1002 1001 1001 1001 1001 1003  ................
+000017f0: 0c03 0804 0a03 0c02 0c01 7a19 4d61 696e  ..........z.Main
+00001800: 5769 6e64 6f77 2e6c 6175 6e63 685f 7365  Window.launch_se
+00001810: 7373 696f 6e63 0100 0000 0000 0000 0000  ssionc..........
+00001820: 0000 0100 0000 0400 0000 4300 0000 7308  ..........C...s.
+00001830: 0100 007c 006a 00a0 0174 026a 036a 0464  ...|.j...t.j.j.d
+00001840: 01a1 0201 007c 006a 056a 0672 4a74 077c  .....|.j.j.rJt.|
+00001850: 006a 0883 0174 096b 0372 187c 00a0 0aa1  .j...t.k.r.|....
+00001860: 0001 0074 077c 006a 0b83 0174 0c6b 0372  ...t.|.j...t.k.r
+00001870: 237c 00a0 0da1 0001 0074 077c 006a 0e83  #|.......t.|.j..
+00001880: 0174 0f6b 0372 2e7c 00a0 10a1 0001 007c  .t.k.r.|.......|
+00001890: 006a 00a0 0174 026a 116a 0464 01a1 0201  .j...t.j.j.d....
+000018a0: 007c 006a 00a0 0174 026a 126a 0464 01a1  .|.j...t.j.j.d..
+000018b0: 0201 007c 006a 00a0 0174 026a 136a 0464  ...|.j...t.j.j.d
+000018c0: 01a1 0201 006e 1b7c 006a 00a0 0174 026a  .....n.|.j...t.j
+000018d0: 116a 0464 02a1 0201 007c 006a 00a0 0174  .j.d.....|.j...t
+000018e0: 026a 126a 0464 02a1 0201 007c 006a 00a0  .j.j.d.....|.j..
+000018f0: 0174 026a 136a 0464 02a1 0201 007c 006a  .t.j.j.d.....|.j
+00001900: 05a0 14a1 0072 797c 00a0 15a1 0001 007c  .....ry|.......|
+00001910: 006a 00a0 0174 026a 166a 0464 01a1 0201  .j...t.j.j.d....
+00001920: 0064 0353 007c 006a 00a0 0174 026a 166a  .d.S.|.j...t.j.j
+00001930: 0464 02a1 0201 0064 0353 0029 0461 0b01  .d.....d.S.).a..
+00001940: 0000 0a20 2020 2020 2020 2054 6162 2075  ...        Tab u
+00001950: 7064 6174 6573 206f 6363 7572 2070 7269  pdates occur pri
+00001960: 6d61 7269 6c79 2061 7420 3220 7469 6d65  marily at 2 time
+00001970: 733a 0a20 2020 2020 2020 2031 2e20 7570  s:.        1. up
+00001980: 6f6e 206d 6169 6e20 7769 6e64 6f77 2069  on main window i
+00001990: 6e69 7469 6174 696f 6e20 7768 656e 206f  nitiation when o
+000019a0: 6666 6c69 6e65 2063 6170 6163 6974 6965  ffline capacitie
+000019b0: 7320 0a20 2020 2020 2020 2028 6361 7074  s .        (capt
+000019c0: 7572 6520 766f 6c75 6d65 2061 6e64 2070  ure volume and p
+000019d0: 6f73 742d 7072 6f63 6573 7369 6e67 2920  ost-processing) 
+000019e0: 6d61 7920 6265 2061 7661 696c 6162 6c65  may be available
+000019f0: 2e0a 0a20 2020 2020 2020 2032 2e20 7570  ...        2. up
+00001a00: 6f6e 206c 6f61 6469 6e67 206f 6620 7374  on loading of st
+00001a10: 7265 616d 2074 6f6f 6c73 2077 6865 6e20  ream tools when 
+00001a20: 6361 6d65 7261 732f 7265 636f 7264 696e  cameras/recordin
+00001a30: 6720 776f 756c 6420 6265 2061 7661 696c  g would be avail
+00001a40: 6162 6c65 0a20 2020 2020 2020 2054 464e  able.        TFN
+00001a50: 2917 724a 0000 0072 5c00 0000 7221 0000  ).rJ...r\...r!..
+00001a60: 0072 2900 0000 725d 0000 0072 6100 0000  .r)...r]...ra...
+00001a70: da13 7374 7265 616d 5f74 6f6f 6c73 5f6c  ..stream_tools_l
+00001a80: 6f61 6465 64da 0474 7970 6572 5e00 0000  oaded..typer^...
+00001a90: 721d 0000 00da 126c 6f61 645f 6361 6d65  r......load_came
+00001aa0: 7261 5f77 6964 6765 7472 6000 0000 721f  ra_widgetr`...r.
+00001ab0: 0000 00da 156c 6f61 645f 7265 636f 7264  .....load_record
+00001ac0: 696e 675f 7769 6467 6574 725f 0000 0072  ing_widgetr_...r
+00001ad0: 1e00 0000 da1a 6c6f 6164 5f63 6170 7475  ......load_captu
+00001ae0: 7265 5f76 6f6c 756d 655f 7769 6467 6574  re_volume_widget
+00001af0: 722a 0000 0072 2c00 0000 722b 0000 00da  r*...r,...r+....
+00001b00: 1b69 735f 706f 7374 5f70 726f 6365 7373  .is_post_process
+00001b10: 696e 675f 656c 6967 6962 6c65 da1b 6c6f  ing_eligible..lo
+00001b20: 6164 5f70 6f73 745f 7072 6f63 6573 7369  ad_post_processi
+00001b30: 6e67 5f77 6964 6765 7472 2d00 0000 7259  ng_widgetr-...rY
+00001b40: 0000 0072 2e00 0000 722e 0000 0072 2f00  ...r....r....r/.
+00001b50: 0000 727b 0000 00dc 0000 0073 2400 0000  ..r{.......s$...
+00001b60: 120a 0803 0e02 0801 0e02 0801 0e02 0801  ................
+00001b70: 1202 1201 1401 1205 1201 1201 0a03 0801  ................
+00001b80: 1601 1602 7a16 4d61 696e 5769 6e64 6f77  ....z.MainWindow
+00001b90: 2e75 7064 6174 655f 7461 6273 6301 0000  .update_tabsc...
+00001ba0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00001bb0: 0043 0000 0073 2400 0000 7c00 6a00 6a01  .C...s$...|.j.j.
+00001bc0: a002 7c00 6a03 a101 0100 7c00 6a00 6a04  ..|.j.....|.j.j.
+00001bd0: a002 7c00 6a05 a101 0100 6401 5300 2902  ..|.j.....d.S.).
+00001be0: 7a90 0a20 2020 2020 2020 2041 6674 6572  z..        After
+00001bf0: 206c 6175 6e63 6869 6e67 2061 2073 6573   launching a ses
+00001c00: 7369 6f6e 2c20 636f 6e6e 6563 7420 7369  sion, connect si
+00001c10: 676e 616c 7320 616e 6420 736c 6f74 732e  gnals and slots.
+00001c20: 0a20 2020 2020 2020 204d 7563 6820 6f66  .        Much of
+00001c30: 2074 6865 7365 2077 696c 6c20 6265 2066   these will be f
+00001c40: 726f 6d20 7468 6520 4755 4920 746f 2074  rom the GUI to t
+00001c50: 6865 2073 6573 7369 6f6e 2061 6e64 2076  he session and v
+00001c60: 6963 652d 7665 7273 610a 2020 2020 2020  ice-versa.      
+00001c70: 2020 4e29 0672 6100 0000 da15 756e 6c6f    N).ra.....unlo
+00001c80: 636b 5f70 6f73 7470 726f 6365 7373 696e  ck_postprocessin
+00001c90: 6772 3f00 0000 7287 0000 0072 6b00 0000  gr?...r....rk...
+00001ca0: 727b 0000 0072 5900 0000 722e 0000 0072  r{...rY...r....r
+00001cb0: 2e00 0000 722f 0000 0072 7e00 0000 0801  ....r/...r~.....
+00001cc0: 0000 7304 0000 0010 0514 017a 224d 6169  ..s........z"Mai
+00001cd0: 6e57 696e 646f 772e 636f 6e6e 6563 745f  nWindow.connect_
+00001ce0: 7365 7373 696f 6e5f 7369 676e 616c 7363  session_signalsc
+00001cf0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001d00: 0500 0000 4300 0000 f346 0000 007c 006a  ....C....F...|.j
+00001d10: 00a0 0174 026a 036a 04a1 0101 007c 006a  ...t.j.j.....|.j
+00001d20: 05a0 06a1 0001 0074 077c 006a 0883 017d  .......t.|.j...}
+00001d30: 017c 006a 00a0 0974 026a 036a 047c 0174  .|.j...t.j.j.|.t
+00001d40: 026a 036a 0aa1 0301 007c 017c 005f 0564  .j.j.....|.|._.d
+00001d50: 0053 0072 5400 0000 290b 724a 0000 00da  .S.rT...).rJ....
+00001d60: 0972 656d 6f76 6554 6162 7221 0000 0072  .removeTabr!...r
+00001d70: 2c00 0000 725d 0000 0072 6000 0000 da0b  ,...r]...r`.....
+00001d80: 6465 6c65 7465 4c61 7465 7272 1f00 0000  deleteLaterr....
+00001d90: 7261 0000 00da 0969 6e73 6572 7454 6162  ra.....insertTab
+00001da0: da04 6e61 6d65 2902 7250 0000 005a 146e  ..name).rP...Z.n
+00001db0: 6577 5f72 6563 6f72 6469 6e67 5f77 6964  ew_recording_wid
+00001dc0: 6765 7472 2e00 0000 722e 0000 0072 2f00  getr....r....r/.
+00001dd0: 0000 7284 0000 0010 0100 0073 0e00 0000  ..r........s....
+00001de0: 1002 0a01 0a01 0601 0e01 04ff 0a03 7a20  ..............z 
+00001df0: 4d61 696e 5769 6e64 6f77 2e6c 6f61 645f  MainWindow.load_
+00001e00: 7265 636f 7264 696e 675f 7769 6467 6574  recording_widget
+00001e10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001e20: 0005 0000 0043 0000 0072 8900 0000 7254  .....C...r....rT
+00001e30: 0000 0029 0b72 4a00 0000 728a 0000 0072  ...).rJ...r....r
+00001e40: 2100 0000 722d 0000 0072 5d00 0000 7273  !...r-...r]...rs
+00001e50: 0000 0072 8b00 0000 7220 0000 0072 6100  ...r....r ...ra.
+00001e60: 0000 728c 0000 0072 8d00 0000 2902 7250  ..r....r....).rP
+00001e70: 0000 005a 156e 6577 5f70 726f 6365 7373  ...Z.new_process
+00001e80: 696e 675f 7769 6467 6574 722e 0000 0072  ing_widgetr....r
+00001e90: 2e00 0000 722f 0000 0072 8700 0000 1a01  ....r/...r......
+00001ea0: 0000 f30e 0000 0010 010a 010a 0106 010e  ................
+00001eb0: 0104 ff0a 037a 264d 6169 6e57 696e 646f  .....z&MainWindo
+00001ec0: 772e 6c6f 6164 5f70 6f73 745f 7072 6f63  w.load_post_proc
+00001ed0: 6573 7369 6e67 5f77 6964 6765 7463 0100  essing_widgetc..
+00001ee0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00001ef0: 0000 4300 0000 7289 0000 0072 5400 0000  ..C...r....rT...
+00001f00: 290b 724a 0000 0072 8a00 0000 7221 0000  ).rJ...r....r!..
+00001f10: 0072 2b00 0000 725d 0000 0072 5f00 0000  .r+...r]...r_...
+00001f20: 728b 0000 0072 1e00 0000 7261 0000 0072  r....r....ra...r
+00001f30: 8c00 0000 728d 0000 0029 0272 5000 0000  ....r....).rP...
+00001f40: 5a19 6e65 775f 6361 7074 7572 655f 766f  Z.new_capture_vo
+00001f50: 6c75 6d65 5f77 6964 6765 7472 2e00 0000  lume_widgetr....
+00001f60: 722e 0000 0072 2f00 0000 7285 0000 0023  r....r/...r....#
+00001f70: 0100 0073 1200 0000 1001 0a01 0a01 0601  ...s............
+00001f80: 0601 0201 0601 04fd 0a05 7a25 4d61 696e  ..........z%Main
+00001f90: 5769 6e64 6f77 2e6c 6f61 645f 6361 7074  Window.load_capt
+00001fa0: 7572 655f 766f 6c75 6d65 5f77 6964 6765  ure_volume_widge
+00001fb0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
+00001fc0: 0000 0500 0000 4300 0000 7289 0000 0072  ......C...r....r
+00001fd0: 5400 0000 290b 724a 0000 0072 8a00 0000  T...).rJ...r....
+00001fe0: 7221 0000 0072 2a00 0000 725d 0000 0072  r!...r*...r]...r
+00001ff0: 5e00 0000 728b 0000 0072 1d00 0000 7261  ^...r....r....ra
+00002000: 0000 0072 8c00 0000 728d 0000 0029 0272  ...r....r....).r
+00002010: 5000 0000 5a11 6e65 775f 6361 6d65 7261  P...Z.new_camera
+00002020: 5f77 6964 6765 7472 2e00 0000 722e 0000  _widgetr....r...
+00002030: 0072 2f00 0000 7283 0000 002e 0100 0072  .r/...r........r
+00002040: 8e00 0000 7a1d 4d61 696e 5769 6e64 6f77  ....z.MainWindow
+00002050: 2e6c 6f61 645f 6361 6d65 7261 5f77 6964  .load_camera_wid
+00002060: 6765 7472 5100 0000 6302 0000 0000 0000  getrQ...c.......
+00002070: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+00002080: 0073 2800 0000 7400 7c01 7c00 8302 7d02  .s(...t.|.|...}.
+00002090: 7c02 6a01 a002 7c00 6a03 a101 0100 7c00  |.j...|.j.....|.
+000020a0: 6a04 a005 7c02 a101 0100 6400 5300 7254  j...|.....d.S.rT
+000020b0: 0000 0029 0672 1000 0000 723e 0000 0072  ...).r....r>...r
+000020c0: 3f00 0000 da13 6f70 656e 5f72 6563 656e  ?.....open_recen
+000020d0: 745f 7072 6f6a 6563 7472 4200 0000 7241  t_projectrB...rA
+000020e0: 0000 0029 0372 5000 0000 7251 0000 005a  ...).rP...rQ...Z
+000020f0: 1572 6563 656e 745f 7072 6f6a 6563 745f  .recent_project_
+00002100: 6163 7469 6f6e 722e 0000 0072 2e00 0000  actionr....r....
+00002110: 722f 0000 0072 4400 0000 3a01 0000 7306  r/...rD...:...s.
+00002120: 0000 000a 010e 0110 017a 204d 6169 6e57  .........z MainW
+00002130: 696e 646f 772e 6164 645f 746f 5f72 6563  indow.add_to_rec
+00002140: 656e 745f 7072 6f6a 6563 7463 0100 0000  ent_projectc....
+00002150: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00002160: 4300 0000 732e 0000 007c 00a0 00a1 007d  C...s....|.....}
+00002170: 017c 01a0 01a1 007d 0274 02a0 0364 017c  .|.....}.t...d.|
+00002180: 029b 009d 02a1 0101 007c 00a0 047c 02a1  .........|...|..
+00002190: 0101 0064 0053 0029 024e 7a21 4f70 656e  ...d.S.).Nz!Open
+000021a0: 696e 6720 7265 6365 6e74 2073 6573 7369  ing recent sessi
+000021b0: 6f6e 2073 746f 7265 6420 6174 2029 05da  on stored at )..
+000021c0: 0673 656e 6465 72da 0474 6578 7472 6300  .sender..textrc.
+000021d0: 0000 7264 0000 0072 8000 0000 2903 7250  ..rd...r....).rP
+000021e0: 0000 00da 0661 6374 696f 6e72 5100 0000  .....actionrQ...
+000021f0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+00002200: 8f00 0000 3f01 0000 7308 0000 0008 0108  ....?...s.......
+00002210: 0110 010e 017a 1e4d 6169 6e57 696e 646f  .....z.MainWindo
+00002220: 772e 6f70 656e 5f72 6563 656e 745f 7072  w.open_recent_pr
+00002230: 6f6a 6563 7463 0100 0000 0000 0000 0000  ojectc..........
+00002240: 0000 0400 0000 0600 0000 4300 0000 735c  ..........C...s\
+00002250: 0000 0074 007c 006a 0164 0119 0083 017d  ...t.|.j.d.....}
+00002260: 0174 0283 007d 027c 026a 0364 0064 0274  .t...}.|.j.d.d.t
+00002270: 047c 0183 0174 026a 056a 0664 038d 047d  .|...t.j.j.d...}
+00002280: 037c 0372 2c74 07a0 0864 047c 0366 02a1  .|.r,t...d.|.f..
+00002290: 0101 007c 00a0 097c 03a1 0101 007c 00a0  ...|...|.....|..
+000022a0: 0a7c 03a1 0101 0064 0053 0064 0053 0029  .|.....d.S.d.S.)
+000022b0: 054e da13 6c61 7374 5f70 726f 6a65 6374  .N..last_project
+000022c0: 5f70 6172 656e 747a 2d4f 7065 6e20 5072  _parentz-Open Pr
+000022d0: 6576 696f 7573 206f 7220 4372 6561 7465  evious or Create
+000022e0: 204e 6577 2050 726f 6a65 6374 2044 6972   New Project Dir
+000022f0: 6563 746f 7279 2904 da06 7061 7265 6e74  ectory)...parent
+00002300: da07 6361 7074 696f 6eda 0964 6972 6563  ..caption..direc
+00002310: 746f 7279 da07 6f70 7469 6f6e 737a 1943  tory..optionsz.C
+00002320: 7265 6174 696e 6720 6e65 7720 7072 6f6a  reating new proj
+00002330: 6563 7420 696e 203a 290b 7205 0000 0072  ect in :).r....r
+00002340: 3700 0000 7204 0000 005a 1467 6574 4578  7...r....Z.getEx
+00002350: 6973 7469 6e67 4469 7265 6374 6f72 7972  istingDirectoryr
+00002360: 3a00 0000 da06 4f70 7469 6f6e 5a0c 5368  :.....OptionZ.Sh
+00002370: 6f77 4469 7273 4f6e 6c79 7263 0000 0072  owDirsOnlyrc...r
+00002380: 6400 0000 da15 6164 645f 7072 6f6a 6563  d.....add_projec
+00002390: 745f 746f 5f72 6563 656e 7472 8000 0000  t_to_recentr....
+000023a0: 2904 7250 0000 005a 0e64 6566 6175 6c74  ).rP...Z.default
+000023b0: 5f66 6f6c 6465 725a 0664 6961 6c6f 6772  _folderZ.dialogr
+000023c0: 7700 0000 722e 0000 0072 2e00 0000 722f  w...r....r....r/
+000023d0: 0000 0072 4000 0000 4501 0000 731a 0000  ...r@...E...s...
+000023e0: 000e 0106 0104 0102 0102 0106 0106 0106  ................
+000023f0: fc04 070e 010a 010e 0104 fd7a 244d 6169  ...........z$Mai
+00002400: 6e57 696e 646f 772e 6372 6561 7465 5f6e  nWindow.create_n
+00002410: 6577 5f70 726f 6a65 6374 5f66 6f6c 6465  ew_project_folde
+00002420: 7263 0200 0000 0000 0000 0000 0000 0200  rc..............
+00002430: 0000 0400 0000 4300 0000 7354 0000 0074  ......C...sT...t
+00002440: 007c 0183 017c 006a 0164 0119 0076 0072  .|...|.j.d...v.r
+00002450: 0b64 0053 007c 006a 0164 0119 00a0 0274  .d.S.|.j.d.....t
+00002460: 007c 0183 01a1 0101 0074 0074 037c 0183  .|.......t.t.|..
+00002470: 016a 0483 017c 006a 0164 023c 007c 00a0  .j...|.j.d.<.|..
+00002480: 05a1 0001 007c 00a0 067c 01a1 0101 0064  .....|...|.....d
+00002490: 0053 0029 034e 7232 0000 0072 9300 0000  .S.).Nr2...r....
+000024a0: 2907 723a 0000 0072 3700 0000 da06 6170  ).r:...r7.....ap
+000024b0: 7065 6e64 7205 0000 0072 9400 0000 da13  pendr....r......
+000024c0: 7570 6461 7465 5f61 7070 5f73 6574 7469  update_app_setti
+000024d0: 6e67 7372 4400 0000 2902 7250 0000 005a  ngsrD...).rP...Z
+000024e0: 0b66 6f6c 6465 725f 7061 7468 722e 0000  .folder_pathr...
+000024f0: 0072 2e00 0000 722f 0000 0072 9900 0000  .r....r/...r....
+00002500: 5401 0000 730c 0000 0012 0104 0114 0214  T...s...........
+00002510: 0108 010e 017a 204d 6169 6e57 696e 646f  .....z MainWindo
+00002520: 772e 6164 645f 7072 6f6a 6563 745f 746f  w.add_project_to
+00002530: 5f72 6563 656e 7463 0100 0000 0000 0000  _recentc........
+00002540: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
+00002550: 733e 0000 0074 0074 0164 0183 028f 107d  s>...t.t.d.....}
+00002560: 0174 02a0 037c 006a 047c 01a1 0201 0057  .t...|.j.|.....W
+00002570: 0064 0004 0004 0083 0301 0064 0053 0031  .d.........d.S.1
+00002580: 0073 1877 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
+00002590: 0053 0029 024e da01 7729 05da 046f 7065  .S.).N..w)...ope
+000025a0: 6e72 1500 0000 7235 0000 00da 0464 756d  nr....r5.....dum
+000025b0: 7072 3700 0000 2902 7250 0000 00da 0166  pr7...).rP.....f
+000025c0: 722e 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
+000025d0: 9b00 0000 5d01 0000 7306 0000 000c 0110  ....]...s.......
+000025e0: 0122 ff7a 1e4d 6169 6e57 696e 646f 772e  .".z.MainWindow.
+000025f0: 7570 6461 7465 5f61 7070 5f73 6574 7469  update_app_setti
+00002600: 6e67 7329 1772 2600 0000 7227 0000 0072  ngs).r&...r'...r
+00002610: 2800 0000 7234 0000 0072 4900 0000 7258  (...r4...rI...rX
+00002620: 0000 0072 6700 0000 7255 0000 0072 7600  ...rg...rU...rv.
+00002630: 0000 723a 0000 0072 8000 0000 727b 0000  ..r:...r....r{..
+00002640: 0072 7e00 0000 7284 0000 0072 8700 0000  .r~...r....r....
+00002650: 7285 0000 0072 8300 0000 7244 0000 0072  r....r....rD...r
+00002660: 8f00 0000 7240 0000 0072 9900 0000 729b  ....r@...r....r.
+00002670: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00002680: 5f5f 722e 0000 0072 2e00 0000 7252 0000  __r....r....rR..
+00002690: 0072 2f00 0000 7230 0000 0031 0000 0073  .r/...r0...1...s
+000026a0: 2600 0000 0800 0c01 0839 0805 0811 0805  &........9......
+000026b0: 080b 0e26 0825 082c 0808 080a 0809 080b  ...&.%.,........
+000026c0: 0e0c 0805 0806 080f 1009 7230 0000 0063  ..........r0...c
+000026d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000026e0: 0300 0000 0000 0000 732c 0000 0065 005a  ........s,...e.Z
+000026f0: 0164 005a 0264 015a 0387 0066 0164 0264  .d.Z.d.Z...f.d.d
+00002700: 0384 085a 0487 0066 0164 0464 0584 085a  ...Z...f.d.d...Z
+00002710: 0587 0004 005a 0653 0029 06da 1043 656e  .....Z.S.)...Cen
+00002720: 7472 616c 5461 6257 6964 6765 7461 8901  tralTabWidgeta..
+00002730: 0000 0a20 2020 2053 7769 7463 6869 6e67  ...    Switching
+00002740: 2062 6574 7765 656e 2074 6162 732c 2070   between tabs, p
+00002750: 6172 7469 6375 6c61 726c 7920 7768 656e  articularly when
+00002760: 2073 7973 7465 6d20 7265 736f 7572 6365   system resource
+00002770: 2075 7469 6c69 7a61 7469 6f6e 2069 7320   utilization is 
+00002780: 6869 6768 2c0a 2020 2020 6973 2070 726f  high,.    is pro
+00002790: 6e65 2074 6f20 7265 7375 6c74 2069 6e20  ne to result in 
+000027a0: 7365 6766 6175 6c74 2063 7261 7368 6573  segfault crashes
+000027b0: 2e20 576f 726b 696e 6720 6879 706f 7468  . Working hypoth
+000027c0: 6573 6973 2069 7320 7468 6174 2074 6869  esis is that thi
+000027d0: 7320 6973 2064 7565 2074 6f20 6d6f 6465  s is due to mode
+000027e0: 0a20 2020 2063 6861 6e67 6573 2068 6170  .    changes hap
+000027f0: 7065 6e69 6e67 2077 6865 6e20 7468 6520  pening when the 
+00002800: 7461 6220 6973 2063 6861 6e67 6564 2061  tab is changed a
+00002810: 6e64 2074 6865 2047 5549 2074 7269 6573  nd the GUI tries
+00002820: 2074 6f20 7265 6e64 6572 2073 6f6d 6574   to render somet
+00002830: 6869 6e67 2069 7420 646f 6573 6e27 7420  hing it doesn't 
+00002840: 6861 7665 0a20 2020 200a 2020 2020 5468  have.    .    Th
+00002850: 6973 206f 7665 7272 6964 6520 736c 6970  is override slip
+00002860: 7320 7468 6520 6d6f 6465 2063 6861 6e67  s the mode chang
+00002870: 6520 6265 7477 6565 6e20 636c 6963 6b20  e between click 
+00002880: 616e 6420 6368 616e 6765 2074 6f20 7472  and change to tr
+00002890: 7920 746f 2073 7461 6269 6c69 7a65 2074  y to stabilize t
+000028a0: 6865 206d 6f64 6520 7377 6974 6368 6573  he mode switches
+000028b0: 2e0a 2020 2020 0a20 2020 2063 0100 0000  ..    .    c....
+000028c0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000028d0: 0300 0000 7312 0000 0074 0074 017c 0083  ....s....t.t.|..
+000028e0: 02a0 02a1 0001 0064 0053 0072 5400 0000  .......d.S.rT...
+000028f0: 2903 7233 0000 0072 a100 0000 7234 0000  ).r3...r....r4..
+00002900: 0072 5900 0000 7252 0000 0072 2e00 0000  .rY...rR...r....
+00002910: 722f 0000 0072 3400 0000 6c01 0000 7302  r/...r4...l...s.
+00002920: 0000 0012 017a 1943 656e 7472 616c 5461  .....z.CentralTa
+00002930: 6257 6964 6765 742e 5f5f 696e 6974 5f5f  bWidget.__init__
+00002940: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00002950: 0005 0000 0003 0000 0073 2600 0000 7400  .........s&...t.
+00002960: a001 6401 7c01 9b00 6402 9d03 a101 0100  ..d.|...d.......
+00002970: 7402 7403 7c00 8302 a004 7c01 a101 0100  t.t.|.....|.....
+00002980: 6400 5300 2903 4e7a 0454 6162 207a 0820  d.S.).Nz.Tab z. 
+00002990: 636c 6963 6b65 6429 0572 6300 0000 7264  clicked).rc...rd
+000029a0: 0000 0072 3300 0000 72a1 0000 00da 0d74  ...r3...r......t
+000029b0: 6162 4261 7243 6c69 636b 6564 7274 0000  abBarClickedrt..
+000029c0: 0072 5200 0000 722e 0000 0072 2f00 0000  .rR...r....r/...
+000029d0: 72a2 0000 006f 0100 0073 0400 0000 1202  r....o...s......
+000029e0: 1403 7a1e 4365 6e74 7261 6c54 6162 5769  ..z.CentralTabWi
+000029f0: 6467 6574 2e74 6162 4261 7243 6c69 636b  dget.tabBarClick
+00002a00: 6564 2907 7226 0000 0072 2700 0000 7228  ed).r&...r'...r(
+00002a10: 0000 00da 075f 5f64 6f63 5f5f 7234 0000  .....__doc__r4..
+00002a20: 0072 a200 0000 72a0 0000 0072 2e00 0000  .r....r....r....
+00002a30: 722e 0000 0072 5200 0000 722f 0000 0072  r....rR...r/...r
+00002a40: a100 0000 6201 0000 7308 0000 0008 0004  ....b...s.......
+00002a50: 010c 0914 0372 a100 0000 6300 0000 0000  .....r....c.....
+00002a60: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00002a70: 0000 0073 2400 0000 7400 7401 6a02 8301  ...s$...t.t.j...
+00002a80: 7d00 7403 8300 7d01 7c01 a004 a100 0100  }.t...}.|.......
+00002a90: 7c00 a005 a100 0100 6400 5300 7254 0000  |.......d.S.rT..
+00002aa0: 0029 0672 0700 0000 da03 7379 73da 0461  .).r......sys..a
+00002ab0: 7267 7672 3000 0000 da04 7368 6f77 da04  rgvr0.....show..
+00002ac0: 6578 6563 2902 da03 6170 70da 0677 696e  exec)...app..win
+00002ad0: 646f 7772 2e00 0000 722e 0000 0072 2f00  dowr....r....r/.
+00002ae0: 0000 da0b 6c61 756e 6368 5f6d 6169 6e76  ....launch_mainv
+00002af0: 0100 0073 0800 0000 0a01 0601 0801 0c02  ...s............
+00002b00: 72aa 0000 00da 085f 5f6d 6169 6e5f 5f29  r......__main__)
+00002b10: 39da 0d70 7978 7933 642e 6c6f 6767 6572  9..pyxy3d.logger
+00002b20: da06 7079 7879 3364 7263 0000 00da 0367  ..pyxy3drc.....g
+00002b30: 6574 7226 0000 00da 0f50 7951 7436 2e51  etr&.....PyQt6.Q
+00002b40: 7457 6964 6765 7473 7202 0000 0072 0300  tWidgetsr....r..
+00002b50: 0000 7204 0000 00da 0770 6174 686c 6962  ..r......pathlib
+00002b60: 7205 0000 00da 0974 6872 6561 6469 6e67  r......threading
+00002b70: 7206 0000 0072 a400 0000 7207 0000 0072  r....r....r....r
+00002b80: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+00002b90: 0000 0072 0c00 0000 720d 0000 0072 3500  ...r....r....r5.
+00002ba0: 0000 da04 656e 756d 720e 0000 005a 0b50  ....enumr....Z.P
+00002bb0: 7951 7436 2e51 7447 7569 720f 0000 0072  yQt6.QtGuir....r
+00002bc0: 1000 0000 7211 0000 0072 1200 0000 da0c  ....r....r......
+00002bd0: 5079 5174 362e 5174 436f 7265 7213 0000  PyQt6.QtCorer...
+00002be0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00002bf0: da16 7079 7879 3364 2e73 6573 7369 6f6e  ..pyxy3d.session
+00002c00: 2e73 6573 7369 6f6e 7217 0000 0072 1800  .sessionr....r..
+00002c10: 0000 5a15 7079 7879 3364 2e67 7569 2e6c  ..Z.pyxy3d.gui.l
+00002c20: 6f67 5f77 6964 6765 7472 1900 0000 da13  og_widgetr......
+00002c30: 7079 7879 3364 2e63 6f6e 6669 6775 7261  pyxy3d.configura
+00002c40: 746f 7272 1a00 0000 da1d 7079 7879 3364  torr......pyxy3d
+00002c50: 2e67 7569 2e63 616c 6962 7261 7469 6f6e  .gui.calibration
+00002c60: 5f77 6964 6765 7472 1b00 0000 da19 7079  _widgetr......py
+00002c70: 7879 3364 2e67 7569 2e63 6861 7275 636f  xy3d.gui.charuco
+00002c80: 5f77 6964 6765 7472 1c00 0000 da35 7079  _widgetr.....5py
+00002c90: 7879 3364 2e67 7569 2e63 616d 6572 615f  xy3d.gui.camera_
+00002ca0: 636f 6e66 6967 2e69 6e74 7269 6e73 6963  config.intrinsic
+00002cb0: 5f63 616c 6962 7261 7469 6f6e 5f77 6964  _calibration_wid
+00002cc0: 6765 7472 1d00 0000 5a2a 7079 7879 3364  getr....Z*pyxy3d
+00002cd0: 2e67 7569 2e63 616c 6962 7261 7465 5f63  .gui.calibrate_c
+00002ce0: 6170 7475 7265 5f76 6f6c 756d 655f 7769  apture_volume_wi
+00002cf0: 6467 6574 721e 0000 00da 1b70 7978 7933  dgetr......pyxy3
+00002d00: 642e 6775 692e 7265 636f 7264 696e 675f  d.gui.recording_
+00002d10: 7769 6467 6574 721f 0000 005a 2170 7978  widgetr....Z!pyx
+00002d20: 7933 642e 6775 692e 706f 7374 5f70 726f  y3d.gui.post_pro
+00002d30: 6365 7373 696e 675f 7769 6467 6574 7220  cessing_widgetr 
+00002d40: 0000 0072 2100 0000 7230 0000 0072 a100  ...r!...r0...r..
+00002d50: 0000 72aa 0000 0072 2e00 0000 722e 0000  ..r....r....r...
+00002d60: 0072 2e00 0000 722f 0000 00da 083c 6d6f  .r....r/.....<mo
+00002d70: 6475 6c65 3e01 0000 0073 4000 0000 0800  dule>....s@.....
+00002d80: 0801 0c02 1402 0c02 0c01 0c01 0801 2c01  ..............,.
+00002d90: 080b 0c01 1801 0c01 1401 1001 0c01 0c01  ................
+00002da0: 0c01 0c01 0c01 0c03 0c01 0c01 1003 1008  ................
+00002db0: 007f 007f 1033 0814 0808 0a01 04ff       .....3........
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 16:49:05 2023 UTC, .py size: 14618 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,747 +1,747 @@
-00000000: 6f0d 0d0a 0000 0000 814c 8764 1a39 0000  o........L.d.9..
+00000000: 6f0d 0d0a 0000 0000 8a50 8b64 9439 0000  o........P.d.9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7a01 0000 6400  .....@...sz...d.
+00000020: 0004 0000 0040 0000 0073 7e01 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6401 6c0c 5a0d 6400 6404 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
 00000080: 0100 6400 6405 6c10 6d11 5a11 0100 6400  ..d.d.l.m.Z...d.
 00000090: 6401 6c12 5a12 6400 6406 6c13 6d14 5a14  d.l.Z.d.d.l.m.Z.
 000000a0: 6d15 5a15 6d16 5a16 0100 6400 6407 6c17  m.Z.m.Z...d.d.l.
 000000b0: 6d18 5a18 6d19 5a19 6d1a 5a1a 0100 6400  m.Z.m.Z.m.Z...d.
 000000c0: 6408 6c1b 6d1c 5a1c 6d1d 5a1d 6d1e 5a1e  d.l.m.Z.m.Z.m.Z.
 000000d0: 6d1f 5a1f 6d20 5a20 6d21 5a21 6d22 5a22  m.Z.m Z m!Z!m"Z"
 000000e0: 6d23 5a23 6d24 5a24 6d25 5a25 6d26 5a26  m#Z#m$Z$m%Z%m&Z&
 000000f0: 6d27 5a27 6d28 5a28 6d29 5a29 6d2a 5a2a  m'Z'm(Z(m)Z)m*Z*
 00000100: 6d2b 5a2b 6d2c 5a2c 0100 6400 6409 6c2d  m+Z+m,Z,..d.d.l-
-00000110: 6d2e 5a2e 0100 6400 640a 6c2f 6d30 5a30  m.Z...d.d.l/m0Z0
-00000120: 0100 6400 640b 6c01 6d31 5a31 0100 6400  ..d.d.l.m1Z1..d.
-00000130: 640c 6c32 6d33 5a33 0100 6400 640d 6c34  d.l2m3Z3..d.d.l4
-00000140: 6d35 5a35 0100 4700 640e 640f 8400 640f  m5Z5..G.d.d...d.
-00000150: 6511 8303 5a36 4700 6410 6411 8400 6411  e...Z6G.d.d...d.
-00000160: 651e 8303 5a37 4700 6412 6413 8400 6413  e...Z7G.d.d...d.
-00000170: 8302 5a38 4700 6414 6415 8400 6415 6516  ..Z8G.d.d...d.e.
-00000180: 8303 5a39 6416 6417 8400 5a3a 6418 6419  ..Z9d.d...Z:d.d.
-00000190: 8400 5a3b 641a 641b 8400 5a3c 641c 641d  ..Z;d.d...Z<d.d.
-000001a0: 8400 5a3d 6401 5300 291e e900 0000 004e  ..Z=d.S.)......N
-000001b0: 2901 da04 5061 7468 2902 da06 5468 7265  )...Path)...Thre
-000001c0: 6164 da05 4576 656e 7429 01da 0551 7565  ad..Event)...Que
-000001d0: 7565 2901 da04 456e 756d 2903 da02 5174  ue)...Enum)...Qt
-000001e0: da0a 7079 7174 5369 676e 616c da07 5154  ..pyqtSignal..QT
-000001f0: 6872 6561 6429 03da 0651 496d 6167 65da  hread)...QImage.
-00000200: 0751 5069 786d 6170 da05 5149 636f 6e29  .QPixmap..QIcon)
-00000210: 11da 0c51 4170 706c 6963 6174 696f 6eda  ...QApplication.
-00000220: 0b51 5369 7a65 506f 6c69 6379 da07 5157  .QSizePolicy..QW
-00000230: 6964 6765 74da 0851 5370 696e 426f 78da  idget..QSpinBox.
-00000240: 0b51 5363 726f 6c6c 4172 6561 da09 5143  .QScrollArea..QC
-00000250: 6f6d 626f 426f 78da 0951 4368 6563 6b42  omboBox..QCheckB
-00000260: 6f78 da09 5154 6578 7445 6469 74da 0951  ox..QTextEdit..Q
-00000270: 4c69 6e65 4564 6974 da07 5144 6961 6c6f  LineEdit..QDialo
-00000280: 67da 0951 4772 6f75 7042 6f78 da0e 5144  g..QGroupBox..QD
-00000290: 6f75 626c 6553 7069 6e42 6f78 da0b 5148  oubleSpinBox..QH
-000002a0: 426f 784c 6179 6f75 74da 0651 4c61 6265  BoxLayout..QLabe
-000002b0: 6cda 0b51 5075 7368 4275 7474 6f6e da07  l..QPushButton..
-000002c0: 5153 6c69 6465 72da 0b51 5642 6f78 4c61  QSlider..QVBoxLa
-000002d0: 796f 7574 2901 da07 5365 7373 696f 6e29  yout)...Session)
-000002e0: 01da 0c53 796e 6368 726f 6e69 7a65 7229  ...Synchronizer)
-000002f0: 01da 085f 5f72 6f6f 745f 5f29 01da 0d56  ...__root__)...V
-00000300: 6964 656f 5265 636f 7264 6572 2901 da0c  ideoRecorder)...
-00000310: 436f 6e66 6967 7572 6174 6f72 6300 0000  Configuratorc...
-00000320: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00000330: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000340: 5a02 6401 5a03 6402 5a04 6403 5a05 6404  Z.d.Z.d.Z.d.Z.d.
-00000350: 5300 2905 da14 4e65 7874 5265 636f 7264  S.)...NextRecord
-00000360: 696e 6741 6374 696f 6e73 7a0f 5374 6172  ingActionsz.Star
-00000370: 7420 5265 636f 7264 696e 677a 0e53 746f  t Recordingz.Sto
-00000380: 7020 5265 636f 7264 696e 677a 112d 2d53  p Recordingz.--S
-00000390: 6176 696e 6720 4672 616d 6573 2d2d 4e29  aving Frames--N)
-000003a0: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000003b0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000003c0: 616d 655f 5fda 0e53 7461 7274 5265 636f  ame__..StartReco
-000003d0: 7264 696e 67da 0d53 746f 7052 6563 6f72  rding..StopRecor
-000003e0: 6469 6e67 da09 4177 6169 7453 6176 65a9  ding..AwaitSave.
-000003f0: 0072 2a00 0000 722a 0000 00fa 3f43 3a5c  .r*...r*....?C:\
-00000400: 5573 6572 735c 4d61 6320 5072 6962 6c65  Users\Mac Prible
-00000410: 5c72 6570 6f73 5c70 7978 7933 645c 7079  \repos\pyxy3d\py
-00000420: 7879 3364 5c67 7569 5c72 6563 6f72 6469  xy3d\gui\recordi
-00000430: 6e67 5f77 6964 6765 742e 7079 7223 0000  ng_widget.pyr#..
-00000440: 002b 0000 0073 0800 0000 0800 0401 0401  .+...s..........
-00000450: 0801 7223 0000 0063 0000 0000 0000 0000  ..r#...c........
-00000460: 0000 0000 0000 0000 0400 0000 0000 0000  ................
-00000470: 7368 0000 0065 005a 0164 005a 0264 0165  sh...e.Z.d.Z.d.e
-00000480: 0366 0287 0066 0164 0264 0384 0c5a 0464  .f...f.d.d...Z.d
-00000490: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
-000004a0: 0864 0984 005a 0764 0a64 0b84 005a 0864  .d...Z.d.d...Z.d
-000004b0: 0c64 0d84 005a 0964 0e64 0f84 005a 0a64  .d...Z.d.d...Z.d
-000004c0: 1065 0b66 0264 1164 1284 045a 0c64 1364  .e.f.d.d...Z.d.d
-000004d0: 1484 005a 0d87 0004 005a 0e53 0029 15da  ...Z.....Z.S.)..
-000004e0: 0f52 6563 6f72 6469 6e67 5769 6467 6574  .RecordingWidget
-000004f0: da07 7365 7373 696f 6e63 0200 0000 0000  ..sessionc......
-00000500: 0000 0000 0000 0200 0000 0300 0000 0300  ................
-00000510: 0000 73be 0000 0074 0074 017c 0083 02a0  ..s....t.t.|....
-00000520: 02a1 0001 007c 017c 005f 037c 006a 036a  .....|.|._.|.j.j
-00000530: 047c 005f 0474 057c 006a 0483 017c 005f  .|._.t.|.j...|._
-00000540: 0674 077c 006a 0683 017c 005f 087c 006a  .t.|.j...|._.|.j
-00000550: 08a0 09a1 0001 0074 0a7c 006a 0483 017c  .......t.|.j...|
-00000560: 005f 0b74 0c83 007c 005f 0d7c 006a 0da0  ._.t...|._.|.j..
-00000570: 0e7c 006a 036a 0fa1 0101 0074 106a 117c  .|.j.j.....t.j.|
-00000580: 005f 1274 137c 006a 126a 1483 017c 005f  ._.t.|.j.j...|._
-00000590: 1574 1664 0183 017c 005f 1774 187c 00a0  .t.d...|._.t.|..
-000005a0: 19a1 0083 017c 005f 1a74 1683 007c 005f  .....|._.t...|._
-000005b0: 1b74 1683 007c 005f 1c7c 00a0 1da1 0001  .t...|._.|......
-000005c0: 007c 00a0 1ea1 0001 007c 00a0 1fa1 0001  .|.......|......
-000005d0: 0064 0053 0029 024e 7a16 5265 636f 7264  .d.S.).Nz.Record
-000005e0: 696e 6720 4465 7374 696e 6174 696f 6e3a  ing Destination:
-000005f0: 2920 da05 7375 7065 7272 2c00 0000 da08  ) ..superr,.....
-00000600: 5f5f 696e 6974 5f5f 722d 0000 00da 0c73  __init__r-.....s
-00000610: 796e 6368 726f 6e69 7a65 72da 1455 6e70  ynchronizer..Unp
-00000620: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
-00000630: 72da 0d66 7261 6d65 5f62 7569 6c64 6572  r..frame_builder
-00000640: da14 556e 7061 6972 6564 4672 616d 6545  ..UnpairedFrameE
-00000650: 6d69 7474 6572 da0d 6672 616d 655f 656d  mitter..frame_em
-00000660: 6974 7465 72da 0573 7461 7274 7221 0000  itter..startr!..
-00000670: 00da 0e76 6964 656f 5f72 6563 6f72 6465  ...video_recorde
-00000680: 7272 1000 0000 da0f 6672 616d 655f 7261  rr......frame_ra
-00000690: 7465 5f73 7069 6eda 0873 6574 5661 6c75  te_spin..setValu
-000006a0: 65da 0d66 7073 5f72 6563 6f72 6469 6e67  e..fps_recording
-000006b0: 7223 0000 0072 2700 0000 da0b 6e65 7874  r#...r'.....next
-000006c0: 5f61 6374 696f 6e72 1b00 0000 da05 7661  _actionr......va
-000006d0: 6c75 65da 0a73 7461 7274 5f73 746f 7072  lue..start_stopr
-000006e0: 1a00 0000 da11 6465 7374 696e 6174 696f  ......destinatio
-000006f0: 6e5f 6c61 6265 6c72 1500 0000 da1c 6765  n_labelr......ge
-00000700: 745f 6e65 7874 5f72 6563 6f72 6469 6e67  t_next_recording
-00000710: 5f64 6972 6563 746f 7279 da13 7265 636f  _directory..reco
-00000720: 7264 696e 675f 6469 7265 6374 6f72 79da  rding_directory.
-00000730: 1164 726f 7070 6564 5f66 7073 5f6c 6162  .dropped_fps_lab
-00000740: 656c da17 7265 636f 7264 696e 675f 6672  el..recording_fr
-00000750: 616d 655f 6469 7370 6c61 79da 0d70 6c61  ame_display..pla
-00000760: 6365 5f77 6964 6765 7473 da0f 636f 6e6e  ce_widgets..conn
-00000770: 6563 745f 7769 6467 6574 73da 1675 7064  ect_widgets..upd
-00000780: 6174 655f 6274 6e5f 656c 6967 6962 696c  ate_btn_eligibil
-00000790: 6974 7929 02da 0473 656c 6672 2d00 0000  ity)...selfr-...
-000007a0: a901 da09 5f5f 636c 6173 735f 5f72 2a00  ....__class__r*.
-000007b0: 0000 722b 0000 0072 2f00 0000 3300 0000  ..r+...r/...3...
-000007c0: 7324 0000 000e 0206 010a 010c 060c 010a  s$..............
-000007d0: 010c 0208 0210 0108 020e 010a 010e 0108  ................
-000007e0: 0208 0208 0208 010c 017a 1852 6563 6f72  .........z.Recor
-000007f0: 6469 6e67 5769 6467 6574 2e5f 5f69 6e69  dingWidget.__ini
-00000800: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000810: 0100 0000 0300 0000 4300 0000 732a 0000  ........C...s*..
-00000820: 007c 006a 00a0 01a1 0072 0d7c 006a 02a0  .|.j.....r.|.j..
-00000830: 0364 01a1 0101 0064 0053 007c 006a 02a0  .d.....d.S.|.j..
-00000840: 0364 02a1 0101 0064 0053 0029 034e 5446  .d.....d.S.).NTF
-00000850: 2904 722d 0000 00da 1569 735f 7265 636f  ).r-.....is_reco
-00000860: 7264 696e 675f 656c 6967 6962 6c65 723c  rding_eligibler<
-00000870: 0000 00da 0a73 6574 456e 6162 6c65 64a9  .....setEnabled.
-00000880: 0172 4500 0000 722a 0000 0072 2a00 0000  .rE...r*...r*...
-00000890: 722b 0000 0072 4400 0000 5300 0000 7306  r+...rD...S...s.
-000008a0: 0000 000a 0110 0110 027a 2652 6563 6f72  .........z&Recor
-000008b0: 6469 6e67 5769 6467 6574 2e75 7064 6174  dingWidget.updat
-000008c0: 655f 6274 6e5f 656c 6967 6962 696c 6974  e_btn_eligibilit
-000008d0: 7963 0100 0000 0000 0000 0000 0000 0500  yc..............
-000008e0: 0000 0400 0000 4300 0000 736c 0000 0064  ......C...sl...d
-000008f0: 0164 0284 007c 006a 006a 01a0 02a1 0044  .d...|.j.j.....D
-00000900: 0083 017d 0164 0364 0284 007c 0144 0083  ...}.d.d...|.D..
-00000910: 017d 0264 0464 0284 007c 0244 0083 017d  .}.d.d...|.D...}
-00000920: 0364 0564 0284 007c 0344 0083 017d 0374  .d.d...|.D...}.t
-00000930: 037c 0383 0164 066b 0272 2a64 077d 047c  .|...d.k.r*d.}.|
-00000940: 0453 0064 0874 0474 057c 0383 0164 0917  .S.d.t.t.|...d..
-00000950: 0083 0117 007d 047c 0453 0029 0a4e 6301  .....}.|.S.).Nc.
-00000960: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000970: 0000 0053 0000 0073 1a00 0000 6700 7c00  ...S...s....g.|.
-00000980: 5d09 7d01 7c01 a000 a100 7202 7c01 6a01  ].}.|.....r.|.j.
-00000990: 9102 7102 5300 722a 0000 0029 02da 0669  ..q.S.r*...)...i
-000009a0: 735f 6469 72da 046e 616d 6529 02da 022e  s_dir..name)....
-000009b0: 30da 0469 7465 6d72 2a00 0000 722a 0000  0..itemr*...r*..
-000009c0: 0072 2b00 0000 da0a 3c6c 6973 7463 6f6d  .r+.....<listcom
-000009d0: 703e 5c00 0000 f302 0000 001a 007a 4052  p>\..........z@R
-000009e0: 6563 6f72 6469 6e67 5769 6467 6574 2e67  ecordingWidget.g
-000009f0: 6574 5f6e 6578 745f 7265 636f 7264 696e  et_next_recordin
-00000a00: 675f 6469 7265 6374 6f72 792e 3c6c 6f63  g_directory.<loc
-00000a10: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
-00000a20: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000a30: 0500 0000 5300 0000 731a 0000 0067 007c  ....S...s....g.|
-00000a40: 005d 097d 017c 01a0 0064 00a1 0172 027c  .].}.|...d...r.|
-00000a50: 0191 0271 0253 0029 01da 0a72 6563 6f72  ...q.S.)...recor
-00000a60: 6469 6e67 5f29 01da 0a73 7461 7274 7377  ding_)...startsw
-00000a70: 6974 68a9 0272 4d00 0000 da06 666f 6c64  ith..rM.....fold
-00000a80: 6572 722a 0000 0072 2a00 0000 722b 0000  err*...r*...r+..
-00000a90: 0072 4f00 0000 5d00 0000 7250 0000 0063  .rO...]...rP...c
-00000aa0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000ab0: 0500 0000 5300 0000 731a 0000 0067 007c  ....S...s....g.|
-00000ac0: 005d 097d 017c 01a0 0064 00a1 0164 0119  .].}.|...d...d..
-00000ad0: 0091 0271 0253 0029 02da 015f e901 0000  ...q.S.)..._....
-00000ae0: 0029 01da 0573 706c 6974 7253 0000 0072  .)...splitrS...r
-00000af0: 2a00 0000 722a 0000 0072 2b00 0000 724f  *...r*...r+...rO
-00000b00: 0000 005e 0000 0072 5000 0000 6301 0000  ...^...rP...c...
-00000b10: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000b20: 0053 0000 0073 1c00 0000 6700 7c00 5d0a  .S...s....g.|.].
-00000b30: 7d01 7c01 a000 a100 7202 7401 7c01 8301  }.|.....r.t.|...
-00000b40: 9102 7102 5300 722a 0000 0029 02da 0969  ..q.S.r*...)...i
-00000b50: 736e 756d 6572 6963 da03 696e 7429 0272  snumeric..int).r
-00000b60: 4d00 0000 5a09 7265 635f 636f 756e 7472  M...Z.rec_countr
-00000b70: 2a00 0000 722a 0000 0072 2b00 0000 724f  *...r*...r+...rO
-00000b80: 0000 005f 0000 00f3 0200 0000 1c00 7201  ..._..........r.
-00000b90: 0000 005a 0b72 6563 6f72 6469 6e67 5f31  ...Z.recording_1
-00000ba0: 7251 0000 0072 5600 0000 2906 722d 0000  rQ...rV...).r-..
-00000bb0: 00da 0470 6174 68da 0769 7465 7264 6972  ...path..iterdir
-00000bc0: da03 6c65 6eda 0373 7472 da03 6d61 7829  ..len..str..max)
-00000bd0: 0572 4500 0000 da07 666f 6c64 6572 735a  .rE.....foldersZ
-00000be0: 1172 6563 6f72 6469 6e67 5f66 6f6c 6465  .recording_folde
-00000bf0: 7273 5a10 7265 636f 7264 696e 675f 636f  rsZ.recording_co
-00000c00: 756e 7473 5a0e 6e65 7874 5f64 6972 6563  untsZ.next_direc
-00000c10: 746f 7279 722a 0000 0072 2a00 0000 722b  toryr*...r*...r+
-00000c20: 0000 0072 3e00 0000 5a00 0000 7312 0000  ...r>...Z...s...
-00000c30: 0016 020e 010e 010e 010c 0204 0104 0514  ................
-00000c40: fe04 027a 2c52 6563 6f72 6469 6e67 5769  ...z,RecordingWi
-00000c50: 6467 6574 2e67 6574 5f6e 6578 745f 7265  dget.get_next_re
-00000c60: 636f 7264 696e 675f 6469 7265 6374 6f72  cording_director
-00000c70: 7963 0100 0000 0000 0000 0000 0000 0100  yc..............
-00000c80: 0000 0400 0000 4300 0000 73da 0000 007c  ......C...s....|
-00000c90: 00a0 0074 0183 00a1 0101 0074 0264 0183  ...t.......t.d..
-00000ca0: 017c 005f 037c 006a 03a0 0074 0483 00a1  .|._.|.j...t....
-00000cb0: 0101 007c 006a 03a0 05a1 00a0 0674 0764  ...|.j.......t.d
-00000cc0: 0283 01a1 0101 007c 006a 03a0 05a1 00a0  .......|.j......
-00000cd0: 067c 006a 08a1 0101 007c 00a0 05a1 00a0  .|.j.....|......
-00000ce0: 067c 006a 03a1 0101 0074 0283 007c 005f  .|.j.....t...|._
-00000cf0: 097c 006a 09a0 0074 0483 00a1 0101 007c  .|.j...t.......|
-00000d00: 006a 09a0 05a1 00a0 067c 006a 0aa1 0101  .j.......|.j....
-00000d10: 007c 006a 09a0 05a1 00a0 067c 006a 0ba1  .|.j.......|.j..
-00000d20: 0101 007c 006a 09a0 05a1 00a0 067c 006a  ...|.j.......|.j
-00000d30: 0ca1 0101 007c 00a0 05a1 00a0 067c 006a  .....|.......|.j
-00000d40: 09a1 0101 007c 00a0 05a1 00a0 067c 006a  .....|.......|.j
-00000d50: 0da1 0101 007c 00a0 05a1 00a0 067c 006a  .....|.......|.j
-00000d60: 0ea1 0101 0064 0053 0029 034e da08 5365  .....d.S.).N..Se
-00000d70: 7474 696e 6773 7a0b 4672 616d 6520 5261  ttingsz.Frame Ra
-00000d80: 7465 3a29 0fda 0973 6574 4c61 796f 7574  te:)...setLayout
-00000d90: 721d 0000 0072 1700 0000 da0e 7365 7474  r....r......sett
-00000da0: 696e 6773 5f67 726f 7570 7219 0000 00da  ings_groupr.....
-00000db0: 066c 6179 6f75 74da 0961 6464 5769 6467  .layout..addWidg
-00000dc0: 6574 721a 0000 0072 3700 0000 5a0f 7265  etr....r7...Z.re
-00000dd0: 636f 7264 5f63 6f6e 7472 6f6c 7372 3c00  cord_controlsr<.
-00000de0: 0000 723d 0000 0072 3f00 0000 7240 0000  ..r=...r?...r@..
-00000df0: 0072 4100 0000 724a 0000 0072 2a00 0000  .rA...rJ...r*...
-00000e00: 722a 0000 0072 2b00 0000 7242 0000 006b  r*...r+...rB...k
-00000e10: 0000 0073 1c00 0000 0c01 0a01 0e01 1401  ...s............
-00000e20: 1201 1001 0802 0e01 1201 1201 1201 1002  ................
-00000e30: 1001 1402 7a1d 5265 636f 7264 696e 6757  ....z.RecordingW
-00000e40: 6964 6765 742e 706c 6163 655f 7769 6467  idget.place_widg
-00000e50: 6574 7363 0100 0000 0000 0000 0000 0000  etsc............
-00000e60: 0100 0000 0300 0000 4300 0000 7356 0000  ........C...sV..
-00000e70: 007c 006a 006a 01a0 027c 006a 03a1 0101  .|.j.j...|.j....
-00000e80: 007c 006a 046a 05a0 027c 006a 066a 07a1  .|.j.j...|.j.j..
-00000e90: 0101 007c 006a 006a 08a0 027c 006a 09a1  ...|.j.j...|.j..
-00000ea0: 0101 007c 006a 0a6a 0ba0 027c 006a 0ca1  ...|.j.j...|.j..
-00000eb0: 0101 007c 006a 066a 0da0 027c 006a 0ea1  ...|.j.j...|.j..
-00000ec0: 0101 0064 0053 00a9 014e 290f 7234 0000  ...d.S...N).r4..
-00000ed0: 00da 0e49 6d61 6765 4272 6f61 6463 6173  ...ImageBroadcas
-00000ee0: 74da 0763 6f6e 6e65 6374 da0f 496d 6167  t..connect..Imag
-00000ef0: 6555 7064 6174 6553 6c6f 7472 3700 0000  eUpdateSlotr7...
-00000f00: da0c 7661 6c75 6543 6861 6e67 6564 722d  ..valueChangedr-
-00000f10: 0000 00da 1373 6574 5f61 6374 6976 655f  .....set_active_
-00000f20: 6d6f 6465 5f66 7073 da0b 6472 6f70 7065  mode_fps..droppe
-00000f30: 645f 6670 73da 1275 7064 6174 655f 6472  d_fps..update_dr
-00000f40: 6f70 7065 645f 6670 7372 3c00 0000 da07  opped_fpsr<.....
-00000f50: 636c 6963 6b65 64da 1174 6f67 676c 655f  clicked..toggle_
-00000f60: 7374 6172 745f 7374 6f70 da19 7265 636f  start_stop..reco
-00000f70: 7264 696e 675f 636f 6d70 6c65 7465 5f73  rding_complete_s
-00000f80: 6967 6e61 6cda 156f 6e5f 7265 636f 7264  ignal..on_record
-00000f90: 696e 675f 636f 6d70 6c65 7465 724a 0000  ing_completerJ..
-00000fa0: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
-00000fb0: 7243 0000 007f 0000 0073 0a00 0000 1002  rC.......s......
-00000fc0: 1201 1001 1001 1401 7a1f 5265 636f 7264  ........z.Record
-00000fd0: 696e 6757 6964 6765 742e 636f 6e6e 6563  ingWidget.connec
-00000fe0: 745f 7769 6467 6574 7363 0100 0000 0000  t_widgetsc......
-00000ff0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00001000: 0000 73c6 0000 007c 006a 0074 016a 026b  ..s....|.j.t.j.k
-00001010: 0272 2f74 016a 037c 005f 007c 006a 04a0  .r/t.j.|._.|.j..
-00001020: 057c 006a 006a 06a1 0101 007c 006a 07a0  .|.j.j.....|.j..
-00001030: 0864 01a1 0101 0074 09a0 0a64 02a1 0101  .d.....t...d....
-00001040: 0074 0b7c 006a 0c6a 0d7c 006a 07a0 0ea1  .t.|.j.j.|.j....
-00001050: 0083 027d 017c 006a 0ca0 0f7c 01a1 0101  ...}.|.j...|....
-00001060: 0064 0053 007c 006a 0074 016a 036b 0272  .d.S.|.j.t.j.k.r
-00001070: 617c 006a 04a0 0864 01a1 0101 0074 016a  a|.j...d.....t.j
-00001080: 107c 005f 007c 006a 04a0 057c 006a 006a  .|._.|.j...|.j.j
-00001090: 06a1 0101 007c 006a 0ca0 11a1 0001 007c  .....|.j.......|
-000010a0: 006a 07a0 0864 03a1 0101 0074 09a0 0a64  .j...d.....t...d
-000010b0: 04a1 0101 007c 006a 07a0 057c 00a0 12a1  .....|.j...|....
-000010c0: 00a1 0101 0064 0053 0064 0053 0029 054e  .....d.S.d.S.).N
-000010d0: 467a 1249 6e69 7469 6174 6520 7265 636f  Fz.Initiate reco
-000010e0: 7264 696e 6754 7a2e 5374 6f70 2072 6563  rdingTz.Stop rec
-000010f0: 6f72 6469 6e67 2061 6e64 2069 6e69 7469  ording and initi
-00001100: 6174 6520 6669 6e61 6c20 7361 7665 206f  ate final save o
-00001110: 6620 6669 6c65 2913 723a 0000 0072 2300  f file).r:...r#.
-00001120: 0000 7227 0000 0072 2800 0000 723c 0000  ..r'...r(...r<..
-00001130: 00da 0773 6574 5465 7874 723b 0000 0072  ...setTextr;...r
-00001140: 3f00 0000 7249 0000 00da 066c 6f67 6765  ?...rI.....logge
-00001150: 72da 0469 6e66 6f72 0200 0000 722d 0000  r..infor....r-..
-00001160: 0072 5b00 0000 da04 7465 7874 da0f 7374  .r[.....text..st
-00001170: 6172 745f 7265 636f 7264 696e 6772 2900  art_recordingr).
-00001180: 0000 da0e 7374 6f70 5f72 6563 6f72 6469  ....stop_recordi
-00001190: 6e67 723e 0000 0029 0272 4500 0000 5a0e  ngr>...).rE...Z.
-000011a0: 7265 636f 7264 696e 675f 7061 7468 722a  recording_pathr*
-000011b0: 0000 0072 2a00 0000 722b 0000 0072 6f00  ...r*...r+...ro.
-000011c0: 0000 8700 0000 7320 0000 000c 0108 0110  ......s ........
-000011d0: 010c 010a 0214 0110 010c 020c 0108 0210  ................
-000011e0: 020a 010c 020a 0114 0104 f67a 2152 6563  ...........z!Rec
-000011f0: 6f72 6469 6e67 5769 6467 6574 2e74 6f67  ordingWidget.tog
-00001200: 676c 655f 7374 6172 745f 7374 6f70 6301  gle_start_stopc.
-00001210: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001220: 0000 0043 0000 0073 3c00 0000 7400 a001  ...C...s<...t...
-00001230: 6401 a101 0100 7402 6a03 7c00 5f04 7c00  d.....t.j.|._.|.
-00001240: 6a05 a006 7c00 6a04 6a07 a101 0100 7c00  j...|.j.j.....|.
-00001250: 6a05 a008 6402 a101 0100 7400 a001 6403  j...d.....t...d.
-00001260: a101 0100 6400 5300 2904 4e7a 4452 6563  ....d.S.).NzDRec
-00001270: 6f72 6469 6e67 2063 6f6d 706c 6574 6520  ording complete 
-00001280: 7369 676e 616c 2072 6563 6569 7665 642e  signal received.
-00001290: 2e2e 7570 6461 7469 6e67 206e 6578 7420  ..updating next 
-000012a0: 6163 7469 6f6e 2061 6e64 2062 7574 746f  action and butto
-000012b0: 6e54 7a24 456e 6162 6c69 6e67 2073 7461  nTz$Enabling sta
-000012c0: 7274 2f73 746f 7020 7265 636f 7264 696e  rt/stop recordin
-000012d0: 6720 6275 7474 6f6e 2909 7273 0000 0072  g button).rs...r
-000012e0: 7400 0000 7223 0000 0072 2700 0000 723a  t...r#...r'...r:
-000012f0: 0000 0072 3c00 0000 7272 0000 0072 3b00  ...r<...rr...r;.
-00001300: 0000 7249 0000 0072 4a00 0000 722a 0000  ..rI...rJ...r*..
-00001310: 0072 2a00 0000 722b 0000 0072 7100 0000  .r*...r+...rq...
-00001320: 9d00 0000 730a 0000 000a 0108 0110 010c  ....s...........
-00001330: 010e 017a 2552 6563 6f72 6469 6e67 5769  ...z%RecordingWi
-00001340: 6467 6574 2e6f 6e5f 7265 636f 7264 696e  dget.on_recordin
-00001350: 675f 636f 6d70 6c65 7465 726c 0000 0063  g_completerl...c
-00001360: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-00001370: 0600 0000 4300 0000 733c 0000 0064 017d  ....C...s<...d.}
-00001380: 027c 01a0 00a1 0044 005d 0f5c 027d 037d  .|.....D.].\.}.}
-00001390: 047c 027c 039b 0064 027c 0464 039b 0464  .|.|...d.|.d...d
-000013a0: 049d 0437 007d 0271 067c 006a 01a0 027c  ...7.}.q.|.j...|
-000013b0: 02a1 0101 0064 0553 0029 067a 3855 6e72  .....d.S.).z8Unr
-000013c0: 6176 656c 2064 726f 7070 6564 2066 7073  avel dropped fps
-000013d0: 2064 6963 7469 6f6e 6172 7920 746f 2061   dictionary to a
-000013e0: 206d 6f72 6520 7265 6164 6162 6c65 2073   more readable s
-000013f0: 7472 696e 677a 2352 6174 6520 6f66 2046  tringz#Rate of F
-00001400: 7261 6d65 2044 726f 7070 696e 6720 6279  rame Dropping by
-00001410: 2050 6f72 743a 2020 2020 7a02 3a20 7a03   Port:    z.: z.
-00001420: 2e30 257a 0820 2020 2020 2020 204e 2903  .0%z.        N).
-00001430: da05 6974 656d 7372 4000 0000 7272 0000  ..itemsr@...rr..
-00001440: 0029 0572 4500 0000 726c 0000 0072 7500  .).rE...rl...ru.
-00001450: 0000 da04 706f 7274 5a09 6472 6f70 5f72  ....portZ.drop_r
-00001460: 6174 6572 2a00 0000 722a 0000 0072 2b00  ater*...r*...r+.
-00001470: 0000 726d 0000 00a4 0000 0073 0800 0000  ..rm.......s....
-00001480: 0402 1001 1801 1002 7a22 5265 636f 7264  ........z"Record
-00001490: 696e 6757 6964 6765 742e 7570 6461 7465  ingWidget.update
-000014a0: 5f64 726f 7070 6564 5f66 7073 6302 0000  _dropped_fpsc...
-000014b0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000014c0: 0043 0000 0073 2c00 0000 7c00 6a00 a001  .C...s,...|.j...
-000014d0: 7c00 6a00 a002 a100 a101 0100 7403 a004  |.j.........t...
-000014e0: 7c01 a101 7d02 7c00 6a00 a005 7c02 a101  |...}.|.j...|...
-000014f0: 0100 6400 5300 7266 0000 0029 0672 4100  ..d.S.rf...).rA.
-00001500: 0000 da06 7265 7369 7a65 da08 7369 7a65  ....resize..size
-00001510: 4869 6e74 720b 0000 00da 0966 726f 6d49  Hintr......fromI
-00001520: 6d61 6765 da09 7365 7450 6978 6d61 7029  mage..setPixmap)
-00001530: 0372 4500 0000 da07 715f 696d 6167 65da  .rE.....q_image.
-00001540: 0771 7069 786d 6170 722a 0000 0072 2a00  .qpixmapr*...r*.
-00001550: 0000 722b 0000 0072 6900 0000 ad00 0000  ..r+...ri.......
-00001560: 7306 0000 0012 010a 0110 017a 1f52 6563  s..........z.Rec
-00001570: 6f72 6469 6e67 5769 6467 6574 2e49 6d61  ordingWidget.Ima
-00001580: 6765 5570 6461 7465 536c 6f74 290f 7224  geUpdateSlot).r$
-00001590: 0000 0072 2500 0000 7226 0000 0072 1e00  ...r%...r&...r..
-000015a0: 0000 722f 0000 0072 4400 0000 723e 0000  ..r/...rD...r>..
-000015b0: 0072 4200 0000 7243 0000 0072 6f00 0000  .rB...rC...ro...
-000015c0: 7271 0000 00da 0464 6963 7472 6d00 0000  rq.....dictrm...
-000015d0: 7269 0000 00da 0d5f 5f63 6c61 7373 6365  ri.....__classce
-000015e0: 6c6c 5f5f 722a 0000 0072 2a00 0000 7246  ll__r*...r*...rF
-000015f0: 0000 0072 2b00 0000 722c 0000 0031 0000  ...r+...r,...1..
-00001600: 0073 1400 0000 0800 1202 0820 0807 0811  .s......... ....
-00001610: 0814 0808 0816 0e07 1009 722c 0000 0063  ..........r,...c
-00001620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001630: 0400 0000 4000 0000 7344 0000 0065 005a  ....@...sD...e.Z
-00001640: 0164 005a 0264 1064 0265 0366 0264 0364  .d.Z.d.d.e.f.d.d
-00001650: 0484 055a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
-00001660: 0884 005a 0664 0964 0a84 005a 0764 0b64  ...Z.d.d...Z.d.d
-00001670: 0c84 005a 0864 0d64 0e84 005a 0964 0f53  ...Z.d.d...Z.d.S
-00001680: 0029 1172 3100 0000 e9fa 0000 0072 3000  .).r1........r0.
-00001690: 0000 6303 0000 0000 0000 0000 0000 0006  ..c.............
-000016a0: 0000 0005 0000 0043 0000 0073 8c00 0000  .......C...s....
-000016b0: 7c01 7c00 5f00 7c02 7c00 5f01 6700 7c00  |.|._.|.|._.g.|.
-000016c0: 5f02 7c00 6a00 6a03 a004 a100 4400 5d0a  _.|.j.j.....D.].
-000016d0: 5c02 7d03 7d04 7c00 6a02 a005 7c03 a101  \.}.}.|.j...|...
-000016e0: 0100 710f 7c00 6a02 a006 a100 0100 7407  ..q.|.j.......t.
-000016f0: 7c00 6a02 8301 7d05 7408 7409 a00a 7c05  |.j...}.t.t...|.
-00001700: 6401 1300 a101 8301 7c00 5f0b 7408 7409  d.......|._.t.t.
-00001710: a00a 7c05 7c00 6a0b 1b00 a101 8301 7c00  ..|.|.j.......|.
-00001720: 5f0c 740d 8300 7c00 5f0e 7c00 6a00 a00f  _.t...|._.|.j...
-00001730: 7c00 6a0e a101 0100 6400 5300 2902 4e67  |.j.....d.S.).Ng
-00001740: 0000 0000 0000 e03f 2910 7230 0000 00da  .......?).r0....
-00001750: 1373 696e 676c 655f 6672 616d 655f 6865  .single_frame_he
-00001760: 6967 6874 da05 706f 7274 73da 0773 7472  ight..ports..str
-00001770: 6561 6d73 7278 0000 00da 0661 7070 656e  eamsrx.....appen
-00001780: 64da 0473 6f72 7472 5d00 0000 7259 0000  d..sortr]...rY..
-00001790: 00da 046d 6174 68da 0463 6569 6cda 0d66  ...math..ceil..f
-000017a0: 7261 6d65 5f63 6f6c 756d 6e73 da0a 6672  rame_columns..fr
-000017b0: 616d 655f 726f 7773 7205 0000 00da 166e  ame_rowsr......n
-000017c0: 6577 5f73 796e 635f 7061 636b 6574 5f6e  ew_sync_packet_n
-000017d0: 6f74 6963 65da 1373 7562 7363 7269 6265  otice..subscribe
-000017e0: 5f74 6f5f 6e6f 7469 6365 2906 7245 0000  _to_notice).rE..
-000017f0: 0072 3000 0000 7283 0000 0072 7900 0000  .r0...r....ry...
-00001800: da06 7374 7265 616d 5a0c 6361 6d65 7261  ..streamZ.camera
-00001810: 5f63 6f75 6e74 722a 0000 0072 2a00 0000  _countr*...r*...
-00001820: 722b 0000 0072 2f00 0000 b300 0000 7316  r+...r/.......s.
-00001830: 0000 0006 0106 0106 0314 010e 030a 010a  ................
-00001840: 0414 0116 0108 0212 017a 1d55 6e70 6169  .........z.Unpai
-00001850: 7265 6446 7261 6d65 4275 696c 6465 722e  redFrameBuilder.
-00001860: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00001870: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00001880: 0073 1c00 0000 7400 a001 6401 a101 0100  .s....t...d.....
-00001890: 7c00 6a02 a003 7c00 6a04 a101 0100 6400  |.j...|.j.....d.
-000018a0: 5300 2902 4e7a 2c55 6e73 7562 7363 7269  S.).Nz,Unsubscri
-000018b0: 6265 2066 7261 6d65 2062 7569 6c64 6572  be frame builder
-000018c0: 2066 726f 6d20 7379 6e63 6872 6f6e 697a   from synchroniz
-000018d0: 6572 2e29 0572 7300 0000 7274 0000 0072  er.).rs...rt...r
-000018e0: 3000 0000 da15 756e 7375 6273 6372 6962  0.....unsubscrib
-000018f0: 655f 746f 5f6e 6f74 6963 6572 8c00 0000  e_to_noticer....
-00001900: 724a 0000 0072 2a00 0000 722a 0000 0072  rJ...r*...r*...r
-00001910: 2b00 0000 da1d 756e 7375 6273 6372 6962  +.....unsubscrib
-00001920: 655f 6672 6f6d 5f73 796e 6368 726f 6e69  e_from_synchroni
-00001930: 7a65 72c8 0000 0073 0400 0000 0a01 1201  zer....s........
-00001940: 7a32 556e 7061 6972 6564 4672 616d 6542  z2UnpairedFrameB
-00001950: 7569 6c64 6572 2e75 6e73 7562 7363 7269  uilder.unsubscri
-00001960: 6265 5f66 726f 6d5f 7379 6e63 6872 6f6e  be_from_synchron
-00001970: 697a 6572 6302 0000 0000 0000 0000 0000  izerc...........
-00001980: 0004 0000 0004 0000 0043 0000 0073 3c00  .........C...s<.
-00001990: 0000 7c00 6a00 7d02 7c01 6401 7500 7219  ..|.j.}.|.d.u.r.
-000019a0: 7401 a002 6402 a101 0100 7403 6a04 7c02  t...d.....t.j.|.
-000019b0: 7c02 6403 6603 7403 6a05 6404 8d02 7d03  |.d.f.t.j.d...}.
-000019c0: 7c03 5300 7c01 6a06 7d03 7c03 5300 2905  |.S.|.j.}.|.S.).
-000019d0: 7a7b 5379 6e63 6872 6f6e 697a 6174 696f  z{Synchronizatio
-000019e0: 6e20 6973 7375 6573 2063 616e 206c 6561  n issues can lea
-000019f0: 6420 746f 2073 6f6d 6520 6672 616d 6573  d to some frames
-00001a00: 2062 6569 6e67 204e 6f6e 6520 616d 6f6e   being None amon
-00001a10: 670a 2020 2020 2020 2020 7468 6520 7379  g.        the sy
-00001a20: 6e63 6865 6420 6672 616d 6573 2c20 736f  nched frames, so
-00001a30: 2070 6c75 6720 7468 6174 2077 6974 6820   plug that with 
-00001a40: 6120 626c 616e 6b20 6672 616d 654e 7a19  a blank frameNz.
-00001a50: 706c 7567 6769 6e67 2062 6c61 6e6b 2066  plugging blank f
-00001a60: 7261 6d65 2064 6174 61e9 0300 0000 2901  rame data.....).
-00001a70: da05 6474 7970 6529 0772 8300 0000 7273  ..dtype).r....rs
-00001a80: 0000 00da 0564 6562 7567 da02 6e70 da05  .....debug..np..
-00001a90: 7a65 726f 73da 0575 696e 7438 da05 6672  zeros..uint8..fr
-00001aa0: 616d 6529 0472 4500 0000 da0c 6672 616d  ame).rE.....fram
-00001ab0: 655f 7061 636b 6574 da04 6564 6765 7297  e_packet..edger.
-00001ac0: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
-00001ad0: 0000 da12 6765 745f 6672 616d 655f 6f72  ....get_frame_or
-00001ae0: 5f62 6c61 6e6b cd00 0000 730e 0000 0006  _blank....s.....
-00001af0: 0408 020a 0116 0104 0406 fe04 027a 2755  .............z'U
-00001b00: 6e70 6169 7265 6446 7261 6d65 4275 696c  npairedFrameBuil
-00001b10: 6465 722e 6765 745f 6672 616d 655f 6f72  der.get_frame_or
-00001b20: 5f62 6c61 6e6b 6302 0000 0000 0000 0000  _blankc.........
-00001b30: 0000 0008 0000 0009 0000 0043 0000 0073  ...........C...s
-00001b40: 8600 0000 7400 a001 6401 a101 0100 7c01  ....t...d.....|.
-00001b50: 6a02 6402 1900 7d02 7c01 6a02 6403 1900  j.d...}.|.j.d...
-00001b60: 7d03 7403 7c02 7c03 8302 7d04 7404 7c04  }.t.|.|...}.t.|.
-00001b70: 7c02 1800 6404 1b00 8301 7d05 7404 7c04  |...d.....}.t.|.
-00001b80: 7c03 1800 6404 1b00 8301 7d06 6700 6405  |...d.....}.g.d.
-00001b90: a201 7d07 7400 a001 6406 a101 0100 7405  ..}.t...d.....t.
-00001ba0: 6a06 7c01 7c05 7c05 7c06 7c06 7405 6a07  j.|.|.|.|.|.t.j.
-00001bb0: 7c07 6407 8d07 7d01 7408 7c01 7c00 6a09  |.d...}.t.|.|.j.
-00001bc0: 6408 8d02 7d01 7c01 5300 2909 7a65 546f  d...}.|.S.).zeTo
-00001bd0: 206d 616b 6520 7375 7265 2074 6861 7420   make sure that 
-00001be0: 6672 616d 6573 2061 6c69 676e 2077 656c  frames align wel
-00001bf0: 6c2c 2073 6361 6c65 2074 6865 6d20 616c  l, scale them al
-00001c00: 6c20 746f 2074 6875 6d62 6e61 696c 730a  l to thumbnails.
-00001c10: 2020 2020 2020 2020 7371 7561 7265 7320          squares 
-00001c20: 7769 7468 2062 6c61 636b 2062 6f72 6465  with black borde
-00001c30: 7273 2e7a 0f72 6573 697a 696e 6720 7371  rs.z.resizing sq
-00001c40: 7561 7265 7201 0000 0072 5600 0000 e902  uarer....rV.....
-00001c50: 0000 0029 0372 0100 0000 7201 0000 0072  ...).r....r....r
-00001c60: 0100 0000 7a13 6162 6f75 7420 746f 2070  ....z.about to p
-00001c70: 6164 2062 6f72 6465 7229 0172 3b00 0000  ad border).r;...
-00001c80: 2901 da0a 6e65 775f 6865 6967 6874 290a  )...new_height).
-00001c90: 7273 0000 0072 9300 0000 da05 7368 6170  rs...r......shap
-00001ca0: 6572 5f00 0000 7259 0000 00da 0363 7632  er_...rY.....cv2
-00001cb0: da0e 636f 7079 4d61 6b65 426f 7264 6572  ..copyMakeBorder
-00001cc0: da0f 424f 5244 4552 5f43 4f4e 5354 414e  ..BORDER_CONSTAN
-00001cd0: 5472 7a00 0000 7283 0000 0029 0872 4500  Trz...r....).rE.
-00001ce0: 0000 7297 0000 00da 0668 6569 6768 74da  ..r......height.
-00001cf0: 0577 6964 7468 da0b 7061 6464 6564 5f73  .width..padded_s
-00001d00: 697a 65da 0a68 6569 6768 745f 7061 64da  ize..height_pad.
-00001d10: 0977 6964 7468 5f70 6164 da09 7061 645f  .width_pad..pad_
-00001d20: 636f 6c6f 7272 2a00 0000 722a 0000 0072  colorr*...r*...r
-00001d30: 2b00 0000 da10 7265 7369 7a65 5f74 6f5f  +.....resize_to_
-00001d40: 7371 7561 7265 dc00 0000 7326 0000 000a  square....s&....
-00001d50: 030a 040a 010a 0210 0210 0108 010a 0204  ................
-00001d60: 0102 0102 0102 0102 0102 0104 0102 0106  ................
-00001d70: f90e 0a04 017a 2555 6e70 6169 7265 6446  .....z%UnpairedF
-00001d80: 7261 6d65 4275 696c 6465 722e 7265 7369  rameBuilder.resi
-00001d90: 7a65 5f74 6f5f 7371 7561 7265 6303 0000  ze_to_squarec...
-00001da0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00001db0: 0043 0000 0073 6c00 0000 7c00 6a00 6a01  .C...sl...|.j.j.
-00001dc0: 7c02 1900 6a02 6a03 7d03 7c03 6401 6b02  |...j.j.}.|.d.k.
-00001dd0: 720f 0900 7c01 5300 7c03 6402 7600 721c  r...|.S.|.d.v.r.
-00001de0: 7404 a005 7c01 7404 6a06 a102 7d01 7c01  t...|.t.j...}.|.
-00001df0: 5300 7c03 6403 7600 7229 7404 a005 7c01  S.|.d.v.r)t...|.
-00001e00: 7404 6a07 a102 7d01 7c01 5300 7c03 6404  t.j...}.|.S.|.d.
-00001e10: 7600 7234 7404 a005 7c01 7404 6a08 a102  v.r4t...|.t.j...
-00001e20: 7d01 7c01 5300 2905 4e72 0100 0000 2902  }.|.S.).Nr....).
-00001e30: 7256 0000 00e9 fdff ffff 2902 729b 0000  rV........).r...
-00001e40: 00e9 feff ffff 2902 e9ff ffff ff72 9100  ......)......r..
-00001e50: 0000 2909 7230 0000 0072 8500 0000 da06  ..).r0...r......
-00001e60: 6361 6d65 7261 da0e 726f 7461 7469 6f6e  camera..rotation
-00001e70: 5f63 6f75 6e74 729e 0000 00da 0672 6f74  _countr......rot
-00001e80: 6174 65da 1352 4f54 4154 455f 3930 5f43  ate..ROTATE_90_C
-00001e90: 4c4f 434b 5749 5345 da0a 524f 5441 5445  LOCKWISE..ROTATE
-00001ea0: 5f31 3830 da1a 524f 5441 5445 5f39 305f  _180..ROTATE_90_
-00001eb0: 434f 554e 5445 5243 4c4f 434b 5749 5345  COUNTERCLOCKWISE
-00001ec0: 2904 7245 0000 0072 9700 0000 7279 0000  ).rE...r....ry..
-00001ed0: 0072 ac00 0000 722a 0000 0072 2a00 0000  .r....r*...r*...
-00001ee0: 722b 0000 00da 0e61 7070 6c79 5f72 6f74  r+.....apply_rot
-00001ef0: 6174 696f 6efb 0000 0073 1a00 0000 1002  ation....s......
-00001f00: 0801 0201 0408 08f9 0e01 0406 08fb 0e01  ................
-00001f10: 0404 08fd 0e01 0402 7a23 556e 7061 6972  ........z#Unpair
-00001f20: 6564 4672 616d 6542 7569 6c64 6572 2e61  edFrameBuilder.a
-00001f30: 7070 6c79 5f72 6f74 6174 696f 6e63 0100  pply_rotationc..
-00001f40: 0000 0000 0000 0000 0000 1100 0000 0a00  ................
-00001f50: 0000 4300 0000 7378 0100 007c 006a 00a0  ..C...sx...|.j..
-00001f60: 01a1 0001 007c 006a 026a 037c 005f 0369  .....|.j.j.|._.i
-00001f70: 007d 017c 006a 0444 005d 3f7d 027c 006a  .}.|.j.D.]?}.|.j
-00001f80: 036a 057c 0219 007d 037c 00a0 067c 03a1  .j.|...}.|...|..
-00001f90: 017d 047c 00a0 077c 04a1 017d 057c 00a0  .}.|...|...}.|..
-00001fa0: 087c 057c 02a1 027d 0674 09a0 0a7c 0664  .|.|...}.t...|.d
-00001fb0: 01a1 027d 0774 096a 0b7c 0774 0c7c 0283  ...}.t.j.|.t.|..
-00001fc0: 0174 0d7c 076a 0e64 0119 0064 021b 0083  .t.|.j.d...d....
-00001fd0: 0174 0d7c 006a 0f64 031b 0083 0166 0274  .t.|.j.d.....f.t
-00001fe0: 096a 1064 0164 0464 0264 058d 077d 087c  .j.d.d.d.d...}.|
-00001ff0: 087c 017c 023c 0071 0f67 007d 0964 067d  .|.|.<.q.g.}.d.}
-00002000: 0a64 077d 0b64 077d 0c74 117c 006a 0483  .d.}.d.}.t.|.j..
-00002010: 017d 0d7c 01a0 12a1 0044 005d 445c 027d  .}.|.....D.]D\.}
-00002020: 027d 0e7c 0a64 0675 0072 6b7c 0e7d 0a6e  .}.|.d.u.rk|.}.n
-00002030: 0774 13a0 147c 0a7c 0e67 02a1 017d 0a7c  .t...|.|.g...}.|
-00002040: 0b64 0137 007d 0b7c 0d64 0138 007d 0d7c  .d.7.}.|.d.8.}.|
-00002050: 0d64 076b 0272 967c 0b7c 006a 156b 0072  .d.k.r.|.|.j.k.r
-00002060: 9674 13a0 147c 0a7c 00a0 0664 06a1 0167  .t...|.|...d...g
-00002070: 02a1 017d 0a7c 0b64 0137 007d 0b7c 0b7c  ...}.|.d.7.}.|.|
-00002080: 006a 156b 0073 837c 0b7c 006a 156b 0272  .j.k.s.|.|.j.k.r
-00002090: a47c 09a0 167c 0aa1 0101 0064 067d 0a64  .|...|.....d.}.d
-000020a0: 077d 0b71 6064 067d 0f7c 0944 005d 107d  .}.q`d.}.|.D.].}
-000020b0: 107c 0f64 0675 0072 b27c 107d 0f71 a974  .|.d.u.r.|.}.q.t
-000020c0: 13a0 177c 0f7c 1067 02a1 017d 0f71 a97c  ...|.|.g...}.q.|
-000020d0: 0f53 0029 087a fb0a 2020 2020 2020 2020  .S.).z..        
-000020e0: 5468 6973 2067 6c75 6573 2074 6f67 6574  This glues toget
-000020f0: 6865 7220 7468 6520 696e 6469 7669 6475  her the individu
-00002100: 616c 2066 7261 6d65 7320 696e 2074 6865  al frames in the
-00002110: 2073 796e 6320 7061 636b 6574 2069 6e74   sync packet int
-00002120: 6f20 6f6e 6520 6c61 7267 6520 626c 6f63  o one large bloc
-00002130: 6b0a 0a20 2020 2020 2020 2043 7572 7265  k..        Curre
-00002140: 6e74 6c79 206a 7573 7420 7374 6163 6b69  ntly just stacki
-00002150: 6e67 2061 6c6c 2066 7261 6d65 7320 7665  ng all frames ve
-00002160: 7274 6963 616c 6c79 2c20 6275 7420 7468  rtically, but th
-00002170: 6973 2073 686f 756c 6420 6265 2065 7870  is should be exp
-00002180: 616e 6465 6420 6f6e 2074 6865 200a 2020  anded on the .  
-00002190: 2020 2020 2020 7468 6520 6675 7475 7265        the future
-000021a0: 2074 6f20 616c 6c6f 7720 7772 6170 7069   to allow wrappi
-000021b0: 6e67 2074 6f20 6120 6d6f 7265 2073 7175  ng to a more squ
-000021c0: 6172 6520 7368 6170 650a 2020 2020 2020  are shape.      
-000021d0: 2020 7256 0000 0072 9b00 0000 e904 0000    rV...r........
-000021e0: 0029 0372 0100 0000 7201 0000 00e9 ff00  .).r....r.......
-000021f0: 0000 2904 da08 666f 6e74 4661 6365 da09  ..)...fontFace..
-00002200: 666f 6e74 5363 616c 65da 0563 6f6c 6f72  fontScale..color
-00002210: da09 7468 6963 6b6e 6573 734e 7201 0000  ..thicknessNr...
-00002220: 0029 1872 8c00 0000 da03 6765 7472 3000  .).r......getr0.
-00002230: 0000 da13 6375 7272 656e 745f 7379 6e63  ....current_sync
-00002240: 5f70 6163 6b65 7472 8400 0000 da0d 6672  _packetr......fr
-00002250: 616d 655f 7061 636b 6574 7372 9a00 0000  ame_packetsr....
-00002260: 72a7 0000 0072 b100 0000 729e 0000 00da  r....r....r.....
-00002270: 0466 6c69 70da 0770 7574 5465 7874 725e  .flip..putTextr^
-00002280: 0000 0072 5900 0000 729d 0000 0072 8300  ...rY...r....r..
-00002290: 0000 da14 464f 4e54 5f48 4552 5348 4559  ....FONT_HERSHEY
-000022a0: 5f53 494d 504c 4558 725d 0000 0072 7800  _SIMPLEXr]...rx.
-000022b0: 0000 7294 0000 00da 0668 7374 6163 6b72  ..r......hstackr
-000022c0: 8a00 0000 7286 0000 00da 0676 7374 6163  ....r......vstac
-000022d0: 6b29 1172 4500 0000 5a10 7468 756d 626e  k).rE...Z.thumbn
-000022e0: 6169 6c5f 6672 616d 6573 7279 0000 0072  ail_framesry...r
-000022f0: 9800 0000 5a09 7261 775f 6672 616d 655a  ....Z.raw_frameZ
-00002300: 0c73 7175 6172 655f 6672 616d 655a 0d72  .square_frameZ.r
-00002310: 6f74 6174 6564 5f66 7261 6d65 5a0d 666c  otated_frameZ.fl
-00002320: 6970 7065 645f 6672 616d 655a 0a74 6578  ipped_frameZ.tex
-00002330: 745f 6672 616d 6572 8b00 0000 5a0b 6375  t_framer....Z.cu
-00002340: 7272 656e 745f 726f 775a 1263 7572 7265  rrent_rowZ.curre
-00002350: 6e74 5f72 6f77 5f6c 656e 6774 685a 0c66  nt_row_lengthZ.f
-00002360: 7261 6d65 735f 6164 6465 645a 1066 7261  rames_addedZ.fra
-00002370: 6d65 735f 7265 6d61 696e 696e 6772 9700  mes_remainingr..
-00002380: 0000 5a0a 6d65 6761 5f66 7261 6d65 da03  ..Z.mega_frame..
-00002390: 726f 7772 2a00 0000 722a 0000 0072 2b00  rowr*...r*...r+.
-000023a0: 0000 da13 6765 745f 7265 636f 7264 696e  ....get_recordin
-000023b0: 675f 6672 616d 650a 0100 0073 5a00 0000  g_frame....sZ...
-000023c0: 0a08 0a01 0402 0a01 0c01 0a01 0a01 0c01  ................
-000023d0: 0c01 0603 0601 1e01 0401 0201 0201 0201  ................
-000023e0: 06fa 0a09 0402 0401 0401 0401 0a01 1001  ................
-000023f0: 0802 0601 0e02 0801 0801 0802 0a02 1401  ................
-00002400: 0801 0afe 0a04 0a01 0401 0401 0280 0402  ................
-00002410: 0801 0801 0601 1002 0403 7a28 556e 7061  ..........z(Unpa
-00002420: 6972 6564 4672 616d 6542 7569 6c64 6572  iredFrameBuilder
-00002430: 2e67 6574 5f72 6563 6f72 6469 6e67 5f66  .get_recording_f
-00002440: 7261 6d65 4e29 0172 8200 0000 290a 7224  rameN).r....).r$
-00002450: 0000 0072 2500 0000 7226 0000 0072 1f00  ...r%...r&...r..
-00002460: 0000 722f 0000 0072 9000 0000 729a 0000  ..r/...r....r...
-00002470: 0072 a700 0000 72b1 0000 0072 c100 0000  .r....r....r....
-00002480: 722a 0000 0072 2a00 0000 722a 0000 0072  r*...r*...r*...r
-00002490: 2b00 0000 7231 0000 00b2 0000 0073 0e00  +...r1.......s..
-000024a0: 0000 0800 1001 0815 0805 080f 081f 0c0f  ................
-000024b0: 7231 0000 0063 0000 0000 0000 0000 0000  r1...c..........
-000024c0: 0000 0000 0000 0400 0000 0000 0000 733a  ..............s:
-000024d0: 0000 0065 005a 0164 005a 0265 0365 0483  ...e.Z.d.Z.e.e..
-000024e0: 015a 0565 0365 0683 015a 0764 0165 0866  .Z.e.e...Z.d.e.f
-000024f0: 0287 0066 0164 0264 0384 0c5a 0964 0464  ...f.d.d...Z.d.d
-00002500: 0584 005a 0a87 0004 005a 0b53 0029 0672  ...Z.....Z.S.).r
-00002510: 3300 0000 da16 756e 7061 6972 6564 5f66  3.....unpaired_f
-00002520: 7261 6d65 5f62 7569 6c64 6572 6302 0000  rame_builderc...
-00002530: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00002540: 0003 0000 0073 2a00 0000 7400 7401 7c00  .....s*...t.t.|.
-00002550: 8302 a002 a100 0100 7c01 7c00 5f03 7404  ........|.|._.t.
-00002560: a005 6401 a101 0100 7406 8300 7c00 5f07  ..d.....t...|._.
-00002570: 6400 5300 2902 4e7a 2149 6e69 7469 6174  d.S.).Nz!Initiat
-00002580: 6564 2072 6563 6f72 6469 6e67 2066 7261  ed recording fra
-00002590: 6d65 2065 6d69 7474 6572 2908 722e 0000  me emitter).r...
-000025a0: 0072 3300 0000 722f 0000 00da 1772 6563  .r3...r/.....rec
-000025b0: 6f72 6469 6e67 5f66 7261 6d65 5f62 7569  ording_frame_bui
-000025c0: 6c64 6572 7273 0000 0072 7400 0000 7204  lderrs...rt...r.
-000025d0: 0000 00da 0f6b 6565 705f 636f 6c6c 6563  .....keep_collec
-000025e0: 7469 6e67 2902 7245 0000 0072 c200 0000  ting).rE...r....
-000025f0: 7246 0000 0072 2a00 0000 722b 0000 0072  rF...r*...r+...r
-00002600: 2f00 0000 5001 0000 7308 0000 000e 0206  /...P...s.......
-00002610: 010a 010c 017a 1d55 6e70 6169 7265 6446  .....z.UnpairedF
-00002620: 7261 6d65 456d 6974 7465 722e 5f5f 696e  rameEmitter.__in
-00002630: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00002640: 0003 0000 0003 0000 0043 0000 0073 6400  .........C...sd.
-00002650: 0000 7c00 6a00 a001 a100 0100 7c00 6a00  ..|.j.......|.j.
-00002660: a002 a100 722b 7c00 6a03 a004 a100 7d01  ....r+|.j.....}.
-00002670: 7c01 6400 7501 7226 7405 7c01 8301 7d02  |.d.u.r&t.|...}.
-00002680: 7c00 6a06 a007 7c02 a101 0100 7c00 6a08  |.j...|.....|.j.
-00002690: a007 7c00 6a03 6a09 6a08 a101 0100 7c00  ..|.j.j.j.....|.
-000026a0: 6a00 a002 a100 730a 740a a00b 6401 a101  j.....s.t...d...
-000026b0: 0100 6400 5300 2902 4e7a 2753 7465 7265  ..d.S.).Nz'Stere
-000026c0: 6f66 7261 6d65 2065 6d69 7474 6572 2072  oframe emitter r
-000026d0: 756e 2074 6872 6561 6420 656e 6465 642e  un thread ended.
-000026e0: 2e2e 290c 72c4 0000 00da 0373 6574 da06  ..).r......set..
-000026f0: 6973 5f73 6574 72c3 0000 0072 c100 0000  is_setr....r....
-00002700: da0d 6376 325f 746f 5f71 6c61 6265 6c72  ..cv2_to_qlabelr
-00002710: 6700 0000 da04 656d 6974 726c 0000 0072  g.....emitrl...r
-00002720: 3000 0000 7273 0000 0072 7400 0000 2903  0...rs...rt...).
-00002730: 7245 0000 005a 0f72 6563 6f72 6469 6e67  rE...Z.recording
-00002740: 5f66 7261 6d65 da05 696d 6167 6572 2a00  _frame..imager*.
-00002750: 0000 722a 0000 0072 2b00 0000 da03 7275  ..r*...r+.....ru
-00002760: 6e57 0100 0073 1200 0000 0a02 0a02 0a04  nW...s..........
-00002770: 0802 0801 0c01 1201 0af7 0e0b 7a18 556e  ............z.Un
-00002780: 7061 6972 6564 4672 616d 6545 6d69 7474  pairedFrameEmitt
-00002790: 6572 2e72 756e 290c 7224 0000 0072 2500  er.run).r$...r%.
-000027a0: 0000 7226 0000 0072 0800 0000 720a 0000  ..r&...r....r...
-000027b0: 0072 6700 0000 7280 0000 0072 6c00 0000  .rg...r....rl...
-000027c0: 7231 0000 0072 2f00 0000 72ca 0000 0072  r1...r/...r....r
-000027d0: 8100 0000 722a 0000 0072 2a00 0000 7246  ....r*...r*...rF
-000027e0: 0000 0072 2b00 0000 7233 0000 004c 0100  ...r+...r3...L..
-000027f0: 0073 0a00 0000 0800 0801 0801 1202 1007  .s..............
-00002800: 7233 0000 0063 0200 0000 0000 0000 0000  r3...c..........
-00002810: 0000 0300 0000 0300 0000 0300 0000 731a  ..............s.
-00002820: 0000 0087 0066 0164 0164 0284 087c 00a0  .....f.d.d...|..
-00002830: 00a1 0044 0083 017d 027c 0253 0029 034e  ...D...}.|.S.).N
-00002840: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00002850: 0004 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
-00002860: 7c00 5d0a 5c02 7d01 7d02 7c02 8800 6b00  |.].\.}.}.|...k.
-00002870: 7202 7c01 9102 7102 5300 722a 0000 0072  r.|...q.S.r*...r
-00002880: 2a00 0000 2903 724d 0000 00da 036b 6579  *...).rM.....key
-00002890: 723b 0000 00a9 01da 0d6d 696e 5f74 6872  r;.......min_thr
-000028a0: 6573 686f 6c64 722a 0000 0072 2b00 0000  esholdr*...r+...
-000028b0: 724f 0000 006b 0100 0072 5a00 0000 7a23  rO...k...rZ...z#
-000028c0: 6765 745f 656d 7074 795f 7061 6972 732e  get_empty_pairs.
-000028d0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000028e0: 6d70 3e29 0172 7800 0000 2903 da0c 626f  mp>).rx...)...bo
-000028f0: 6172 645f 636f 756e 7473 72cd 0000 00da  ard_countsr.....
-00002900: 0b65 6d70 7479 5f70 6169 7273 722a 0000  .empty_pairsr*..
-00002910: 0072 cc00 0000 722b 0000 00da 0f67 6574  .r....r+.....get
-00002920: 5f65 6d70 7479 5f70 6169 7273 6a01 0000  _empty_pairsj...
-00002930: 7304 0000 0016 0104 0172 d000 0000 6302  s........r....c.
-00002940: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-00002950: 0000 0043 0000 0073 4400 0000 7c00 6a00  ...C...sD...|.j.
-00002960: 6400 6401 8502 1900 5c02 7d02 7d03 7c01  d.d.....\.}.}.|.
-00002970: 7401 7c02 8301 1b00 7d04 7402 7c03 7c04  t.|.....}.t.|.|.
-00002980: 1400 8301 7c01 6602 7d05 7403 6a04 7c00  ....|.f.}.t.j.|.
-00002990: 7c05 7403 6a05 6402 8d03 7d06 7c06 5300  |.t.j.d...}.|.S.
-000029a0: 2903 4e72 9b00 0000 2901 da0d 696e 7465  ).Nr....)...inte
-000029b0: 7270 6f6c 6174 696f 6e29 0672 9d00 0000  rpolation).r....
-000029c0: da05 666c 6f61 7472 5900 0000 729e 0000  ..floatrY...r...
-000029d0: 0072 7a00 0000 da0a 494e 5445 525f 4152  .rz.....INTER_AR
-000029e0: 4541 2907 72c9 0000 0072 9c00 0000 da0e  EA).r....r......
-000029f0: 6375 7272 656e 745f 6865 6967 6874 da0d  current_height..
-00002a00: 6375 7272 656e 745f 7769 6474 68da 0572  current_width..r
-00002a10: 6174 696f da03 6469 6dda 0772 6573 697a  atio..dim..resiz
-00002a20: 6564 722a 0000 0072 2a00 0000 722b 0000  edr*...r*...r+..
-00002a30: 0072 7a00 0000 6e01 0000 730a 0000 0012  .rz...n...s.....
-00002a40: 010c 0110 0112 0104 0172 7a00 0000 6301  .........rz...c.
-00002a50: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00002a60: 0000 0043 0000 0073 3200 0000 7400 a001  ...C...s2...t...
-00002a70: 7c00 7400 6a02 a102 7d01 7403 7c01 6a04  |.t.j...}.t.|.j.
-00002a80: 7c01 6a05 6401 1900 7c01 6a05 6402 1900  |.j.d...|.j.d...
-00002a90: 7403 6a06 6a07 8304 7d02 7c02 5300 2903  t.j.j...}.|.S.).
-00002aa0: 4e72 5600 0000 7201 0000 0029 0872 9e00  NrV...r....).r..
-00002ab0: 0000 da08 6376 7443 6f6c 6f72 da0d 434f  ....cvtColor..CO
-00002ac0: 4c4f 525f 4247 5232 5247 4272 0a00 0000  LOR_BGR2RGBr....
-00002ad0: da04 6461 7461 729d 0000 00da 0646 6f72  ..datar......For
-00002ae0: 6d61 74da 0d46 6f72 6d61 745f 5247 4238  mat..Format_RGB8
-00002af0: 3838 2903 7297 0000 0072 c900 0000 da08  88).r....r......
-00002b00: 7174 5f66 7261 6d65 722a 0000 0072 2a00  qt_framer*...r*.
-00002b10: 0000 722b 0000 0072 c700 0000 7701 0000  ..r+...r....w...
-00002b20: 7310 0000 000e 0102 0204 0108 0108 0106  s...............
-00002b30: 0104 fc04 0672 c700 0000 6301 0000 0000  .....r....c.....
-00002b40: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-00002b50: 0000 0073 4c00 0000 7400 7c00 8301 7d01  ...sL...t.|...}.
-00002b60: 7401 7c01 8301 7d02 7c02 a002 a100 0100  t.|...}.|.......
-00002b70: 7c02 a003 a100 0100 7404 7405 6a06 8301  |.......t.t.j...
-00002b80: 7d03 7407 7c02 8301 7d04 7c04 a008 a100  }.t.|...}.|.....
-00002b90: 0100 7405 a009 7c03 a00a a100 a101 0100  ..t...|.........
-00002ba0: 6400 5300 7266 0000 0029 0b72 2200 0000  d.S.rf...).r"...
-00002bb0: 721e 0000 00da 116c 6f61 645f 7374 7265  r......load_stre
-00002bc0: 616d 5f74 6f6f 6c73 da13 5f61 646a 7573  am_tools.._adjus
-00002bd0: 745f 7265 736f 6c75 7469 6f6e 7372 0d00  t_resolutionsr..
-00002be0: 0000 da03 7379 73da 0461 7267 7672 2c00  ....sys..argvr,.
-00002bf0: 0000 da04 7368 6f77 da04 6578 6974 da04  ....show..exit..
-00002c00: 6578 6563 2905 da0c 7365 7373 696f 6e5f  exec)...session_
-00002c10: 7061 7468 da06 636f 6e66 6967 722d 0000  path..configr-..
-00002c20: 00da 0341 7070 5a10 7265 636f 7264 696e  ...AppZ.recordin
-00002c30: 675f 6469 616c 6f67 722a 0000 0072 2a00  g_dialogr*...r*.
-00002c40: 0000 722b 0000 00da 176c 6175 6e63 685f  ..r+.....launch_
-00002c50: 7265 636f 7264 696e 675f 7769 6467 6574  recording_widget
-00002c60: 8301 0000 7310 0000 0008 0108 0108 0108  ....s...........
-00002c70: 010a 0208 0108 0112 0272 e900 0000 293e  .........r....)>
-00002c80: da0d 7079 7879 3364 2e6c 6f67 6765 72da  ..pyxy3d.logger.
-00002c90: 0670 7978 7933 6472 7300 0000 72b8 0000  .pyxy3drs...r...
-00002ca0: 0072 2400 0000 72e1 0000 0072 8800 0000  .r$...r....r....
-00002cb0: da07 7061 7468 6c69 6272 0200 0000 da09  ..pathlibr......
-00002cc0: 7468 7265 6164 696e 6772 0300 0000 7204  threadingr....r.
-00002cd0: 0000 00da 056e 756d 7079 7294 0000 00da  .....numpyr.....
-00002ce0: 0571 7565 7565 7205 0000 00da 0465 6e75  .queuer......enu
-00002cf0: 6d72 0600 0000 729e 0000 00da 0c50 7951  mr....r......PyQ
-00002d00: 7436 2e51 7443 6f72 6572 0700 0000 7208  t6.QtCorer....r.
-00002d10: 0000 0072 0900 0000 5a0b 5079 5174 362e  ...r....Z.PyQt6.
-00002d20: 5174 4775 6972 0a00 0000 720b 0000 0072  QtGuir....r....r
-00002d30: 0c00 0000 da0f 5079 5174 362e 5174 5769  ......PyQt6.QtWi
-00002d40: 6467 6574 7372 0d00 0000 720e 0000 0072  dgetsr....r....r
-00002d50: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
-00002d60: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
-00002d70: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00002d80: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00002d90: 721c 0000 0072 1d00 0000 da16 7079 7879  r....r......pyxy
-00002da0: 3364 2e73 6573 7369 6f6e 2e73 6573 7369  3d.session.sessi
-00002db0: 6f6e 721e 0000 00da 1b70 7978 7933 642e  onr......pyxy3d.
-00002dc0: 6361 6d65 7261 732e 7379 6e63 6872 6f6e  cameras.synchron
-00002dd0: 697a 6572 721f 0000 0072 2000 0000 da1f  izerr....r .....
-00002de0: 7079 7879 3364 2e72 6563 6f72 6469 6e67  pyxy3d.recording
-00002df0: 2e76 6964 656f 5f72 6563 6f72 6465 7272  .video_recorderr
-00002e00: 2100 0000 da13 7079 7879 3364 2e63 6f6e  !.....pyxy3d.con
-00002e10: 6669 6775 7261 746f 7272 2200 0000 7223  figuratorr"...r#
-00002e20: 0000 0072 2c00 0000 7231 0000 0072 3300  ...r,...r1...r3.
-00002e30: 0000 72d0 0000 0072 7a00 0000 72c7 0000  ..r....rz...r...
-00002e40: 0072 e900 0000 722a 0000 0072 2a00 0000  .r....r*...r*...
-00002e50: 722a 0000 0072 2b00 0000 da08 3c6d 6f64  r*...r+.....<mod
-00002e60: 756c 653e 0100 0000 7338 0000 0008 020c  ule>....s8......
-00002e70: 0108 0208 010c 0110 0108 010c 010c 0108  ................
-00002e80: 0214 0114 014c 010c 140c 010c 010c 010c  .....L..........
-00002e90: 0110 0210 0600 7f0e 0200 7f10 1b08 1e08  ................
-00002ea0: 0408 090c 0c                             .....
+00000110: 6d2e 5a2e 6d2f 5a2f 0100 6400 640a 6c30  m.Z.m/Z/..d.d.l0
+00000120: 6d31 5a31 0100 6400 640b 6c01 6d32 5a32  m1Z1..d.d.l.m2Z2
+00000130: 0100 6400 640c 6c33 6d34 5a34 0100 6400  ..d.d.l3m4Z4..d.
+00000140: 640d 6c35 6d36 5a36 0100 4700 640e 640f  d.l5m6Z6..G.d.d.
+00000150: 8400 640f 6511 8303 5a37 4700 6410 6411  ..d.e...Z7G.d.d.
+00000160: 8400 6411 651e 8303 5a38 4700 6412 6413  ..d.e...Z8G.d.d.
+00000170: 8400 6413 8302 5a39 4700 6414 6415 8400  ..d...Z9G.d.d...
+00000180: 6415 6516 8303 5a3a 6416 6417 8400 5a3b  d.e...Z:d.d...Z;
+00000190: 6418 6419 8400 5a3c 641a 641b 8400 5a3d  d.d...Z<d.d...Z=
+000001a0: 641c 641d 8400 5a3e 6401 5300 291e e900  d.d...Z>d.S.)...
+000001b0: 0000 004e 2901 da04 5061 7468 2902 da06  ...N)...Path)...
+000001c0: 5468 7265 6164 da05 4576 656e 7429 01da  Thread..Event)..
+000001d0: 0551 7565 7565 2901 da04 456e 756d 2903  .Queue)...Enum).
+000001e0: da02 5174 da0a 7079 7174 5369 676e 616c  ..Qt..pyqtSignal
+000001f0: da07 5154 6872 6561 6429 03da 0651 496d  ..QThread)...QIm
+00000200: 6167 65da 0751 5069 786d 6170 da05 5149  age..QPixmap..QI
+00000210: 636f 6e29 11da 0c51 4170 706c 6963 6174  con)...QApplicat
+00000220: 696f 6eda 0b51 5369 7a65 506f 6c69 6379  ion..QSizePolicy
+00000230: da07 5157 6964 6765 74da 0851 5370 696e  ..QWidget..QSpin
+00000240: 426f 78da 0b51 5363 726f 6c6c 4172 6561  Box..QScrollArea
+00000250: da09 5143 6f6d 626f 426f 78da 0951 4368  ..QComboBox..QCh
+00000260: 6563 6b42 6f78 da09 5154 6578 7445 6469  eckBox..QTextEdi
+00000270: 74da 0951 4c69 6e65 4564 6974 da07 5144  t..QLineEdit..QD
+00000280: 6961 6c6f 67da 0951 4772 6f75 7042 6f78  ialog..QGroupBox
+00000290: da0e 5144 6f75 626c 6553 7069 6e42 6f78  ..QDoubleSpinBox
+000002a0: da0b 5148 426f 784c 6179 6f75 74da 0651  ..QHBoxLayout..Q
+000002b0: 4c61 6265 6cda 0b51 5075 7368 4275 7474  Label..QPushButt
+000002c0: 6f6e da07 5153 6c69 6465 72da 0b51 5642  on..QSlider..QVB
+000002d0: 6f78 4c61 796f 7574 2902 da07 5365 7373  oxLayout)...Sess
+000002e0: 696f 6eda 0b53 6573 7369 6f6e 4d6f 6465  ion..SessionMode
+000002f0: 2901 da0c 5379 6e63 6872 6f6e 697a 6572  )...Synchronizer
+00000300: 2901 da08 5f5f 726f 6f74 5f5f 2901 da0d  )...__root__)...
+00000310: 5669 6465 6f52 6563 6f72 6465 7229 01da  VideoRecorder)..
+00000320: 0c43 6f6e 6669 6775 7261 746f 7263 0000  .Configuratorc..
+00000330: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000340: 0000 4000 0000 7318 0000 0065 005a 0164  ..@...s....e.Z.d
+00000350: 005a 0264 015a 0364 025a 0464 035a 0564  .Z.d.Z.d.Z.d.Z.d
+00000360: 0453 0029 05da 144e 6578 7452 6563 6f72  .S.)...NextRecor
+00000370: 6469 6e67 4163 7469 6f6e 737a 0f53 7461  dingActionsz.Sta
+00000380: 7274 2052 6563 6f72 6469 6e67 7a0e 5374  rt Recordingz.St
+00000390: 6f70 2052 6563 6f72 6469 6e67 7a11 2d2d  op Recordingz.--
+000003a0: 5361 7669 6e67 2046 7261 6d65 732d 2d4e  Saving Frames--N
+000003b0: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000003c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000003d0: 6e61 6d65 5f5f da0e 5374 6172 7452 6563  name__..StartRec
+000003e0: 6f72 6469 6e67 da0d 5374 6f70 5265 636f  ording..StopReco
+000003f0: 7264 696e 67da 0941 7761 6974 5361 7665  rding..AwaitSave
+00000400: a900 722b 0000 0072 2b00 0000 fa3f 433a  ..r+...r+....?C:
+00000410: 5c55 7365 7273 5c4d 6163 2050 7269 626c  \Users\Mac Pribl
+00000420: 655c 7265 706f 735c 7079 7879 3364 5c70  e\repos\pyxy3d\p
+00000430: 7978 7933 645c 6775 695c 7265 636f 7264  yxy3d\gui\record
+00000440: 696e 675f 7769 6467 6574 2e70 7972 2400  ing_widget.pyr$.
+00000450: 0000 2b00 0000 7308 0000 0008 0004 0104  ..+...s.........
+00000460: 0108 0172 2400 0000 6300 0000 0000 0000  ...r$...c.......
+00000470: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00000480: 0073 6800 0000 6500 5a01 6400 5a02 6401  .sh...e.Z.d.Z.d.
+00000490: 6503 6602 8700 6601 6402 6403 840c 5a04  e.f...f.d.d...Z.
+000004a0: 6404 6405 8400 5a05 6406 6407 8400 5a06  d.d...Z.d.d...Z.
+000004b0: 6408 6409 8400 5a07 640a 640b 8400 5a08  d.d...Z.d.d...Z.
+000004c0: 640c 640d 8400 5a09 640e 640f 8400 5a0a  d.d...Z.d.d...Z.
+000004d0: 6410 650b 6602 6411 6412 8404 5a0c 6413  d.e.f.d.d...Z.d.
+000004e0: 6414 8400 5a0d 8700 0400 5a0e 5300 2915  d...Z.....Z.S.).
+000004f0: da0f 5265 636f 7264 696e 6757 6964 6765  ..RecordingWidge
+00000500: 74da 0773 6573 7369 6f6e 6302 0000 0000  t..sessionc.....
+00000510: 0000 0000 0000 0002 0000 0003 0000 0003  ................
+00000520: 0000 0073 be00 0000 7400 7401 7c00 8302  ...s....t.t.|...
+00000530: a002 a100 0100 7c01 7c00 5f03 7c00 6a03  ......|.|._.|.j.
+00000540: 6a04 7c00 5f04 7405 7c00 6a04 8301 7c00  j.|._.t.|.j...|.
+00000550: 5f06 7407 7c00 6a06 8301 7c00 5f08 7c00  _.t.|.j...|._.|.
+00000560: 6a08 a009 a100 0100 740a 7c00 6a04 8301  j.......t.|.j...
+00000570: 7c00 5f0b 740c 8300 7c00 5f0d 7c00 6a0d  |._.t...|._.|.j.
+00000580: a00e 7c00 6a03 6a0f a101 0100 7410 6a11  ..|.j.j.....t.j.
+00000590: 7c00 5f12 7413 7c00 6a12 6a14 8301 7c00  |._.t.|.j.j...|.
+000005a0: 5f15 7416 6401 8301 7c00 5f17 7418 7c00  _.t.d...|._.t.|.
+000005b0: a019 a100 8301 7c00 5f1a 7416 8300 7c00  ......|._.t...|.
+000005c0: 5f1b 7416 8300 7c00 5f1c 7c00 a01d a100  _.t...|._.|.....
+000005d0: 0100 7c00 a01e a100 0100 7c00 a01f a100  ..|.......|.....
+000005e0: 0100 6400 5300 2902 4e7a 1652 6563 6f72  ..d.S.).Nz.Recor
+000005f0: 6469 6e67 2044 6573 7469 6e61 7469 6f6e  ding Destination
+00000600: 3a29 20da 0573 7570 6572 722d 0000 00da  :) ..superr-....
+00000610: 085f 5f69 6e69 745f 5f72 2e00 0000 da0c  .__init__r......
+00000620: 7379 6e63 6872 6f6e 697a 6572 da14 556e  synchronizer..Un
+00000630: 7061 6972 6564 4672 616d 6542 7569 6c64  pairedFrameBuild
+00000640: 6572 da16 756e 7061 6972 6564 5f66 7261  er..unpaired_fra
+00000650: 6d65 5f62 7569 6c64 6572 da14 556e 7061  me_builder..Unpa
+00000660: 6972 6564 4672 616d 6545 6d69 7474 6572  iredFrameEmitter
+00000670: da16 756e 7061 6972 6564 5f66 7261 6d65  ..unpaired_frame
+00000680: 5f65 6d69 7474 6572 da05 7374 6172 7472  _emitter..startr
+00000690: 2200 0000 da0e 7669 6465 6f5f 7265 636f  ".....video_reco
+000006a0: 7264 6572 7210 0000 00da 0f66 7261 6d65  rderr......frame
+000006b0: 5f72 6174 655f 7370 696e da08 7365 7456  _rate_spin..setV
+000006c0: 616c 7565 da0d 6670 735f 7265 636f 7264  alue..fps_record
+000006d0: 696e 6772 2400 0000 7228 0000 00da 0b6e  ingr$...r(.....n
+000006e0: 6578 745f 6163 7469 6f6e 721b 0000 00da  ext_actionr.....
+000006f0: 0576 616c 7565 da0a 7374 6172 745f 7374  .value..start_st
+00000700: 6f70 721a 0000 00da 1164 6573 7469 6e61  opr......destina
+00000710: 7469 6f6e 5f6c 6162 656c 7215 0000 00da  tion_labelr.....
+00000720: 1c67 6574 5f6e 6578 745f 7265 636f 7264  .get_next_record
+00000730: 696e 675f 6469 7265 6374 6f72 79da 1372  ing_directory..r
+00000740: 6563 6f72 6469 6e67 5f64 6972 6563 746f  ecording_directo
+00000750: 7279 da11 6472 6f70 7065 645f 6670 735f  ry..dropped_fps_
+00000760: 6c61 6265 6cda 1772 6563 6f72 6469 6e67  label..recording
+00000770: 5f66 7261 6d65 5f64 6973 706c 6179 da0d  _frame_display..
+00000780: 706c 6163 655f 7769 6467 6574 73da 0f63  place_widgets..c
+00000790: 6f6e 6e65 6374 5f77 6964 6765 7473 da16  onnect_widgets..
+000007a0: 7570 6461 7465 5f62 746e 5f65 6c69 6769  update_btn_eligi
+000007b0: 6269 6c69 7479 2902 da04 7365 6c66 722e  bility)...selfr.
+000007c0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+000007d0: 722b 0000 0072 2c00 0000 7230 0000 0033  r+...r,...r0...3
+000007e0: 0000 0073 2400 0000 0e02 0601 0a01 0c06  ...s$...........
+000007f0: 0c01 0a01 0c02 0802 1001 0802 0e01 0a01  ................
+00000800: 0e01 0802 0802 0802 0801 0c01 7a18 5265  ............z.Re
+00000810: 636f 7264 696e 6757 6964 6765 742e 5f5f  cordingWidget.__
+00000820: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000830: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000840: 2a00 0000 7c00 6a00 a001 a100 720d 7c00  *...|.j.....r.|.
+00000850: 6a02 a003 6401 a101 0100 6400 5300 7c00  j...d.....d.S.|.
+00000860: 6a02 a003 6402 a101 0100 6400 5300 2903  j...d.....d.S.).
+00000870: 4e54 4629 0472 2e00 0000 da15 6973 5f72  NTF).r......is_r
+00000880: 6563 6f72 6469 6e67 5f65 6c69 6769 626c  ecording_eligibl
+00000890: 6572 3d00 0000 da0a 7365 7445 6e61 626c  er=.....setEnabl
+000008a0: 6564 a901 7246 0000 0072 2b00 0000 722b  ed..rF...r+...r+
+000008b0: 0000 0072 2c00 0000 7245 0000 0053 0000  ...r,...rE...S..
+000008c0: 0073 0600 0000 0a01 1001 1002 7a26 5265  .s..........z&Re
+000008d0: 636f 7264 696e 6757 6964 6765 742e 7570  cordingWidget.up
+000008e0: 6461 7465 5f62 746e 5f65 6c69 6769 6269  date_btn_eligibi
+000008f0: 6c69 7479 6301 0000 0000 0000 0000 0000  lityc...........
+00000900: 0005 0000 0004 0000 0043 0000 0073 6c00  .........C...sl.
+00000910: 0000 6401 6402 8400 7c00 6a00 6a01 a002  ..d.d...|.j.j...
+00000920: a100 4400 8301 7d01 6403 6402 8400 7c01  ..D...}.d.d...|.
+00000930: 4400 8301 7d02 6404 6402 8400 7c02 4400  D...}.d.d...|.D.
+00000940: 8301 7d03 6405 6402 8400 7c03 4400 8301  ..}.d.d...|.D...
+00000950: 7d03 7403 7c03 8301 6406 6b02 722a 6407  }.t.|...d.k.r*d.
+00000960: 7d04 7c04 5300 6408 7404 7405 7c03 8301  }.|.S.d.t.t.|...
+00000970: 6409 1700 8301 1700 7d04 7c04 5300 290a  d.......}.|.S.).
+00000980: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00000990: 0000 0400 0000 5300 0000 731a 0000 0067  ......S...s....g
+000009a0: 007c 005d 097d 017c 01a0 00a1 0072 027c  .|.].}.|.....r.|
+000009b0: 016a 0191 0271 0253 0072 2b00 0000 2902  .j...q.S.r+...).
+000009c0: da06 6973 5f64 6972 da04 6e61 6d65 2902  ..is_dir..name).
+000009d0: da02 2e30 da04 6974 656d 722b 0000 0072  ...0..itemr+...r
+000009e0: 2b00 0000 722c 0000 00da 0a3c 6c69 7374  +...r,.....<list
+000009f0: 636f 6d70 3e5c 0000 00f3 0200 0000 1a00  comp>\..........
+00000a00: 7a40 5265 636f 7264 696e 6757 6964 6765  z@RecordingWidge
+00000a10: 742e 6765 745f 6e65 7874 5f72 6563 6f72  t.get_next_recor
+00000a20: 6469 6e67 5f64 6972 6563 746f 7279 2e3c  ding_directory.<
+00000a30: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000a40: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
+00000a50: 0000 0005 0000 0053 0000 0073 1a00 0000  .......S...s....
+00000a60: 6700 7c00 5d09 7d01 7c01 a000 6400 a101  g.|.].}.|...d...
+00000a70: 7202 7c01 9102 7102 5300 2901 da0a 7265  r.|...q.S.)...re
+00000a80: 636f 7264 696e 675f 2901 da0a 7374 6172  cording_)...star
+00000a90: 7473 7769 7468 a902 724e 0000 00da 0666  tswith..rN.....f
+00000aa0: 6f6c 6465 7272 2b00 0000 722b 0000 0072  olderr+...r+...r
+00000ab0: 2c00 0000 7250 0000 005d 0000 0072 5100  ,...rP...]...rQ.
+00000ac0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00000ad0: 0000 0005 0000 0053 0000 0073 1a00 0000  .......S...s....
+00000ae0: 6700 7c00 5d09 7d01 7c01 a000 6400 a101  g.|.].}.|...d...
+00000af0: 6401 1900 9102 7102 5300 2902 da01 5fe9  d.....q.S.)..._.
+00000b00: 0100 0000 2901 da05 7370 6c69 7472 5400  ....)...splitrT.
+00000b10: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
+00000b20: 0072 5000 0000 5e00 0000 7251 0000 0063  .rP...^...rQ...c
+00000b30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000b40: 0400 0000 5300 0000 731c 0000 0067 007c  ....S...s....g.|
+00000b50: 005d 0a7d 017c 01a0 00a1 0072 0274 017c  .].}.|.....r.t.|
+00000b60: 0183 0191 0271 0253 0072 2b00 0000 2902  .....q.S.r+...).
+00000b70: da09 6973 6e75 6d65 7269 63da 0369 6e74  ..isnumeric..int
+00000b80: 2902 724e 0000 005a 0972 6563 5f63 6f75  ).rN...Z.rec_cou
+00000b90: 6e74 722b 0000 0072 2b00 0000 722c 0000  ntr+...r+...r,..
+00000ba0: 0072 5000 0000 5f00 0000 f302 0000 001c  .rP..._.........
+00000bb0: 0072 0100 0000 5a0b 7265 636f 7264 696e  .r....Z.recordin
+00000bc0: 675f 3172 5200 0000 7257 0000 0029 0672  g_1rR...rW...).r
+00000bd0: 2e00 0000 da04 7061 7468 da07 6974 6572  ......path..iter
+00000be0: 6469 72da 036c 656e da03 7374 72da 036d  dir..len..str..m
+00000bf0: 6178 2905 7246 0000 005a 0766 6f6c 6465  ax).rF...Z.folde
+00000c00: 7273 5a11 7265 636f 7264 696e 675f 666f  rsZ.recording_fo
+00000c10: 6c64 6572 735a 1072 6563 6f72 6469 6e67  ldersZ.recording
+00000c20: 5f63 6f75 6e74 735a 0e6e 6578 745f 6469  _countsZ.next_di
+00000c30: 7265 6374 6f72 7972 2b00 0000 722b 0000  rectoryr+...r+..
+00000c40: 0072 2c00 0000 723f 0000 005a 0000 0073  .r,...r?...Z...s
+00000c50: 1200 0000 1602 0e01 0e01 0e01 0c02 0401  ................
+00000c60: 0405 14fe 0402 7a2c 5265 636f 7264 696e  ......z,Recordin
+00000c70: 6757 6964 6765 742e 6765 745f 6e65 7874  gWidget.get_next
+00000c80: 5f72 6563 6f72 6469 6e67 5f64 6972 6563  _recording_direc
+00000c90: 746f 7279 6301 0000 0000 0000 0000 0000  toryc...........
+00000ca0: 0001 0000 0004 0000 0043 0000 0073 da00  .........C...s..
+00000cb0: 0000 7c00 a000 7401 8300 a101 0100 7402  ..|...t.......t.
+00000cc0: 6401 8301 7c00 5f03 7c00 6a03 a000 7404  d...|._.|.j...t.
+00000cd0: 8300 a101 0100 7c00 6a03 a005 a100 a006  ......|.j.......
+00000ce0: 7407 6402 8301 a101 0100 7c00 6a03 a005  t.d.......|.j...
+00000cf0: a100 a006 7c00 6a08 a101 0100 7c00 a005  ....|.j.....|...
+00000d00: a100 a006 7c00 6a03 a101 0100 7402 8300  ....|.j.....t...
+00000d10: 7c00 5f09 7c00 6a09 a000 7404 8300 a101  |._.|.j...t.....
+00000d20: 0100 7c00 6a09 a005 a100 a006 7c00 6a0a  ..|.j.......|.j.
+00000d30: a101 0100 7c00 6a09 a005 a100 a006 7c00  ....|.j.......|.
+00000d40: 6a0b a101 0100 7c00 6a09 a005 a100 a006  j.....|.j.......
+00000d50: 7c00 6a0c a101 0100 7c00 a005 a100 a006  |.j.....|.......
+00000d60: 7c00 6a09 a101 0100 7c00 a005 a100 a006  |.j.....|.......
+00000d70: 7c00 6a0d a101 0100 7c00 a005 a100 a006  |.j.....|.......
+00000d80: 7c00 6a0e a101 0100 6400 5300 2903 4eda  |.j.....d.S.).N.
+00000d90: 0853 6574 7469 6e67 737a 0b46 7261 6d65  .Settingsz.Frame
+00000da0: 2052 6174 653a 290f da09 7365 744c 6179   Rate:)...setLay
+00000db0: 6f75 7472 1d00 0000 7217 0000 00da 0e73  outr....r......s
+00000dc0: 6574 7469 6e67 735f 6772 6f75 7072 1900  ettings_groupr..
+00000dd0: 0000 da06 6c61 796f 7574 da09 6164 6457  ....layout..addW
+00000de0: 6964 6765 7472 1a00 0000 7238 0000 005a  idgetr....r8...Z
+00000df0: 0f72 6563 6f72 645f 636f 6e74 726f 6c73  .record_controls
+00000e00: 723d 0000 0072 3e00 0000 7240 0000 0072  r=...r>...r@...r
+00000e10: 4100 0000 7242 0000 0072 4b00 0000 722b  A...rB...rK...r+
+00000e20: 0000 0072 2b00 0000 722c 0000 0072 4300  ...r+...r,...rC.
+00000e30: 0000 6b00 0000 731c 0000 000c 010a 010e  ..k...s.........
+00000e40: 0114 0112 0110 0108 020e 0112 0112 0112  ................
+00000e50: 0110 0210 0114 027a 1d52 6563 6f72 6469  .......z.Recordi
+00000e60: 6e67 5769 6467 6574 2e70 6c61 6365 5f77  ngWidget.place_w
+00000e70: 6964 6765 7473 6301 0000 0000 0000 0000  idgetsc.........
+00000e80: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000e90: 5600 0000 7c00 6a00 6a01 a002 7c00 6a03  V...|.j.j...|.j.
+00000ea0: a101 0100 7c00 6a04 6a05 a002 7c00 6a06  ....|.j.j...|.j.
+00000eb0: 6a07 a101 0100 7c00 6a00 6a08 a002 7c00  j.....|.j.j...|.
+00000ec0: 6a09 a101 0100 7c00 6a0a 6a0b a002 7c00  j.....|.j.j...|.
+00000ed0: 6a0c a101 0100 7c00 6a06 6a0d a002 7c00  j.....|.j.j...|.
+00000ee0: 6a0e a101 0100 6400 5300 a901 4e29 0f72  j.....d.S...N).r
+00000ef0: 3500 0000 da0e 496d 6167 6542 726f 6164  5.....ImageBroad
+00000f00: 6361 7374 da07 636f 6e6e 6563 74da 0f49  cast..connect..I
+00000f10: 6d61 6765 5570 6461 7465 536c 6f74 7238  mageUpdateSlotr8
+00000f20: 0000 00da 0c76 616c 7565 4368 616e 6765  .....valueChange
+00000f30: 6472 2e00 0000 da13 7365 745f 6163 7469  dr......set_acti
+00000f40: 7665 5f6d 6f64 655f 6670 73da 0b64 726f  ve_mode_fps..dro
+00000f50: 7070 6564 5f66 7073 da12 7570 6461 7465  pped_fps..update
+00000f60: 5f64 726f 7070 6564 5f66 7073 723d 0000  _dropped_fpsr=..
+00000f70: 00da 0763 6c69 636b 6564 da11 746f 6767  ...clicked..togg
+00000f80: 6c65 5f73 7461 7274 5f73 746f 70da 1972  le_start_stop..r
+00000f90: 6563 6f72 6469 6e67 5f63 6f6d 706c 6574  ecording_complet
+00000fa0: 655f 7369 676e 616c da15 6f6e 5f72 6563  e_signal..on_rec
+00000fb0: 6f72 6469 6e67 5f63 6f6d 706c 6574 6572  ording_completer
+00000fc0: 4b00 0000 722b 0000 0072 2b00 0000 722c  K...r+...r+...r,
+00000fd0: 0000 0072 4400 0000 7f00 0000 730a 0000  ...rD.......s...
+00000fe0: 0010 0212 0110 0110 0114 017a 1f52 6563  ...........z.Rec
+00000ff0: 6f72 6469 6e67 5769 6467 6574 2e63 6f6e  ordingWidget.con
+00001000: 6e65 6374 5f77 6964 6765 7473 6301 0000  nect_widgetsc...
+00001010: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00001020: 0043 0000 0073 c600 0000 7c00 6a00 7401  .C...s....|.j.t.
+00001030: 6a02 6b02 722f 7401 6a03 7c00 5f00 7c00  j.k.r/t.j.|._.|.
+00001040: 6a04 a005 7c00 6a00 6a06 a101 0100 7c00  j...|.j.j.....|.
+00001050: 6a07 a008 6401 a101 0100 7409 a00a 6402  j...d.....t...d.
+00001060: a101 0100 740b 7c00 6a0c 6a0d 7c00 6a07  ....t.|.j.j.|.j.
+00001070: a00e a100 8302 7d01 7c00 6a0c a00f 7c01  ......}.|.j...|.
+00001080: a101 0100 6400 5300 7c00 6a00 7401 6a03  ....d.S.|.j.t.j.
+00001090: 6b02 7261 7c00 6a04 a008 6401 a101 0100  k.ra|.j...d.....
+000010a0: 7401 6a10 7c00 5f00 7c00 6a04 a005 7c00  t.j.|._.|.j...|.
+000010b0: 6a00 6a06 a101 0100 7c00 6a0c a011 a100  j.j.....|.j.....
+000010c0: 0100 7c00 6a07 a008 6403 a101 0100 7409  ..|.j...d.....t.
+000010d0: a00a 6404 a101 0100 7c00 6a07 a005 7c00  ..d.....|.j...|.
+000010e0: a012 a100 a101 0100 6400 5300 6400 5300  ........d.S.d.S.
+000010f0: 2905 4e46 7a12 496e 6974 6961 7465 2072  ).NFz.Initiate r
+00001100: 6563 6f72 6469 6e67 547a 2e53 746f 7020  ecordingTz.Stop 
+00001110: 7265 636f 7264 696e 6720 616e 6420 696e  recording and in
+00001120: 6974 6961 7465 2066 696e 616c 2073 6176  itiate final sav
+00001130: 6520 6f66 2066 696c 6529 1372 3b00 0000  e of file).r;...
+00001140: 7224 0000 0072 2800 0000 7229 0000 0072  r$...r(...r)...r
+00001150: 3d00 0000 da07 7365 7454 6578 7472 3c00  =.....setTextr<.
+00001160: 0000 7240 0000 0072 4a00 0000 da06 6c6f  ..r@...rJ.....lo
+00001170: 6767 6572 da04 696e 666f 7202 0000 0072  gger..infor....r
+00001180: 2e00 0000 725c 0000 00da 0474 6578 74da  ....r\.....text.
+00001190: 0f73 7461 7274 5f72 6563 6f72 6469 6e67  .start_recording
+000011a0: 722a 0000 00da 0e73 746f 705f 7265 636f  r*.....stop_reco
+000011b0: 7264 696e 6772 3f00 0000 2902 7246 0000  rdingr?...).rF..
+000011c0: 005a 0e72 6563 6f72 6469 6e67 5f70 6174  .Z.recording_pat
+000011d0: 6872 2b00 0000 722b 0000 0072 2c00 0000  hr+...r+...r,...
+000011e0: 726f 0000 0087 0000 0073 2000 0000 0c01  ro.......s .....
+000011f0: 0801 1001 0c01 0a02 1401 1001 0c02 0c01  ................
+00001200: 0802 1002 0a01 0c02 0a01 1401 04f6 7a21  ..............z!
+00001210: 5265 636f 7264 696e 6757 6964 6765 742e  RecordingWidget.
+00001220: 746f 6767 6c65 5f73 7461 7274 5f73 746f  toggle_start_sto
+00001230: 7063 0100 0000 0000 0000 0000 0000 0100  pc..............
+00001240: 0000 0300 0000 4300 0000 733c 0000 0074  ......C...s<...t
+00001250: 00a0 0164 01a1 0101 0074 026a 037c 005f  ...d.....t.j.|._
+00001260: 047c 006a 05a0 067c 006a 046a 07a1 0101  .|.j...|.j.j....
+00001270: 007c 006a 05a0 0864 02a1 0101 0074 00a0  .|.j...d.....t..
+00001280: 0164 03a1 0101 0064 0053 0029 044e 7a44  .d.....d.S.).NzD
+00001290: 5265 636f 7264 696e 6720 636f 6d70 6c65  Recording comple
+000012a0: 7465 2073 6967 6e61 6c20 7265 6365 6976  te signal receiv
+000012b0: 6564 2e2e 2e75 7064 6174 696e 6720 6e65  ed...updating ne
+000012c0: 7874 2061 6374 696f 6e20 616e 6420 6275  xt action and bu
+000012d0: 7474 6f6e 547a 2445 6e61 626c 696e 6720  ttonTz$Enabling 
+000012e0: 7374 6172 742f 7374 6f70 2072 6563 6f72  start/stop recor
+000012f0: 6469 6e67 2062 7574 746f 6e29 0972 7300  ding button).rs.
+00001300: 0000 7274 0000 0072 2400 0000 7228 0000  ..rt...r$...r(..
+00001310: 0072 3b00 0000 723d 0000 0072 7200 0000  .r;...r=...rr...
+00001320: 723c 0000 0072 4a00 0000 724b 0000 0072  r<...rJ...rK...r
+00001330: 2b00 0000 722b 0000 0072 2c00 0000 7271  +...r+...r,...rq
+00001340: 0000 009d 0000 0073 0a00 0000 0a01 0801  .......s........
+00001350: 1001 0c01 0e01 7a25 5265 636f 7264 696e  ......z%Recordin
+00001360: 6757 6964 6765 742e 6f6e 5f72 6563 6f72  gWidget.on_recor
+00001370: 6469 6e67 5f63 6f6d 706c 6574 6572 6c00  ding_completerl.
+00001380: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
+00001390: 0000 0006 0000 0043 0000 0073 3c00 0000  .......C...s<...
+000013a0: 6401 7d02 7c01 a000 a100 4400 5d0f 5c02  d.}.|.....D.].\.
+000013b0: 7d03 7d04 7c02 7c03 9b00 6402 7c04 6403  }.}.|.|...d.|.d.
+000013c0: 9b04 6404 9d04 3700 7d02 7106 7c00 6a01  ..d...7.}.q.|.j.
+000013d0: a002 7c02 a101 0100 6405 5300 2906 7a38  ..|.....d.S.).z8
+000013e0: 556e 7261 7665 6c20 6472 6f70 7065 6420  Unravel dropped 
+000013f0: 6670 7320 6469 6374 696f 6e61 7279 2074  fps dictionary t
+00001400: 6f20 6120 6d6f 7265 2072 6561 6461 626c  o a more readabl
+00001410: 6520 7374 7269 6e67 7a23 5261 7465 206f  e stringz#Rate o
+00001420: 6620 4672 616d 6520 4472 6f70 7069 6e67  f Frame Dropping
+00001430: 2062 7920 506f 7274 3a20 2020 207a 023a   by Port:    z.:
+00001440: 207a 032e 3025 7a08 2020 2020 2020 2020   z..0%z.        
+00001450: 4e29 03da 0569 7465 6d73 7241 0000 0072  N)...itemsrA...r
+00001460: 7200 0000 2905 7246 0000 0072 6c00 0000  r...).rF...rl...
+00001470: 7275 0000 00da 0470 6f72 745a 0964 726f  ru.....portZ.dro
+00001480: 705f 7261 7465 722b 0000 0072 2b00 0000  p_rater+...r+...
+00001490: 722c 0000 0072 6d00 0000 a400 0000 7308  r,...rm.......s.
+000014a0: 0000 0004 0210 0118 0110 027a 2252 6563  ...........z"Rec
+000014b0: 6f72 6469 6e67 5769 6467 6574 2e75 7064  ordingWidget.upd
+000014c0: 6174 655f 6472 6f70 7065 645f 6670 7363  ate_dropped_fpsc
+000014d0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+000014e0: 0400 0000 4300 0000 732c 0000 007c 006a  ....C...s,...|.j
+000014f0: 00a0 017c 006a 00a0 02a1 00a1 0101 0074  ...|.j.........t
+00001500: 03a0 047c 01a1 017d 027c 006a 00a0 057c  ...|...}.|.j...|
+00001510: 02a1 0101 0064 0053 0072 6600 0000 2906  .....d.S.rf...).
+00001520: 7242 0000 00da 0672 6573 697a 65da 0873  rB.....resize..s
+00001530: 697a 6548 696e 7472 0b00 0000 da09 6672  izeHintr......fr
+00001540: 6f6d 496d 6167 65da 0973 6574 5069 786d  omImage..setPixm
+00001550: 6170 2903 7246 0000 00da 0771 5f69 6d61  ap).rF.....q_ima
+00001560: 6765 da07 7170 6978 6d61 7072 2b00 0000  ge..qpixmapr+...
+00001570: 722b 0000 0072 2c00 0000 7269 0000 00ad  r+...r,...ri....
+00001580: 0000 0073 0600 0000 1201 0a01 1001 7a1f  ...s..........z.
+00001590: 5265 636f 7264 696e 6757 6964 6765 742e  RecordingWidget.
+000015a0: 496d 6167 6555 7064 6174 6553 6c6f 7429  ImageUpdateSlot)
+000015b0: 0f72 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+000015c0: 721e 0000 0072 3000 0000 7245 0000 0072  r....r0...rE...r
+000015d0: 3f00 0000 7243 0000 0072 4400 0000 726f  ?...rC...rD...ro
+000015e0: 0000 0072 7100 0000 da04 6469 6374 726d  ...rq.....dictrm
+000015f0: 0000 0072 6900 0000 da0d 5f5f 636c 6173  ...ri.....__clas
+00001600: 7363 656c 6c5f 5f72 2b00 0000 722b 0000  scell__r+...r+..
+00001610: 0072 4700 0000 722c 0000 0072 2d00 0000  .rG...r,...r-...
+00001620: 3100 0000 7314 0000 0008 0012 0208 2008  1...s......... .
+00001630: 0708 1108 1408 0808 160e 0710 0972 2d00  .............r-.
+00001640: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001650: 0000 0004 0000 0040 0000 0073 4400 0000  .......@...sD...
+00001660: 6500 5a01 6400 5a02 6410 6402 6503 6602  e.Z.d.Z.d.d.e.f.
+00001670: 6403 6404 8405 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
+00001680: 6407 6408 8400 5a06 6409 640a 8400 5a07  d.d...Z.d.d...Z.
+00001690: 640b 640c 8400 5a08 640d 640e 8400 5a09  d.d...Z.d.d...Z.
+000016a0: 640f 5300 2911 7232 0000 00e9 fa00 0000  d.S.).r2........
+000016b0: 7231 0000 0063 0300 0000 0000 0000 0000  r1...c..........
+000016c0: 0000 0600 0000 0500 0000 4300 0000 738c  ..........C...s.
+000016d0: 0000 007c 017c 005f 007c 027c 005f 0167  ...|.|._.|.|._.g
+000016e0: 007c 005f 027c 006a 006a 03a0 04a1 0044  .|._.|.j.j.....D
+000016f0: 005d 0a5c 027d 037d 047c 006a 02a0 057c  .].\.}.}.|.j...|
+00001700: 03a1 0101 0071 0f7c 006a 02a0 06a1 0001  .....q.|.j......
+00001710: 0074 077c 006a 0283 017d 0574 0874 09a0  .t.|.j...}.t.t..
+00001720: 0a7c 0564 0113 00a1 0183 017c 005f 0b74  .|.d.......|._.t
+00001730: 0874 09a0 0a7c 057c 006a 0b1b 00a1 0183  .t...|.|.j......
+00001740: 017c 005f 0c74 0d83 007c 005f 0e7c 006a  .|._.t...|._.|.j
+00001750: 00a0 0f7c 006a 0ea1 0101 0064 0053 0029  ...|.j.....d.S.)
+00001760: 024e 6700 0000 0000 00e0 3f29 1072 3100  .Ng.......?).r1.
+00001770: 0000 da13 7369 6e67 6c65 5f66 7261 6d65  ....single_frame
+00001780: 5f68 6569 6768 74da 0570 6f72 7473 da07  _height..ports..
+00001790: 7374 7265 616d 7372 7800 0000 da06 6170  streamsrx.....ap
+000017a0: 7065 6e64 da04 736f 7274 725e 0000 0072  pend..sortr^...r
+000017b0: 5a00 0000 da04 6d61 7468 da04 6365 696c  Z.....math..ceil
+000017c0: da0d 6672 616d 655f 636f 6c75 6d6e 73da  ..frame_columns.
+000017d0: 0a66 7261 6d65 5f72 6f77 7372 0500 0000  .frame_rowsr....
+000017e0: da16 6e65 775f 7379 6e63 5f70 6163 6b65  ..new_sync_packe
+000017f0: 745f 6e6f 7469 6365 da13 7375 6273 6372  t_notice..subscr
+00001800: 6962 655f 746f 5f6e 6f74 6963 6529 0672  ibe_to_notice).r
+00001810: 4600 0000 7231 0000 0072 8300 0000 7279  F...r1...r....ry
+00001820: 0000 00da 0673 7472 6561 6d5a 0c63 616d  .....streamZ.cam
+00001830: 6572 615f 636f 756e 7472 2b00 0000 722b  era_countr+...r+
+00001840: 0000 0072 2c00 0000 7230 0000 00b3 0000  ...r,...r0......
+00001850: 0073 1600 0000 0601 0601 0603 1401 0e03  .s..............
+00001860: 0a01 0a04 1401 1601 0802 1201 7a1d 556e  ............z.Un
+00001870: 7061 6972 6564 4672 616d 6542 7569 6c64  pairedFrameBuild
+00001880: 6572 2e5f 5f69 6e69 745f 5f63 0100 0000  er.__init__c....
+00001890: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000018a0: 4300 0000 731c 0000 0074 00a0 0164 01a1  C...s....t...d..
+000018b0: 0101 007c 006a 02a0 037c 006a 04a1 0101  ...|.j...|.j....
+000018c0: 0064 0053 0029 024e 7a2c 556e 7375 6273  .d.S.).Nz,Unsubs
+000018d0: 6372 6962 6520 6672 616d 6520 6275 696c  cribe frame buil
+000018e0: 6465 7220 6672 6f6d 2073 796e 6368 726f  der from synchro
+000018f0: 6e69 7a65 722e 2905 7273 0000 0072 7400  nizer.).rs...rt.
+00001900: 0000 7231 0000 00da 1575 6e73 7562 7363  ..r1.....unsubsc
+00001910: 7269 6265 5f74 6f5f 6e6f 7469 6365 728c  ribe_to_noticer.
+00001920: 0000 0072 4b00 0000 722b 0000 0072 2b00  ...rK...r+...r+.
+00001930: 0000 722c 0000 00da 1d75 6e73 7562 7363  ..r,.....unsubsc
+00001940: 7269 6265 5f66 726f 6d5f 7379 6e63 6872  ribe_from_synchr
+00001950: 6f6e 697a 6572 c800 0000 7304 0000 000a  onizer....s.....
+00001960: 0112 017a 3255 6e70 6169 7265 6446 7261  ...z2UnpairedFra
+00001970: 6d65 4275 696c 6465 722e 756e 7375 6273  meBuilder.unsubs
+00001980: 6372 6962 655f 6672 6f6d 5f73 796e 6368  cribe_from_synch
+00001990: 726f 6e69 7a65 7263 0200 0000 0000 0000  ronizerc........
+000019a0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+000019b0: 733c 0000 007c 006a 007d 027c 0164 0175  s<...|.j.}.|.d.u
+000019c0: 0072 1974 01a0 0264 02a1 0101 0074 036a  .r.t...d.....t.j
+000019d0: 047c 027c 0264 0366 0374 036a 0564 048d  .|.|.d.f.t.j.d..
+000019e0: 027d 037c 0353 007c 016a 067d 037c 0353  .}.|.S.|.j.}.|.S
+000019f0: 0029 057a 7b53 796e 6368 726f 6e69 7a61  .).z{Synchroniza
+00001a00: 7469 6f6e 2069 7373 7565 7320 6361 6e20  tion issues can 
+00001a10: 6c65 6164 2074 6f20 736f 6d65 2066 7261  lead to some fra
+00001a20: 6d65 7320 6265 696e 6720 4e6f 6e65 2061  mes being None a
+00001a30: 6d6f 6e67 0a20 2020 2020 2020 2074 6865  mong.        the
+00001a40: 2073 796e 6368 6564 2066 7261 6d65 732c   synched frames,
+00001a50: 2073 6f20 706c 7567 2074 6861 7420 7769   so plug that wi
+00001a60: 7468 2061 2062 6c61 6e6b 2066 7261 6d65  th a blank frame
+00001a70: 4e7a 1970 6c75 6767 696e 6720 626c 616e  Nz.plugging blan
+00001a80: 6b20 6672 616d 6520 6461 7461 e903 0000  k frame data....
+00001a90: 0029 01da 0564 7479 7065 2907 7283 0000  .)...dtype).r...
+00001aa0: 0072 7300 0000 da05 6465 6275 67da 026e  .rs.....debug..n
+00001ab0: 70da 057a 6572 6f73 da05 7569 6e74 38da  p..zeros..uint8.
+00001ac0: 0566 7261 6d65 2904 7246 0000 00da 0c66  .frame).rF.....f
+00001ad0: 7261 6d65 5f70 6163 6b65 74da 0465 6467  rame_packet..edg
+00001ae0: 6572 9700 0000 722b 0000 0072 2b00 0000  er....r+...r+...
+00001af0: 722c 0000 00da 1267 6574 5f66 7261 6d65  r,.....get_frame
+00001b00: 5f6f 725f 626c 616e 6bcd 0000 0073 0e00  _or_blank....s..
+00001b10: 0000 0604 0802 0a01 1601 0404 06fe 0402  ................
+00001b20: 7a27 556e 7061 6972 6564 4672 616d 6542  z'UnpairedFrameB
+00001b30: 7569 6c64 6572 2e67 6574 5f66 7261 6d65  uilder.get_frame
+00001b40: 5f6f 725f 626c 616e 6b63 0200 0000 0000  _or_blankc......
+00001b50: 0000 0000 0000 0800 0000 0900 0000 4300  ..............C.
+00001b60: 0000 7386 0000 0074 00a0 0164 01a1 0101  ..s....t...d....
+00001b70: 007c 016a 0264 0219 007d 027c 016a 0264  .|.j.d...}.|.j.d
+00001b80: 0319 007d 0374 037c 027c 0383 027d 0474  ...}.t.|.|...}.t
+00001b90: 047c 047c 0218 0064 041b 0083 017d 0574  .|.|...d.....}.t
+00001ba0: 047c 047c 0318 0064 041b 0083 017d 0667  .|.|...d.....}.g
+00001bb0: 0064 05a2 017d 0774 00a0 0164 06a1 0101  .d...}.t...d....
+00001bc0: 0074 056a 067c 017c 057c 057c 067c 0674  .t.j.|.|.|.|.|.t
+00001bd0: 056a 077c 0764 078d 077d 0174 087c 017c  .j.|.d...}.t.|.|
+00001be0: 006a 0964 088d 027d 017c 0153 0029 097a  .j.d...}.|.S.).z
+00001bf0: 6554 6f20 6d61 6b65 2073 7572 6520 7468  eTo make sure th
+00001c00: 6174 2066 7261 6d65 7320 616c 6967 6e20  at frames align 
+00001c10: 7765 6c6c 2c20 7363 616c 6520 7468 656d  well, scale them
+00001c20: 2061 6c6c 2074 6f20 7468 756d 626e 6169   all to thumbnai
+00001c30: 6c73 0a20 2020 2020 2020 2073 7175 6172  ls.        squar
+00001c40: 6573 2077 6974 6820 626c 6163 6b20 626f  es with black bo
+00001c50: 7264 6572 732e 7a0f 7265 7369 7a69 6e67  rders.z.resizing
+00001c60: 2073 7175 6172 6572 0100 0000 7257 0000   squarer....rW..
+00001c70: 00e9 0200 0000 2903 7201 0000 0072 0100  ......).r....r..
+00001c80: 0000 7201 0000 007a 1361 626f 7574 2074  ..r....z.about t
+00001c90: 6f20 7061 6420 626f 7264 6572 2901 723c  o pad border).r<
+00001ca0: 0000 0029 01da 0a6e 6577 5f68 6569 6768  ...)...new_heigh
+00001cb0: 7429 0a72 7300 0000 7293 0000 00da 0573  t).rs...r......s
+00001cc0: 6861 7065 7260 0000 0072 5a00 0000 da03  haper`...rZ.....
+00001cd0: 6376 32da 0e63 6f70 794d 616b 6542 6f72  cv2..copyMakeBor
+00001ce0: 6465 72da 0f42 4f52 4445 525f 434f 4e53  der..BORDER_CONS
+00001cf0: 5441 4e54 727a 0000 0072 8300 0000 2908  TANTrz...r....).
+00001d00: 7246 0000 0072 9700 0000 da06 6865 6967  rF...r......heig
+00001d10: 6874 da05 7769 6474 68da 0b70 6164 6465  ht..width..padde
+00001d20: 645f 7369 7a65 da0a 6865 6967 6874 5f70  d_size..height_p
+00001d30: 6164 da09 7769 6474 685f 7061 64da 0970  ad..width_pad..p
+00001d40: 6164 5f63 6f6c 6f72 722b 0000 0072 2b00  ad_colorr+...r+.
+00001d50: 0000 722c 0000 00da 1072 6573 697a 655f  ..r,.....resize_
+00001d60: 746f 5f73 7175 6172 65dc 0000 0073 2600  to_square....s&.
+00001d70: 0000 0a03 0a04 0a01 0a02 1002 1001 0801  ................
+00001d80: 0a02 0401 0201 0201 0201 0201 0201 0401  ................
+00001d90: 0201 06f9 0e0a 0401 7a25 556e 7061 6972  ........z%Unpair
+00001da0: 6564 4672 616d 6542 7569 6c64 6572 2e72  edFrameBuilder.r
+00001db0: 6573 697a 655f 746f 5f73 7175 6172 6563  esize_to_squarec
+00001dc0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+00001dd0: 0400 0000 4300 0000 736c 0000 007c 006a  ....C...sl...|.j
+00001de0: 006a 017c 0219 006a 026a 037d 037c 0364  .j.|...j.j.}.|.d
+00001df0: 016b 0272 0f09 007c 0153 007c 0364 0276  .k.r...|.S.|.d.v
+00001e00: 0072 1c74 04a0 057c 0174 046a 06a1 027d  .r.t...|.t.j...}
+00001e10: 017c 0153 007c 0364 0376 0072 2974 04a0  .|.S.|.d.v.r)t..
+00001e20: 057c 0174 046a 07a1 027d 017c 0153 007c  .|.t.j...}.|.S.|
+00001e30: 0364 0476 0072 3474 04a0 057c 0174 046a  .d.v.r4t...|.t.j
+00001e40: 08a1 027d 017c 0153 0029 054e 7201 0000  ...}.|.S.).Nr...
+00001e50: 0029 0272 5700 0000 e9fd ffff ff29 0272  .).rW........).r
+00001e60: 9b00 0000 e9fe ffff ff29 02e9 ffff ffff  .........)......
+00001e70: 7291 0000 0029 0972 3100 0000 7285 0000  r....).r1...r...
+00001e80: 00da 0663 616d 6572 61da 0e72 6f74 6174  ...camera..rotat
+00001e90: 696f 6e5f 636f 756e 7472 9e00 0000 da06  ion_countr......
+00001ea0: 726f 7461 7465 da13 524f 5441 5445 5f39  rotate..ROTATE_9
+00001eb0: 305f 434c 4f43 4b57 4953 45da 0a52 4f54  0_CLOCKWISE..ROT
+00001ec0: 4154 455f 3138 30da 1a52 4f54 4154 455f  ATE_180..ROTATE_
+00001ed0: 3930 5f43 4f55 4e54 4552 434c 4f43 4b57  90_COUNTERCLOCKW
+00001ee0: 4953 4529 0472 4600 0000 7297 0000 0072  ISE).rF...r....r
+00001ef0: 7900 0000 72ac 0000 0072 2b00 0000 722b  y...r....r+...r+
+00001f00: 0000 0072 2c00 0000 da0e 6170 706c 795f  ...r,.....apply_
+00001f10: 726f 7461 7469 6f6e fb00 0000 731a 0000  rotation....s...
+00001f20: 0010 0208 0102 0104 0808 f90e 0104 0608  ................
+00001f30: fb0e 0104 0408 fd0e 0104 027a 2355 6e70  ...........z#Unp
+00001f40: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
+00001f50: 722e 6170 706c 795f 726f 7461 7469 6f6e  r.apply_rotation
+00001f60: 6301 0000 0000 0000 0000 0000 0011 0000  c...............
+00001f70: 000a 0000 0043 0000 0073 7801 0000 7c00  .....C...sx...|.
+00001f80: 6a00 a001 a100 0100 7c00 6a02 6a03 7c00  j.......|.j.j.|.
+00001f90: 5f03 6900 7d01 7c00 6a04 4400 5d3f 7d02  _.i.}.|.j.D.]?}.
+00001fa0: 7c00 6a03 6a05 7c02 1900 7d03 7c00 a006  |.j.j.|...}.|...
+00001fb0: 7c03 a101 7d04 7c00 a007 7c04 a101 7d05  |...}.|...|...}.
+00001fc0: 7c00 a008 7c05 7c02 a102 7d06 7409 a00a  |...|.|...}.t...
+00001fd0: 7c06 6401 a102 7d07 7409 6a0b 7c07 740c  |.d...}.t.j.|.t.
+00001fe0: 7c02 8301 740d 7c07 6a0e 6401 1900 6402  |...t.|.j.d...d.
+00001ff0: 1b00 8301 740d 7c00 6a0f 6403 1b00 8301  ....t.|.j.d.....
+00002000: 6602 7409 6a10 6401 6404 6402 6405 8d07  f.t.j.d.d.d.d...
+00002010: 7d08 7c08 7c01 7c02 3c00 710f 6700 7d09  }.|.|.|.<.q.g.}.
+00002020: 6406 7d0a 6407 7d0b 6407 7d0c 7411 7c00  d.}.d.}.d.}.t.|.
+00002030: 6a04 8301 7d0d 7c01 a012 a100 4400 5d44  j...}.|.....D.]D
+00002040: 5c02 7d02 7d0e 7c0a 6406 7500 726b 7c0e  \.}.}.|.d.u.rk|.
+00002050: 7d0a 6e07 7413 a014 7c0a 7c0e 6702 a101  }.n.t...|.|.g...
+00002060: 7d0a 7c0b 6401 3700 7d0b 7c0d 6401 3800  }.|.d.7.}.|.d.8.
+00002070: 7d0d 7c0d 6407 6b02 7296 7c0b 7c00 6a15  }.|.d.k.r.|.|.j.
+00002080: 6b00 7296 7413 a014 7c0a 7c00 a006 6406  k.r.t...|.|...d.
+00002090: a101 6702 a101 7d0a 7c0b 6401 3700 7d0b  ..g...}.|.d.7.}.
+000020a0: 7c0b 7c00 6a15 6b00 7383 7c0b 7c00 6a15  |.|.j.k.s.|.|.j.
+000020b0: 6b02 72a4 7c09 a016 7c0a a101 0100 6406  k.r.|...|.....d.
+000020c0: 7d0a 6407 7d0b 7160 6406 7d0f 7c09 4400  }.d.}.q`d.}.|.D.
+000020d0: 5d10 7d10 7c0f 6406 7500 72b2 7c10 7d0f  ].}.|.d.u.r.|.}.
+000020e0: 71a9 7413 a017 7c0f 7c10 6702 a101 7d0f  q.t...|.|.g...}.
+000020f0: 71a9 7c0f 5300 2908 7afb 0a20 2020 2020  q.|.S.).z..     
+00002100: 2020 2054 6869 7320 676c 7565 7320 746f     This glues to
+00002110: 6765 7468 6572 2074 6865 2069 6e64 6976  gether the indiv
+00002120: 6964 7561 6c20 6672 616d 6573 2069 6e20  idual frames in 
+00002130: 7468 6520 7379 6e63 2070 6163 6b65 7420  the sync packet 
+00002140: 696e 746f 206f 6e65 206c 6172 6765 2062  into one large b
+00002150: 6c6f 636b 0a0a 2020 2020 2020 2020 4375  lock..        Cu
+00002160: 7272 656e 746c 7920 6a75 7374 2073 7461  rrently just sta
+00002170: 636b 696e 6720 616c 6c20 6672 616d 6573  cking all frames
+00002180: 2076 6572 7469 6361 6c6c 792c 2062 7574   vertically, but
+00002190: 2074 6869 7320 7368 6f75 6c64 2062 6520   this should be 
+000021a0: 6578 7061 6e64 6564 206f 6e20 7468 6520  expanded on the 
+000021b0: 0a20 2020 2020 2020 2074 6865 2066 7574  .        the fut
+000021c0: 7572 6520 746f 2061 6c6c 6f77 2077 7261  ure to allow wra
+000021d0: 7070 696e 6720 746f 2061 206d 6f72 6520  pping to a more 
+000021e0: 7371 7561 7265 2073 6861 7065 0a20 2020  square shape.   
+000021f0: 2020 2020 2072 5700 0000 729b 0000 00e9       rW...r.....
+00002200: 0400 0000 2903 7201 0000 0072 0100 0000  ....).r....r....
+00002210: e9ff 0000 0029 04da 0866 6f6e 7446 6163  .....)...fontFac
+00002220: 65da 0966 6f6e 7453 6361 6c65 da05 636f  e..fontScale..co
+00002230: 6c6f 72da 0974 6869 636b 6e65 7373 4e72  lor..thicknessNr
+00002240: 0100 0000 2918 728c 0000 00da 0367 6574  ....).r......get
+00002250: 7231 0000 00da 1363 7572 7265 6e74 5f73  r1.....current_s
+00002260: 796e 635f 7061 636b 6574 7284 0000 00da  ync_packetr.....
+00002270: 0d66 7261 6d65 5f70 6163 6b65 7473 729a  .frame_packetsr.
+00002280: 0000 0072 a700 0000 72b1 0000 0072 9e00  ...r....r....r..
+00002290: 0000 da04 666c 6970 da07 7075 7454 6578  ....flip..putTex
+000022a0: 7472 5f00 0000 725a 0000 0072 9d00 0000  tr_...rZ...r....
+000022b0: 7283 0000 00da 1446 4f4e 545f 4845 5253  r......FONT_HERS
+000022c0: 4845 595f 5349 4d50 4c45 5872 5e00 0000  HEY_SIMPLEXr^...
+000022d0: 7278 0000 0072 9400 0000 da06 6873 7461  rx...r......hsta
+000022e0: 636b 728a 0000 0072 8600 0000 da06 7673  ckr....r......vs
+000022f0: 7461 636b 2911 7246 0000 005a 1074 6875  tack).rF...Z.thu
+00002300: 6d62 6e61 696c 5f66 7261 6d65 7372 7900  mbnail_framesry.
+00002310: 0000 7298 0000 005a 0972 6177 5f66 7261  ..r....Z.raw_fra
+00002320: 6d65 5a0c 7371 7561 7265 5f66 7261 6d65  meZ.square_frame
+00002330: 5a0d 726f 7461 7465 645f 6672 616d 655a  Z.rotated_frameZ
+00002340: 0d66 6c69 7070 6564 5f66 7261 6d65 5a0a  .flipped_frameZ.
+00002350: 7465 7874 5f66 7261 6d65 728b 0000 005a  text_framer....Z
+00002360: 0b63 7572 7265 6e74 5f72 6f77 5a12 6375  .current_rowZ.cu
+00002370: 7272 656e 745f 726f 775f 6c65 6e67 7468  rrent_row_length
+00002380: 5a0c 6672 616d 6573 5f61 6464 6564 5a10  Z.frames_addedZ.
+00002390: 6672 616d 6573 5f72 656d 6169 6e69 6e67  frames_remaining
+000023a0: 7297 0000 005a 0a6d 6567 615f 6672 616d  r....Z.mega_fram
+000023b0: 65da 0372 6f77 722b 0000 0072 2b00 0000  e..rowr+...r+...
+000023c0: 722c 0000 00da 1367 6574 5f72 6563 6f72  r,.....get_recor
+000023d0: 6469 6e67 5f66 7261 6d65 0a01 0000 735a  ding_frame....sZ
+000023e0: 0000 000a 080a 0104 020a 010c 010a 010a  ................
+000023f0: 010c 010c 0106 0306 011e 0104 0102 0102  ................
+00002400: 0102 0106 fa0a 0904 0204 0104 0104 010a  ................
+00002410: 0110 0108 0206 010e 0208 0108 0108 020a  ................
+00002420: 0214 0108 010a fe0a 040a 0104 0104 0102  ................
+00002430: 8004 0208 0108 0106 0110 0204 037a 2855  .............z(U
+00002440: 6e70 6169 7265 6446 7261 6d65 4275 696c  npairedFrameBuil
+00002450: 6465 722e 6765 745f 7265 636f 7264 696e  der.get_recordin
+00002460: 675f 6672 616d 654e 2901 7282 0000 0029  g_frameN).r....)
+00002470: 0a72 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+00002480: 7220 0000 0072 3000 0000 7290 0000 0072  r ...r0...r....r
+00002490: 9a00 0000 72a7 0000 0072 b100 0000 72c1  ....r....r....r.
+000024a0: 0000 0072 2b00 0000 722b 0000 0072 2b00  ...r+...r+...r+.
+000024b0: 0000 722c 0000 0072 3200 0000 b200 0000  ..r,...r2.......
+000024c0: 730e 0000 0008 0010 0108 1508 0508 0f08  s...............
+000024d0: 1f0c 0f72 3200 0000 6300 0000 0000 0000  ...r2...c.......
+000024e0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+000024f0: 0073 3a00 0000 6500 5a01 6400 5a02 6503  .s:...e.Z.d.Z.e.
+00002500: 6504 8301 5a05 6503 6506 8301 5a07 6401  e...Z.e.e...Z.d.
+00002510: 6508 6602 8700 6601 6402 6403 840c 5a09  e.f...f.d.d...Z.
+00002520: 6404 6405 8400 5a0a 8700 0400 5a0b 5300  d.d...Z.....Z.S.
+00002530: 2906 7234 0000 0072 3300 0000 6302 0000  ).r4...r3...c...
+00002540: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00002550: 0003 0000 0073 2a00 0000 7400 7401 7c00  .....s*...t.t.|.
+00002560: 8302 a002 a100 0100 7c01 7c00 5f03 7404  ........|.|._.t.
+00002570: a005 6401 a101 0100 7406 8300 7c00 5f07  ..d.....t...|._.
+00002580: 6400 5300 2902 4e7a 2149 6e69 7469 6174  d.S.).Nz!Initiat
+00002590: 6564 2072 6563 6f72 6469 6e67 2066 7261  ed recording fra
+000025a0: 6d65 2065 6d69 7474 6572 2908 722f 0000  me emitter).r/..
+000025b0: 0072 3400 0000 7230 0000 00da 1772 6563  .r4...r0.....rec
+000025c0: 6f72 6469 6e67 5f66 7261 6d65 5f62 7569  ording_frame_bui
+000025d0: 6c64 6572 7273 0000 0072 7400 0000 7204  lderrs...rt...r.
+000025e0: 0000 00da 0f6b 6565 705f 636f 6c6c 6563  .....keep_collec
+000025f0: 7469 6e67 2902 7246 0000 0072 3300 0000  ting).rF...r3...
+00002600: 7247 0000 0072 2b00 0000 722c 0000 0072  rG...r+...r,...r
+00002610: 3000 0000 5001 0000 7308 0000 000e 0206  0...P...s.......
+00002620: 010a 010c 017a 1d55 6e70 6169 7265 6446  .....z.UnpairedF
+00002630: 7261 6d65 456d 6974 7465 722e 5f5f 696e  rameEmitter.__in
+00002640: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00002650: 0003 0000 0003 0000 0043 0000 0073 6400  .........C...sd.
+00002660: 0000 7c00 6a00 a001 a100 0100 7c00 6a00  ..|.j.......|.j.
+00002670: a002 a100 722b 7c00 6a03 a004 a100 7d01  ....r+|.j.....}.
+00002680: 7c01 6400 7501 7226 7405 7c01 8301 7d02  |.d.u.r&t.|...}.
+00002690: 7c00 6a06 a007 7c02 a101 0100 7c00 6a08  |.j...|.....|.j.
+000026a0: a007 7c00 6a03 6a09 6a08 a101 0100 7c00  ..|.j.j.j.....|.
+000026b0: 6a00 a002 a100 730a 740a a00b 6401 a101  j.....s.t...d...
+000026c0: 0100 6400 5300 2902 4e7a 2753 7465 7265  ..d.S.).Nz'Stere
+000026d0: 6f66 7261 6d65 2065 6d69 7474 6572 2072  oframe emitter r
+000026e0: 756e 2074 6872 6561 6420 656e 6465 642e  un thread ended.
+000026f0: 2e2e 290c 72c3 0000 00da 0373 6574 da06  ..).r......set..
+00002700: 6973 5f73 6574 72c2 0000 0072 c100 0000  is_setr....r....
+00002710: da0d 6376 325f 746f 5f71 6c61 6265 6c72  ..cv2_to_qlabelr
+00002720: 6700 0000 da04 656d 6974 726c 0000 0072  g.....emitrl...r
+00002730: 3100 0000 7273 0000 0072 7400 0000 2903  1...rs...rt...).
+00002740: 7246 0000 005a 0f72 6563 6f72 6469 6e67  rF...Z.recording
+00002750: 5f66 7261 6d65 da05 696d 6167 6572 2b00  _frame..imager+.
+00002760: 0000 722b 0000 0072 2c00 0000 da03 7275  ..r+...r,.....ru
+00002770: 6e57 0100 0073 1200 0000 0a02 0a02 0a04  nW...s..........
+00002780: 0802 0801 0c01 1201 0af7 0e0b 7a18 556e  ............z.Un
+00002790: 7061 6972 6564 4672 616d 6545 6d69 7474  pairedFrameEmitt
+000027a0: 6572 2e72 756e 290c 7225 0000 0072 2600  er.run).r%...r&.
+000027b0: 0000 7227 0000 0072 0800 0000 720a 0000  ..r'...r....r...
+000027c0: 0072 6700 0000 7280 0000 0072 6c00 0000  .rg...r....rl...
+000027d0: 7232 0000 0072 3000 0000 72c9 0000 0072  r2...r0...r....r
+000027e0: 8100 0000 722b 0000 0072 2b00 0000 7247  ....r+...r+...rG
+000027f0: 0000 0072 2c00 0000 7234 0000 004c 0100  ...r,...r4...L..
+00002800: 0073 0a00 0000 0800 0801 0801 1202 1007  .s..............
+00002810: 7234 0000 0063 0200 0000 0000 0000 0000  r4...c..........
+00002820: 0000 0300 0000 0300 0000 0300 0000 731a  ..............s.
+00002830: 0000 0087 0066 0164 0164 0284 087c 00a0  .....f.d.d...|..
+00002840: 00a1 0044 0083 017d 027c 0253 0029 034e  ...D...}.|.S.).N
+00002850: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00002860: 0004 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
+00002870: 7c00 5d0a 5c02 7d01 7d02 7c02 8800 6b00  |.].\.}.}.|...k.
+00002880: 7202 7c01 9102 7102 5300 722b 0000 0072  r.|...q.S.r+...r
+00002890: 2b00 0000 2903 724e 0000 00da 036b 6579  +...).rN.....key
+000028a0: 723c 0000 00a9 01da 0d6d 696e 5f74 6872  r<.......min_thr
+000028b0: 6573 686f 6c64 722b 0000 0072 2c00 0000  esholdr+...r,...
+000028c0: 7250 0000 006b 0100 0072 5b00 0000 7a23  rP...k...r[...z#
+000028d0: 6765 745f 656d 7074 795f 7061 6972 732e  get_empty_pairs.
+000028e0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000028f0: 6d70 3e29 0172 7800 0000 2903 da0c 626f  mp>).rx...)...bo
+00002900: 6172 645f 636f 756e 7473 72cc 0000 00da  ard_countsr.....
+00002910: 0b65 6d70 7479 5f70 6169 7273 722b 0000  .empty_pairsr+..
+00002920: 0072 cb00 0000 722c 0000 00da 0f67 6574  .r....r,.....get
+00002930: 5f65 6d70 7479 5f70 6169 7273 6a01 0000  _empty_pairsj...
+00002940: 7304 0000 0016 0104 0172 cf00 0000 6302  s........r....c.
+00002950: 0000 0000 0000 0000 0000 0007 0000 0005  ................
+00002960: 0000 0043 0000 0073 4400 0000 7c00 6a00  ...C...sD...|.j.
+00002970: 6400 6401 8502 1900 5c02 7d02 7d03 7c01  d.d.....\.}.}.|.
+00002980: 7401 7c02 8301 1b00 7d04 7402 7c03 7c04  t.|.....}.t.|.|.
+00002990: 1400 8301 7c01 6602 7d05 7403 6a04 7c00  ....|.f.}.t.j.|.
+000029a0: 7c05 7403 6a05 6402 8d03 7d06 7c06 5300  |.t.j.d...}.|.S.
+000029b0: 2903 4e72 9b00 0000 2901 da0d 696e 7465  ).Nr....)...inte
+000029c0: 7270 6f6c 6174 696f 6e29 0672 9d00 0000  rpolation).r....
+000029d0: da05 666c 6f61 7472 5a00 0000 729e 0000  ..floatrZ...r...
+000029e0: 0072 7a00 0000 da0a 494e 5445 525f 4152  .rz.....INTER_AR
+000029f0: 4541 2907 72c8 0000 0072 9c00 0000 da0e  EA).r....r......
+00002a00: 6375 7272 656e 745f 6865 6967 6874 da0d  current_height..
+00002a10: 6375 7272 656e 745f 7769 6474 68da 0572  current_width..r
+00002a20: 6174 696f da03 6469 6dda 0772 6573 697a  atio..dim..resiz
+00002a30: 6564 722b 0000 0072 2b00 0000 722c 0000  edr+...r+...r,..
+00002a40: 0072 7a00 0000 6e01 0000 730a 0000 0012  .rz...n...s.....
+00002a50: 010c 0110 0112 0104 0172 7a00 0000 6301  .........rz...c.
+00002a60: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00002a70: 0000 0043 0000 0073 3200 0000 7400 a001  ...C...s2...t...
+00002a80: 7c00 7400 6a02 a102 7d01 7403 7c01 6a04  |.t.j...}.t.|.j.
+00002a90: 7c01 6a05 6401 1900 7c01 6a05 6402 1900  |.j.d...|.j.d...
+00002aa0: 7403 6a06 6a07 8304 7d02 7c02 5300 2903  t.j.j...}.|.S.).
+00002ab0: 4e72 5700 0000 7201 0000 0029 0872 9e00  NrW...r....).r..
+00002ac0: 0000 da08 6376 7443 6f6c 6f72 da0d 434f  ....cvtColor..CO
+00002ad0: 4c4f 525f 4247 5232 5247 4272 0a00 0000  LOR_BGR2RGBr....
+00002ae0: da04 6461 7461 729d 0000 00da 0646 6f72  ..datar......For
+00002af0: 6d61 74da 0d46 6f72 6d61 745f 5247 4238  mat..Format_RGB8
+00002b00: 3838 2903 7297 0000 0072 c800 0000 da08  88).r....r......
+00002b10: 7174 5f66 7261 6d65 722b 0000 0072 2b00  qt_framer+...r+.
+00002b20: 0000 722c 0000 0072 c600 0000 7701 0000  ..r,...r....w...
+00002b30: 7310 0000 000e 0102 0204 0108 0108 0106  s...............
+00002b40: 0104 fc04 0672 c600 0000 6301 0000 0000  .....r....c.....
+00002b50: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
+00002b60: 0000 0073 4800 0000 7400 7c00 8301 7d01  ...sH...t.|...}.
+00002b70: 7401 7c01 8301 7d02 7c02 a002 7403 6a04  t.|...}.|...t.j.
+00002b80: a101 0100 7405 7406 6a07 8301 7d03 7408  ....t.t.j...}.t.
+00002b90: 7c02 8301 7d04 7c04 a009 a100 0100 7406  |...}.|.......t.
+00002ba0: a00a 7c03 a00b a100 a101 0100 6400 5300  ..|.........d.S.
+00002bb0: 7266 0000 0029 0c72 2300 0000 721e 0000  rf...).r#...r...
+00002bc0: 00da 0873 6574 5f6d 6f64 6572 1f00 0000  ...set_moder....
+00002bd0: da09 5265 636f 7264 696e 6772 0d00 0000  ..Recordingr....
+00002be0: da03 7379 73da 0461 7267 7672 2d00 0000  ..sys..argvr-...
+00002bf0: da04 7368 6f77 da04 6578 6974 da04 6578  ..show..exit..ex
+00002c00: 6563 2905 da0c 7365 7373 696f 6e5f 7061  ec)...session_pa
+00002c10: 7468 da06 636f 6e66 6967 722e 0000 00da  th..configr.....
+00002c20: 0341 7070 5a10 7265 636f 7264 696e 675f  .AppZ.recording_
+00002c30: 6469 616c 6f67 722b 0000 0072 2b00 0000  dialogr+...r+...
+00002c40: 722c 0000 00da 176c 6175 6e63 685f 7265  r,.....launch_re
+00002c50: 636f 7264 696e 675f 7769 6467 6574 8301  cording_widget..
+00002c60: 0000 730e 0000 0008 0108 010c 030a 0108  ..s.............
+00002c70: 0108 0112 0272 e800 0000 293f da0d 7079  .....r....)?..py
+00002c80: 7879 3364 2e6c 6f67 6765 72da 0670 7978  xy3d.logger..pyx
+00002c90: 7933 6472 7300 0000 72b8 0000 0072 2500  y3drs...r....r%.
+00002ca0: 0000 72e0 0000 0072 8800 0000 da07 7061  ..r....r......pa
+00002cb0: 7468 6c69 6272 0200 0000 da09 7468 7265  thlibr......thre
+00002cc0: 6164 696e 6772 0300 0000 7204 0000 00da  adingr....r.....
+00002cd0: 056e 756d 7079 7294 0000 00da 0571 7565  .numpyr......que
+00002ce0: 7565 7205 0000 00da 0465 6e75 6d72 0600  uer......enumr..
+00002cf0: 0000 729e 0000 00da 0c50 7951 7436 2e51  ..r......PyQt6.Q
+00002d00: 7443 6f72 6572 0700 0000 7208 0000 0072  tCorer....r....r
+00002d10: 0900 0000 5a0b 5079 5174 362e 5174 4775  ....Z.PyQt6.QtGu
+00002d20: 6972 0a00 0000 720b 0000 0072 0c00 0000  ir....r....r....
+00002d30: da0f 5079 5174 362e 5174 5769 6467 6574  ..PyQt6.QtWidget
+00002d40: 7372 0d00 0000 720e 0000 0072 0f00 0000  sr....r....r....
+00002d50: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00002d60: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
+00002d70: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+00002d80: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00002d90: 0072 1d00 0000 da16 7079 7879 3364 2e73  .r......pyxy3d.s
+00002da0: 6573 7369 6f6e 2e73 6573 7369 6f6e 721e  ession.sessionr.
+00002db0: 0000 0072 1f00 0000 da1b 7079 7879 3364  ...r......pyxy3d
+00002dc0: 2e63 616d 6572 6173 2e73 796e 6368 726f  .cameras.synchro
+00002dd0: 6e69 7a65 7272 2000 0000 7221 0000 00da  nizerr ...r!....
+00002de0: 1f70 7978 7933 642e 7265 636f 7264 696e  .pyxy3d.recordin
+00002df0: 672e 7669 6465 6f5f 7265 636f 7264 6572  g.video_recorder
+00002e00: 7222 0000 00da 1370 7978 7933 642e 636f  r".....pyxy3d.co
+00002e10: 6e66 6967 7572 6174 6f72 7223 0000 0072  nfiguratorr#...r
+00002e20: 2400 0000 722d 0000 0072 3200 0000 7234  $...r-...r2...r4
+00002e30: 0000 0072 cf00 0000 727a 0000 0072 c600  ...r....rz...r..
+00002e40: 0000 72e8 0000 0072 2b00 0000 722b 0000  ..r....r+...r+..
+00002e50: 0072 2b00 0000 722c 0000 00da 083c 6d6f  .r+...r,.....<mo
+00002e60: 6475 6c65 3e01 0000 0073 3800 0000 0802  dule>....s8.....
+00002e70: 0c01 0802 0801 0c01 1001 0801 0c01 0c01  ................
+00002e80: 0802 1401 1401 4c01 1014 0c01 0c01 0c01  ......L.........
+00002e90: 0c01 1002 1006 007f 0e02 007f 101b 081e  ................
+00002ea0: 0804 0809 0c0c                           ......
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/calibration_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/calibration_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,27 +118,27 @@
     ###################### Stereocalibration  ######################################
     def refresh_stereoframe(self):
         logger.info("Set current widget to config temporarily")
         self.setCurrentWidget(self.intrinsic_calibration_widget)
 
         logger.info("Remove stereoframe")
         self.removeWidget(self.extrinsic_calibration_widget)
-        self.extrinsic_calibration_widget.frame_builder.unsubscribe_from_synchronizer()
+        self.extrinsic_calibration_widget.paired_frame_builder.unsubscribe_from_synchronizer()
         del self.extrinsic_calibration_widget
 
         logger.info("Create new stereoframe")
         self.launch_new_stereoframe()
 
 
     def back_to_camera_config_wizard(self):
         logger.info("Moving back to camera config from stereoframe")
         self.setCurrentWidget(self.intrinsic_calibration_widget)
         self.session.pause_synchronizer()
 
-        self.extrinsic_calibration_widget.frame_builder.unsubscribe_from_synchronizer()
+        self.extrinsic_calibration_widget.paired_frame_builder.unsubscribe_from_synchronizer()
         self.removeWidget(self.extrinsic_calibration_widget)
         del self.extrinsic_calibration_widget
 
         active_port = self.intrinsic_calibration_widget.camera_tabs.currentIndex()
         self.intrinsic_calibration_widget.camera_tabs.activate_current_tab(active_port)
 
     def next_to_capture_volume(self):
@@ -160,15 +160,15 @@
         self.setCurrentWidget(self.intrinsic_calibration_widget)
 
         logger.info("Remove stereoframe")
         self.removeWidget(self.extrinsic_calibration_widget)
         logger.info("Remove capture volume")
         self.removeWidget(self.capture_volume)
         del self.capture_volume
-        self.extrinsic_calibration_widget.frame_builder.unsubscribe_from_synchronizer()
+        self.extrinsic_calibration_widget.paired_frame_builder.unsubscribe_from_synchronizer()
         del self.extrinsic_calibration_widget
 
         logger.info("Create new stereoframe")
         self.launch_new_stereoframe()
         self.session.unpause_synchronizer()
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,44 +52,51 @@
      
     def __init__(self,session:Session):
 
         super(ExtrinsicCalibrationWidget, self).__init__()
         self.session = session
         self.synchronizer:Synchronizer = self.session.synchronizer
 
-        self.create_stereoframe_tools()
+        self.paired_frame_builder = PairedFrameBuilder(self.synchronizer, board_count_target=30)
+        self.paired_frame_emitter = PairedFrameEmitter(self.paired_frame_builder)
+        self.paired_frame_emitter.start()
 
         self.frame_rate_spin = QSpinBox()
         self.frame_rate_spin.setValue(self.synchronizer.fps_target)
         self.board_count_spin = QSpinBox()
-        self.board_count_spin.setValue(self.frame_builder.board_count_target)
+        self.board_count_spin.setValue(self.paired_frame_builder.board_count_target)
         
         self.stereo_frame_display = QLabel()
         # self.navigation_bar = NavigationBarNext() 
         self.possible_action = PossibleActions.CollectData
         self.calibrate_collect_btn = QPushButton(self.possible_action.value)
         
         self.place_widgets()
         self.connect_widgets()        
 
         self.update_btn_eligibility()
     
+    def shutdown_threads(self):
+        """
+        There may be some lingering threads running when the extrinsic calibrator loses focus
+        This may be causing python to overload and pyqt to segfault during the calibration process
+        if I've moved from the extrinsic calibration widget to a different one...
+        """
+        logger.info("Unsubscribe paired frame builder from sync notice")
+        self.paired_frame_builder.unsubscribe_from_synchronizer()
+        logger.info("signal paired frame emitter to stop collecting frames")
+        self.paired_frame_emitter.keep_collecting.clear()
+
     def update_btn_eligibility(self):
         if self.session.is_extrinsic_calibration_eligible():
             self.calibrate_collect_btn.setEnabled(True)
         else:
             self.calibrate_collect_btn.setEnabled(False)
     
 
-    def create_stereoframe_tools(self):
-
-        self.frame_builder = PairedFrameBuilder(self.synchronizer, board_count_target=30)
-        self.frame_emitter = PairedFrameEmitter(self.frame_builder)
-        self.frame_emitter.start()
-
     def place_widgets(self):
         self.setLayout(QVBoxLayout())
         
         self.settings_group = QGroupBox("Settings")
         self.settings_group.setLayout(QHBoxLayout())
         self.settings_group.layout().addWidget(QLabel("Frame Rate:"))
         self.settings_group.layout().addWidget(self.frame_rate_spin)       
@@ -110,46 +117,44 @@
         self.layout().addWidget(self.calibrate_collect_btn)
 
 
 
     def connect_widgets(self):
         
         self.calibrate_collect_btn.clicked.connect(self.on_calibrate_collect_click)
-        self.frame_emitter.ImageBroadcast.connect(self.ImageUpdateSlot)
-        self.frame_emitter.possible_to_initialize_array.connect(self.enable_calibration)
+        self.paired_frame_emitter.ImageBroadcast.connect(self.ImageUpdateSlot)
+        self.paired_frame_emitter.possible_to_initialize_array.connect(self.enable_calibration)
         self.frame_rate_spin.valueChanged.connect(self.synchronizer.set_stream_fps)
         self.board_count_spin.valueChanged.connect(self.update_board_count_target)
-        self.frame_emitter.calibration_data_collected.connect(self.initiate_calibration)
+        self.paired_frame_emitter.calibration_data_collected.connect(self.initiate_calibration)
     
     def update_board_count_target(self, target):
-        self.frame_builder.board_count_target = target
+        self.paired_frame_builder.board_count_target = target
         
     def on_calibrate_collect_click(self):
         if self.possible_action == PossibleActions.CollectData:
             logger.info("Begin collecting calibration data")
             # by default, data saved to session folder
-            self.frame_builder.store_points.set()
+            self.paired_frame_builder.store_points.set()
             extrinsic_calibration_path = Path(self.session.path, "calibration", "extrinsic")
             self.session.start_recording(extrinsic_calibration_path,store_point_history=True)
             self.possible_action = PossibleActions.Terminate
             self.calibrate_collect_btn.setText(self.possible_action.value)
             self.calibrate_collect_btn.setEnabled(True)
             self.navigation_bar.back_btn.setEnabled(False)
 
         elif self.possible_action == PossibleActions.Terminate:
             logger.info("Terminating current data collection")
             self.terminate.emit()
-            # self.session.stop_recording()
-            # self.frame_builder.reset()
             self.possible_action = PossibleActions.CollectData
             self.calibrate_collect_btn.setText(self.possible_action.value)
 
         elif self.possible_action == PossibleActions.Calibrate:
             logger.info("Prematurely end data collection to initiate calibration")
-            self.frame_builder.store_points.clear()
+            self.paired_frame_builder.store_points.clear()
             self.initiate_calibration()
             
 
 
     def enable_calibration(self):
         self.possible_action = PossibleActions.Calibrate
         self.calibrate_collect_btn.setText(self.possible_action.value)
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  2 00:29:03 2023 UTC, .py size: 14193 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cf37 7964 7137 0000  o........7ydq7..
+00000000: 6f0d 0d0a 0000 0000 b243 8b64 1b36 0000  o........C.d.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6402 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6401 6c07 5a07 6400 6401 6c08 5a09 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c0a 6d0b 5a0b 0100 6400 6404 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6400 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -11,603 +11,595 @@
 000000a0: 640a 640b 8400 5a14 640c 640d 8400 5a15  d.d...Z.d.d...Z.
 000000b0: 6401 5300 290e e900 0000 004e 2901 da04  d.S.)......N)...
 000000c0: 5061 7468 2901 da0c 5379 6e63 6872 6f6e  Path)...Synchron
 000000d0: 697a 6572 2901 da0c 636f 6d62 696e 6174  izer)...combinat
 000000e0: 696f 6e73 2901 da05 5175 6575 6529 01da  ions)...Queue)..
 000000f0: 0545 7665 6e74 e904 0000 0063 0000 0000  .Event.....c....
 00000100: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000110: 4000 0000 738a 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000120: 0264 2264 0365 0366 0264 0464 0584 055a  .d"d.e.f.d.d...Z
+00000110: 4000 0000 7382 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000120: 0264 2064 0365 0366 0264 0464 0584 055a  .d d.e.f.d.d...Z
 00000130: 0464 0664 0784 005a 0564 0864 0984 005a  .d.d...Z.d.d...Z
 00000140: 0664 0a64 0b84 005a 0764 0c64 0d84 005a  .d.d...Z.d.d...Z
 00000150: 0864 0e64 0f84 005a 0964 1064 1184 005a  .d.d...Z.d.d...Z
 00000160: 0a64 1264 1384 005a 0b64 1464 1584 005a  .d.d...Z.d.d...Z
 00000170: 0c64 1664 1784 005a 0d64 1864 1984 005a  .d.d...Z.d.d...Z
-00000180: 0e64 1a64 1b84 005a 0f64 1c64 1d84 005a  .d.d...Z.d.d...Z
-00000190: 1064 1e65 1166 0264 1f64 2084 045a 1264  .d.e.f.d.d ..Z.d
-000001a0: 2153 0029 23da 1250 6169 7265 6446 7261  !S.)#..PairedFra
-000001b0: 6d65 4275 696c 6465 72e9 fa00 0000 e932  meBuilder......2
-000001c0: 0000 00da 0c73 796e 6368 726f 6e69 7a65  .....synchronize
-000001d0: 7263 0400 0000 0000 0000 0000 0000 0400  rc..............
-000001e0: 0000 0300 0000 4300 0000 734c 0000 007c  ......C...sL...|
-000001f0: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
-00000200: 0274 037c 005f 047c 00a0 05a1 007c 005f  .t.|._.|.....|._
-00000210: 0674 0783 007c 005f 087c 006a 00a0 097c  .t...|._.|.j...|
-00000220: 006a 08a1 0101 0074 0a83 007c 005f 0b7c  .j.....t...|._.|
-00000230: 00a0 0ca1 0001 0064 0053 0029 014e 290d  .......d.S.).N).
-00000240: 720b 0000 00da 1373 696e 676c 655f 6672  r......single_fr
-00000250: 616d 655f 6865 6967 6874 da12 626f 6172  ame_height..boar
-00000260: 645f 636f 756e 745f 7461 7267 6574 da14  d_count_target..
-00000270: 434f 4d4d 4f4e 5f43 4f52 4e45 525f 5441  COMMON_CORNER_TA
-00000280: 5247 4554 da14 636f 6d6d 6f6e 5f63 6f72  RGET..common_cor
-00000290: 6e65 725f 7461 7267 6574 da09 6765 745f  ner_target..get_
-000002a0: 7061 6972 73da 0570 6169 7273 7205 0000  pairs..pairsr...
-000002b0: 00da 166e 6577 5f73 796e 635f 7061 636b  ...new_sync_pack
-000002c0: 6574 5f6e 6f74 6963 65da 1373 7562 7363  et_notice..subsc
-000002d0: 7269 6265 5f74 6f5f 6e6f 7469 6365 7206  ribe_to_noticer.
-000002e0: 0000 00da 0c73 746f 7265 5f70 6f69 6e74  .....store_point
-000002f0: 73da 0572 6573 6574 2904 da04 7365 6c66  s..reset)...self
-00000300: 720b 0000 0072 0c00 0000 720d 0000 00a9  r....r....r.....
-00000310: 0072 1700 0000 fa52 433a 5c55 7365 7273  .r.....RC:\Users
-00000320: 5c4d 6163 2050 7269 626c 655c 7265 706f  \Mac Prible\repo
-00000330: 735c 7079 7879 3364 5c70 7978 7933 645c  s\pyxy3d\pyxy3d\
-00000340: 6775 695c 6672 616d 655f 6275 696c 6465  gui\frame_builde
-00000350: 7273 5c70 6169 7265 645f 6672 616d 655f  rs\paired_frame_
-00000360: 6275 696c 6465 722e 7079 da08 5f5f 696e  builder.py..__in
-00000370: 6974 5f5f 1100 0000 7312 0000 0006 0106  it__....s.......
-00000380: 0106 0306 010a 0708 020e 0108 010c 027a  ...............z
-00000390: 1b50 6169 7265 6446 7261 6d65 4275 696c  .PairedFrameBuil
-000003a0: 6465 722e 5f5f 696e 6974 5f5f 6301 0000  der.__init__c...
-000003b0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-000003c0: 0043 0000 0073 4800 0000 7400 a001 6401  .C...sH...t...d.
-000003d0: a101 0100 6402 6403 8400 7c00 6a02 4400  ....d.d...|.j.D.
-000003e0: 8301 7c00 5f03 7c00 6a02 a004 a100 7c00  ..|._.|.j.....|.
-000003f0: 5f05 6404 6403 8400 7c00 6a02 4400 8301  _.d.d...|.j.D...
-00000400: 7c00 5f06 7c00 6a07 a008 a100 0100 6400  |._.|.j.......d.
-00000410: 5300 2905 4e7a 1752 6573 6574 7469 6e67  S.).Nz.Resetting
-00000420: 2046 7261 6d65 2042 7569 6c64 6572 6301   Frame Builderc.
-00000430: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000440: 0000 0053 0000 0073 1200 0000 6900 7c00  ...S...s....i.|.
-00000450: 5d05 7d01 7c01 6400 9302 7102 5300 a901  ].}.|.d...q.S...
-00000460: 7201 0000 0072 1700 0000 a902 da02 2e30  r....r.........0
-00000470: da04 7061 6972 7217 0000 0072 1700 0000  ..pairr....r....
-00000480: 7218 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
-00000490: 3e2c 0000 0073 0200 0000 1200 7a2c 5061  >,...s......z,Pa
-000004a0: 6972 6564 4672 616d 6542 7569 6c64 6572  iredFrameBuilder
-000004b0: 2e72 6573 6574 2e3c 6c6f 6361 6c73 3e2e  .reset.<locals>.
-000004c0: 3c64 6963 7463 6f6d 703e 6301 0000 0000  <dictcomp>c.....
-000004d0: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
-000004e0: 0000 0073 1800 0000 6900 7c00 5d08 7d01  ...s....i.|.].}.
-000004f0: 7c01 6700 6700 6400 9c02 9302 7102 5300  |.g.g.d.....q.S.
-00000500: 2901 2902 da09 696d 675f 6c6f 635f 41da  ).)...img_loc_A.
-00000510: 0969 6d67 5f6c 6f63 5f42 7217 0000 0072  .img_loc_Br....r
-00000520: 1b00 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00000530: 0000 0072 1e00 0000 2e00 0000 7302 0000  ...r........s...
-00000540: 0018 0029 09da 066c 6f67 6765 72da 0469  ...)...logger..i
-00000550: 6e66 6f72 1100 0000 da0c 626f 6172 645f  nfor......board_
-00000560: 636f 756e 7473 da04 636f 7079 da0b 7374  counts..copy..st
-00000570: 6572 656f 5f6c 6973 74da 0e73 7465 7265  ereo_list..stere
-00000580: 6f5f 6869 7374 6f72 7972 1400 0000 da05  o_historyr......
-00000590: 636c 6561 72a9 0172 1600 0000 7217 0000  clear..r....r...
-000005a0: 0072 1700 0000 7218 0000 0072 1500 0000  .r....r....r....
-000005b0: 2a00 0000 730a 0000 000a 0112 010c 0112  *...s...........
-000005c0: 010e 017a 1850 6169 7265 6446 7261 6d65  ...z.PairedFrame
-000005d0: 4275 696c 6465 722e 7265 7365 7463 0100  Builder.resetc..
-000005e0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000005f0: 0000 4300 0000 731c 0000 0074 00a0 0164  ..C...s....t...d
-00000600: 01a1 0101 007c 006a 02a0 037c 006a 04a1  .....|.j...|.j..
-00000610: 0101 0064 0053 0029 024e 7a2c 556e 7375  ...d.S.).Nz,Unsu
-00000620: 6273 6372 6962 6520 6672 616d 6520 6275  bscribe frame bu
-00000630: 696c 6465 7220 6672 6f6d 2073 796e 6368  ilder from synch
-00000640: 726f 6e69 7a65 722e 2905 7221 0000 0072  ronizer.).r!...r
-00000650: 2200 0000 720b 0000 00da 1575 6e73 7562  "...r......unsub
-00000660: 7363 7269 6265 5f74 6f5f 6e6f 7469 6365  scribe_to_notice
-00000670: 7212 0000 0072 2800 0000 7217 0000 0072  r....r(...r....r
-00000680: 1700 0000 7218 0000 00da 1d75 6e73 7562  ....r......unsub
-00000690: 7363 7269 6265 5f66 726f 6d5f 7379 6e63  scribe_from_sync
-000006a0: 6872 6f6e 697a 6572 3100 0000 7304 0000  hronizer1...s...
-000006b0: 000a 0112 017a 3050 6169 7265 6446 7261  .....z0PairedFra
-000006c0: 6d65 4275 696c 6465 722e 756e 7375 6273  meBuilder.unsubs
-000006d0: 6372 6962 655f 6672 6f6d 5f73 796e 6368  cribe_from_synch
-000006e0: 726f 6e69 7a65 7263 0100 0000 0000 0000  ronizerc........
-000006f0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000700: 7332 0000 0064 0164 0284 0074 007c 006a  s2...d.d...t.|.j
-00000710: 016a 0264 0383 0244 0083 017d 0164 0464  .j.d...D...}.d.d
-00000720: 0284 007c 0144 0083 017d 0274 037c 0283  ...|.D...}.t.|..
-00000730: 017d 027c 0253 0029 054e 6301 0000 0000  .}.|.S.).Nc.....
-00000740: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00000750: 0000 0073 1000 0000 6700 7c00 5d04 7d01  ...s....g.|.].}.
-00000760: 7c01 9102 7102 5300 7217 0000 0072 1700  |...q.S.r....r..
-00000770: 0000 721b 0000 0072 1700 0000 7217 0000  ..r....r....r...
-00000780: 0072 1800 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00000790: 703e 3600 0000 7302 0000 0010 007a 3050  p>6...s......z0P
-000007a0: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
-000007b0: 722e 6765 745f 7061 6972 732e 3c6c 6f63  r.get_pairs.<loc
-000007c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3ee9  als>.<listcomp>.
-000007d0: 0200 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000007e0: 0002 0000 0005 0000 0053 0000 0073 1c00  .........S...s..
-000007f0: 0000 6700 7c00 5d0a 7d01 7400 7c01 8301  ..g.|.].}.t.|...
-00000800: 7401 7c01 8301 6602 9102 7102 5300 7217  t.|...f...q.S.r.
-00000810: 0000 0029 02da 036d 696e da03 6d61 7872  ...)...min..maxr
-00000820: 1b00 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00000830: 0000 0072 2b00 0000 3700 0000 7306 0000  ...r+...7...s...
-00000840: 0006 0010 0106 ff29 0472 0400 0000 720b  .......).r....r.
-00000850: 0000 00da 0570 6f72 7473 da06 736f 7274  .....ports..sort
-00000860: 6564 2903 7216 0000 0072 1100 0000 5a0c  ed).r....r....Z.
-00000870: 736f 7274 6564 5f70 6f72 7473 7217 0000  sorted_portsr...
-00000880: 0072 1700 0000 7218 0000 0072 1000 0000  .r....r....r....
-00000890: 3500 0000 7310 0000 0018 0106 0102 0106  5...s...........
-000008a0: ff02 0302 0104 ff04 037a 1c50 6169 7265  .........z.Paire
-000008b0: 6446 7261 6d65 4275 696c 6465 722e 6765  dFrameBuilder.ge
-000008c0: 745f 7061 6972 7363 0100 0000 0000 0000  t_pairsc........
-000008d0: 0000 0000 0100 0000 0500 0000 0300 0000  ................
-000008e0: 7334 0000 0087 0066 0164 0164 0284 0888  s4.....f.d.d....
-000008f0: 006a 00a0 01a1 0044 0083 0188 005f 0274  .j.....D....._.t
-00000900: 0388 006a 0288 006a 006a 0464 0364 048d  ...j...j.j.d.d..
-00000910: 0388 005f 0264 0053 0029 054e 6301 0000  ..._.d.S.).Nc...
-00000920: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000930: 0013 0000 0073 1e00 0000 6700 7c00 5d0b  .....s....g.|.].
-00000940: 5c02 7d01 7d02 7c02 8800 6a00 6b00 7202  \.}.}.|...j.k.r.
-00000950: 7c01 9102 7102 5300 7217 0000 0029 0172  |...q.S.r....).r
-00000960: 0d00 0000 a903 721c 0000 00da 036b 6579  ......r......key
-00000970: da05 7661 6c75 6572 2800 0000 7217 0000  ..valuer(...r...
-00000980: 0072 1800 0000 722b 0000 0040 0000 0073  .r....r+...@...s
-00000990: 0c00 0000 0600 0602 0801 02fd 0201 06ff  ................
-000009a0: 7a39 5061 6972 6564 4672 616d 6542 7569  z9PairedFrameBui
-000009b0: 6c64 6572 2e75 7064 6174 655f 7374 6572  lder.update_ster
-000009c0: 656f 5f6c 6973 742e 3c6c 6f63 616c 733e  eo_list.<locals>
-000009d0: 2e3c 6c69 7374 636f 6d70 3e54 2902 7232  .<listcomp>T).r2
-000009e0: 0000 00da 0772 6576 6572 7365 2905 7223  .....reverse).r#
-000009f0: 0000 00da 0569 7465 6d73 7225 0000 0072  .....itemsr%...r
-00000a00: 3000 0000 da03 6765 7472 2800 0000 7217  0.....getr(...r.
-00000a10: 0000 0072 2800 0000 7218 0000 00da 1275  ...r(...r......u
-00000a20: 7064 6174 655f 7374 6572 656f 5f6c 6973  pdate_stereo_lis
-00000a30: 743f 0000 0073 0800 0000 0a01 0802 08fe  t?...s..........
-00000a40: 1a05 7a25 5061 6972 6564 4672 616d 6542  ..z%PairedFrameB
-00000a50: 7569 6c64 6572 2e75 7064 6174 655f 7374  uilder.update_st
-00000a60: 6572 656f 5f6c 6973 7463 0200 0000 0000  ereo_listc......
-00000a70: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
-00000a80: 0000 734c 0000 007c 006a 007d 027c 006a  ..sL...|.j.}.|.j
-00000a90: 016a 027c 0119 007d 037c 0364 0175 0072  .j.|...}.|.d.u.r
-00000aa0: 1f74 03a0 0464 02a1 0101 0074 056a 067c  .t...d.....t.j.|
-00000ab0: 027c 0264 0366 0374 056a 0764 048d 027d  .|.d.f.t.j.d...}
-00000ac0: 047c 0453 007c 036a 08a0 09a1 007d 047c  .|.S.|.j.....}.|
-00000ad0: 0453 0029 057a 7b53 796e 6368 726f 6e69  .S.).z{Synchroni
-00000ae0: 7a61 7469 6f6e 2069 7373 7565 7320 6361  zation issues ca
-00000af0: 6e20 6c65 6164 2074 6f20 736f 6d65 2066  n lead to some f
-00000b00: 7261 6d65 7320 6265 696e 6720 4e6f 6e65  rames being None
-00000b10: 2061 6d6f 6e67 0a20 2020 2020 2020 2074   among.        t
-00000b20: 6865 2073 796e 6368 6564 2066 7261 6d65  he synched frame
-00000b30: 732c 2073 6f20 706c 7567 2074 6861 7420  s, so plug that 
-00000b40: 7769 7468 2061 2062 6c61 6e6b 2066 7261  with a blank fra
-00000b50: 6d65 4e7a 1970 6c75 6767 696e 6720 626c  meNz.plugging bl
-00000b60: 616e 6b20 6672 616d 6520 6461 7461 e903  ank frame data..
-00000b70: 0000 0029 01da 0564 7479 7065 290a 720c  ...)...dtype).r.
-00000b80: 0000 00da 1363 7572 7265 6e74 5f73 796e  .....current_syn
-00000b90: 635f 7061 636b 6574 da0d 6672 616d 655f  c_packet..frame_
-00000ba0: 7061 636b 6574 7372 2100 0000 da05 6465  packetsr!.....de
-00000bb0: 6275 67da 026e 70da 057a 6572 6f73 da05  bug..np..zeros..
-00000bc0: 7569 6e74 38da 0566 7261 6d65 7224 0000  uint8..framer$..
-00000bd0: 0029 0572 1600 0000 da04 706f 7274 da04  .).r......port..
-00000be0: 6564 6765 da0c 6672 616d 655f 7061 636b  edge..frame_pack
-00000bf0: 6574 7240 0000 0072 1700 0000 7217 0000  etr@...r....r...
-00000c00: 0072 1800 0000 da12 6765 745f 6672 616d  .r......get_fram
-00000c10: 655f 6f72 5f62 6c61 6e6b 4700 0000 7310  e_or_blankG...s.
-00000c20: 0000 0006 040c 0108 010a 0116 0104 040a  ................
-00000c30: fe04 027a 2550 6169 7265 6446 7261 6d65  ...z%PairedFrame
-00000c40: 4275 696c 6465 722e 6765 745f 6672 616d  Builder.get_fram
-00000c50: 655f 6f72 5f62 6c61 6e6b 6305 0000 0000  e_or_blankc.....
-00000c60: 0000 0000 0000 0010 0000 0008 0000 0043  ...............C
-00000c70: 0000 0073 c201 0000 7c00 6a00 6a01 7c02  ...s....|.j.j.|.
-00000c80: 1900 6401 7500 7214 7402 a003 6402 7c02  ..d.u.r.t...d.|.
-00000c90: 9b00 9d02 a101 0100 7c01 7c03 6602 5300  ........|.|.f.S.
-00000ca0: 7c00 6a00 6a01 7c04 1900 6401 7500 7228  |.j.j.|...d.u.r(
-00000cb0: 7402 a003 6402 7c04 9b00 9d02 a101 0100  t...d.|.........
-00000cc0: 7c01 7c03 6602 5300 7c00 6a00 6a01 7c02  |.|.f.S.|.j.j.|.
-00000cd0: 1900 7d05 7c00 6a00 6a01 7c04 1900 7d06  ..}.|.j.j.|...}.
-00000ce0: 7c05 6a04 6401 7500 733e 7c06 6a04 6401  |.j.d.u.s>|.j.d.
-00000cf0: 7500 7242 7c01 7c03 6602 5300 7c05 6a04  u.rB|.|.f.S.|.j.
-00000d00: 6a05 7d07 7c06 6a04 6a05 7d08 7406 a007  j.}.|.j.j.}.t...
-00000d10: 7c07 7c08 a102 7d09 7c05 6a04 6a08 7d0a  |.|...}.|.j.j.}.
-00000d20: 7c06 6a04 6a08 7d0b 7409 7c09 8301 7c00  |.j.j.}.t.|...|.
-00000d30: 6a0a 6b05 728b 7c00 6a0b a00c a100 728b  j.k.r.|.j.....r.
-00000d40: 7c00 6a0d 7c02 7c04 6602 1900 6403 1900  |.j.|.|.f...d...
-00000d50: a00e 7c0a a00f a100 a101 0100 7c00 6a0d  ..|.........|.j.
-00000d60: 7c02 7c04 6602 1900 6404 1900 a00e 7c0b  |.|.f...d.....|.
-00000d70: a00f a100 a101 0100 7c00 6a10 7c02 7c04  ........|.j.|.|.
-00000d80: 6602 0500 1900 6405 3700 0300 3c00 7411  f.....d.7...<.t.
-00000d90: 7c07 7c0a 8302 4400 5d23 5c02 7d0c 7d0d  |.|...D.]#\.}.}.
-00000da0: 7c0c 7c09 7600 72b3 7412 7413 7c0d 6406  |.|.v.r.t.t.|.d.
-00000db0: 1900 8301 8301 7d0e 7412 7413 7c0d 6405  ......}.t.t.|.d.
-00000dc0: 1900 8301 8301 7d0f 7414 a015 7c01 7c0e  ......}.t...|.|.
-00000dd0: 7c0f 6602 6407 6408 6409 a105 0100 7190  |.f.d.d.d.....q.
-00000de0: 7411 7c08 7c0b 8302 4400 5d23 5c02 7d0c  t.|.|...D.]#\.}.
-00000df0: 7d0d 7c0c 7c09 7600 72dc 7412 7413 7c0d  }.|.|.v.r.t.t.|.
-00000e00: 6406 1900 8301 8301 7d0e 7412 7413 7c0d  d.......}.t.t.|.
-00000e10: 6405 1900 8301 8301 7d0f 7414 a015 7c03  d.......}.t...|.
-00000e20: 7c0e 7c0f 6602 6407 6408 6409 a105 0100  |.|.f.d.d.d.....
-00000e30: 71b9 7c01 7c03 6602 5300 290a 7acf 0a20  q.|.|.f.S.).z.. 
-00000e40: 2020 2020 2020 2052 6574 7572 6e20 756e         Return un
-00000e50: 616c 7465 7265 6420 6672 616d 6520 6966  altered frame if
-00000e60: 206e 6f20 636f 726e 6572 2069 6e66 6f72   no corner infor
-00000e70: 6d61 7469 6f6e 2064 6574 6563 7465 642c  mation detected,
-00000e80: 206f 7468 6572 7769 7365 0a20 2020 2020   otherwise.     
-00000e90: 2020 2072 6563 6f72 6420 7468 6520 636f     record the co
-00000ea0: 726e 6572 7320 7468 6174 2061 7265 2073  rners that are s
-00000eb0: 6861 7265 6420 6265 7477 6565 6e20 7468  hared between th
-00000ec0: 6520 7477 6f20 6672 616d 6573 0a20 2020  e two frames.   
-00000ed0: 2020 2020 2061 6e64 2072 6574 7572 6e20       and return 
-00000ee0: 7477 6f20 6672 616d 6573 2077 6974 6820  two frames with 
-00000ef0: 7368 6172 6564 2063 6f72 6e65 7273 2064  shared corners d
-00000f00: 7261 776e 0a20 2020 2020 2020 204e 7a16  rawn.        Nz.
-00000f10: 4472 6f70 7065 6420 6672 616d 6520 6174  Dropped frame at
-00000f20: 2070 6f72 7420 721f 0000 0072 2000 0000   port r....r ...
-00000f30: e901 0000 0072 0100 0000 e905 0000 0029  .....r.........)
-00000f40: 0372 0100 0000 7201 0000 00e9 dc00 0000  .r....r.........
-00000f50: 7238 0000 0029 1672 3a00 0000 723b 0000  r8...).r:...r;..
-00000f60: 0072 2100 0000 da07 7761 726e 696e 67da  .r!.....warning.
-00000f70: 0670 6f69 6e74 73da 0870 6f69 6e74 5f69  .points..point_i
-00000f80: 6472 3d00 0000 da0b 696e 7465 7273 6563  dr=.....intersec
-00000f90: 7431 64da 0769 6d67 5f6c 6f63 da03 6c65  t1d..img_loc..le
-00000fa0: 6e72 0f00 0000 7214 0000 00da 0669 735f  nr....r......is_
-00000fb0: 7365 7472 2600 0000 da06 6578 7465 6e64  setr&.....extend
-00000fc0: da06 746f 6c69 7374 7223 0000 00da 037a  ..tolistr#.....z
-00000fd0: 6970 da05 726f 756e 64da 0566 6c6f 6174  ip..round..float
-00000fe0: da03 6376 32da 0663 6972 636c 6529 1072  ..cv2..circle).r
-00000ff0: 1600 0000 da06 6672 616d 6541 da05 706f  ......frameA..po
-00001000: 7274 41da 0666 7261 6d65 42da 0570 6f72  rtA..frameB..por
-00001010: 7442 5a0e 6672 616d 655f 7061 636b 6574  tBZ.frame_packet
-00001020: 5f41 5a0e 6672 616d 655f 7061 636b 6574  _AZ.frame_packet
-00001030: 5f42 5a05 6964 735f 415a 0569 6473 5f42  _BZ.ids_AZ.ids_B
-00001040: da0a 636f 6d6d 6f6e 5f69 6473 721f 0000  ..common_idsr...
-00001050: 0072 2000 0000 da03 5f69 6472 4c00 0000  .r ....._idrL...
-00001060: da01 78da 0179 7217 0000 0072 1700 0000  ..x..yr....r....
-00001070: 7218 0000 00da 1a64 7261 775f 636f 6d6d  r......draw_comm
-00001080: 6f6e 5f63 6f72 6e65 725f 6375 7272 656e  on_corner_curren
-00001090: 7455 0000 0073 4000 0000 1007 1001 0801  tU...s@.........
-000010a0: 1002 1001 0801 0c02 0c01 1402 0801 0802  ................
-000010b0: 0801 0c01 0802 0801 1806 1c04 1c01 1601  ................
-000010c0: 1202 0801 1001 1001 1602 0280 1202 0801  ................
-000010d0: 1001 1001 1602 0280 0801 7a2d 5061 6972  ..........z-Pair
-000010e0: 6564 4672 616d 6542 7569 6c64 6572 2e64  edFrameBuilder.d
-000010f0: 7261 775f 636f 6d6d 6f6e 5f63 6f72 6e65  raw_common_corne
-00001100: 725f 6375 7272 656e 7463 0500 0000 0000  r_currentc......
-00001110: 0000 0000 0000 0a00 0000 0900 0000 4300  ..............C.
-00001120: 0000 7398 0000 007c 027c 0466 027d 057c  ..s....|.|.f.}.|
-00001130: 006a 007c 0519 0064 0119 007d 067c 006a  .j.|...d...}.|.j
-00001140: 007c 0519 0064 0219 007d 077c 0644 005d  .|...d...}.|.D.]
-00001150: 187d 0874 017c 0864 0319 0083 0174 017c  .}.t.|.d.....t.|
-00001160: 0864 0419 0083 0166 027d 0974 02a0 037c  .d.....f.}.t...|
-00001170: 017c 0964 0564 0664 0564 04a1 0601 0071  .|.d.d.d.d.....q
-00001180: 147c 0744 005d 187d 0874 017c 0864 0319  .|.D.].}.t.|.d..
-00001190: 0083 0174 017c 0864 0419 0083 0166 027d  ...t.|.d.....f.}
-000011a0: 0974 02a0 037c 037c 0964 0564 0664 0564  .t...|.|.d.d.d.d
-000011b0: 04a1 0601 0071 2f7c 017c 0366 0253 0029  .....q/|.|.f.S.)
-000011c0: 074e 721f 0000 0072 2000 0000 7201 0000  .Nr....r ...r...
-000011d0: 0072 4500 0000 722c 0000 00a9 03e9 ff00  .rE...r,........
-000011e0: 0000 e9a5 0000 0072 0100 0000 2904 7226  .......r....).r&
-000011f0: 0000 00da 0369 6e74 7254 0000 0072 5500  .....intrT...rU.
-00001200: 0000 290a 7216 0000 0072 5600 0000 7257  ..).r....rV...rW
-00001210: 0000 0072 5800 0000 7259 0000 0072 1d00  ...rX...rY...r..
-00001220: 0000 721f 0000 0072 2000 0000 5a08 636f  ..r....r ...Z.co
-00001230: 6f72 645f 7879 da06 636f 726e 6572 7217  ord_xy..cornerr.
-00001240: 0000 0072 1700 0000 7218 0000 00da 1a64  ...r....r......d
-00001250: 7261 775f 636f 6d6d 6f6e 5f63 6f72 6e65  raw_common_corne
-00001260: 725f 6869 7374 6f72 798c 0000 0073 1400  r_history....s..
-00001270: 0000 0801 0e01 0e01 0802 1801 1601 0802  ................
-00001280: 1801 1601 0802 7a2d 5061 6972 6564 4672  ......z-PairedFr
-00001290: 616d 6542 7569 6c64 6572 2e64 7261 775f  ameBuilder.draw_
-000012a0: 636f 6d6d 6f6e 5f63 6f72 6e65 725f 6869  common_corner_hi
-000012b0: 7374 6f72 7963 0200 0000 0000 0000 0000  storyc..........
-000012c0: 0000 0800 0000 0900 0000 4300 0000 7386  ..........C...s.
-000012d0: 0000 0074 00a0 0164 01a1 0101 007c 016a  ...t...d.....|.j
-000012e0: 0264 0219 007d 027c 016a 0264 0319 007d  .d...}.|.j.d...}
-000012f0: 0374 037c 027c 0383 027d 0474 047c 047c  .t.|.|...}.t.|.|
-00001300: 0218 0064 041b 0083 017d 0574 047c 047c  ...d.....}.t.|.|
-00001310: 0318 0064 041b 0083 017d 0667 0064 05a2  ...d.....}.g.d..
-00001320: 017d 0774 00a0 0164 06a1 0101 0074 056a  .}.t...d.....t.j
-00001330: 067c 017c 057c 057c 067c 0674 056a 077c  .|.|.|.|.|.t.j.|
-00001340: 0764 078d 077d 0174 087c 017c 006a 0964  .d...}.t.|.|.j.d
-00001350: 088d 027d 017c 0153 0029 097a 6554 6f20  ...}.|.S.).zeTo 
-00001360: 6d61 6b65 2073 7572 6520 7468 6174 2066  make sure that f
-00001370: 7261 6d65 7320 616c 6967 6e20 7765 6c6c  rames align well
-00001380: 2c20 7363 616c 6520 7468 656d 2061 6c6c  , scale them all
-00001390: 2074 6f20 7468 756d 626e 6169 6c73 0a20   to thumbnails. 
-000013a0: 2020 2020 2020 2073 7175 6172 6573 2077         squares w
-000013b0: 6974 6820 626c 6163 6b20 626f 7264 6572  ith black border
-000013c0: 732e 7a0f 7265 7369 7a69 6e67 2073 7175  s.z.resizing squ
-000013d0: 6172 6572 0100 0000 7245 0000 0072 2c00  arer....rE...r,.
-000013e0: 0000 2903 7201 0000 0072 0100 0000 7201  ..).r....r....r.
-000013f0: 0000 007a 1361 626f 7574 2074 6f20 7061  ...z.about to pa
-00001400: 6420 626f 7264 6572 2901 7233 0000 0029  d border).r3...)
-00001410: 01da 0a6e 6577 5f68 6569 6768 7429 0a72  ...new_height).r
-00001420: 2100 0000 723c 0000 00da 0573 6861 7065  !...r<.....shape
-00001430: 722e 0000 0072 6200 0000 7254 0000 00da  r....rb...rT....
-00001440: 0e63 6f70 794d 616b 6542 6f72 6465 72da  .copyMakeBorder.
-00001450: 0f42 4f52 4445 525f 434f 4e53 5441 4e54  .BORDER_CONSTANT
-00001460: da06 7265 7369 7a65 720c 0000 0029 0872  ..resizer....).r
-00001470: 1600 0000 7240 0000 00da 0668 6569 6768  ....r@.....heigh
-00001480: 74da 0577 6964 7468 da0b 7061 6464 6564  t..width..padded
-00001490: 5f73 697a 65da 0a68 6569 6768 745f 7061  _size..height_pa
-000014a0: 64da 0977 6964 7468 5f70 6164 da09 7061  d..width_pad..pa
-000014b0: 645f 636f 6c6f 7272 1700 0000 7217 0000  d_colorr....r...
-000014c0: 0072 1800 0000 da10 7265 7369 7a65 5f74  .r......resize_t
-000014d0: 6f5f 7371 7561 7265 9b00 0000 7326 0000  o_square....s&..
-000014e0: 000a 030a 020a 010a 0210 0210 0108 010a  ................
-000014f0: 0204 0102 0102 0102 0102 0102 0104 0102  ................
-00001500: 0106 f90e 0a04 017a 2350 6169 7265 6446  .......z#PairedF
-00001510: 7261 6d65 4275 696c 6465 722e 7265 7369  rameBuilder.resi
-00001520: 7a65 5f74 6f5f 7371 7561 7265 6303 0000  ze_to_squarec...
-00001530: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00001540: 0043 0000 0073 6c00 0000 7c00 6a00 6a01  .C...sl...|.j.j.
-00001550: 7c02 1900 6a02 6a03 7d03 7c03 6401 6b02  |...j.j.}.|.d.k.
-00001560: 720f 0900 7c01 5300 7c03 6402 7600 721c  r...|.S.|.d.v.r.
-00001570: 7404 a005 7c01 7404 6a06 a102 7d01 7c01  t...|.t.j...}.|.
-00001580: 5300 7c03 6403 7600 7229 7404 a005 7c01  S.|.d.v.r)t...|.
-00001590: 7404 6a07 a102 7d01 7c01 5300 7c03 6404  t.j...}.|.S.|.d.
-000015a0: 7600 7234 7404 a005 7c01 7404 6a08 a102  v.r4t...|.t.j...
-000015b0: 7d01 7c01 5300 2905 4e72 0100 0000 2902  }.|.S.).Nr....).
-000015c0: 7245 0000 00e9 fdff ffff 2902 722c 0000  rE........).r,..
-000015d0: 00e9 feff ffff 2902 e9ff ffff ff72 3800  ......)......r8.
-000015e0: 0000 2909 720b 0000 00da 0773 7472 6561  ..).r......strea
-000015f0: 6d73 da06 6361 6d65 7261 da0e 726f 7461  ms..camera..rota
-00001600: 7469 6f6e 5f63 6f75 6e74 7254 0000 00da  tion_countrT....
-00001610: 0672 6f74 6174 65da 1352 4f54 4154 455f  .rotate..ROTATE_
-00001620: 3930 5f43 4c4f 434b 5749 5345 da0a 524f  90_CLOCKWISE..RO
-00001630: 5441 5445 5f31 3830 da1a 524f 5441 5445  TATE_180..ROTATE
-00001640: 5f39 305f 434f 554e 5445 5243 4c4f 434b  _90_COUNTERCLOCK
-00001650: 5749 5345 2904 7216 0000 0072 4000 0000  WISE).r....r@...
-00001660: 7241 0000 0072 7600 0000 7217 0000 0072  rA...rv...r....r
-00001670: 1700 0000 7218 0000 00da 0e61 7070 6c79  ....r......apply
-00001680: 5f72 6f74 6174 696f 6eb8 0000 0073 1a00  _rotation....s..
-00001690: 0000 1002 0803 0201 0408 08f9 0e01 0406  ................
-000016a0: 08fb 0e01 0404 08fd 0e01 0402 7a21 5061  ............z!Pa
-000016b0: 6972 6564 4672 616d 6542 7569 6c64 6572  iredFrameBuilder
-000016c0: 2e61 7070 6c79 5f72 6f74 6174 696f 6e63  .apply_rotationc
-000016d0: 0300 0000 0000 0000 0000 0000 0800 0000  ................
-000016e0: 0900 0000 4300 0000 734e 0100 007c 015c  ....C...sN...|.\
-000016f0: 027d 037d 0474 00a0 0164 01a1 0101 007c  .}.}.t...d.....|
-00001700: 00a0 027c 03a1 017d 057c 00a0 027c 04a1  ...|...}.|...|..
-00001710: 017d 067c 00a0 037c 057c 037c 067c 04a1  .}.|...|.|.|.|..
-00001720: 045c 027d 057d 067c 00a0 047c 057c 037c  .\.}.}.|...|.|.|
-00001730: 067c 04a1 045c 027d 057d 067c 00a0 057c  .|...\.}.}.|...|
-00001740: 05a1 017d 057c 00a0 057c 06a1 017d 067c  ...}.|...|...}.|
-00001750: 00a0 067c 057c 03a1 027d 057c 00a0 067c  ...|.|...}.|...|
-00001760: 067c 04a1 027d 0674 07a0 087c 0564 02a1  .|...}.t...|.d..
-00001770: 027d 0574 07a0 087c 0664 02a1 027d 0674  .}.t...|.d...}.t
-00001780: 076a 097c 0574 0a7c 0383 0174 0b7c 056a  .j.|.t.|...t.|.j
-00001790: 0c64 0219 0064 031b 0083 0174 0b7c 006a  .d...d.....t.|.j
-000017a0: 0d64 041b 0083 0166 0274 076a 0e64 0264  .d.....f.t.j.d.d
-000017b0: 0564 0364 068d 077d 0574 076a 097c 0674  .d.d...}.t.j.|.t
-000017c0: 0a7c 0483 0174 0b7c 066a 0c64 0219 0064  .|...t.|.j.d...d
-000017d0: 031b 0083 0174 0b7c 006a 0d64 041b 0083  .....t.|.j.d....
-000017e0: 0166 0274 076a 0e64 0264 0564 0364 068d  .f.t.j.d.d.d.d..
-000017f0: 077d 0674 0fa0 107c 057c 0666 02a1 017d  .}.t...|.|.f...}
-00001800: 0774 076a 097c 0774 0a7c 0283 017c 006a  .t.j.|.t.|...|.j
-00001810: 0d64 0718 0074 0b7c 006a 0d64 0414 0064  .d...t.|.j.d...d
-00001820: 081b 0083 0166 0274 076a 0e64 0264 0564  .....f.t.j.d.d.d
-00001830: 0364 068d 077d 077c 0753 0029 097a 3d70  .d...}.|.S.).z=p
-00001840: 6c61 6365 2070 6169 7265 6420 6672 616d  lace paired fram
-00001850: 6573 2073 6964 6520 6279 2073 6964 6520  es side by side 
-00001860: 7769 7468 2061 6e20 696e 666f 2062 6f78  with an info box
-00001870: 2074 6f20 7468 6520 6c65 6674 7a23 486f   to the leftz#Ho
-00001880: 7269 7a6f 6e74 616c 6c79 2073 7461 636b  rizontally stack
-00001890: 696e 6720 7061 6972 6564 2066 7261 6d65  ing paired frame
-000018a0: 7372 4500 0000 722c 0000 0072 0700 0000  srE...r,...r....
-000018b0: 2903 7201 0000 0072 0100 0000 7260 0000  ).r....r....r`..
-000018c0: 00a9 045a 0866 6f6e 7446 6163 655a 0966  ...Z.fontFaceZ.f
-000018d0: 6f6e 7453 6361 6c65 da05 636f 6c6f 72da  ontScale..color.
-000018e0: 0974 6869 636b 6e65 7373 e916 0000 0072  .thickness.....r
-000018f0: 4600 0000 2911 7221 0000 0072 3c00 0000  F...).r!...r<...
-00001900: 7244 0000 0072 6400 0000 725e 0000 0072  rD...rd...r^...r
-00001910: 7000 0000 727b 0000 0072 5400 0000 da04  p...r{...rT.....
-00001920: 666c 6970 da07 7075 7454 6578 74da 0373  flip..putText..s
-00001930: 7472 7262 0000 0072 6600 0000 720c 0000  trrb...rf...r...
-00001940: 00da 1446 4f4e 545f 4845 5253 4845 595f  ...FONT_HERSHEY_
-00001950: 5349 4d50 4c45 5872 3d00 0000 da06 6873  SIMPLEXr=.....hs
-00001960: 7461 636b 2908 7216 0000 0072 1d00 0000  tack).r....r....
-00001970: da0b 626f 6172 645f 636f 756e 7472 5700  ..board_countrW.
-00001980: 0000 7259 0000 0072 5600 0000 7258 0000  ..rY...rV...rX..
-00001990: 005a 0d68 7374 6163 6b65 645f 7061 6972  .Z.hstacked_pair
-000019a0: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-000019b0: 0d68 7374 6163 6b5f 6672 616d 6573 c800  .hstack_frames..
-000019c0: 0000 734e 0000 0008 030a 010a 010a 0114  ..sN............
-000019d0: 0314 010a 020a 010c 020c 010c 020c 0106  ................
-000019e0: 0206 011e 0104 0102 0102 0102 0106 fa06  ................
-000019f0: 0906 011e 0104 0102 0102 0102 0106 fa0e  ................
-00001a00: 0a04 0202 0106 011a 0104 0102 0102 0102  ................
-00001a10: 0106 f904 0b7a 2050 6169 7265 6446 7261  .....z PairedFra
-00001a20: 6d65 4275 696c 6465 722e 6873 7461 636b  meBuilder.hstack
-00001a30: 5f66 7261 6d65 7363 0100 0000 0000 0000  _framesc........
-00001a40: 0000 0000 0400 0000 0900 0000 4300 0000  ............C...
-00001a50: 735c 0000 0074 007c 006a 0183 017d 0164  s\...t.|.j...}.d
-00001a60: 017d 0174 007c 006a 0164 0214 0083 017d  .}.t.|.j.d.....}
-00001a70: 0274 02a0 037c 017c 0264 0366 0374 026a  .t...|.|.d.f.t.j
-00001a80: 04a1 027d 0374 056a 067c 0364 0464 0574  ...}.t.j.|.d.d.t
-00001a90: 007c 006a 0164 061b 0083 0166 0274 056a  .|.j.d.....f.t.j
-00001aa0: 0764 0164 0764 0164 088d 077d 037c 0353  .d.d.d.d...}.|.S
-00001ab0: 0029 094e 7245 0000 0067 0000 0000 0000  .).NrE...g......
-00001ac0: 0440 7238 0000 00da 00e9 1400 0000 722c  .@r8..........r,
-00001ad0: 0000 0072 5f00 0000 727c 0000 0029 0872  ...r_...r|...).r
-00001ae0: 6200 0000 720c 0000 0072 3d00 0000 723e  b...r....r=...r>
-00001af0: 0000 0072 3f00 0000 7254 0000 0072 8100  ...r?...rT...r..
-00001b00: 0000 7283 0000 0029 0472 1600 0000 726a  ..r....).r....rj
-00001b10: 0000 0072 6b00 0000 da05 626c 616e 6b72  ...rk.....blankr
-00001b20: 1700 0000 7217 0000 0072 1800 0000 da14  ....r....r......
-00001b30: 6765 745f 636f 6d70 6c65 7469 6f6e 5f66  get_completion_f
-00001b40: 7261 6d65 0001 0000 731c 0000 000a 0104  rame....s.......
-00001b50: 010e 0214 0204 0202 0102 0110 0104 0102  ................
-00001b60: 0102 0102 0106 f904 0a7a 2750 6169 7265  .........z'Paire
-00001b70: 6446 7261 6d65 4275 696c 6465 722e 6765  dFrameBuilder.ge
-00001b80: 745f 636f 6d70 6c65 7469 6f6e 5f66 7261  t_completion_fra
-00001b90: 6d65 6301 0000 0000 0000 0000 0000 0005  mec.............
-00001ba0: 0000 0008 0000 0043 0000 0073 9000 0000  .......C...s....
-00001bb0: 7c00 6a00 a001 a100 0100 7c00 6a02 6a03  |.j.......|.j.j.
-00001bc0: 7c00 5f03 6401 7d01 6402 7d02 7c00 6a04  |._.d.}.d.}.|.j.
-00001bd0: 4400 5d26 7d03 7c00 6a05 7c03 1900 7d04  D.]&}.|.j.|...}.
-00001be0: 7c04 7c00 6a06 6403 1800 6b04 7221 6404  |.|.j.d...k.r!d.
-00001bf0: 7d02 7c01 6401 7500 722c 7c00 a007 7c03  }.|.d.u.r,|...|.
-00001c00: 7c04 a102 7d01 7111 7408 a009 7c01 7c00  |...}.q.t...|.|.
-00001c10: a007 7c03 7c04 a102 6702 a101 7d01 7111  ..|.|...g...}.q.
-00001c20: 7c02 723e 7c00 a00a a100 0100 7c01 6401  |.r>|.......|.d.
-00001c30: 7500 7246 7c00 a00b a100 7d01 7c01 5300  u.rF|.....}.|.S.
-00001c40: 2905 7a63 0a20 2020 2020 2020 2054 6869  ).zc.        Thi
-00001c50: 7320 676c 7565 7320 746f 6765 7468 6572  s glues together
-00001c60: 2074 6865 2073 7465 7265 6f70 6169 7273   the stereopairs
-00001c70: 2077 6974 6820 7375 6d6d 6172 7920 626c   with summary bl
-00001c80: 6f63 6b73 206f 6620 7468 6520 636f 6d6d  ocks of the comm
-00001c90: 6f6e 2062 6f61 7264 2063 6f75 6e74 0a20  on board count. 
-00001ca0: 2020 2020 2020 204e 4672 4500 0000 5429         NFrE...T)
-00001cb0: 0c72 1200 0000 7236 0000 0072 0b00 0000  .r....r6...r....
-00001cc0: 723a 0000 0072 2500 0000 7223 0000 0072  r:...r%...r#...r
-00001cd0: 0d00 0000 7286 0000 0072 3d00 0000 da06  ....r....r=.....
-00001ce0: 7673 7461 636b 7237 0000 0072 8a00 0000  vstackr7...r....
-00001cf0: 2905 7216 0000 00da 0c73 7465 7265 6f5f  ).r......stereo_
-00001d00: 6672 616d 655a 1462 6f61 7264 5f74 6172  frameZ.board_tar
-00001d10: 6765 745f 7265 6163 6865 6472 1d00 0000  get_reachedr....
-00001d20: 7285 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-00001d30: 1800 0000 da10 6765 745f 7374 6572 656f  ......get_stereo
-00001d40: 5f66 7261 6d65 1401 0000 7324 0000 000a  _frame....s$....
-00001d50: 050a 0104 0204 010a 010a 030e 0104 0108  ................
-00001d60: 020e 0104 020e 0106 ff04 0408 0108 0208  ................
-00001d70: 0104 017a 2350 6169 7265 6446 7261 6d65  ...z#PairedFrame
-00001d80: 4275 696c 6465 722e 6765 745f 7374 6572  Builder.get_ster
-00001d90: 656f 5f66 7261 6d65 da06 7265 7475 726e  eo_frame..return
-00001da0: 6302 0000 0000 0000 0000 0000 000f 0000  c...............
-00001db0: 0008 0000 0003 0000 0073 2e01 0000 7c00  .........s....|.
-00001dc0: 6a00 a001 a100 7d02 6401 6402 8400 7c02  j.....}.d.d...|.
-00001dd0: a002 a100 4400 8301 7d03 7c02 a003 7c03  ....D...}.|...|.
-00001de0: a101 0100 6403 7d04 7404 7405 7c02 7c01  ....d.}.t.t.|.|.
-00001df0: 8302 0400 7d05 8301 7c04 6b03 7289 7404  ....}...|.k.r.t.
-00001e00: 7c05 8301 7d04 7c05 4400 5d57 7d06 7c06  |...}.|.D.]W}.|.
-00001e10: 6404 1900 8900 7c06 6405 1900 8901 8700  d.....|.d.......
-00001e20: 6601 6406 6407 8408 7c02 a006 a100 4400  f.d.d...|.....D.
-00001e30: 8301 7d07 8701 6601 6408 6407 8408 7c02  ..}...f.d.d...|.
-00001e40: a006 a100 4400 8301 7d08 6400 7d09 7c07  ....D...}.d.}.|.
-00001e50: 4400 5d32 7d0a 7c08 4400 5d2d 7d0b 7c0a  D.]2}.|.D.]-}.|.
-00001e60: 6405 1900 7c0b 6404 1900 6b02 727b 7c02  d...|.d...k.r{|.
-00001e70: 7c0a 1900 7d0c 7c02 7c0b 1900 7d0d 7c0c  |...}.|.|...}.|.
-00001e80: 7c01 6b04 727b 7c0d 7c01 6b04 727b 7407  |.k.r{|.|.k.r{t.
-00001e90: 7c0c 7c0d 8302 7d09 7c09 7c02 7c06 3c00  |.|...}.|.|.|.<.
-00001ea0: 7c09 7c02 7c06 6405 1900 7c06 6404 1900  |.|.|.d...|.d...
-00001eb0: 6602 3c00 714e 714a 7126 7404 7405 7c02  f.<.qNqJq&t.t.|.
-00001ec0: 7c01 8302 0400 7d05 8301 7c04 6b03 7320  |.....}...|.k.s 
-00001ed0: 7404 7c05 8301 6404 6b04 7293 6409 7d0e  t.|...d.k.r.d.}.
-00001ee0: 7c0e 5300 640a 7d0e 7c0e 5300 290b 4e63  |.S.d.}.|.S.).Nc
-00001ef0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001f00: 0500 0000 5300 0000 731e 0000 0069 007c  ....S...s....i.|
-00001f10: 005d 0b5c 027d 017d 0274 0074 017c 0183  .].\.}.}.t.t.|..
-00001f20: 0183 017c 0293 0271 0253 0072 1700 0000  ...|...q.S.r....
-00001f30: 2902 da05 7475 706c 65da 0872 6576 6572  )...tuple..rever
-00001f40: 7365 6472 3100 0000 7217 0000 0072 1700  sedr1...r....r..
-00001f50: 0000 7218 0000 0072 1e00 0000 3a01 0000  ..r....r....:...
-00001f60: 7302 0000 001e 007a 4350 6169 7265 6446  s......zCPairedF
-00001f70: 7261 6d65 4275 696c 6465 722e 706f 7373  rameBuilder.poss
-00001f80: 6962 6c65 5f74 6f5f 696e 6974 6961 6c69  ible_to_initiali
-00001f90: 7a65 5f61 7272 6179 2e3c 6c6f 6361 6c73  ze_array.<locals
-00001fa0: 3e2e 3c64 6963 7463 6f6d 703e 7273 0000  >.<dictcomp>rs..
-00001fb0: 0072 0100 0000 7245 0000 0063 0100 0000  .r....rE...c....
-00001fc0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001fd0: 1300 0000 f31c 0000 0067 007c 005d 0a7d  .........g.|.].}
-00001fe0: 017c 0164 0019 0088 006b 0272 027c 0191  .|.d.....k.r.|..
-00001ff0: 0271 0253 0072 1a00 0000 7217 0000 0072  .q.S.r....r....r
-00002000: 1b00 0000 2901 da06 706f 7274 5f41 7217  ....)...port_Ar.
-00002010: 0000 0072 1800 0000 722b 0000 0049 0100  ...r....r+...I..
-00002020: 00f3 0200 0000 1c00 7a43 5061 6972 6564  ........zCPaired
-00002030: 4672 616d 6542 7569 6c64 6572 2e70 6f73  FrameBuilder.pos
-00002040: 7369 626c 655f 746f 5f69 6e69 7469 616c  sible_to_initial
-00002050: 697a 655f 6172 7261 792e 3c6c 6f63 616c  ize_array.<local
-00002060: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-00002070: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00002080: 0000 1300 0000 7291 0000 0029 0172 4500  ......r....).rE.
-00002090: 0000 7217 0000 0072 1b00 0000 2901 da06  ..r....r....)...
-000020a0: 706f 7274 5f43 7217 0000 0072 1800 0000  port_Cr....r....
-000020b0: 722b 0000 004a 0100 0072 9300 0000 4654  r+...J...r....FT
-000020c0: 2908 7223 0000 0072 2400 0000 7235 0000  ).r#...r$...r5..
-000020d0: 00da 0675 7064 6174 6572 4d00 0000 da0f  ...updaterM.....
-000020e0: 6765 745f 656d 7074 795f 7061 6972 73da  get_empty_pairs.
-000020f0: 046b 6579 7372 2d00 0000 290f 7216 0000  .keysr-...).r...
-00002100: 00da 0d6d 696e 5f74 6872 6573 686f 6c64  ...min_threshold
-00002110: 5a14 776f 726b 696e 675f 626f 6172 645f  Z.working_board_
-00002120: 636f 756e 7473 5a14 666c 6970 7065 645f  countsZ.flipped_
-00002130: 626f 6172 645f 636f 756e 7473 5a16 656d  board_countsZ.em
-00002140: 7074 795f 636f 756e 745f 6c61 7374 5f63  pty_count_last_c
-00002150: 7963 6c65 da0b 656d 7074 795f 7061 6972  ycle..empty_pair
-00002160: 7372 1d00 0000 da0d 616c 6c5f 7061 6972  sr......all_pair
-00002170: 735f 415f 58da 0d61 6c6c 5f70 6169 7273  s_A_X..all_pairs
-00002180: 5f58 5f43 5a0f 626f 6172 645f 636f 756e  _X_CZ.board_coun
-00002190: 745f 415f 43da 0870 6169 725f 415f 58da  t_A_C..pair_A_X.
-000021a0: 0870 6169 725f 585f 435a 0f62 6f61 7264  .pair_X_CZ.board
-000021b0: 5f63 6f75 6e74 5f41 5f58 5a0f 626f 6172  _count_A_XZ.boar
-000021c0: 645f 636f 756e 745f 585f 435a 0b69 735f  d_count_X_CZ.is_
-000021d0: 706f 7373 6962 6c65 7217 0000 0029 0272  possibler....).r
-000021e0: 9200 0000 7294 0000 0072 1800 0000 da1c  ....r....r......
-000021f0: 706f 7373 6962 6c65 5f74 6f5f 696e 6974  possible_to_init
-00002200: 6961 6c69 7a65 5f61 7272 6179 3601 0000  ialize_array6...
-00002210: 733c 0000 000a 0312 010a 0104 0216 0208  s<..............
-00002220: 0308 0208 0208 0116 0216 0104 0208 0208  ................
-00002230: 0110 0108 0208 0110 020a 0108 0114 0102  ................
-00002240: 8002 f702 ff16 f10c 1b04 0104 0404 fe04  ................
-00002250: 027a 2f50 6169 7265 6446 7261 6d65 4275  .z/PairedFrameBu
-00002260: 696c 6465 722e 706f 7373 6962 6c65 5f74  ilder.possible_t
-00002270: 6f5f 696e 6974 6961 6c69 7a65 5f61 7272  o_initialize_arr
-00002280: 6179 4e29 0272 0900 0000 720a 0000 0029  ayN).r....r....)
-00002290: 13da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000022a0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000022b0: 616d 655f 5f72 0300 0000 7219 0000 0072  ame__r....r....r
-000022c0: 1500 0000 722a 0000 0072 1000 0000 7237  ....r*...r....r7
-000022d0: 0000 0072 4400 0000 725e 0000 0072 6400  ...rD...r^...rd.
-000022e0: 0000 7270 0000 0072 7b00 0000 7286 0000  ..rp...r{...r...
-000022f0: 0072 8a00 0000 728d 0000 00da 0462 6f6f  .r....r......boo
-00002300: 6c72 9e00 0000 7217 0000 0072 1700 0000  lr....r....r....
-00002310: 7217 0000 0072 1800 0000 7208 0000 0010  r....r....r.....
-00002320: 0000 0073 1e00 0000 0800 1001 0819 0807  ...s............
-00002330: 0804 080a 0808 080e 0837 080f 081d 0810  .........7......
-00002340: 0838 0814 1222 7208 0000 0063 0200 0000  .8..."r....c....
-00002350: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00002360: 0300 0000 731a 0000 0087 0066 0164 0164  ....s......f.d.d
-00002370: 0284 087c 00a0 00a1 0044 0083 017d 027c  ...|.....D...}.|
-00002380: 0253 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-00002390: 0000 0003 0000 0004 0000 0013 0000 0073  ...............s
-000023a0: 1c00 0000 6700 7c00 5d0a 5c02 7d01 7d02  ....g.|.].\.}.}.
-000023b0: 7c02 8800 6b00 7202 7c01 9102 7102 5300  |...k.r.|...q.S.
-000023c0: 7217 0000 0072 1700 0000 7231 0000 00a9  r....r....r1....
-000023d0: 0172 9800 0000 7217 0000 0072 1800 0000  .r....r....r....
-000023e0: 722b 0000 0063 0100 0072 9300 0000 7a23  r+...c...r....z#
-000023f0: 6765 745f 656d 7074 795f 7061 6972 732e  get_empty_pairs.
-00002400: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00002410: 6d70 3e29 0172 3500 0000 2903 7223 0000  mp>).r5...).r#..
-00002420: 0072 9800 0000 7299 0000 0072 1700 0000  .r....r....r....
-00002430: 72a3 0000 0072 1800 0000 7296 0000 0062  r....r....r....b
-00002440: 0100 0073 0400 0000 1601 0401 7296 0000  ...s........r...
-00002450: 0063 0200 0000 0000 0000 0000 0000 0700  .c..............
-00002460: 0000 0500 0000 4300 0000 7344 0000 007c  ......C...sD...|
-00002470: 006a 0064 0064 0185 0219 005c 027d 027d  .j.d.d.....\.}.}
-00002480: 037c 0174 017c 0283 011b 007d 0474 027c  .|.t.|.....}.t.|
-00002490: 037c 0414 0083 017c 0166 027d 0574 036a  .|.....|.f.}.t.j
-000024a0: 047c 007c 0574 036a 0564 028d 037d 067c  .|.|.t.j.d...}.|
-000024b0: 0653 0029 034e 722c 0000 0029 01da 0d69  .S.).Nr,...)...i
-000024c0: 6e74 6572 706f 6c61 7469 6f6e 2906 7266  nterpolation).rf
-000024d0: 0000 0072 5300 0000 7262 0000 0072 5400  ...rS...rb...rT.
-000024e0: 0000 7269 0000 00da 0a49 4e54 4552 5f41  ..ri.....INTER_A
-000024f0: 5245 4129 07da 0569 6d61 6765 7265 0000  REA)...imagere..
-00002500: 005a 0e63 7572 7265 6e74 5f68 6569 6768  .Z.current_heigh
-00002510: 745a 0d63 7572 7265 6e74 5f77 6964 7468  tZ.current_width
-00002520: da05 7261 7469 6fda 0364 696d 5a07 7265  ..ratio..dimZ.re
-00002530: 7369 7a65 6472 1700 0000 7217 0000 0072  sizedr....r....r
-00002540: 1800 0000 7269 0000 0066 0100 0073 0a00  ....ri...f...s..
-00002550: 0000 1201 0c01 1001 1201 0401 7269 0000  ............ri..
-00002560: 0029 16da 0d70 7978 7933 642e 6c6f 6767  .)...pyxy3d.logg
-00002570: 6572 da06 7079 7879 3364 7221 0000 0072  er..pyxy3dr!...r
-00002580: 3600 0000 729f 0000 00da 0770 6174 686c  6...r......pathl
-00002590: 6962 7202 0000 0072 5400 0000 da05 6e75  ibr....rT.....nu
-000025a0: 6d70 7972 3d00 0000 da1b 7079 7879 3364  mpyr=.....pyxy3d
-000025b0: 2e63 616d 6572 6173 2e73 796e 6368 726f  .cameras.synchro
-000025c0: 6e69 7a65 7272 0300 0000 da09 6974 6572  nizerr......iter
-000025d0: 746f 6f6c 7372 0400 0000 da05 7175 6575  toolsr......queu
-000025e0: 6572 0500 0000 da09 7468 7265 6164 696e  er......threadin
-000025f0: 6772 0600 0000 720e 0000 0072 0800 0000  gr....r....r....
-00002600: 7296 0000 0072 6900 0000 7217 0000 0072  r....ri...r....r
-00002610: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
-00002620: 3c6d 6f64 756c 653e 0100 0000 731e 0000  <module>....s...
-00002630: 0008 000c 010c 0208 0208 010c 020c 010c  ................
-00002640: 010c 0104 020e 0200 7f00 7f08 540c 04    ............T..
+00000180: 0e64 1a64 1b84 005a 0f64 1c65 1066 0264  .d.d...Z.d.e.f.d
+00000190: 1d64 1e84 045a 1164 1f53 0029 21da 1250  .d...Z.d.S.)!..P
+000001a0: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
+000001b0: 72e9 fa00 0000 e932 0000 00da 0c73 796e  r......2.....syn
+000001c0: 6368 726f 6e69 7a65 7263 0400 0000 0000  chronizerc......
+000001d0: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
+000001e0: 0000 7388 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
+000001f0: 005f 017c 037c 005f 0274 037c 005f 047c  ._.|.|._.t.|._.|
+00000200: 00a0 05a1 007c 005f 0674 0783 007c 005f  .....|._.t...|._
+00000210: 087c 006a 00a0 097c 006a 08a1 0101 0074  .|.j...|.j.....t
+00000220: 0a83 007c 005f 0b74 0ca0 0d64 01a1 0101  ...|._.t...d....
+00000230: 0064 0264 0384 007c 006a 0644 0083 017c  .d.d...|.j.D...|
+00000240: 005f 0e7c 006a 06a0 0fa1 007c 005f 1064  ._.|.j.....|._.d
+00000250: 0464 0384 007c 006a 0644 0083 017c 005f  .d...|.j.D...|._
+00000260: 117c 006a 0ba0 12a1 0001 0064 0053 0029  .|.j.......d.S.)
+00000270: 054e 7a17 5265 7365 7474 696e 6720 4672  .Nz.Resetting Fr
+00000280: 616d 6520 4275 696c 6465 7263 0100 0000  ame Builderc....
+00000290: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000002a0: 5300 0000 7312 0000 0069 007c 005d 057d  S...s....i.|.].}
+000002b0: 017c 0164 0093 0271 0253 00a9 0172 0100  .|.d...q.S...r..
+000002c0: 0000 a900 a902 da02 2e30 da04 7061 6972  .........0..pair
+000002d0: 720d 0000 0072 0d00 0000 fa52 433a 5c55  r....r.....RC:\U
+000002e0: 7365 7273 5c4d 6163 2050 7269 626c 655c  sers\Mac Prible\
+000002f0: 7265 706f 735c 7079 7879 3364 5c70 7978  repos\pyxy3d\pyx
+00000300: 7933 645c 6775 695c 6672 616d 655f 6275  y3d\gui\frame_bu
+00000310: 696c 6465 7273 5c70 6169 7265 645f 6672  ilders\paired_fr
+00000320: 616d 655f 6275 696c 6465 722e 7079 da0a  ame_builder.py..
+00000330: 3c64 6963 7463 6f6d 703e 2500 0000 7302  <dictcomp>%...s.
+00000340: 0000 0012 007a 2f50 6169 7265 6446 7261  .....z/PairedFra
+00000350: 6d65 4275 696c 6465 722e 5f5f 696e 6974  meBuilder.__init
+00000360: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  __.<locals>.<dic
+00000370: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
+00000380: 0000 0002 0000 0006 0000 0053 0000 0073  ...........S...s
+00000390: 1800 0000 6900 7c00 5d08 7d01 7c01 6700  ....i.|.].}.|.g.
+000003a0: 6700 6400 9c02 9302 7102 5300 2901 2902  g.d.....q.S.).).
+000003b0: da09 696d 675f 6c6f 635f 41da 0969 6d67  ..img_loc_A..img
+000003c0: 5f6c 6f63 5f42 720d 0000 0072 0e00 0000  _loc_Br....r....
+000003d0: 720d 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
+000003e0: 1200 0000 2700 0000 7302 0000 0018 0029  ....'...s......)
+000003f0: 1372 0b00 0000 da13 7369 6e67 6c65 5f66  .r......single_f
+00000400: 7261 6d65 5f68 6569 6768 74da 1262 6f61  rame_height..boa
+00000410: 7264 5f63 6f75 6e74 5f74 6172 6765 74da  rd_count_target.
+00000420: 1443 4f4d 4d4f 4e5f 434f 524e 4552 5f54  .COMMON_CORNER_T
+00000430: 4152 4745 54da 1463 6f6d 6d6f 6e5f 636f  ARGET..common_co
+00000440: 726e 6572 5f74 6172 6765 74da 0967 6574  rner_target..get
+00000450: 5f70 6169 7273 da05 7061 6972 7372 0500  _pairs..pairsr..
+00000460: 0000 da16 6e65 775f 7379 6e63 5f70 6163  ....new_sync_pac
+00000470: 6b65 745f 6e6f 7469 6365 da13 7375 6273  ket_notice..subs
+00000480: 6372 6962 655f 746f 5f6e 6f74 6963 6572  cribe_to_noticer
+00000490: 0600 0000 da0c 7374 6f72 655f 706f 696e  ......store_poin
+000004a0: 7473 da06 6c6f 6767 6572 da04 696e 666f  ts..logger..info
+000004b0: da0c 626f 6172 645f 636f 756e 7473 da04  ..board_counts..
+000004c0: 636f 7079 da0b 7374 6572 656f 5f6c 6973  copy..stereo_lis
+000004d0: 74da 0e73 7465 7265 6f5f 6869 7374 6f72  t..stereo_histor
+000004e0: 79da 0563 6c65 6172 2904 da04 7365 6c66  y..clear)...self
+000004f0: 720b 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000500: 0d00 0000 720d 0000 0072 1100 0000 da08  ....r....r......
+00000510: 5f5f 696e 6974 5f5f 1100 0000 731a 0000  __init__....s...
+00000520: 0006 0106 0106 0306 010a 0708 020e 0108  ................
+00000530: 010a 0212 010c 0112 010e 017a 1b50 6169  ...........z.Pai
+00000540: 7265 6446 7261 6d65 4275 696c 6465 722e  redFrameBuilder.
+00000550: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000560: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000570: 0073 1c00 0000 7400 a001 6401 a101 0100  .s....t...d.....
+00000580: 7c00 6a02 a003 7c00 6a04 a101 0100 6400  |.j...|.j.....d.
+00000590: 5300 2902 4e7a 2c55 6e73 7562 7363 7269  S.).Nz,Unsubscri
+000005a0: 6265 2066 7261 6d65 2062 7569 6c64 6572  be frame builder
+000005b0: 2066 726f 6d20 7379 6e63 6872 6f6e 697a   from synchroniz
+000005c0: 6572 2e29 0572 1e00 0000 721f 0000 0072  er.).r....r....r
+000005d0: 0b00 0000 da15 756e 7375 6273 6372 6962  ......unsubscrib
+000005e0: 655f 746f 5f6e 6f74 6963 6572 1b00 0000  e_to_noticer....
+000005f0: a901 7225 0000 0072 0d00 0000 720d 0000  ..r%...r....r...
+00000600: 0072 1100 0000 da1d 756e 7375 6273 6372  .r......unsubscr
+00000610: 6962 655f 6672 6f6d 5f73 796e 6368 726f  ibe_from_synchro
+00000620: 6e69 7a65 722a 0000 0073 0400 0000 0a01  nizer*...s......
+00000630: 1201 7a30 5061 6972 6564 4672 616d 6542  ..z0PairedFrameB
+00000640: 7569 6c64 6572 2e75 6e73 7562 7363 7269  uilder.unsubscri
+00000650: 6265 5f66 726f 6d5f 7379 6e63 6872 6f6e  be_from_synchron
+00000660: 697a 6572 6301 0000 0000 0000 0000 0000  izerc...........
+00000670: 0003 0000 0004 0000 0043 0000 0073 3200  .........C...s2.
+00000680: 0000 6401 6402 8400 7400 7c00 6a01 6a02  ..d.d...t.|.j.j.
+00000690: 6403 8302 4400 8301 7d01 6404 6402 8400  d...D...}.d.d...
+000006a0: 7c01 4400 8301 7d02 7403 7c02 8301 7d02  |.D...}.t.|...}.
+000006b0: 7c02 5300 2905 4e63 0100 0000 0000 0000  |.S.).Nc........
+000006c0: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+000006d0: 7310 0000 0067 007c 005d 047d 017c 0191  s....g.|.].}.|..
+000006e0: 0271 0253 0072 0d00 0000 720d 0000 0072  .q.S.r....r....r
+000006f0: 0e00 0000 720d 0000 0072 0d00 0000 7211  ....r....r....r.
+00000700: 0000 00da 0a3c 6c69 7374 636f 6d70 3e2f  .....<listcomp>/
+00000710: 0000 0073 0200 0000 1000 7a30 5061 6972  ...s......z0Pair
+00000720: 6564 4672 616d 6542 7569 6c64 6572 2e67  edFrameBuilder.g
+00000730: 6574 5f70 6169 7273 2e3c 6c6f 6361 6c73  et_pairs.<locals
+00000740: 3e2e 3c6c 6973 7463 6f6d 703e e902 0000  >.<listcomp>....
+00000750: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000760: 0000 0500 0000 5300 0000 731c 0000 0067  ......S...s....g
+00000770: 007c 005d 0a7d 0174 007c 0183 0174 017c  .|.].}.t.|...t.|
+00000780: 0183 0166 0291 0271 0253 0072 0d00 0000  ...f...q.S.r....
+00000790: 2902 da03 6d69 6eda 036d 6178 720e 0000  )...min..maxr...
+000007a0: 0072 0d00 0000 720d 0000 0072 1100 0000  .r....r....r....
+000007b0: 722a 0000 0030 0000 0073 0600 0000 0600  r*...0...s......
+000007c0: 1001 06ff 2904 7204 0000 0072 0b00 0000  ....).r....r....
+000007d0: da05 706f 7274 73da 0673 6f72 7465 6429  ..ports..sorted)
+000007e0: 0372 2500 0000 721a 0000 005a 0c73 6f72  .r%...r....Z.sor
+000007f0: 7465 645f 706f 7274 7372 0d00 0000 720d  ted_portsr....r.
+00000800: 0000 0072 1100 0000 7219 0000 002e 0000  ...r....r.......
+00000810: 0073 1000 0000 1801 0601 0201 06ff 0203  .s..............
+00000820: 0201 04ff 0403 7a1c 5061 6972 6564 4672  ......z.PairedFr
+00000830: 616d 6542 7569 6c64 6572 2e67 6574 5f70  ameBuilder.get_p
+00000840: 6169 7273 6301 0000 0000 0000 0000 0000  airsc...........
+00000850: 0001 0000 0005 0000 0003 0000 0073 3400  .............s4.
+00000860: 0000 8700 6601 6401 6402 8408 8800 6a00  ....f.d.d.....j.
+00000870: a001 a100 4400 8301 8800 5f02 7403 8800  ....D....._.t...
+00000880: 6a02 8800 6a00 6a04 6403 6404 8d03 8800  j...j.j.d.d.....
+00000890: 5f02 6400 5300 2905 4e63 0100 0000 0000  _.d.S.).Nc......
+000008a0: 0000 0000 0000 0300 0000 0400 0000 1300  ................
+000008b0: 0000 731e 0000 0067 007c 005d 0b5c 027d  ..s....g.|.].\.}
+000008c0: 017d 027c 0288 006a 006b 0072 027c 0191  .}.|...j.k.r.|..
+000008d0: 0271 0253 0072 0d00 0000 2901 7216 0000  .q.S.r....).r...
+000008e0: 00a9 0372 0f00 0000 da03 6b65 79da 0576  ...r......key..v
+000008f0: 616c 7565 7228 0000 0072 0d00 0000 7211  aluer(...r....r.
+00000900: 0000 0072 2a00 0000 3900 0000 730c 0000  ...r*...9...s...
+00000910: 0006 0006 0208 0102 fd02 0106 ff7a 3950  .............z9P
+00000920: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
+00000930: 722e 7570 6461 7465 5f73 7465 7265 6f5f  r.update_stereo_
+00000940: 6c69 7374 2e3c 6c6f 6361 6c73 3e2e 3c6c  list.<locals>.<l
+00000950: 6973 7463 6f6d 703e 5429 0272 3100 0000  istcomp>T).r1...
+00000960: da07 7265 7665 7273 6529 0572 2000 0000  ..reverse).r ...
+00000970: da05 6974 656d 7372 2200 0000 722f 0000  ..itemsr"...r/..
+00000980: 00da 0367 6574 7228 0000 0072 0d00 0000  ...getr(...r....
+00000990: 7228 0000 0072 1100 0000 da12 7570 6461  r(...r......upda
+000009a0: 7465 5f73 7465 7265 6f5f 6c69 7374 3800  te_stereo_list8.
+000009b0: 0000 7308 0000 000a 0108 0208 fe1a 057a  ..s............z
+000009c0: 2550 6169 7265 6446 7261 6d65 4275 696c  %PairedFrameBuil
+000009d0: 6465 722e 7570 6461 7465 5f73 7465 7265  der.update_stere
+000009e0: 6f5f 6c69 7374 6302 0000 0000 0000 0000  o_listc.........
+000009f0: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
+00000a00: 4c00 0000 7c00 6a00 7d02 7c00 6a01 6a02  L...|.j.}.|.j.j.
+00000a10: 7c01 1900 7d03 7c03 6401 7500 721f 7403  |...}.|.d.u.r.t.
+00000a20: a004 6402 a101 0100 7405 6a06 7c02 7c02  ..d.....t.j.|.|.
+00000a30: 6403 6603 7405 6a07 6404 8d02 7d04 7c04  d.f.t.j.d...}.|.
+00000a40: 5300 7c03 6a08 a009 a100 7d04 7c04 5300  S.|.j.....}.|.S.
+00000a50: 2905 7a7b 5379 6e63 6872 6f6e 697a 6174  ).z{Synchronizat
+00000a60: 696f 6e20 6973 7375 6573 2063 616e 206c  ion issues can l
+00000a70: 6561 6420 746f 2073 6f6d 6520 6672 616d  ead to some fram
+00000a80: 6573 2062 6569 6e67 204e 6f6e 6520 616d  es being None am
+00000a90: 6f6e 670a 2020 2020 2020 2020 7468 6520  ong.        the 
+00000aa0: 7379 6e63 6865 6420 6672 616d 6573 2c20  synched frames, 
+00000ab0: 736f 2070 6c75 6720 7468 6174 2077 6974  so plug that wit
+00000ac0: 6820 6120 626c 616e 6b20 6672 616d 654e  h a blank frameN
+00000ad0: 7a19 706c 7567 6769 6e67 2062 6c61 6e6b  z.plugging blank
+00000ae0: 2066 7261 6d65 2064 6174 61e9 0300 0000   frame data.....
+00000af0: 2901 da05 6474 7970 6529 0a72 1500 0000  )...dtype).r....
+00000b00: da13 6375 7272 656e 745f 7379 6e63 5f70  ..current_sync_p
+00000b10: 6163 6b65 74da 0d66 7261 6d65 5f70 6163  acket..frame_pac
+00000b20: 6b65 7473 721e 0000 00da 0564 6562 7567  ketsr......debug
+00000b30: da02 6e70 da05 7a65 726f 73da 0575 696e  ..np..zeros..uin
+00000b40: 7438 da05 6672 616d 6572 2100 0000 2905  t8..framer!...).
+00000b50: 7225 0000 00da 0470 6f72 74da 0465 6467  r%.....port..edg
+00000b60: 65da 0c66 7261 6d65 5f70 6163 6b65 7472  e..frame_packetr
+00000b70: 3f00 0000 720d 0000 0072 0d00 0000 7211  ?...r....r....r.
+00000b80: 0000 00da 1267 6574 5f66 7261 6d65 5f6f  .....get_frame_o
+00000b90: 725f 626c 616e 6b40 0000 0073 1000 0000  r_blank@...s....
+00000ba0: 0604 0c01 0801 0a01 1601 0404 0afe 0402  ................
+00000bb0: 7a25 5061 6972 6564 4672 616d 6542 7569  z%PairedFrameBui
+00000bc0: 6c64 6572 2e67 6574 5f66 7261 6d65 5f6f  lder.get_frame_o
+00000bd0: 725f 626c 616e 6b63 0500 0000 0000 0000  r_blankc........
+00000be0: 0000 0000 1000 0000 0800 0000 4300 0000  ............C...
+00000bf0: 73c2 0100 007c 006a 006a 017c 0219 0064  s....|.j.j.|...d
+00000c00: 0175 0072 1474 02a0 0364 027c 029b 009d  .u.r.t...d.|....
+00000c10: 02a1 0101 007c 017c 0366 0253 007c 006a  .....|.|.f.S.|.j
+00000c20: 006a 017c 0419 0064 0175 0072 2874 02a0  .j.|...d.u.r(t..
+00000c30: 0364 027c 049b 009d 02a1 0101 007c 017c  .d.|.........|.|
+00000c40: 0366 0253 007c 006a 006a 017c 0219 007d  .f.S.|.j.j.|...}
+00000c50: 057c 006a 006a 017c 0419 007d 067c 056a  .|.j.j.|...}.|.j
+00000c60: 0464 0175 0073 3e7c 066a 0464 0175 0072  .d.u.s>|.j.d.u.r
+00000c70: 427c 017c 0366 0253 007c 056a 046a 057d  B|.|.f.S.|.j.j.}
+00000c80: 077c 066a 046a 057d 0874 06a0 077c 077c  .|.j.j.}.t...|.|
+00000c90: 08a1 027d 097c 056a 046a 087d 0a7c 066a  ...}.|.j.j.}.|.j
+00000ca0: 046a 087d 0b74 097c 0983 017c 006a 0a6b  .j.}.t.|...|.j.k
+00000cb0: 0572 8b7c 006a 0ba0 0ca1 0072 8b7c 006a  .r.|.j.....r.|.j
+00000cc0: 0d7c 027c 0466 0219 0064 0319 00a0 0e7c  .|.|.f...d.....|
+00000cd0: 0aa0 0fa1 00a1 0101 007c 006a 0d7c 027c  .........|.j.|.|
+00000ce0: 0466 0219 0064 0419 00a0 0e7c 0ba0 0fa1  .f...d.....|....
+00000cf0: 00a1 0101 007c 006a 107c 027c 0466 0205  .....|.j.|.|.f..
+00000d00: 0019 0064 0537 0003 003c 0074 117c 077c  ...d.7...<.t.|.|
+00000d10: 0a83 0244 005d 235c 027d 0c7d 0d7c 0c7c  ...D.]#\.}.}.|.|
+00000d20: 0976 0072 b374 1274 137c 0d64 0619 0083  .v.r.t.t.|.d....
+00000d30: 0183 017d 0e74 1274 137c 0d64 0519 0083  ...}.t.t.|.d....
+00000d40: 0183 017d 0f74 14a0 157c 017c 0e7c 0f66  ...}.t...|.|.|.f
+00000d50: 0264 0764 0864 09a1 0501 0071 9074 117c  .d.d.d.....q.t.|
+00000d60: 087c 0b83 0244 005d 235c 027d 0c7d 0d7c  .|...D.]#\.}.}.|
+00000d70: 0c7c 0976 0072 dc74 1274 137c 0d64 0619  .|.v.r.t.t.|.d..
+00000d80: 0083 0183 017d 0e74 1274 137c 0d64 0519  .....}.t.t.|.d..
+00000d90: 0083 0183 017d 0f74 14a0 157c 037c 0e7c  .....}.t...|.|.|
+00000da0: 0f66 0264 0764 0864 09a1 0501 0071 b97c  .f.d.d.d.....q.|
+00000db0: 017c 0366 0253 0029 0a7a cf0a 2020 2020  .|.f.S.).z..    
+00000dc0: 2020 2020 5265 7475 726e 2075 6e61 6c74      Return unalt
+00000dd0: 6572 6564 2066 7261 6d65 2069 6620 6e6f  ered frame if no
+00000de0: 2063 6f72 6e65 7220 696e 666f 726d 6174   corner informat
+00000df0: 696f 6e20 6465 7465 6374 6564 2c20 6f74  ion detected, ot
+00000e00: 6865 7277 6973 650a 2020 2020 2020 2020  herwise.        
+00000e10: 7265 636f 7264 2074 6865 2063 6f72 6e65  record the corne
+00000e20: 7273 2074 6861 7420 6172 6520 7368 6172  rs that are shar
+00000e30: 6564 2062 6574 7765 656e 2074 6865 2074  ed between the t
+00000e40: 776f 2066 7261 6d65 730a 2020 2020 2020  wo frames.      
+00000e50: 2020 616e 6420 7265 7475 726e 2074 776f    and return two
+00000e60: 2066 7261 6d65 7320 7769 7468 2073 6861   frames with sha
+00000e70: 7265 6420 636f 726e 6572 7320 6472 6177  red corners draw
+00000e80: 6e0a 2020 2020 2020 2020 4e7a 1644 726f  n.        Nz.Dro
+00000e90: 7070 6564 2066 7261 6d65 2061 7420 706f  pped frame at po
+00000ea0: 7274 2072 1300 0000 7214 0000 00e9 0100  rt r....r.......
+00000eb0: 0000 7201 0000 00e9 0500 0000 2903 7201  ..r.........).r.
+00000ec0: 0000 0072 0100 0000 e9dc 0000 0072 3700  ...r.........r7.
+00000ed0: 0000 2916 7239 0000 0072 3a00 0000 721e  ..).r9...r:...r.
+00000ee0: 0000 00da 0777 6172 6e69 6e67 da06 706f  .....warning..po
+00000ef0: 696e 7473 da08 706f 696e 745f 6964 723c  ints..point_idr<
+00000f00: 0000 00da 0b69 6e74 6572 7365 6374 3164  .....intersect1d
+00000f10: da07 696d 675f 6c6f 63da 036c 656e 7218  ..img_loc..lenr.
+00000f20: 0000 0072 1d00 0000 da06 6973 5f73 6574  ...r......is_set
+00000f30: 7223 0000 00da 0665 7874 656e 64da 0674  r#.....extend..t
+00000f40: 6f6c 6973 7472 2000 0000 da03 7a69 70da  olistr .....zip.
+00000f50: 0572 6f75 6e64 da05 666c 6f61 74da 0363  .round..float..c
+00000f60: 7632 da06 6369 7263 6c65 2910 7225 0000  v2..circle).r%..
+00000f70: 00da 0666 7261 6d65 41da 0570 6f72 7441  ...frameA..portA
+00000f80: da06 6672 616d 6542 da05 706f 7274 425a  ..frameB..portBZ
+00000f90: 0e66 7261 6d65 5f70 6163 6b65 745f 415a  .frame_packet_AZ
+00000fa0: 0e66 7261 6d65 5f70 6163 6b65 745f 425a  .frame_packet_BZ
+00000fb0: 0569 6473 5f41 5a05 6964 735f 42da 0a63  .ids_AZ.ids_B..c
+00000fc0: 6f6d 6d6f 6e5f 6964 7372 1300 0000 7214  ommon_idsr....r.
+00000fd0: 0000 00da 035f 6964 724b 0000 00da 0178  ....._idrK.....x
+00000fe0: da01 7972 0d00 0000 720d 0000 0072 1100  ..yr....r....r..
+00000ff0: 0000 da1a 6472 6177 5f63 6f6d 6d6f 6e5f  ....draw_common_
+00001000: 636f 726e 6572 5f63 7572 7265 6e74 4e00  corner_currentN.
+00001010: 0000 7340 0000 0010 0710 0108 0110 0210  ..s@............
+00001020: 0108 010c 020c 0114 0208 0108 0208 010c  ................
+00001030: 0108 0208 0118 061c 041c 0116 0112 0208  ................
+00001040: 0110 0110 0116 0202 8012 0208 0110 0110  ................
+00001050: 0116 0202 8008 017a 2d50 6169 7265 6446  .......z-PairedF
+00001060: 7261 6d65 4275 696c 6465 722e 6472 6177  rameBuilder.draw
+00001070: 5f63 6f6d 6d6f 6e5f 636f 726e 6572 5f63  _common_corner_c
+00001080: 7572 7265 6e74 6305 0000 0000 0000 0000  urrentc.........
+00001090: 0000 000a 0000 0009 0000 0043 0000 0073  ...........C...s
+000010a0: 9800 0000 7c02 7c04 6602 7d05 7c00 6a00  ....|.|.f.}.|.j.
+000010b0: 7c05 1900 6401 1900 7d06 7c00 6a00 7c05  |...d...}.|.j.|.
+000010c0: 1900 6402 1900 7d07 7c06 4400 5d18 7d08  ..d...}.|.D.].}.
+000010d0: 7401 7c08 6403 1900 8301 7401 7c08 6404  t.|.d.....t.|.d.
+000010e0: 1900 8301 6602 7d09 7402 a003 7c01 7c09  ....f.}.t...|.|.
+000010f0: 6405 6406 6405 6404 a106 0100 7114 7c07  d.d.d.d.....q.|.
+00001100: 4400 5d18 7d08 7401 7c08 6403 1900 8301  D.].}.t.|.d.....
+00001110: 7401 7c08 6404 1900 8301 6602 7d09 7402  t.|.d.....f.}.t.
+00001120: a003 7c03 7c09 6405 6406 6405 6404 a106  ..|.|.d.d.d.d...
+00001130: 0100 712f 7c01 7c03 6602 5300 2907 4e72  ..q/|.|.f.S.).Nr
+00001140: 1300 0000 7214 0000 0072 0100 0000 7244  ....r....r....rD
+00001150: 0000 0072 2b00 0000 a903 e9ff 0000 00e9  ...r+...........
+00001160: a500 0000 7201 0000 0029 0472 2300 0000  ....r....).r#...
+00001170: da03 696e 7472 5300 0000 7254 0000 0029  ..intrS...rT...)
+00001180: 0a72 2500 0000 7255 0000 0072 5600 0000  .r%...rU...rV...
+00001190: 7257 0000 0072 5800 0000 7210 0000 0072  rW...rX...r....r
+000011a0: 1300 0000 7214 0000 005a 0863 6f6f 7264  ....r....Z.coord
+000011b0: 5f78 79da 0663 6f72 6e65 7272 0d00 0000  _xy..cornerr....
+000011c0: 720d 0000 0072 1100 0000 da1a 6472 6177  r....r......draw
+000011d0: 5f63 6f6d 6d6f 6e5f 636f 726e 6572 5f68  _common_corner_h
+000011e0: 6973 746f 7279 8500 0000 7314 0000 0008  istory....s.....
+000011f0: 010e 010e 0108 0218 0116 0108 0218 0116  ................
+00001200: 0108 027a 2d50 6169 7265 6446 7261 6d65  ...z-PairedFrame
+00001210: 4275 696c 6465 722e 6472 6177 5f63 6f6d  Builder.draw_com
+00001220: 6d6f 6e5f 636f 726e 6572 5f68 6973 746f  mon_corner_histo
+00001230: 7279 6302 0000 0000 0000 0000 0000 0008  ryc.............
+00001240: 0000 0009 0000 0043 0000 0073 8600 0000  .......C...s....
+00001250: 7400 a001 6401 a101 0100 7c01 6a02 6402  t...d.....|.j.d.
+00001260: 1900 7d02 7c01 6a02 6403 1900 7d03 7403  ..}.|.j.d...}.t.
+00001270: 7c02 7c03 8302 7d04 7404 7c04 7c02 1800  |.|...}.t.|.|...
+00001280: 6404 1b00 8301 7d05 7404 7c04 7c03 1800  d.....}.t.|.|...
+00001290: 6404 1b00 8301 7d06 6700 6405 a201 7d07  d.....}.g.d...}.
+000012a0: 7400 a001 6406 a101 0100 7405 6a06 7c01  t...d.....t.j.|.
+000012b0: 7c05 7c05 7c06 7c06 7405 6a07 7c07 6407  |.|.|.|.t.j.|.d.
+000012c0: 8d07 7d01 7408 7c01 7c00 6a09 6408 8d02  ..}.t.|.|.j.d...
+000012d0: 7d01 7c01 5300 2909 7a65 546f 206d 616b  }.|.S.).zeTo mak
+000012e0: 6520 7375 7265 2074 6861 7420 6672 616d  e sure that fram
+000012f0: 6573 2061 6c69 676e 2077 656c 6c2c 2073  es align well, s
+00001300: 6361 6c65 2074 6865 6d20 616c 6c20 746f  cale them all to
+00001310: 2074 6875 6d62 6e61 696c 730a 2020 2020   thumbnails.    
+00001320: 2020 2020 7371 7561 7265 7320 7769 7468      squares with
+00001330: 2062 6c61 636b 2062 6f72 6465 7273 2e7a   black borders.z
+00001340: 0f72 6573 697a 696e 6720 7371 7561 7265  .resizing square
+00001350: 7201 0000 0072 4400 0000 722b 0000 0029  r....rD...r+...)
+00001360: 0372 0100 0000 7201 0000 0072 0100 0000  .r....r....r....
+00001370: 7a13 6162 6f75 7420 746f 2070 6164 2062  z.about to pad b
+00001380: 6f72 6465 7229 0172 3200 0000 2901 da0a  order).r2...)...
+00001390: 6e65 775f 6865 6967 6874 290a 721e 0000  new_height).r...
+000013a0: 0072 3b00 0000 da05 7368 6170 6572 2d00  .r;.....shaper-.
+000013b0: 0000 7261 0000 0072 5300 0000 da0e 636f  ..ra...rS.....co
+000013c0: 7079 4d61 6b65 426f 7264 6572 da0f 424f  pyMakeBorder..BO
+000013d0: 5244 4552 5f43 4f4e 5354 414e 54da 0672  RDER_CONSTANT..r
+000013e0: 6573 697a 6572 1500 0000 2908 7225 0000  esizer....).r%..
+000013f0: 0072 3f00 0000 da06 6865 6967 6874 da05  .r?.....height..
+00001400: 7769 6474 68da 0b70 6164 6465 645f 7369  width..padded_si
+00001410: 7a65 da0a 6865 6967 6874 5f70 6164 da09  ze..height_pad..
+00001420: 7769 6474 685f 7061 64da 0970 6164 5f63  width_pad..pad_c
+00001430: 6f6c 6f72 720d 0000 0072 0d00 0000 7211  olorr....r....r.
+00001440: 0000 00da 1072 6573 697a 655f 746f 5f73  .....resize_to_s
+00001450: 7175 6172 6594 0000 0073 2600 0000 0a03  quare....s&.....
+00001460: 0a02 0a01 0a02 1002 1001 0801 0a02 0401  ................
+00001470: 0201 0201 0201 0201 0201 0401 0201 06f9  ................
+00001480: 0e0a 0401 7a23 5061 6972 6564 4672 616d  ....z#PairedFram
+00001490: 6542 7569 6c64 6572 2e72 6573 697a 655f  eBuilder.resize_
+000014a0: 746f 5f73 7175 6172 6563 0300 0000 0000  to_squarec......
+000014b0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
+000014c0: 0000 736c 0000 007c 006a 006a 017c 0219  ..sl...|.j.j.|..
+000014d0: 006a 026a 037d 037c 0364 016b 0272 0f09  .j.j.}.|.d.k.r..
+000014e0: 007c 0153 007c 0364 0276 0072 1c74 04a0  .|.S.|.d.v.r.t..
+000014f0: 057c 0174 046a 06a1 027d 017c 0153 007c  .|.t.j...}.|.S.|
+00001500: 0364 0376 0072 2974 04a0 057c 0174 046a  .d.v.r)t...|.t.j
+00001510: 07a1 027d 017c 0153 007c 0364 0476 0072  ...}.|.S.|.d.v.r
+00001520: 3474 04a0 057c 0174 046a 08a1 027d 017c  4t...|.t.j...}.|
+00001530: 0153 0029 054e 7201 0000 0029 0272 4400  .S.).Nr....).rD.
+00001540: 0000 e9fd ffff ff29 0272 2b00 0000 e9fe  .......).r+.....
+00001550: ffff ff29 02e9 ffff ffff 7237 0000 0029  ...)......r7...)
+00001560: 0972 0b00 0000 da07 7374 7265 616d 73da  .r......streams.
+00001570: 0663 616d 6572 61da 0e72 6f74 6174 696f  .camera..rotatio
+00001580: 6e5f 636f 756e 7472 5300 0000 da06 726f  n_countrS.....ro
+00001590: 7461 7465 da13 524f 5441 5445 5f39 305f  tate..ROTATE_90_
+000015a0: 434c 4f43 4b57 4953 45da 0a52 4f54 4154  CLOCKWISE..ROTAT
+000015b0: 455f 3138 30da 1a52 4f54 4154 455f 3930  E_180..ROTATE_90
+000015c0: 5f43 4f55 4e54 4552 434c 4f43 4b57 4953  _COUNTERCLOCKWIS
+000015d0: 4529 0472 2500 0000 723f 0000 0072 4000  E).r%...r?...r@.
+000015e0: 0000 7275 0000 0072 0d00 0000 720d 0000  ..ru...r....r...
+000015f0: 0072 1100 0000 da0e 6170 706c 795f 726f  .r......apply_ro
+00001600: 7461 7469 6f6e b100 0000 731a 0000 0010  tation....s.....
+00001610: 0208 0302 0104 0808 f90e 0104 0608 fb0e  ................
+00001620: 0104 0408 fd0e 0104 027a 2150 6169 7265  .........z!Paire
+00001630: 6446 7261 6d65 4275 696c 6465 722e 6170  dFrameBuilder.ap
+00001640: 706c 795f 726f 7461 7469 6f6e 6303 0000  ply_rotationc...
+00001650: 0000 0000 0000 0000 0008 0000 0009 0000  ................
+00001660: 0043 0000 0073 4e01 0000 7c01 5c02 7d03  .C...sN...|.\.}.
+00001670: 7d04 7400 a001 6401 a101 0100 7c00 a002  }.t...d.....|...
+00001680: 7c03 a101 7d05 7c00 a002 7c04 a101 7d06  |...}.|...|...}.
+00001690: 7c00 a003 7c05 7c03 7c06 7c04 a104 5c02  |...|.|.|.|...\.
+000016a0: 7d05 7d06 7c00 a004 7c05 7c03 7c06 7c04  }.}.|...|.|.|.|.
+000016b0: a104 5c02 7d05 7d06 7c00 a005 7c05 a101  ..\.}.}.|...|...
+000016c0: 7d05 7c00 a005 7c06 a101 7d06 7c00 a006  }.|...|...}.|...
+000016d0: 7c05 7c03 a102 7d05 7c00 a006 7c06 7c04  |.|...}.|...|.|.
+000016e0: a102 7d06 7407 a008 7c05 6402 a102 7d05  ..}.t...|.d...}.
+000016f0: 7407 a008 7c06 6402 a102 7d06 7407 6a09  t...|.d...}.t.j.
+00001700: 7c05 740a 7c03 8301 740b 7c05 6a0c 6402  |.t.|...t.|.j.d.
+00001710: 1900 6403 1b00 8301 740b 7c00 6a0d 6404  ..d.....t.|.j.d.
+00001720: 1b00 8301 6602 7407 6a0e 6402 6405 6403  ....f.t.j.d.d.d.
+00001730: 6406 8d07 7d05 7407 6a09 7c06 740a 7c04  d...}.t.j.|.t.|.
+00001740: 8301 740b 7c06 6a0c 6402 1900 6403 1b00  ..t.|.j.d...d...
+00001750: 8301 740b 7c00 6a0d 6404 1b00 8301 6602  ..t.|.j.d.....f.
+00001760: 7407 6a0e 6402 6405 6403 6406 8d07 7d06  t.j.d.d.d.d...}.
+00001770: 740f a010 7c05 7c06 6602 a101 7d07 7407  t...|.|.f...}.t.
+00001780: 6a09 7c07 740a 7c02 8301 7c00 6a0d 6407  j.|.t.|...|.j.d.
+00001790: 1800 740b 7c00 6a0d 6404 1400 6408 1b00  ..t.|.j.d...d...
+000017a0: 8301 6602 7407 6a0e 6402 6405 6403 6406  ..f.t.j.d.d.d.d.
+000017b0: 8d07 7d07 7c07 5300 2909 7a3d 706c 6163  ..}.|.S.).z=plac
+000017c0: 6520 7061 6972 6564 2066 7261 6d65 7320  e paired frames 
+000017d0: 7369 6465 2062 7920 7369 6465 2077 6974  side by side wit
+000017e0: 6820 616e 2069 6e66 6f20 626f 7820 746f  h an info box to
+000017f0: 2074 6865 206c 6566 747a 2348 6f72 697a   the leftz#Horiz
+00001800: 6f6e 7461 6c6c 7920 7374 6163 6b69 6e67  ontally stacking
+00001810: 2070 6169 7265 6420 6672 616d 6573 7244   paired framesrD
+00001820: 0000 0072 2b00 0000 7207 0000 0029 0372  ...r+...r....).r
+00001830: 0100 0000 7201 0000 0072 5f00 0000 a904  ....r....r_.....
+00001840: 5a08 666f 6e74 4661 6365 5a09 666f 6e74  Z.fontFaceZ.font
+00001850: 5363 616c 65da 0563 6f6c 6f72 da09 7468  Scale..color..th
+00001860: 6963 6b6e 6573 73e9 1600 0000 7245 0000  ickness.....rE..
+00001870: 0029 1172 1e00 0000 723b 0000 0072 4300  .).r....r;...rC.
+00001880: 0000 7263 0000 0072 5d00 0000 726f 0000  ..rc...r]...ro..
+00001890: 0072 7a00 0000 7253 0000 00da 0466 6c69  .rz...rS.....fli
+000018a0: 70da 0770 7574 5465 7874 da03 7374 7272  p..putText..strr
+000018b0: 6100 0000 7265 0000 0072 1500 0000 da14  a...re...r......
+000018c0: 464f 4e54 5f48 4552 5348 4559 5f53 494d  FONT_HERSHEY_SIM
+000018d0: 504c 4558 723c 0000 00da 0668 7374 6163  PLEXr<.....hstac
+000018e0: 6b29 0872 2500 0000 7210 0000 00da 0b62  k).r%...r......b
+000018f0: 6f61 7264 5f63 6f75 6e74 7256 0000 0072  oard_countrV...r
+00001900: 5800 0000 7255 0000 0072 5700 0000 5a0d  X...rU...rW...Z.
+00001910: 6873 7461 636b 6564 5f70 6169 7272 0d00  hstacked_pairr..
+00001920: 0000 720d 0000 0072 1100 0000 da0d 6873  ..r....r......hs
+00001930: 7461 636b 5f66 7261 6d65 73c1 0000 0073  tack_frames....s
+00001940: 4e00 0000 0803 0a01 0a01 0a01 1403 1401  N...............
+00001950: 0a02 0a01 0c02 0c01 0c02 0c01 0602 0601  ................
+00001960: 1e01 0401 0201 0201 0201 06fa 0609 0601  ................
+00001970: 1e01 0401 0201 0201 0201 06fa 0e0a 0402  ................
+00001980: 0201 0601 1a01 0401 0201 0201 0201 06f9  ................
+00001990: 040b 7a20 5061 6972 6564 4672 616d 6542  ..z PairedFrameB
+000019a0: 7569 6c64 6572 2e68 7374 6163 6b5f 6672  uilder.hstack_fr
+000019b0: 616d 6573 6301 0000 0000 0000 0000 0000  amesc...........
+000019c0: 0004 0000 0009 0000 0043 0000 0073 5c00  .........C...s\.
+000019d0: 0000 7400 7c00 6a01 8301 7d01 6401 7d01  ..t.|.j...}.d.}.
+000019e0: 7400 7c00 6a01 6402 1400 8301 7d02 7402  t.|.j.d.....}.t.
+000019f0: a003 7c01 7c02 6403 6603 7402 6a04 a102  ..|.|.d.f.t.j...
+00001a00: 7d03 7405 6a06 7c03 6404 6405 7400 7c00  }.t.j.|.d.d.t.|.
+00001a10: 6a01 6406 1b00 8301 6602 7405 6a07 6401  j.d.....f.t.j.d.
+00001a20: 6407 6401 6408 8d07 7d03 7c03 5300 2909  d.d.d...}.|.S.).
+00001a30: 4e72 4400 0000 6700 0000 0000 0004 4072  NrD...g.......@r
+00001a40: 3700 0000 da00 e914 0000 0072 2b00 0000  7..........r+...
+00001a50: 725e 0000 0072 7b00 0000 2908 7261 0000  r^...r{...).ra..
+00001a60: 0072 1500 0000 723c 0000 0072 3d00 0000  .r....r<...r=...
+00001a70: 723e 0000 0072 5300 0000 7280 0000 0072  r>...rS...r....r
+00001a80: 8200 0000 2904 7225 0000 0072 6900 0000  ....).r%...ri...
+00001a90: 726a 0000 00da 0562 6c61 6e6b 720d 0000  rj.....blankr...
+00001aa0: 0072 0d00 0000 7211 0000 00da 1467 6574  .r....r......get
+00001ab0: 5f63 6f6d 706c 6574 696f 6e5f 6672 616d  _completion_fram
+00001ac0: 65f9 0000 0073 1c00 0000 0a01 0401 0e02  e....s..........
+00001ad0: 1402 0402 0201 0201 1001 0401 0201 0201  ................
+00001ae0: 0201 06f9 040a 7a27 5061 6972 6564 4672  ......z'PairedFr
+00001af0: 616d 6542 7569 6c64 6572 2e67 6574 5f63  ameBuilder.get_c
+00001b00: 6f6d 706c 6574 696f 6e5f 6672 616d 6563  ompletion_framec
+00001b10: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00001b20: 0800 0000 4300 0000 7390 0000 007c 006a  ....C...s....|.j
+00001b30: 00a0 01a1 0001 007c 006a 026a 037c 005f  .......|.j.j.|._
+00001b40: 0364 017d 0164 027d 027c 006a 0444 005d  .d.}.d.}.|.j.D.]
+00001b50: 267d 037c 006a 057c 0319 007d 047c 047c  &}.|.j.|...}.|.|
+00001b60: 006a 0664 0318 006b 0472 2164 047d 027c  .j.d...k.r!d.}.|
+00001b70: 0164 0175 0072 2c7c 00a0 077c 037c 04a1  .d.u.r,|...|.|..
+00001b80: 027d 0171 1174 08a0 097c 017c 00a0 077c  .}.q.t...|.|...|
+00001b90: 037c 04a1 0267 02a1 017d 0171 117c 0272  .|...g...}.q.|.r
+00001ba0: 3e7c 00a0 0aa1 0001 007c 0164 0175 0072  >|.......|.d.u.r
+00001bb0: 467c 00a0 0ba1 007d 017c 0153 0029 057a  F|.....}.|.S.).z
+00001bc0: 630a 2020 2020 2020 2020 5468 6973 2067  c.        This g
+00001bd0: 6c75 6573 2074 6f67 6574 6865 7220 7468  lues together th
+00001be0: 6520 7374 6572 656f 7061 6972 7320 7769  e stereopairs wi
+00001bf0: 7468 2073 756d 6d61 7279 2062 6c6f 636b  th summary block
+00001c00: 7320 6f66 2074 6865 2063 6f6d 6d6f 6e20  s of the common 
+00001c10: 626f 6172 6420 636f 756e 740a 2020 2020  board count.    
+00001c20: 2020 2020 4e46 7244 0000 0054 290c 721b      NFrD...T).r.
+00001c30: 0000 0072 3500 0000 720b 0000 0072 3900  ...r5...r....r9.
+00001c40: 0000 7222 0000 0072 2000 0000 7216 0000  ..r"...r ...r...
+00001c50: 0072 8500 0000 723c 0000 00da 0676 7374  .r....r<.....vst
+00001c60: 6163 6b72 3600 0000 7289 0000 0029 0572  ackr6...r....).r
+00001c70: 2500 0000 da0c 7374 6572 656f 5f66 7261  %.....stereo_fra
+00001c80: 6d65 5a14 626f 6172 645f 7461 7267 6574  meZ.board_target
+00001c90: 5f72 6561 6368 6564 7210 0000 0072 8400  _reachedr....r..
+00001ca0: 0000 720d 0000 0072 0d00 0000 7211 0000  ..r....r....r...
+00001cb0: 00da 1067 6574 5f73 7465 7265 6f5f 6672  ...get_stereo_fr
+00001cc0: 616d 650d 0100 0073 2400 0000 0a05 0a01  ame....s$.......
+00001cd0: 0402 0401 0a01 0a03 0e01 0401 0802 0e01  ................
+00001ce0: 0402 0e01 06ff 0404 0801 0802 0801 0401  ................
+00001cf0: 7a23 5061 6972 6564 4672 616d 6542 7569  z#PairedFrameBui
+00001d00: 6c64 6572 2e67 6574 5f73 7465 7265 6f5f  lder.get_stereo_
+00001d10: 6672 616d 65da 0672 6574 7572 6e63 0200  frame..returnc..
+00001d20: 0000 0000 0000 0000 0000 0f00 0000 0800  ................
+00001d30: 0000 0300 0000 732e 0100 007c 006a 00a0  ......s....|.j..
+00001d40: 01a1 007d 0264 0164 0284 007c 02a0 02a1  ...}.d.d...|....
+00001d50: 0044 0083 017d 037c 02a0 037c 03a1 0101  .D...}.|...|....
+00001d60: 0064 037d 0474 0474 057c 027c 0183 0204  .d.}.t.t.|.|....
+00001d70: 007d 0583 017c 046b 0372 8974 047c 0583  .}...|.k.r.t.|..
+00001d80: 017d 047c 0544 005d 577d 067c 0664 0419  .}.|.D.]W}.|.d..
+00001d90: 0089 007c 0664 0519 0089 0187 0066 0164  ...|.d.......f.d
+00001da0: 0664 0784 087c 02a0 06a1 0044 0083 017d  .d...|.....D...}
+00001db0: 0787 0166 0164 0864 0784 087c 02a0 06a1  ...f.d.d...|....
+00001dc0: 0044 0083 017d 0864 007d 097c 0744 005d  .D...}.d.}.|.D.]
+00001dd0: 327d 0a7c 0844 005d 2d7d 0b7c 0a64 0519  2}.|.D.]-}.|.d..
+00001de0: 007c 0b64 0419 006b 0272 7b7c 027c 0a19  .|.d...k.r{|.|..
+00001df0: 007d 0c7c 027c 0b19 007d 0d7c 0c7c 016b  .}.|.|...}.|.|.k
+00001e00: 0472 7b7c 0d7c 016b 0472 7b74 077c 0c7c  .r{|.|.k.r{t.|.|
+00001e10: 0d83 027d 097c 097c 027c 063c 007c 097c  ...}.|.|.|.<.|.|
+00001e20: 027c 0664 0519 007c 0664 0419 0066 023c  .|.d...|.d...f.<
+00001e30: 0071 4e71 4a71 2674 0474 057c 027c 0183  .qNqJq&t.t.|.|..
+00001e40: 0204 007d 0583 017c 046b 0373 2074 047c  ...}...|.k.s t.|
+00001e50: 0583 0164 046b 0472 9364 097d 0e7c 0e53  ...d.k.r.d.}.|.S
+00001e60: 0064 0a7d 0e7c 0e53 0029 0b4e 6301 0000  .d.}.|.S.).Nc...
+00001e70: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00001e80: 0053 0000 0073 1e00 0000 6900 7c00 5d0b  .S...s....i.|.].
+00001e90: 5c02 7d01 7d02 7400 7401 7c01 8301 8301  \.}.}.t.t.|.....
+00001ea0: 7c02 9302 7102 5300 720d 0000 0029 02da  |...q.S.r....)..
+00001eb0: 0574 7570 6c65 da08 7265 7665 7273 6564  .tuple..reversed
+00001ec0: 7230 0000 0072 0d00 0000 720d 0000 0072  r0...r....r....r
+00001ed0: 1100 0000 7212 0000 0033 0100 0073 0200  ....r....3...s..
+00001ee0: 0000 1e00 7a43 5061 6972 6564 4672 616d  ....zCPairedFram
+00001ef0: 6542 7569 6c64 6572 2e70 6f73 7369 626c  eBuilder.possibl
+00001f00: 655f 746f 5f69 6e69 7469 616c 697a 655f  e_to_initialize_
+00001f10: 6172 7261 792e 3c6c 6f63 616c 733e 2e3c  array.<locals>.<
+00001f20: 6469 6374 636f 6d70 3e72 7200 0000 7201  dictcomp>rr...r.
+00001f30: 0000 0072 4400 0000 6301 0000 0000 0000  ...rD...c.......
+00001f40: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+00001f50: 00f3 1c00 0000 6700 7c00 5d0a 7d01 7c01  ......g.|.].}.|.
+00001f60: 6400 1900 8800 6b02 7202 7c01 9102 7102  d.....k.r.|...q.
+00001f70: 5300 720c 0000 0072 0d00 0000 720e 0000  S.r....r....r...
+00001f80: 0029 01da 0670 6f72 745f 4172 0d00 0000  .)...port_Ar....
+00001f90: 7211 0000 0072 2a00 0000 4201 0000 f302  r....r*...B.....
+00001fa0: 0000 001c 007a 4350 6169 7265 6446 7261  .....zCPairedFra
+00001fb0: 6d65 4275 696c 6465 722e 706f 7373 6962  meBuilder.possib
+00001fc0: 6c65 5f74 6f5f 696e 6974 6961 6c69 7a65  le_to_initialize
+00001fd0: 5f61 7272 6179 2e3c 6c6f 6361 6c73 3e2e  _array.<locals>.
+00001fe0: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
+00001ff0: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00002000: 0000 0072 9000 0000 2901 7244 0000 0072  ...r....).rD...r
+00002010: 0d00 0000 720e 0000 0029 01da 0670 6f72  ....r....)...por
+00002020: 745f 4372 0d00 0000 7211 0000 0072 2a00  t_Cr....r....r*.
+00002030: 0000 4301 0000 7292 0000 0046 5429 0872  ..C...r....FT).r
+00002040: 2000 0000 7221 0000 0072 3400 0000 da06   ...r!...r4.....
+00002050: 7570 6461 7465 724c 0000 00da 0f67 6574  updaterL.....get
+00002060: 5f65 6d70 7479 5f70 6169 7273 da04 6b65  _empty_pairs..ke
+00002070: 7973 722c 0000 0029 0f72 2500 0000 da0d  ysr,...).r%.....
+00002080: 6d69 6e5f 7468 7265 7368 6f6c 645a 1477  min_thresholdZ.w
+00002090: 6f72 6b69 6e67 5f62 6f61 7264 5f63 6f75  orking_board_cou
+000020a0: 6e74 735a 1466 6c69 7070 6564 5f62 6f61  ntsZ.flipped_boa
+000020b0: 7264 5f63 6f75 6e74 735a 1665 6d70 7479  rd_countsZ.empty
+000020c0: 5f63 6f75 6e74 5f6c 6173 745f 6379 636c  _count_last_cycl
+000020d0: 65da 0b65 6d70 7479 5f70 6169 7273 7210  e..empty_pairsr.
+000020e0: 0000 00da 0d61 6c6c 5f70 6169 7273 5f41  .....all_pairs_A
+000020f0: 5f58 da0d 616c 6c5f 7061 6972 735f 585f  _X..all_pairs_X_
+00002100: 435a 0f62 6f61 7264 5f63 6f75 6e74 5f41  CZ.board_count_A
+00002110: 5f43 da08 7061 6972 5f41 5f58 da08 7061  _C..pair_A_X..pa
+00002120: 6972 5f58 5f43 5a0f 626f 6172 645f 636f  ir_X_CZ.board_co
+00002130: 756e 745f 415f 585a 0f62 6f61 7264 5f63  unt_A_XZ.board_c
+00002140: 6f75 6e74 5f58 5f43 5a0b 6973 5f70 6f73  ount_X_CZ.is_pos
+00002150: 7369 626c 6572 0d00 0000 2902 7291 0000  sibler....).r...
+00002160: 0072 9300 0000 7211 0000 00da 1c70 6f73  .r....r......pos
+00002170: 7369 626c 655f 746f 5f69 6e69 7469 616c  sible_to_initial
+00002180: 697a 655f 6172 7261 792f 0100 0073 3c00  ize_array/...s<.
+00002190: 0000 0a03 1201 0a01 0402 1602 0803 0802  ................
+000021a0: 0802 0801 1602 1601 0402 0802 0801 1001  ................
+000021b0: 0802 0801 1002 0a01 0801 1401 0280 02f7  ................
+000021c0: 02ff 16f1 0c1b 0401 0404 04fe 0402 7a2f  ..............z/
+000021d0: 5061 6972 6564 4672 616d 6542 7569 6c64  PairedFrameBuild
+000021e0: 6572 2e70 6f73 7369 626c 655f 746f 5f69  er.possible_to_i
+000021f0: 6e69 7469 616c 697a 655f 6172 7261 794e  nitialize_arrayN
+00002200: 2902 7209 0000 0072 0a00 0000 2912 da08  ).r....r....)...
+00002210: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00002220: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00002230: 5f5f 7203 0000 0072 2600 0000 7229 0000  __r....r&...r)..
+00002240: 0072 1900 0000 7236 0000 0072 4300 0000  .r....r6...rC...
+00002250: 725d 0000 0072 6300 0000 726f 0000 0072  r]...rc...ro...r
+00002260: 7a00 0000 7285 0000 0072 8900 0000 728c  z...r....r....r.
+00002270: 0000 00da 0462 6f6f 6c72 9d00 0000 720d  .....boolr....r.
+00002280: 0000 0072 0d00 0000 720d 0000 0072 1100  ...r....r....r..
+00002290: 0000 7208 0000 0010 0000 0073 1c00 0000  ..r........s....
+000022a0: 0800 1001 0819 0804 080a 0808 080e 0837  ...............7
+000022b0: 080f 081d 0810 0838 0814 1222 7208 0000  .......8..."r...
+000022c0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+000022d0: 0000 0300 0000 0300 0000 731a 0000 0087  ..........s.....
+000022e0: 0066 0164 0164 0284 087c 00a0 00a1 0044  .f.d.d...|.....D
+000022f0: 0083 017d 027c 0253 0029 034e 6301 0000  ...}.|.S.).Nc...
+00002300: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00002310: 0013 0000 0073 1c00 0000 6700 7c00 5d0a  .....s....g.|.].
+00002320: 5c02 7d01 7d02 7c02 8800 6b00 7202 7c01  \.}.}.|...k.r.|.
+00002330: 9102 7102 5300 720d 0000 0072 0d00 0000  ..q.S.r....r....
+00002340: 7230 0000 00a9 0172 9700 0000 720d 0000  r0.....r....r...
+00002350: 0072 1100 0000 722a 0000 005c 0100 0072  .r....r*...\...r
+00002360: 9200 0000 7a23 6765 745f 656d 7074 795f  ....z#get_empty_
+00002370: 7061 6972 732e 3c6c 6f63 616c 733e 2e3c  pairs.<locals>.<
+00002380: 6c69 7374 636f 6d70 3e29 0172 3400 0000  listcomp>).r4...
+00002390: 2903 7220 0000 0072 9700 0000 7298 0000  ).r ...r....r...
+000023a0: 0072 0d00 0000 72a2 0000 0072 1100 0000  .r....r....r....
+000023b0: 7295 0000 005b 0100 0073 0400 0000 1601  r....[...s......
+000023c0: 0401 7295 0000 0063 0200 0000 0000 0000  ..r....c........
+000023d0: 0000 0000 0700 0000 0500 0000 4300 0000  ............C...
+000023e0: 7344 0000 007c 006a 0064 0064 0185 0219  sD...|.j.d.d....
+000023f0: 005c 027d 027d 037c 0174 017c 0283 011b  .\.}.}.|.t.|....
+00002400: 007d 0474 027c 037c 0414 0083 017c 0166  .}.t.|.|.....|.f
+00002410: 027d 0574 036a 047c 007c 0574 036a 0564  .}.t.j.|.|.t.j.d
+00002420: 028d 037d 067c 0653 0029 034e 722b 0000  ...}.|.S.).Nr+..
+00002430: 0029 01da 0d69 6e74 6572 706f 6c61 7469  .)...interpolati
+00002440: 6f6e 2906 7265 0000 0072 5200 0000 7261  on).re...rR...ra
+00002450: 0000 0072 5300 0000 7268 0000 00da 0a49  ...rS...rh.....I
+00002460: 4e54 4552 5f41 5245 4129 07da 0569 6d61  NTER_AREA)...ima
+00002470: 6765 7264 0000 005a 0e63 7572 7265 6e74  gerd...Z.current
+00002480: 5f68 6569 6768 745a 0d63 7572 7265 6e74  _heightZ.current
+00002490: 5f77 6964 7468 da05 7261 7469 6fda 0364  _width..ratio..d
+000024a0: 696d 5a07 7265 7369 7a65 6472 0d00 0000  imZ.resizedr....
+000024b0: 720d 0000 0072 1100 0000 7268 0000 005f  r....r....rh..._
+000024c0: 0100 0073 0a00 0000 1201 0c01 1001 1201  ...s............
+000024d0: 0401 7268 0000 0029 16da 0d70 7978 7933  ..rh...)...pyxy3
+000024e0: 642e 6c6f 6767 6572 da06 7079 7879 3364  d.logger..pyxy3d
+000024f0: 721e 0000 0072 3500 0000 729e 0000 00da  r....r5...r.....
+00002500: 0770 6174 686c 6962 7202 0000 0072 5300  .pathlibr....rS.
+00002510: 0000 da05 6e75 6d70 7972 3c00 0000 da1b  ....numpyr<.....
+00002520: 7079 7879 3364 2e63 616d 6572 6173 2e73  pyxy3d.cameras.s
+00002530: 796e 6368 726f 6e69 7a65 7272 0300 0000  ynchronizerr....
+00002540: da09 6974 6572 746f 6f6c 7372 0400 0000  ..itertoolsr....
+00002550: da05 7175 6575 6572 0500 0000 da09 7468  ..queuer......th
+00002560: 7265 6164 696e 6772 0600 0000 7217 0000  readingr....r...
+00002570: 0072 0800 0000 7295 0000 0072 6800 0000  .r....r....rh...
+00002580: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00002590: 1100 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000025a0: 0000 731e 0000 0008 000c 010c 0208 0208  ..s.............
+000025b0: 010c 020c 010c 010c 0104 020e 0200 7f00  ................
+000025c0: 7f08 4d0c 04                             ..M..
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.0.22/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,14 @@
 
         self.pairs = self.get_pairs()
 
         self.new_sync_packet_notice = Queue()
         self.synchronizer.subscribe_to_notice(self.new_sync_packet_notice)
         self.store_points = Event()
     
-        self.reset() 
-        # self.board_counts = {pair: 0 for pair in self.pairs} 
-        # self.stereo_list = self.pairs.copy()
-        # self.stereo_history = {pair:{"img_loc_A":[], "img_loc_B":[]} for pair in self.pairs}
-        # self.store_points.clear()   # don't default to storing tracked points
-    
-    def reset(self): 
         logger.info("Resetting Frame Builder")
         self.board_counts = {pair: 0 for pair in self.pairs} 
         self.stereo_list = self.pairs.copy()
         self.stereo_history = {pair:{"img_loc_A":[], "img_loc_B":[]} for pair in self.pairs}
         self.store_points.clear()   # don't default to storing tracked points
 
     def unsubscribe_from_synchronizer(self):
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.0.22/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.0.22/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.0.22/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/log_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/main_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/main_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 class MainWindow(QMainWindow):
     def __init__(self):
         super(MainWindow, self).__init__()
 
         self.app_settings = toml.load(__settings_path__)
 
-        self.setWindowTitle("PyXY3D")
+        self.setWindowTitle("Pyxy3D")
         self.setWindowIcon(QIcon(str(Path(__root__, "pyxy3d/gui/icons/pyxy_logo.svg"))))
         self.setMinimumSize(500, 500)
 
         # File Menu
         self.menu = self.menuBar()
         self.file_menu = self.menu.addMenu("File")
 
@@ -86,14 +86,15 @@
         self.cameras_menu.addAction(self.disconnect_cameras_action)
         self.disconnect_cameras_action.setEnabled(False)
 
         self.connect_menu_actions()
 
         # Set up layout (based on splitter)
         self.tab_widget = QTabWidget()
+        # self.tab_widget = CentralTabWidget()
         self.setCentralWidget(self.tab_widget)
 
         # create log window which is fixed below main window
         self.docked_logger = QDockWidget("Log", self)
         self.docked_logger.setFeatures(QDockWidget.DockWidgetFeature.DockWidgetMovable)
         self.docked_logger.setAllowedAreas(Qt.DockWidgetArea.BottomDockWidgetArea)
         self.log_widget = LogWidget()
@@ -121,48 +122,64 @@
         self.recording_widget = QWidget()
                 
         self.session.set_mode(SessionMode.Charuco)
         self.session.disconnect_cameras() 
         self.disconnect_cameras_action.setEnabled(False)
         self.connect_cameras_action.setEnabled(True)
 
-        
+    def pause_all_frame_reading(self):
+        logger.info("Pausing all frame reading at load of stream tools; should be on charuco tab right now")
+        self.session.pause_all_monocalibrators()
+        self.session.pause_synchronizer()  
 
     def load_stream_tools(self):
         self.connect_cameras_action.setEnabled(False)
         self.disconnect_cameras_action.setEnabled(True)
+        self.session.stream_tools_loaded_signal.connect(self.pause_all_frame_reading)
         self.thread = Thread(
             target=self.session.load_stream_tools, args=(), daemon=True
         )
         self.thread.start()
 
+            
+            
     def on_tab_changed(self, index):
         logger.info(f"Switching main window to tab {index}")
         match index:
             case TabIndex.Charuco.value:
                 logger.info(f"Activating Charuco Widget")
+                # self.silence_extrinsic_cal_widget()
                 self.session.set_mode(SessionMode.Charuco)
             case TabIndex.Cameras.value:
                 logger.info(f"Activating Camera Setup Widget")
+                # self.silence_extrinsic_cal_widget()
                 self.session.set_mode(SessionMode.IntrinsicCalibration)
             case TabIndex.CaptureVolume.value:
                 logger.info(f"Activating Calibrate Capture Volume Widget")
 
                 if self.session.is_capture_volume_eligible():
                     logger.info(f"Session is eligible for setting of origin...activating capture volume origin widget")
                     self.calibrate_capture_volume_widget.activate_capture_volume_widget()
                 else:
                     logger.info(f"Session is not eligible for setting of origin...activating extrinsic calibration widget")
                     self.calibrate_capture_volume_widget.activate_extrinsic_calibration_widget()
 
             case TabIndex.Recording.value:
                 logger.info(f"Activate Recording Mode")
+
+                try:
+                    logger.info("Attempting to spin down the extrinsic calibration widget")
+                    self.calibrate_capture_volume_widget.extrinsic_calibration_widget.shutdown_threads()
+                except:
+                    logger.info("No extrinsic calibration calibration widget exists")
+
                 self.session.set_mode(SessionMode.Recording)
             case TabIndex.Processing.value:
                 logger.info(f"Activate Processing Mode")
+                # self.silence_extrinsic_cal_widget()
                 self.session.set_mode(SessionMode.PostProcessing)
                 # may have acquired new recordings
                 self.processing_widget.update_recording_folders()
 
     def launch_session(self, path_to_folder: str):
         session_path = Path(path_to_folder)
         self.config = Configurator(session_path)
@@ -330,14 +347,34 @@
             self.add_to_recent_project(folder_path)
 
     def update_app_settings(self):
         with open(__settings_path__, "w") as f:
             toml.dump(self.app_settings, f)
 
 
+class CentralTabWidget(QTabWidget):
+    """
+    Switching between tabs, particularly when system resource utilization is high,
+    is prone to result in segfault crashes. Working hypothesis is that this is due to mode
+    changes happening when the tab is changed and the GUI tries to render something it doesn't have
+    
+    This override slips the mode change between click and change to try to stabilize the mode switches.
+    
+    """
+    
+    def __init__(self):
+        super(CentralTabWidget, self).__init__()
+        
+    def tabBarClicked(self, index):
+        # Emit a custom signal or perform any desired action before the tab changes
+        logger.info(f"Tab {index} clicked")
+        
+        # Uncomment the following line to allow the tab to change after the signal is emitted
+        super(CentralTabWidget, self).tabBarClicked(index)
+
 def launch_main():
     app = QApplication(sys.argv)
     window = MainWindow()
     window.show()
 
     app.exec()
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.0.22/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/playback_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/playback_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.0.22/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/recording_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     QHBoxLayout,
     QLabel,
     QPushButton,
     QSlider,
     QVBoxLayout,
 )
 
-from pyxy3d.session.session import Session
+from pyxy3d.session.session import Session, SessionMode
 from pyxy3d.cameras.synchronizer import Synchronizer
 from pyxy3d import __root__
 from pyxy3d.recording.video_recorder import VideoRecorder
 from pyxy3d.configurator import Configurator
 
 class NextRecordingActions(Enum):
     StartRecording = "Start Recording"
@@ -54,17 +54,17 @@
         self.session = session
         self.synchronizer:Synchronizer = self.session.synchronizer
         
         # don't let point tracking slow down the frame reading
         # self.synchronizer.set_tracking_on_streams(False)
 
         # create tools to build and emit the displayed frame
-        self.frame_builder = UnpairedFrameBuilder(self.synchronizer)
-        self.frame_emitter = UnpairedFrameEmitter(self.frame_builder)
-        self.frame_emitter.start()
+        self.unpaired_frame_builder = UnpairedFrameBuilder(self.synchronizer)
+        self.unpaired_frame_emitter = UnpairedFrameEmitter(self.unpaired_frame_builder)
+        self.unpaired_frame_emitter.start()
 
         self.video_recorder = VideoRecorder(self.synchronizer)
         
         self.frame_rate_spin = QSpinBox()
         self.frame_rate_spin.setValue(self.session.fps_recording)
 
         self.next_action = NextRecordingActions.StartRecording
@@ -122,17 +122,17 @@
         self.layout().addWidget(self.dropped_fps_label)
 
         self.layout().addWidget(self.recording_frame_display)
 
 
     def connect_widgets(self):
     
-        self.frame_emitter.ImageBroadcast.connect(self.ImageUpdateSlot)
+        self.unpaired_frame_emitter.ImageBroadcast.connect(self.ImageUpdateSlot)
         self.frame_rate_spin.valueChanged.connect(self.session.set_active_mode_fps)
-        self.frame_emitter.dropped_fps.connect(self.update_dropped_fps)
+        self.unpaired_frame_emitter.dropped_fps.connect(self.update_dropped_fps)
         self.start_stop.clicked.connect(self.toggle_start_stop)
         self.session.recording_complete_signal.connect(self.on_recording_complete)
 
     def toggle_start_stop(self):
         if self.next_action == NextRecordingActions.StartRecording:
             self.next_action = NextRecordingActions.StopRecording
             self.start_stop.setText(self.next_action.value)
@@ -383,15 +383,15 @@
     )
     return qt_frame
 
 
 def launch_recording_widget(session_path):
             config = Configurator(session_path)
             session = Session(config)
-            session.load_stream_tools()
-            session._adjust_resolutions()
-
+            # session.load_stream_tools()
+            # session._adjust_resolutions()
+            session.set_mode(SessionMode.Recording)
             App = QApplication(sys.argv)
             recording_dialog = RecordingWidget(session)
             recording_dialog.show()
 
             sys.exit(App.exec())
```

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.0.22/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/helper.py` & `pyxy3d-0.0.22/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/interface.py` & `pyxy3d-0.0.22/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/logger.py` & `pyxy3d-0.0.22/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/post_processor.py` & `pyxy3d-0.0.22/pyxy3d/post_processor.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.0.22/pyxy3d/recording/recorded_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.0.22/pyxy3d/recording/video_recorder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/session/__pycache__/session.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/session/__pycache__/session.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 22:04:16 2023 UTC, .py size: 20674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6096 8764 c250 0000  o.......`..d.P..
+00000000: 6f0d 0d0a 0000 0000 244e 8b64 bd53 0000  o.......$N.d.S..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6402 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6403 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6400 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -285,699 +285,735 @@
 000011c0: 0072 2600 0000 da15 6973 5f72 6563 6f72  .r&.....is_recor
 000011d0: 6469 6e67 5f65 6c69 6769 626c 659b 0000  ding_eligible...
 000011e0: 0073 2a00 0000 0a07 0c01 0403 1001 0401  .s*.............
 000011f0: 1402 0a01 0801 02ff 0801 02ff 0403 0401  ................
 00001200: 0a01 04ff 0280 0403 0401 0404 04fe 0402  ................
 00001210: 7a1d 5365 7373 696f 6e2e 6973 5f72 6563  z.Session.is_rec
 00001220: 6f72 6469 6e67 5f65 6c69 6769 626c 6563  ording_eligiblec
-00001230: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001240: 0400 0000 4300 0000 7324 0000 0064 017d  ....C...s$...d.}
-00001250: 017c 006a 00a0 01a1 0044 005d 087d 0274  .|.j.....D.].}.t
-00001260: 02a0 037c 029b 00a1 0101 0071 077c 0153  ...|.......q.|.S
-00001270: 0029 027a 690a 2020 2020 2020 2020 506f  .).zi.        Po
-00001280: 7374 2070 726f 6365 7373 696e 6720 6361  st processing ca
-00001290: 6e20 6f6e 6c79 2062 6520 7065 7266 6f72  n only be perfor
-000012a0: 6d65 6420 6966 2072 6563 6f72 6469 6e67  med if recording
-000012b0: 7320 6578 6973 7420 616e 6420 6578 7472  s exist and extr
-000012c0: 696e 7369 6373 2061 7265 2063 616c 6962  insics are calib
-000012d0: 7261 7465 640a 2020 2020 2020 2020 4629  rated.        F)
-000012e0: 0472 2c00 0000 da07 6974 6572 6469 7272  .r,.....iterdirr
-000012f0: 5400 0000 da04 7761 726e 2903 723b 0000  T.....warn).r;..
-00001300: 0072 4a00 0000 da01 6672 2500 0000 7225  .rJ.....fr%...r%
-00001310: 0000 0072 2600 0000 da1b 6973 5f70 6f73  ...r&.....is_pos
-00001320: 745f 7072 6f63 6573 7369 6e67 5f65 6c69  t_processing_eli
-00001330: 6769 626c 65b9 0000 0073 0800 0000 0406  gible....s......
-00001340: 0e01 0e01 0403 7a23 5365 7373 696f 6e2e  ......z#Session.
-00001350: 6973 5f70 6f73 745f 7072 6f63 6573 7369  is_post_processi
-00001360: 6e67 5f65 6c69 6769 626c 6572 3a00 0000  ng_eligibler:...
-00001370: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001380: 0003 0000 0043 0000 0073 8001 0000 7c01  .....C...s....|.
-00001390: 7c00 5f00 7c00 a001 a100 0100 7c00 6a00  |._.|.......|.j.
-000013a0: 0400 7402 6a03 6b02 721f 0100 7c00 6a04  ..t.j.k.r...|.j.
-000013b0: 721d 7c00 6a05 a006 a100 0100 7c00 a007  r.|.j.......|...
-000013c0: a100 0100 6403 5300 6403 5300 0400 7402  ....d.S.d.S...t.
-000013d0: 6a08 6b02 7235 0100 7c00 6a04 7233 7c00  j.k.r5..|.j.r3|.
-000013e0: 6a05 a006 a100 0100 7c00 a007 a100 0100  j.......|.......
-000013f0: 6403 5300 6403 5300 0400 7402 6a09 6b02  d.S.d.S...t.j.k.
-00001400: 7262 0100 740a 7c00 6a0b 8301 7c00 5f0c  rb..t.|.j...|._.
-00001410: 7c00 6a04 7348 7c00 a00d a100 0100 7c00  |.j.sH|.......|.
-00001420: 6a05 a006 a100 0100 7c00 a007 a100 0100  j.......|.......
-00001430: 7c00 a00e a100 0100 7c00 a00f 6401 a101  |.......|...d...
-00001440: 0100 7c00 a010 7c00 6a11 a101 0100 6403  ..|...|.j.....d.
-00001450: 5300 0400 7402 6a12 6b02 7289 0100 740a  S...t.j.k.r...t.
-00001460: 7c00 6a0b 8301 7c00 5f0c 7c00 6a04 7375  |.j...|._.|.j.su
-00001470: 7c00 a00d a100 0100 7c00 a007 a100 0100  |.......|.......
-00001480: 7c00 a00e a100 0100 7c00 a00f 6401 a101  |.......|...d...
-00001490: 0100 7c00 6a05 a013 a100 0100 6403 5300  ..|.j.......d.S.
-000014a0: 0400 7402 6a14 6b02 729f 0100 7c00 6a04  ..t.j.k.r...|.j.
-000014b0: 729d 7c00 a007 a100 0100 7c00 6a05 a006  r.|.......|.j...
-000014c0: a100 0100 6403 5300 6403 5300 7402 6a15  ....d.S.d.S.t.j.
-000014d0: 6b02 72be 7c00 6a04 73aa 7c00 a00d a100  k.r.|.j.s.|.....
-000014e0: 0100 7c00 a007 a100 0100 7c00 a00f 6402  ..|.......|...d.
-000014f0: a101 0100 7c00 a001 a100 0100 7c00 6a05  ....|.......|.j.
-00001500: a013 a100 0100 6403 5300 6403 5300 2904  ......d.S.d.S.).
-00001510: 7aaf 0a20 2020 2020 2020 2056 6961 2074  z..        Via t
-00001520: 6869 7320 6d65 7468 6f64 2c20 7468 6520  his method, the 
-00001530: 6672 616d 6520 7265 6164 696e 6720 6265  frame reading be
-00001540: 6861 7669 6f72 2077 696c 6c20 6265 2063  havior will be c
-00001550: 6861 6e67 6564 2062 7920 7468 6520 4755  hanged by the GU
-00001560: 492e 2049 6620 736f 6d65 2070 726f 7065  I. If some prope
-00001570: 7274 6965 7320 6172 650a 2020 2020 2020  rties are.      
-00001580: 2020 6e6f 7420 6176 6169 6c61 626c 6520    not available 
-00001590: 2869 2e65 2e20 7379 6e63 6872 6f6e 697a  (i.e. synchroniz
-000015a0: 6572 2920 7468 6579 2077 696c 6c20 6265  er) they will be
-000015b0: 2063 7265 6174 6564 0a20 2020 2020 2020   created.       
-000015c0: 2054 464e 2916 723a 0000 00da 1275 7064   TFN).r:.....upd
-000015d0: 6174 655f 7374 7265 616d 735f 6670 7372  ate_streams_fpsr
-000015e0: 1900 0000 721f 0000 0072 3100 0000 7241  ....r....r1...rA
-000015f0: 0000 00da 1875 6e73 7562 7363 7269 6265  .....unsubscribe
-00001600: 5f66 726f 6d5f 7374 7265 616d 73da 1970  _from_streams..p
-00001610: 6175 7365 5f61 6c6c 5f6d 6f6e 6f63 616c  ause_all_monocal
-00001620: 6962 7261 746f 7273 7224 0000 0072 2000  ibratorsr$...r .
-00001630: 0000 7209 0000 0072 3800 0000 7239 0000  ..r....r8...r9..
-00001640: 00da 116c 6f61 645f 7374 7265 616d 5f74  ...load_stream_t
-00001650: 6f6f 6c73 da13 7365 745f 7374 7265 616d  ools..set_stream
-00001660: 735f 6368 6172 7563 6fda 1473 6574 5f73  s_charuco..set_s
-00001670: 7472 6561 6d73 5f74 7261 636b 696e 67da  treams_tracking.
-00001680: 1761 6374 6976 6174 655f 6d6f 6e6f 6361  .activate_monoca
-00001690: 6c69 6272 6174 6f72 7233 0000 0072 2100  libratorr3...r!.
-000016a0: 0000 da14 7375 6273 6372 6962 655f 746f  ....subscribe_to
-000016b0: 5f73 7472 6561 6d73 7222 0000 0072 2300  _streamsr"...r#.
-000016c0: 0000 2902 723b 0000 0072 3a00 0000 7225  ..).r;...r:...r%
-000016d0: 0000 0072 2500 0000 7226 0000 00da 0873  ...r%...r&.....s
-000016e0: 6574 5f6d 6f64 65c6 0000 0073 5600 0000  et_mode....sV...
-000016f0: 0605 0801 0402 0c01 0601 0a01 0c01 04fe  ................
-00001700: 0c04 0601 0a01 0c01 04fe 0c04 0c02 0602  ................
-00001710: 0801 0a01 0801 0801 0a01 1001 0c02 0c02  ................
-00001720: 0601 0801 0802 0801 0a01 0e01 0c02 0601  ................
-00001730: 0801 0e01 04fe 0804 0601 0801 0802 0a01  ................
-00001740: 0801 0e01 04f9 7a10 5365 7373 696f 6e2e  ......z.Session.
-00001750: 7365 745f 6d6f 6465 da0a 6670 735f 7461  set_mode..fps_ta
-00001760: 7267 6574 6302 0000 0000 0000 0000 0000  rgetc...........
-00001770: 0002 0000 0003 0000 0043 0000 0073 8600  .........C...s..
-00001780: 0000 7c00 6a00 0400 7401 6a02 6b02 7209  ..|.j...t.j.k.r.
-00001790: 0100 6e34 0400 7401 6a03 6b02 7210 0100  ..n4..t.j.k.r...
-000017a0: 6e2d 0400 7401 6a04 6b02 7220 0100 7c01  n-..t.j.k.r ..|.
-000017b0: 7c00 5f05 7c00 6a06 a007 7c01 a101 0100  |._.|.j...|.....
-000017c0: 6e1d 0400 7401 6a08 6b02 7230 0100 7c01  n...t.j.k.r0..|.
-000017d0: 7c00 5f09 7c00 6a06 a00a 7c01 a101 0100  |._.|.j...|.....
-000017e0: 6e0d 7401 6a0b 6b02 723d 7c01 7c00 5f0c  n.t.j.k.r=|.|._.
-000017f0: 7c00 6a06 a00d 7c01 a101 0100 7c00 a00e  |.j...|.....|...
-00001800: a100 0100 6401 5300 2902 7a78 0a20 2020  ....d.S.).zx.   
-00001810: 2020 2020 2055 7064 6174 6573 2074 6865       Updates the
-00001820: 2046 5053 2075 7365 6420 6279 2074 6865   FPS used by the
-00001830: 2063 7572 7265 6e74 6c79 2061 6374 6976   currently activ
-00001840: 6520 7365 7373 696f 6e20 6d6f 6465 0a20  e session mode. 
-00001850: 2020 2020 2020 2054 6869 7320 7570 6461         This upda
-00001860: 7465 2069 6e63 6c75 6465 7320 7468 6520  te includes the 
-00001870: 636f 6e66 6967 2e74 6f6d 6c0a 2020 2020  config.toml.    
-00001880: 2020 2020 4e29 0f72 3a00 0000 7219 0000      N).r:...r...
-00001890: 0072 1f00 0000 7224 0000 0072 2000 0000  .r....r$...r ...
-000018a0: 7236 0000 0072 2800 0000 5a1e 7361 7665  r6...r(...Z.save
-000018b0: 5f66 7073 5f69 6e74 7269 6e73 6963 5f63  _fps_intrinsic_c
-000018c0: 616c 6962 7261 7469 6f6e 7221 0000 0072  alibrationr!...r
-000018d0: 3500 0000 5a1e 7361 7665 5f66 7073 5f65  5...Z.save_fps_e
-000018e0: 7874 7269 6e73 6963 5f63 616c 6962 7261  xtrinsic_calibra
-000018f0: 7469 6f6e 7223 0000 0072 3400 0000 5a12  tionr#...r4...Z.
-00001900: 7361 7665 5f66 7073 5f72 6563 6f72 6469  save_fps_recordi
-00001910: 6e67 725e 0000 0029 0272 3b00 0000 7267  ngr^...).r;...rg
-00001920: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00001930: 0000 da13 7365 745f 6163 7469 7665 5f6d  ....set_active_m
-00001940: 6f64 655f 6670 73fe 0000 0073 1e00 0000  ode_fps....s....
-00001950: 0405 0c01 0201 0c01 0201 0c01 0601 0e01  ................
-00001960: 0c01 0601 0e01 0801 0601 0c01 0c02 7a1b  ..............z.
-00001970: 5365 7373 696f 6e2e 7365 745f 6163 7469  Session.set_acti
-00001980: 7665 5f6d 6f64 655f 6670 73da 0672 6574  ve_mode_fps..ret
-00001990: 7572 6e63 0100 0000 0000 0000 0000 0000  urnc............
-000019a0: 0200 0000 0300 0000 4300 0000 736e 0000  ........C...sn..
-000019b0: 0064 007d 017c 006a 0004 0074 016a 026b  .d.}.|.j...t.j.k
-000019c0: 0272 0d01 0009 007c 0153 0004 0074 016a  .r.....|.S...t.j
-000019d0: 036b 0272 1601 0009 007c 0153 0004 0074  .k.r.....|.S...t
-000019e0: 016a 046b 0272 2101 007c 006a 057d 017c  .j.k.r!..|.j.}.|
-000019f0: 0153 0004 0074 016a 066b 0272 2c01 007c  .S...t.j.k.r,..|
-00001a00: 006a 077d 017c 0153 0074 016a 086b 0272  .j.}.|.S.t.j.k.r
-00001a10: 357c 006a 097d 017c 0153 007c 0153 00a9  5|.j.}.|.S.|.S..
-00001a20: 014e 290a 723a 0000 0072 1900 0000 721f  .N).r:...r....r.
-00001a30: 0000 0072 2400 0000 7220 0000 0072 3600  ...r$...r ...r6.
-00001a40: 0000 7221 0000 0072 3500 0000 7223 0000  ..r!...r5...r#..
-00001a50: 0072 3400 0000 2902 723b 0000 005a 0366  .r4...).r;...Z.f
-00001a60: 7073 7225 0000 0072 2500 0000 7226 0000  psr%...r%...r&..
-00001a70: 00da 1367 6574 5f61 6374 6976 655f 6d6f  ...get_active_mo
-00001a80: 6465 5f66 7073 1401 0000 7322 0000 0004  de_fps....s"....
-00001a90: 0104 010c 0102 0104 090c f802 0104 070c  ................
-00001aa0: fa06 0104 050c fc06 0104 0308 fe06 0108  ................
-00001ab0: 017a 1b53 6573 7369 6f6e 2e67 6574 5f61  .z.Session.get_a
-00001ac0: 6374 6976 655f 6d6f 6465 5f66 7073 6301  ctive_mode_fpsc.
-00001ad0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00001ae0: 0000 0043 0000 0073 3600 0000 7c00 a000  ...C...s6...|...
-00001af0: a100 7d01 7c01 6400 7501 7217 7c00 6a01  ..}.|.d.u.r.|.j.
-00001b00: a002 a100 4400 5d0b 5c02 7d02 7d03 7c03  ....D.].\.}.}.|.
-00001b10: a003 7c01 a101 0100 710d 6400 5300 6400  ..|.....q.d.S.d.
-00001b20: 5300 726a 0000 0029 0472 6b00 0000 722f  S.rj...).rk...r/
-00001b30: 0000 0072 3e00 0000 5a0e 7365 745f 6670  ...r>...Z.set_fp
-00001b40: 735f 7461 7267 6574 2904 723b 0000 005a  s_target).r;...Z
-00001b50: 0f61 6374 6976 655f 6d6f 6465 5f66 7073  .active_mode_fps
-00001b60: 7244 0000 0072 4500 0000 7225 0000 0072  rD...rE...r%...r
-00001b70: 2500 0000 7226 0000 0072 5e00 0000 2301  %...r&...r^...#.
-00001b80: 0000 730c 0000 0008 0108 0112 010c 0104  ..s.............
-00001b90: fe04 017a 1a53 6573 7369 6f6e 2e75 7064  ...z.Session.upd
-00001ba0: 6174 655f 7374 7265 616d 735f 6670 73da  ate_streams_fps.
-00001bb0: 0b74 7261 636b 696e 675f 6f6e 6302 0000  .tracking_onc...
-00001bc0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00001bd0: 0043 0000 0073 2200 0000 7c00 6a00 a001  .C...s"...|.j...
-00001be0: a100 4400 5d09 5c02 7d02 7d03 7c03 a002  ..D.].\.}.}.|...
-00001bf0: 7c01 a101 0100 7105 6400 5300 726a 0000  |.....q.d.S.rj..
-00001c00: 0029 0372 2f00 0000 723e 0000 005a 0f73  .).r/...r>...Z.s
-00001c10: 6574 5f74 7261 636b 696e 675f 6f6e 2904  et_tracking_on).
-00001c20: 723b 0000 0072 6c00 0000 7244 0000 0072  r;...rl...rD...r
-00001c30: 4500 0000 7225 0000 0072 2500 0000 7226  E...r%...r%...r&
-00001c40: 0000 0072 6300 0000 2901 0000 7306 0000  ...rc...)...s...
-00001c50: 0012 010c 0104 ff7a 1c53 6573 7369 6f6e  .......z.Session
-00001c60: 2e73 6574 5f73 7472 6561 6d73 5f74 7261  .set_streams_tra
-00001c70: 636b 696e 6763 0100 0000 0000 0000 0000  ckingc..........
-00001c80: 0000 0300 0000 0400 0000 4300 0000 733a  ..........C...s:
-00001c90: 0000 0074 00a0 0164 01a1 0101 0074 027c  ...t...d.....t.|
-00001ca0: 006a 0383 017c 005f 047c 006a 05a0 06a1  .j...|._.|.j....
-00001cb0: 0044 005d 0a5c 027d 017d 027c 02a0 077c  .D.].\.}.}.|...|
-00001cc0: 006a 04a1 0101 0071 1064 0053 0029 024e  .j.....q.d.S.).N
-00001cd0: 7a22 7570 6461 7469 6e67 2063 6861 7275  z"updating charu
-00001ce0: 636f 2069 6e20 6361 7365 206e 6563 6573  co in case neces
-00001cf0: 7361 7279 2908 7254 0000 0072 5500 0000  sary).rT...rU...
-00001d00: 7209 0000 0072 3800 0000 7239 0000 0072  r....r8...r9...r
-00001d10: 2f00 0000 723e 0000 005a 0e75 7064 6174  /...r>...Z.updat
-00001d20: 655f 7472 6163 6b65 7229 0372 3b00 0000  e_tracker).r;...
-00001d30: 7244 0000 0072 4500 0000 7225 0000 0072  rD...rE...r%...r
-00001d40: 2500 0000 7226 0000 0072 6200 0000 2d01  %...r&...rb...-.
-00001d50: 0000 730a 0000 000a 010c 0112 010e 0104  ..s.............
-00001d60: ff7a 1b53 6573 7369 6f6e 2e73 6574 5f73  .z.Session.set_s
-00001d70: 7472 6561 6d73 5f63 6861 7275 636f 6301  treams_charucoc.
-00001d80: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001d90: 0000 0043 0000 0073 1800 0000 7400 a001  ...C...s....t...
-00001da0: 6401 a101 0100 7c00 6a02 a003 a100 0100  d.....|.j.......
-00001db0: 6400 5300 2902 4e7a 1470 6175 7369 6e67  d.S.).Nz.pausing
-00001dc0: 2073 796e 6368 726f 6e69 7a65 7229 0472   synchronizer).r
-00001dd0: 5400 0000 7255 0000 0072 4100 0000 725f  T...rU...rA...r_
-00001de0: 0000 00a9 0172 3b00 0000 7225 0000 0072  .....r;...r%...r
-00001df0: 2500 0000 7226 0000 00da 1270 6175 7365  %...r&.....pause
-00001e00: 5f73 796e 6368 726f 6e69 7a65 7233 0100  _synchronizer3..
-00001e10: 0073 0400 0000 0a01 0e01 7a1a 5365 7373  .s........z.Sess
-00001e20: 696f 6e2e 7061 7573 655f 7379 6e63 6872  ion.pause_synchr
-00001e30: 6f6e 697a 6572 6301 0000 0000 0000 0000  onizerc.........
-00001e40: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00001e50: 1e00 0000 7c00 6a00 a001 a100 0100 7c00  ....|.j.......|.
-00001e60: 6a00 a002 7c00 6a00 6a03 a101 0100 6400  j...|.j.j.....d.
-00001e70: 5300 726a 0000 0029 0472 4100 0000 7265  S.rj...).rA...re
-00001e80: 0000 005a 0e73 6574 5f73 7472 6561 6d5f  ...Z.set_stream_
-00001e90: 6670 7372 6700 0000 726d 0000 0072 2500  fpsrg...rm...r%.
-00001ea0: 0000 7225 0000 0072 2600 0000 da14 756e  ..r%...r&.....un
-00001eb0: 7061 7573 655f 7379 6e63 6872 6f6e 697a  pause_synchroniz
-00001ec0: 6572 3701 0000 7304 0000 000a 0114 017a  er7...s........z
-00001ed0: 1c53 6573 7369 6f6e 2e75 6e70 6175 7365  .Session.unpause
-00001ee0: 5f73 796e 6368 726f 6e69 7a65 7263 0100  _synchronizerc..
-00001ef0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00001f00: 0000 4300 0000 7334 0000 0064 017d 017c  ..C...s4...d.}.|
-00001f10: 006a 006a 01a0 02a1 00a0 03a1 0044 005d  .j.j.........D.]
-00001f20: 0d5c 027d 027d 037c 02a0 0464 02a1 0172  .\.}.}.|...d...r
-00001f30: 177c 0164 0337 007d 0171 0a7c 0153 0029  .|.d.7.}.q.|.S.)
-00001f40: 044e 7201 0000 0072 4600 0000 e901 0000  .Nr....rF.......
-00001f50: 0029 0572 2800 0000 da04 6469 6374 da04  .).r(.....dict..
-00001f60: 636f 7079 723e 0000 00da 0a73 7461 7274  copyr>.....start
-00001f70: 7377 6974 6829 0472 3b00 0000 da05 636f  swith).r;.....co
-00001f80: 756e 74da 036b 6579 da06 7061 7261 6d73  unt..key..params
-00001f90: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-00001fa0: 1b67 6574 5f63 6f6e 6669 6775 7265 645f  .get_configured_
-00001fb0: 6361 6d65 7261 5f63 6f75 6e74 3b01 0000  camera_count;...
-00001fc0: 730c 0000 0004 0118 010a 0108 0102 8004  s...............
-00001fd0: 017a 2353 6573 7369 6f6e 2e67 6574 5f63  .z#Session.get_c
-00001fe0: 6f6e 6669 6775 7265 645f 6361 6d65 7261  onfigured_camera
-00001ff0: 5f63 6f75 6e74 6301 0000 0000 0000 0000  _countc.........
-00002000: 0000 0005 0000 0008 0000 0003 0000 0073  ...............s
-00002010: 8c00 0000 8700 6601 6401 6402 8408 7d01  ......f.d.d...}.
-00002020: 7400 8300 8f1e 7d02 7401 6403 7402 8302  t.....}.t.d.t...
-00002030: 4400 5d10 7d03 7c03 8800 6a03 a004 a100  D.].}.|...j.....
-00002040: 7600 7219 710f 7c02 a005 7c01 7c03 a102  v.r.q.|...|.|...
-00002050: 0100 710f 5700 6404 0400 0400 8303 0100  ..q.W.d.........
-00002060: 6e08 3100 732a 7701 0100 0100 0100 5900  n.1.s*w.......Y.
-00002070: 0100 8800 6a06 6a07 a008 a100 a004 a100  ....j.j.........
-00002080: 4400 5d0c 7d04 7c04 a009 6405 a101 7243  D.].}.|...d...rC
-00002090: 8800 6a06 6a07 7c04 3d00 7137 6404 5300  ..j.j.|.=.q7d.S.
-000020a0: 2906 7aa3 0a20 2020 2020 2020 2043 616c  ).z..        Cal
-000020b0: 6c65 6420 6279 206c 6f61 645f 7374 7265  led by load_stre
-000020c0: 616d 7320 696e 2074 6865 2065 7665 6e74  ams in the event
-000020d0: 2074 6861 7420 6e6f 2063 616d 6572 6173   that no cameras
-000020e0: 2061 7265 2072 6574 7572 6e65 6420 6279   are returned by
-000020f0: 2074 6865 2063 6f6e 6669 6775 7261 746f   the configurato
-00002100: 722e 2e2e 0a20 2020 2020 2020 2057 696c  r....        Wil
-00002110: 6c20 706f 7075 6c61 7465 2073 656c 662e  l populate self.
-00002120: 6361 6d65 7261 7320 7573 696e 6720 6d75  cameras using mu
-00002130: 6c74 6970 6c65 2074 6872 6561 6473 0a20  ltiple threads. 
-00002140: 2020 2020 2020 2063 0100 0000 0000 0000         c........
-00002150: 0000 0000 0200 0000 0700 0000 1300 0000  ................
-00002160: 738c 0000 007a 3774 00a0 0164 017c 009b  s....z7t...d.|..
-00002170: 009d 02a1 0101 0074 027c 0083 017d 0174  .......t.|...}.t
-00002180: 00a0 0164 027c 009b 009d 02a1 0101 007c  ...d.|.........|
-00002190: 0188 006a 037c 003c 0088 006a 04a0 057c  ...j.|.<...j...|
-000021a0: 01a1 0101 0074 00a0 0164 037c 009b 0064  .....t...d.|...d
-000021b0: 049d 03a1 0101 0074 067c 0174 0788 006a  .......t.|.t...j
-000021c0: 0883 0164 058d 0288 006a 097c 003c 0057  ...d.....j.|.<.W
-000021d0: 0064 0053 0001 0001 0001 0074 00a0 0164  .d.S.......t...d
-000021e0: 067c 009b 009d 02a1 0101 0059 0064 0053  .|.........Y.d.S
-000021f0: 0029 074e 7a0c 5472 7969 6e67 2070 6f72  .).Nz.Trying por
-00002200: 7420 7a10 5375 6363 6573 7320 6174 2070  t z.Success at p
-00002210: 6f72 7420 7a17 4c6f 6164 696e 6720 7374  ort z.Loading st
-00002220: 7265 616d 2061 7420 706f 7274 207a 2520  ream at port z% 
-00002230: 7769 7468 2063 6861 7275 636f 2074 7261  with charuco tra
-00002240: 636b 6572 2066 6f72 2063 616c 6962 7261  cker for calibra
-00002250: 7469 6f6e a901 da07 7472 6163 6b65 727a  tion....trackerz
-00002260: 124e 6f20 6361 6d65 7261 2061 7420 706f  .No camera at po
-00002270: 7274 2029 0a72 5400 0000 7255 0000 0072  rt ).rT...rU...r
-00002280: 0b00 0000 722e 0000 0072 2800 0000 5a0b  ....r....r(...Z.
-00002290: 7361 7665 5f63 616d 6572 6172 1600 0000  save_camerar....
-000022a0: 7209 0000 0072 3800 0000 722f 0000 0029  r....r8...r/...)
-000022b0: 0272 4400 0000 7246 0000 0072 6d00 0000  .rD...rF...rm...
-000022c0: 7225 0000 0072 2600 0000 da07 6164 645f  r%...r&.....add_
-000022d0: 6361 6d48 0100 0073 1c00 0000 0201 1001  camH...s........
-000022e0: 0801 1001 0a01 0c01 0401 0a01 04ff 0203  ................
-000022f0: 0a01 12ff 0603 1601 7a26 5365 7373 696f  ........z&Sessio
-00002300: 6e2e 5f66 696e 645f 6361 6d65 7261 732e  n._find_cameras.
-00002310: 3c6c 6f63 616c 733e 2e61 6464 5f63 616d  <locals>.add_cam
-00002320: 7201 0000 004e 5a06 7374 6572 656f 290a  r....NZ.stereo).
-00002330: 7204 0000 00da 0572 616e 6765 da15 4d41  r......range..MA
-00002340: 585f 4341 4d45 5241 5f50 4f52 545f 4348  X_CAMERA_PORT_CH
-00002350: 4543 4b72 2e00 0000 da04 6b65 7973 da06  ECKr......keys..
-00002360: 7375 626d 6974 7228 0000 0072 7100 0000  submitr(...rq...
-00002370: 7272 0000 0072 7300 0000 2905 723b 0000  rr...rs...).r;..
-00002380: 0072 7a00 0000 da08 6578 6563 7574 6f72  .rz.....executor
-00002390: da01 6972 7500 0000 7225 0000 0072 6d00  ..iru...r%...rm.
-000023a0: 0000 7226 0000 00da 0d5f 6669 6e64 5f63  ..r&....._find_c
-000023b0: 616d 6572 6173 4201 0000 731a 0000 000c  amerasB...s.....
-000023c0: 0608 100e 010e 0102 020e 0202 fb1c ff14  ................
-000023d0: 090a 010a 0102 8004 fe7a 1553 6573 7369  .........z.Sessi
-000023e0: 6f6e 2e5f 6669 6e64 5f63 616d 6572 6173  on._find_cameras
-000023f0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00002400: 0005 0000 0043 0000 0073 d000 0000 6401  .....C...s....d.
-00002410: 7c00 5f00 7c00 6a01 a002 a100 7c00 5f03  |._.|.j.....|._.
-00002420: 7404 7c00 6a03 8301 6402 6b02 7214 7c00  t.|.j...d.k.r.|.
-00002430: a005 a100 0100 7c00 6a03 a006 a100 4400  ......|.j.....D.
-00002440: 5d1e 5c02 7d01 7d02 7c01 7c00 6a07 a008  ].\.}.}.|.|.j...
-00002450: a100 7600 7225 7119 7409 a00a 6403 7c01  ..v.r%q.t...d.|.
-00002460: 9b00 9d02 a101 0100 740b 7c02 7c00 6a0c  ........t.|.|.j.
-00002470: 6404 8d02 7c00 6a07 7c01 3c00 7119 7c00  d...|.j.|.<.q.|.
-00002480: a00d a100 0100 7c00 a00e a100 0100 740f  ......|.......t.
-00002490: 7c00 6a10 a008 a100 8301 7c00 5f11 7412  |.j.......|._.t.
-000024a0: 7c00 6a07 8301 7c00 5f13 6401 7c00 5f14  |.j...|._.d.|._.
-000024b0: 6405 7c00 5f00 7409 a00a 6406 a101 0100  d.|._.t...d.....
-000024c0: 7c00 6a15 a016 a100 0100 7c00 a017 a100  |.j.......|.....
-000024d0: 0100 7c00 a018 a100 0100 6407 5300 2908  ..|.......d.S.).
-000024e0: 7aad 0a20 2020 2020 2020 2043 6f6e 6e65  z..        Conne
-000024f0: 6374 7320 746f 2073 746f 7265 6420 6361  cts to stored ca
-00002500: 6d65 7261 7320 616e 6420 6372 6561 7465  meras and create
-00002510: 7320 7374 7265 616d 7320 7769 7468 2070  s streams with p
-00002520: 726f 7669 6465 6420 7472 6163 6b69 6e67  rovided tracking
-00002530: 0a20 2020 2020 2020 2042 6563 6175 7365  .        Because
-00002540: 2074 6865 7365 2073 7472 6561 6d73 2061   these streams a
-00002550: 7265 2061 7661 696c 6162 6c65 2c20 7468  re available, th
-00002560: 6520 7379 6e63 6872 6f6e 697a 6572 2063  e synchronizer c
-00002570: 616e 2074 6865 6e20 6265 2069 6e69 7469  an then be initi
-00002580: 616c 697a 6564 0a20 2020 2020 2020 2054  alized.        T
-00002590: 7201 0000 007a 184c 6f61 6469 6e67 2053  r....z.Loading S
-000025a0: 7472 6561 6d20 666f 7220 706f 7274 2072  tream for port r
-000025b0: 7800 0000 467a 2d53 6967 6e61 6c6c 696e  x...Fz-Signallin
-000025c0: 6720 7375 6363 6573 7366 756c 206c 6f61  g successful loa
-000025d0: 6469 6e67 206f 6620 7374 7265 616d 2074  ding of stream t
-000025e0: 6f6f 6c73 4e29 1972 3000 0000 7228 0000  oolsN).r0...r(..
-000025f0: 005a 0b67 6574 5f63 616d 6572 6173 722e  .Z.get_camerasr.
-00002600: 0000 0072 4900 0000 7281 0000 0072 3e00  ...rI...r....r>.
-00002610: 0000 722f 0000 0072 7d00 0000 7254 0000  ..r/...r}...rT..
-00002620: 0072 5500 0000 7216 0000 0072 3900 0000  .rU...r....r9...
-00002630: da13 5f61 646a 7573 745f 7265 736f 6c75  .._adjust_resolu
-00002640: 7469 6f6e 73da 155f 6c6f 6164 5f6d 6f6e  tions.._load_mon
-00002650: 6f63 616c 6962 7261 746f 7273 da03 6d69  ocalibrators..mi
-00002660: 6e72 3200 0000 7233 0000 0072 0c00 0000  nr2...r3...r....
-00002670: 7241 0000 0072 3100 0000 da1a 7374 7265  rA...r1.....stre
-00002680: 616d 5f74 6f6f 6c73 5f6c 6f61 6465 645f  am_tools_loaded_
-00002690: 7369 676e 616c 7243 0000 0072 6000 0000  signalrC...r`...
-000026a0: 726e 0000 00a9 0372 3b00 0000 7244 0000  rn.....r;...rD..
-000026b0: 0072 4600 0000 7225 0000 0072 2500 0000  .rF...r%...r%...
-000026c0: 7226 0000 0072 6100 0000 6501 0000 732a  r&...ra...e...s*
-000026d0: 0000 0006 050c 020e 0208 0112 020e 0102  ................
-000026e0: 0110 0216 0108 0208 0110 0302 0204 0106  ................
-000026f0: ff06 0506 010a 010a 0108 020c 017a 1953  .............z.S
-00002700: 6573 7369 6f6e 2e6c 6f61 645f 7374 7265  ession.load_stre
-00002710: 616d 5f74 6f6f 6c73 6301 0000 0000 0000  am_toolsc.......
-00002720: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
-00002730: 0073 5e00 0000 7c00 6a00 a001 a100 4400  .s^...|.j.....D.
-00002740: 5d27 5c02 7d01 7d02 7c01 7c00 6a02 a003  ]'\.}.}.|.|.j...
-00002750: a100 7600 721a 7404 a005 6401 7c01 9b00  ..v.r.t...d.|...
-00002760: 6402 9d03 a101 0100 7105 7404 a005 6403  d.......q.t...d.
-00002770: 7c01 9b00 9d02 a101 0100 7406 7c00 6a07  |.........t.|.j.
-00002780: 7c01 1900 8301 7c00 6a02 7c01 3c00 7105  |.....|.j.|.<.q.
-00002790: 6400 5300 2904 4e7a 2f53 6b69 7070 696e  d.S.).Nz/Skippin
-000027a0: 6720 6f76 6572 206d 6f6e 6f63 616c 6962  g over monocalib
-000027b0: 7261 746f 7220 6372 6561 7469 6f6e 2066  rator creation f
-000027c0: 6f72 2070 6f72 7420 7a1b 2062 6563 6175  or port z. becau
-000027d0: 7365 2069 7420 616c 7265 6164 7920 6578  se it already ex
-000027e0: 6973 7473 2e7a 204c 6f61 6469 6e67 204d  ists.z Loading M
-000027f0: 6f6e 6f63 616c 6962 7261 746f 7220 666f  onocalibrator fo
-00002800: 7220 706f 7274 2029 0872 2e00 0000 723e  r port ).r....r>
-00002810: 0000 0072 3200 0000 727d 0000 0072 5400  ...r2...r}...rT.
-00002820: 0000 7255 0000 0072 0a00 0000 722f 0000  ..rU...r....r/..
-00002830: 0072 8600 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00002840: 7226 0000 0072 8300 0000 8b01 0000 7312  r&...r........s.
-00002850: 0000 0012 010e 0104 010a 0104 ff02 0310  ................
-00002860: 0216 0104 f87a 1d53 6573 7369 6f6e 2e5f  .....z.Session._
-00002870: 6c6f 6164 5f6d 6f6e 6f63 616c 6962 7261  load_monocalibra
-00002880: 746f 7273 4eda 0b61 6374 6976 655f 706f  torsN..active_po
-00002890: 7274 6302 0000 0000 0000 0000 0000 0002  rtc.............
-000028a0: 0000 0005 0000 0043 0000 0073 4600 0000  .......C...sF...
-000028b0: 7c01 6401 7501 720f 7400 a001 6402 7c01  |.d.u.r.t...d.|.
-000028c0: 9b00 9d02 a101 0100 7c01 7c00 5f02 7400  ........|.|._.t.
-000028d0: a001 6403 7c00 6a02 9b00 6404 9d03 a101  ..d.|.j...d.....
-000028e0: 0100 7c00 6a03 7c00 6a02 1900 a004 a100  ..|.j.|.j.......
-000028f0: 0100 6401 5300 2905 7a7e 0a20 2020 2020  ..d.S.).z~.     
-00002900: 2020 2055 7365 6420 746f 206d 616b 6520     Used to make 
-00002910: 7375 7265 2074 6861 7420 6f6e 6c79 2074  sure that only t
-00002920: 6865 2061 6374 6976 6520 6361 6d65 7261  he active camera
-00002930: 2074 6162 2069 7320 7265 6164 696e 6720   tab is reading 
-00002940: 6672 616d 6573 2064 7572 696e 6720 7468  frames during th
-00002950: 6520 696e 7472 696e 7369 6320 6361 6c69  e intrinsic cali
-00002960: 6272 6174 696f 6e20 7072 6f63 6573 730a  bration process.
-00002970: 2020 2020 2020 2020 4e7a 2953 6574 7469          Nz)Setti
-00002980: 6e67 2073 6573 7369 6f6e 2061 6374 6976  ng session activ
-00002990: 6520 6d6f 6e6f 6361 6c69 6272 6174 6f72  e monocalibrator
-000029a0: 2074 6f20 7a1a 4163 7469 7661 7465 2074   to z.Activate t
-000029b0: 7261 636b 696e 6720 6f6e 2070 6f72 7420  racking on port 
-000029c0: 7a16 2061 6e64 2064 6561 6374 6976 6174  z. and deactivat
-000029d0: 6520 6f74 6865 7273 2905 7254 0000 0072  e others).rT...r
-000029e0: 5500 0000 7233 0000 0072 3200 0000 5a13  U...r3...r2...Z.
-000029f0: 7375 6273 6372 6962 655f 746f 5f73 7472  subscribe_to_str
-00002a00: 6561 6d29 0272 3b00 0000 7287 0000 0072  eam).r;...r....r
-00002a10: 2500 0000 7225 0000 0072 2600 0000 7264  %...r%...r&...rd
-00002a20: 0000 0096 0100 0073 0e00 0000 0805 1001  .......s........
-00002a30: 0601 0401 0c01 04ff 1403 7a1f 5365 7373  ..........z.Sess
-00002a40: 696f 6e2e 6163 7469 7661 7465 5f6d 6f6e  ion.activate_mon
-00002a50: 6f63 616c 6962 7261 746f 7263 0100 0000  ocalibratorc....
-00002a60: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00002a70: 4300 0000 732a 0000 0074 00a0 0164 01a1  C...s*...t...d..
-00002a80: 0101 007c 006a 02a0 03a1 0044 005d 085c  ...|.j.....D.].\
-00002a90: 027d 017d 027c 02a0 04a1 0001 0071 0a64  .}.}.|.......q.d
-00002aa0: 0253 0029 037a 8b0a 2020 2020 2020 2020  .S.).z..        
-00002ab0: 7573 6564 2077 6865 6e20 6e6f 7420 6163  used when not ac
-00002ac0: 7469 7665 6c79 206f 6e20 7468 6520 6361  tively on the ca
-00002ad0: 6d65 7261 2063 616c 6962 7261 7469 6f6e  mera calibration
-00002ae0: 2074 6162 0a20 2020 2020 2020 206f 7220   tab.        or 
-00002af0: 7768 656e 2073 696c 656e 6369 6e67 2061  when silencing a
-00002b00: 6c6c 2069 6e20 7072 6570 6172 6174 696f  ll in preparatio
-00002b10: 6e20 666f 7220 6163 7469 7661 7469 6e67  n for activating
-00002b20: 206f 6e6c 7920 6f6e 650a 2020 2020 2020   only one.      
-00002b30: 2020 7a25 5061 7573 696e 6720 616c 6c20    z%Pausing all 
-00002b40: 6d6f 6e6f 6361 6c69 6272 6174 6f72 206c  monocalibrator l
-00002b50: 6f6f 7069 6e67 2e2e 2e4e 2905 7254 0000  ooping...N).rT..
-00002b60: 0072 5500 0000 7232 0000 0072 3e00 0000  .rU...r2...r>...
-00002b70: 5a15 756e 7375 6273 6372 6962 655f 746f  Z.unsubscribe_to
-00002b80: 5f73 7472 6561 6d29 0372 3b00 0000 7244  _stream).r;...rD
-00002b90: 0000 0072 4700 0000 7225 0000 0072 2500  ...rG...r%...r%.
-00002ba0: 0000 7226 0000 0072 6000 0000 a301 0000  ..r&...r`.......
-00002bb0: 7308 0000 000a 0512 010a 0104 ff7a 2153  s............z!S
-00002bc0: 6573 7369 6f6e 2e70 6175 7365 5f61 6c6c  ession.pause_all
-00002bd0: 5f6d 6f6e 6f63 616c 6962 7261 746f 7273  _monocalibrators
-00002be0: 46da 1564 6573 7469 6e61 7469 6f6e 5f64  F..destination_d
-00002bf0: 6972 6563 746f 7279 da13 7374 6f72 655f  irectory..store_
-00002c00: 706f 696e 745f 6869 7374 6f72 7963 0300  point_historyc..
-00002c10: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00002c20: 0000 4300 0000 733e 0000 0074 00a0 0164  ..C...s>...t...d
-00002c30: 01a1 0101 007c 016a 0264 0264 0264 038d  .....|.j.d.d.d..
-00002c40: 0201 0074 037c 006a 0483 017c 005f 057c  ...t.|.j...|._.|
-00002c50: 006a 056a 067c 017c 0264 048d 0201 0064  .j.j.|.|.d.....d
-00002c60: 027c 005f 0764 0053 0029 054e 7a17 496e  .|._.d.S.).Nz.In
-00002c70: 6974 6961 7469 6e67 2072 6563 6f72 6469  itiating recordi
-00002c80: 6e67 2e2e 2e54 2902 da07 7061 7265 6e74  ng...T)...parent
-00002c90: 73da 0865 7869 7374 5f6f 6b29 0172 8900  s..exist_ok).r..
-00002ca0: 0000 2908 7254 0000 0072 5500 0000 da05  ..).rT...rU.....
-00002cb0: 6d6b 6469 7272 1700 0000 7241 0000 00da  mkdirr....rA....
-00002cc0: 0e76 6964 656f 5f72 6563 6f72 6465 72da  .video_recorder.
-00002cd0: 0f73 7461 7274 5f72 6563 6f72 6469 6e67  .start_recording
-00002ce0: 7237 0000 0029 0372 3b00 0000 7288 0000  r7...).r;...r...
-00002cf0: 0072 8900 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00002d00: 7226 0000 0072 8e00 0000 ac01 0000 730e  r&...r........s.
-00002d10: 0000 000a 030e 010c 0206 0104 0106 ff0a  ................
-00002d20: 037a 1753 6573 7369 6f6e 2e73 7461 7274  .z.Session.start
-00002d30: 5f72 6563 6f72 6469 6e67 6301 0000 0000  _recordingc.....
-00002d40: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00002d50: 0000 0073 6a00 0000 7400 a001 6401 a101  ...sj...t...d...
-00002d60: 0100 7c00 6a02 a003 a100 0100 7c00 6a02  ..|.j.......|.j.
-00002d70: 6a04 721b 7400 a001 6402 a101 0100 7405  j.r.t...d.....t.
-00002d80: 6403 8301 0100 7c00 6a02 6a04 730e 6404  d.....|.j.j.s.d.
-00002d90: 7c00 5f06 7400 a001 6405 a101 0100 7c00  |._.t...d.....|.
-00002da0: 6a07 a008 a100 0100 7c00 a009 a100 7233  j.......|.....r3
-00002db0: 7c00 6a0a a008 a100 0100 6400 5300 6400  |.j.......d.S.d.
-00002dc0: 5300 2906 4e7a 1553 746f 7070 696e 6720  S.).Nz.Stopping 
-00002dd0: 7265 636f 7264 696e 672e 2e2e 7a2e 5761  recording...z.Wa
-00002de0: 6974 696e 6720 666f 7220 7669 6465 6f20  iting for video 
-00002df0: 7265 636f 7264 6572 2074 6f20 7361 7665  recorder to save
-00002e00: 206f 7574 2064 6174 612e 2e2e 6700 0000   out data...g...
-00002e10: 0000 00e0 3f46 7a3d 5265 636f 7264 696e  ....?Fz=Recordin
-00002e20: 6720 6f66 2066 7261 6d65 7320 6973 2063  g of frames is c
-00002e30: 6f6d 706c 6574 652e 2e2e 7369 676e 616c  omplete...signal
-00002e40: 6c69 6e67 2063 6861 6e67 6520 696e 2073  ling change in s
-00002e50: 7461 7475 7329 0b72 5400 0000 7255 0000  tatus).rT...rU..
-00002e60: 0072 8d00 0000 da0e 7374 6f70 5f72 6563  .r......stop_rec
-00002e70: 6f72 6469 6e67 5a09 7265 636f 7264 696e  ordingZ.recordin
-00002e80: 6772 0600 0000 7237 0000 00da 1972 6563  gr....r7.....rec
-00002e90: 6f72 6469 6e67 5f63 6f6d 706c 6574 655f  ording_complete_
-00002ea0: 7369 676e 616c 7243 0000 0072 5d00 0000  signalrC...r]...
-00002eb0: da15 756e 6c6f 636b 5f70 6f73 7470 726f  ..unlock_postpro
-00002ec0: 6365 7373 696e 6772 6d00 0000 7225 0000  cessingrm...r%..
-00002ed0: 0072 2500 0000 7226 0000 0072 8f00 0000  .r%...r&...r....
-00002ee0: b801 0000 7318 0000 000a 010a 0108 010a  ....s...........
-00002ef0: 0108 0108 fe06 040a 020a 0108 020e 0104  ................
-00002f00: ff7a 1653 6573 7369 6f6e 2e73 746f 705f  .z.Session.stop_
-00002f10: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
-00002f20: 0000 0000 0000 0400 0000 0800 0000 0300  ................
-00002f30: 0000 7354 0000 0087 0066 0164 0164 0284  ..sT.....f.d.d..
-00002f40: 087d 0174 0083 008f 177d 0288 006a 01a0  .}.t.....}...j..
-00002f50: 02a1 0044 005d 087d 037c 02a0 037c 017c  ...D.].}.|...|.|
-00002f60: 03a1 0201 0071 0f57 0064 0304 0004 0083  .....q.W.d......
-00002f70: 0301 0064 0353 0031 0073 2377 0101 0001  ...d.S.1.s#w....
-00002f80: 0001 0059 0001 0064 0353 0029 047a 8243  ...Y...d.S.).z.C
-00002f90: 6861 6e67 6573 2074 6865 2063 616d 6572  hanges the camer
-00002fa0: 6120 7265 736f 6c75 7469 6f6e 2074 6f20  a resolution to 
-00002fb0: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
-00002fc0: 2063 6f6e 6669 6775 7261 7469 6f6e 2c20   configuration, 
-00002fd0: 6173 0a20 2020 2020 2020 206c 6f67 2061  as.        log a
-00002fe0: 7320 6974 2069 7320 6e6f 7420 636f 6e66  s it is not conf
-00002ff0: 6967 7572 6564 2066 6f72 2074 6865 2064  igured for the d
-00003000: 6566 6175 6c74 2072 6573 6f6c 7574 696f  efault resolutio
-00003010: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
-00003020: 0000 0a00 0000 1300 0000 73b6 0000 0088  ..........s.....
-00003030: 006a 007c 0019 007d 0188 006a 016a 0264  .j.|...}...j.j.d
-00003040: 017c 009b 009d 0219 0064 0219 007d 0288  .|.......d...}..
-00003050: 006a 037c 0019 006a 047d 037c 0264 0319  .j.|...j.}.|.d..
-00003060: 007c 0364 0319 006b 0373 267c 0264 0419  .|.d...k.s&|.d..
-00003070: 007c 0364 0419 006b 0372 5974 05a0 0664  .|.d...k.rYt...d
-00003080: 057c 009b 0064 067c 0364 0364 0785 0219  .|...d.|.d.d....
-00003090: 009b 0064 087c 0264 0364 0785 0219 009b  ...d.|.d.d......
-000030a0: 009d 06a1 0101 007c 01a0 077c 02a1 0101  .......|...|....
-000030b0: 0074 05a0 0664 097c 009b 0064 067c 0364  .t...d.|...d.|.d
-000030c0: 0364 0785 0219 009b 0064 087c 0264 0364  .d.......d.|.d.d
-000030d0: 0785 0219 009b 009d 06a1 0101 0064 0053  .............d.S
-000030e0: 0064 0053 0029 0a4e 5a04 6361 6d5f da04  .d.S.).NZ.cam_..
-000030f0: 7369 7a65 7201 0000 0072 7000 0000 7a27  sizer....rp...z'
-00003100: 4265 6769 6e6e 696e 6720 746f 2063 6861  Beginning to cha
-00003110: 6e67 6520 7265 736f 6c75 7469 6f6e 2061  nge resolution a
-00003120: 7420 706f 7274 207a 0620 6672 6f6d 2072  t port z. from r
-00003130: 5100 0000 7a04 2074 6f20 7a27 436f 6d70  Q...z. to z'Comp
-00003140: 6c65 7465 6420 6368 616e 6765 206f 6620  leted change of 
-00003150: 7265 736f 6c75 7469 6f6e 2061 7420 706f  resolution at po
-00003160: 7274 2029 0872 2f00 0000 7228 0000 0072  rt ).r/...r(...r
-00003170: 7100 0000 722e 0000 005a 1264 6566 6175  q...r....Z.defau
-00003180: 6c74 5f72 6573 6f6c 7574 696f 6e72 5400  lt_resolutionrT.
-00003190: 0000 7255 0000 005a 1163 6861 6e67 655f  ..rU...Z.change_
-000031a0: 7265 736f 6c75 7469 6f6e 2904 7244 0000  resolution).rD..
-000031b0: 0072 4500 0000 7292 0000 005a 0c64 6566  .rE...r....Z.def
-000031c0: 6175 6c74 5f73 697a 6572 6d00 0000 7225  ault_sizerm...r%
-000031d0: 0000 0072 2600 0000 da11 6164 6a75 7374  ...r&.....adjust
-000031e0: 5f72 6573 5f77 6f72 6b65 72cb 0100 0073  _res_worker....s
-000031f0: 1800 0000 0a01 1601 0c01 2002 0401 2401  .......... ...$.
-00003200: 04ff 0a03 0401 2401 08ff 04fb 7a36 5365  ......$.....z6Se
-00003210: 7373 696f 6e2e 5f61 646a 7573 745f 7265  ssion._adjust_re
-00003220: 736f 6c75 7469 6f6e 732e 3c6c 6f63 616c  solutions.<local
-00003230: 733e 2e61 646a 7573 745f 7265 735f 776f  s>.adjust_res_wo
-00003240: 726b 6572 4e29 0472 0400 0000 722e 0000  rkerN).r....r...
-00003250: 0072 7d00 0000 727e 0000 0029 0472 3b00  .r}...r~...).r;.
-00003260: 0000 7293 0000 0072 7f00 0000 7244 0000  ..r....r....rD..
-00003270: 0072 2500 0000 726d 0000 0072 2600 0000  .r%...rm...r&...
-00003280: 7282 0000 00c7 0100 0073 0c00 0000 0c04  r........s......
-00003290: 080e 0e01 0e01 02ff 22ff 7a1b 5365 7373  ........".z.Sess
-000032a0: 696f 6e2e 5f61 646a 7573 745f 7265 736f  ion._adjust_reso
-000032b0: 6c75 7469 6f6e 7363 0100 0000 0000 0000  lutionsc........
-000032c0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-000032d0: 737a 0000 007c 006a 00a0 01a1 007c 005f  sz...|.j.....|._
-000032e0: 027c 006a 00a0 03a1 007c 005f 0474 057c  .|.j.....|._.t.|
-000032f0: 006a 047c 006a 0283 027c 005f 067c 006a  .j.|.j...|._.|.j
-00003300: 006a 0764 0119 0064 0219 007c 006a 065f  .j.d...d...|.j._
-00003310: 0864 037c 006a 006a 0764 0119 00a0 09a1  .d.|.j.j.d......
-00003320: 0076 0072 327c 006a 006a 0764 0119 0064  .v.r2|.j.j.d...d
-00003330: 0319 007c 006a 065f 0a74 0b7c 006a 067c  ...|.j._.t.|.j.|
-00003340: 006a 0c64 048d 027c 005f 0d64 0553 0029  .j.d...|._.d.S.)
-00003350: 067a f30a 2020 2020 2020 2020 466f 6c6c  .z..        Foll
-00003360: 6f77 696e 6720 6361 7074 7572 6520 766f  owing capture vo
-00003370: 6c75 6d65 206f 7074 696d 697a 6174 696f  lume optimizatio
-00003380: 6e20 7669 6120 6275 6e64 6c65 2061 646a  n via bundle adj
-00003390: 7573 746d 656e 742c 206f 7220 616c 7465  ustment, or alte
-000033a0: 7261 7469 6f6e 0a20 2020 2020 2020 2076  ration.        v
-000033b0: 6961 2061 2074 7261 6e73 666f 726d 206f  ia a transform o
-000033c0: 6620 7468 6520 6f72 6967 696e 2c20 7468  f the origin, th
-000033d0: 6520 656e 7469 7265 2063 6170 7475 7265  e entire capture
-000033e0: 2076 6f6c 756d 6520 6361 6e20 6265 2072   volume can be r
-000033f0: 656c 6f61 6465 640a 2020 2020 2020 2020  eloaded.        
-00003400: 6672 6f6d 2074 6865 2063 6f6e 6669 6720  from the config 
-00003410: 6461 7461 2077 6974 686f 7574 206e 6565  data without nee
-00003420: 6469 6e67 2074 6f20 676f 2074 6872 6f75  ding to go throu
-00003430: 6768 2074 6865 2073 7465 7073 0a0a 2020  gh the steps..  
-00003440: 2020 2020 2020 da0e 6361 7074 7572 655f        ..capture_
-00003450: 766f 6c75 6d65 da05 7374 6167 65da 116f  volume..stage..o
-00003460: 7269 6769 6e5f 7379 6e63 5f69 6e64 6578  rigin_sync_index
-00003470: 2901 7238 0000 004e 290e 7228 0000 0072  ).r8...N).r(...r
-00003480: 1400 0000 da0f 706f 696e 745f 6573 7469  ......point_esti
-00003490: 6d61 7465 7372 4d00 0000 724e 0000 0072  matesrM...rN...r
-000034a0: 1100 0000 7294 0000 0072 7100 0000 7295  ....r....rq...r.
-000034b0: 0000 0072 7d00 0000 7296 0000 0072 1200  ...r}...r....r..
-000034c0: 0000 7238 0000 00da 1271 7561 6c69 7479  ..r8.....quality
-000034d0: 5f63 6f6e 7472 6f6c 6c65 7272 6d00 0000  _controllerrm...
-000034e0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-000034f0: 1d6c 6f61 645f 6573 7469 6d61 7465 645f  .load_estimated_
-00003500: 6361 7074 7572 655f 766f 6c75 6d65 dd01  capture_volume..
-00003510: 0000 7316 0000 000c 070c 0110 0114 0214  ..s.............
-00003520: 010a 0102 0108 ff02 0508 010c ff7a 2553  .............z%S
-00003530: 6573 7369 6f6e 2e6c 6f61 645f 6573 7469  ession.load_esti
-00003540: 6d61 7465 645f 6361 7074 7572 655f 766f  mated_capture_vo
-00003550: 6c75 6d65 6301 0000 0000 0000 0000 0000  lumec...........
-00003560: 0002 0000 0005 0000 0043 0000 0073 a600  .........C...s..
-00003570: 0000 7400 7c00 6a01 6a02 7c00 6a03 8302  ..t.|.j.j.|.j...
-00003580: 7d01 7c01 6a04 6401 6402 8d01 0100 7405  }.|.j.d.d.....t.
-00003590: 7c00 6a01 6a02 8301 a006 a100 7c00 5f07  |.j.j.......|._.
-000035a0: 7408 7c00 6a07 7c00 6a03 8302 7c00 5f09  t.|.j.|.j...|._.
-000035b0: 740a 7c00 6a07 7c00 6a09 8302 7c00 5f0b  t.|.j.|.j...|._.
-000035c0: 7c00 6a0b a00c a100 0100 740d 7c00 6a0b  |.j.......t.|.j.
-000035d0: 7c00 6a0e 8302 7c00 5f0f 7410 a011 6403  |.j...|._.t...d.
-000035e0: 7412 6404 1400 9b00 6405 9d03 a101 0100  t.d.....d.......
-000035f0: 7c00 6a0f a013 7412 a101 0100 7c00 6a0b  |.j...t.....|.j.
-00003600: a00c a100 0100 7c00 6a01 a014 7c00 6a0b  ......|.j...|.j.
-00003610: a101 0100 6406 5300 2907 7ad7 0a20 2020  ....d.S.).z..   
-00003620: 2020 2020 2054 6869 7320 6973 2077 6865       This is whe
-00003630: 7265 2074 6865 2063 616d 6572 6120 6172  re the camera ar
-00003640: 7261 7920 3620 446f 4620 6973 2073 6574  ray 6 DoF is set
-00003650: 2e20 4d61 6e79 2c20 6d61 6e79 2074 6869  . Many, many thi
-00003660: 6e67 7320 6172 6520 6861 7070 656e 696e  ngs are happenin
-00003670: 670a 2020 2020 2020 2020 6865 7265 2c20  g.        here, 
-00003680: 6275 7420 7468 6579 2061 7265 2061 6c6c  but they are all
-00003690: 206e 6563 6573 7361 7279 2073 7465 7073   necessary steps
-000036a0: 206f 6620 7468 6520 7072 6f63 6573 7320   of the process 
-000036b0: 736f 2049 2064 6964 6e27 7420 7761 6e74  so I didn't want
-000036c0: 2074 6f0a 2020 2020 2020 2020 7472 7920   to.        try 
-000036d0: 746f 2065 6e63 6170 7375 6c61 7465 2061  to encapsulate a
-000036e0: 6e79 2066 7572 7468 6572 0a20 2020 2020  ny further.     
-000036f0: 2020 2072 1800 0000 2901 5a0e 626f 6172     r....).Z.boar
-00003700: 6473 5f73 616d 706c 6564 7a1b 5265 6d6f  ds_sampledz.Remo
-00003710: 7669 6e67 2074 6865 2077 6f72 7374 2066  ving the worst f
-00003720: 6974 7469 6e67 20e9 6400 0000 7a21 2070  itting .d...z! p
-00003730: 6572 6365 6e74 206f 6620 706f 696e 7473  ercent of points
-00003740: 2066 726f 6d20 7468 6520 6d6f 6465 6c4e   from the modelN
-00003750: 2915 720f 0000 0072 2800 0000 5a09 746f  ).r....r(...Z.to
-00003760: 6d6c 5f70 6174 6872 2d00 0000 5a14 7374  ml_pathr-...Z.st
-00003770: 6572 656f 5f63 616c 6962 7261 7465 5f61  ereo_calibrate_a
-00003780: 6c6c 720d 0000 005a 1567 6574 5f62 6573  llr....Z.get_bes
-00003790: 745f 6361 6d65 7261 5f61 7272 6179 724e  t_camera_arrayrN
-000037a0: 0000 0072 1400 0000 7297 0000 0072 1100  ...r....r....r..
-000037b0: 0000 7294 0000 00da 086f 7074 696d 697a  ..r......optimiz
-000037c0: 6572 1200 0000 7238 0000 0072 9800 0000  er....r8...r....
-000037d0: 7254 0000 0072 5500 0000 da11 4649 4c54  rT...rU.....FILT
-000037e0: 4552 4544 5f46 5241 4354 494f 4e5a 1666  ERED_FRACTIONZ.f
-000037f0: 696c 7465 725f 706f 696e 745f 6573 7469  ilter_point_esti
-00003800: 6d61 7465 735a 1373 6176 655f 6361 7074  matesZ.save_capt
-00003810: 7572 655f 766f 6c75 6d65 2902 723b 0000  ure_volume).r;..
-00003820: 005a 1073 7465 7265 6f63 616c 6962 7261  .Z.stereocalibra
-00003830: 746f 7272 2500 0000 7225 0000 0072 2600  torr%...r%...r&.
-00003840: 0000 da13 6573 7469 6d61 7465 5f65 7874  ....estimate_ext
-00003850: 7269 6e73 6963 73f3 0100 0073 2a00 0000  rinsics....s*...
-00003860: 0206 0a01 04ff 0c03 0202 0601 02ff 0402  ................
-00003870: 04fe 0204 0801 06ff 1004 0a01 1002 0402  ................
-00003880: 0e01 04ff 0c03 0a01 1202 7a1b 5365 7373  ..........z.Sess
-00003890: 696f 6e2e 6573 7469 6d61 7465 5f65 7874  ion.estimate_ext
-000038a0: 7269 6e73 6963 7372 6a00 0000 2901 4629  rinsicsrj...).F)
-000038b0: 2972 1b00 0000 721c 0000 0072 1d00 0000  )r....r....r....
-000038c0: 7203 0000 0072 8500 0000 7242 0000 0072  r....r....rB...r
-000038d0: 9100 0000 7290 0000 0072 1900 0000 5a13  ....r....r....Z.
-000038e0: 6d6f 6465 5f63 6861 6e67 655f 7375 6363  mode_change_succ
-000038f0: 6573 7372 1500 0000 722a 0000 0072 4800  essr....r*...rH.
-00003900: 0000 724b 0000 0072 5000 0000 7257 0000  ..rK...rP...rW..
-00003910: 0072 5900 0000 725d 0000 0072 6600 0000  .rY...r]...rf...
-00003920: da03 696e 7472 6800 0000 726b 0000 0072  ..intrh...rk...r
-00003930: 5e00 0000 da04 626f 6f6c 7263 0000 0072  ^.....boolrc...r
-00003940: 6200 0000 726e 0000 0072 6f00 0000 7277  b...rn...ro...rw
-00003950: 0000 0072 8100 0000 7261 0000 0072 8300  ...r....ra...r..
-00003960: 0000 7264 0000 0072 6000 0000 7205 0000  ..rd...r`...r...
-00003970: 0072 8e00 0000 728f 0000 0072 8200 0000  .r....r....r....
-00003980: 7299 0000 0072 9d00 0000 da0d 5f5f 636c  r....r......__cl
-00003990: 6173 7363 656c 6c5f 5f72 2500 0000 7225  asscell__r%...r%
-000039a0: 0000 0072 3c00 0000 7226 0000 0072 2700  ...r<...r&...r'.
-000039b0: 0000 3000 0000 734a 0000 0008 0006 0106  ..0...sJ........
-000039c0: 0106 0106 0108 0212 0208 2208 1208 0708  ..........".....
-000039d0: 0b08 1d08 1e0e 0d0e 380e 1608 0f0e 0608  ........8.......
-000039e0: 0408 0608 0408 0408 0708 2308 2610 0b08  ..........#.&...
-000039f0: 0d02 0a04 ff02 0102 ff02 010a ff08 0c08  ................
-00003a00: 0f08 1610 1672 2700 0000 2933 da0d 7079  .....r'...)3..py
-00003a10: 7879 3364 2e6c 6f67 6765 72da 0670 7978  xy3d.logger..pyx
-00003a20: 7933 6472 5400 0000 da03 6765 7472 1b00  y3drT.....getr..
-00003a30: 0000 da0c 5079 5174 362e 5174 436f 7265  ....PyQt6.QtCore
-00003a40: 7202 0000 0072 0300 0000 5a12 636f 6e63  r....r....Z.conc
-00003a50: 7572 7265 6e74 2e66 7574 7572 6573 7204  urrent.futuresr.
-00003a60: 0000 00da 0770 6174 686c 6962 7205 0000  .....pathlibr...
-00003a70: 00da 0474 696d 6572 0600 0000 da04 656e  ...timer......en
-00003a80: 756d 7207 0000 0072 0800 0000 5a1f 7079  umr....r....Z.py
-00003a90: 7879 3364 2e74 7261 636b 6572 732e 6368  xy3d.trackers.ch
-00003aa0: 6172 7563 6f5f 7472 6163 6b65 7272 0900  aruco_trackerr..
-00003ab0: 0000 5a21 7079 7879 3364 2e63 616c 6962  ..Z!pyxy3d.calib
-00003ac0: 7261 7469 6f6e 2e6d 6f6e 6f63 616c 6962  ration.monocalib
-00003ad0: 7261 746f 7272 0a00 0000 5a15 7079 7879  ratorr....Z.pyxy
-00003ae0: 3364 2e63 616d 6572 6173 2e63 616d 6572  3d.cameras.camer
-00003af0: 6172 0b00 0000 5a1b 7079 7879 3364 2e63  ar....Z.pyxy3d.c
-00003b00: 616d 6572 6173 2e73 796e 6368 726f 6e69  ameras.synchroni
-00003b10: 7a65 7272 0c00 0000 5a27 7079 7879 3364  zerr....Z'pyxy3d
-00003b20: 2e63 616d 6572 6173 2e63 616d 6572 615f  .cameras.camera_
-00003b30: 6172 7261 795f 696e 6974 6961 6c69 7a65  array_initialize
-00003b40: 7272 0d00 0000 5a10 7079 7879 3364 2e69  rr....Z.pyxy3d.i
-00003b50: 6e74 6572 6661 6365 720e 0000 005a 2370  nterfacer....Z#p
-00003b60: 7978 7933 642e 6361 6c69 6272 6174 696f  yxy3d.calibratio
-00003b70: 6e2e 7374 6572 656f 6361 6c69 6272 6174  n.stereocalibrat
-00003b80: 6f72 720f 0000 005a 3170 7978 7933 642e  orr....Z1pyxy3d.
-00003b90: 6361 6c69 6272 6174 696f 6e2e 6361 7074  calibration.capt
-00003ba0: 7572 655f 766f 6c75 6d65 2e70 6f69 6e74  ure_volume.point
-00003bb0: 5f65 7374 696d 6174 6573 7210 0000 005a  _estimatesr....Z
-00003bc0: 3070 7978 7933 642e 6361 6c69 6272 6174  0pyxy3d.calibrat
-00003bd0: 696f 6e2e 6361 7074 7572 655f 766f 6c75  ion.capture_volu
-00003be0: 6d65 2e63 6170 7475 7265 5f76 6f6c 756d  me.capture_volum
-00003bf0: 6572 1100 0000 5a34 7079 7879 3364 2e63  er....Z4pyxy3d.c
-00003c00: 616c 6962 7261 7469 6f6e 2e63 6170 7475  alibration.captu
-00003c10: 7265 5f76 6f6c 756d 652e 7175 616c 6974  re_volume.qualit
-00003c20: 795f 636f 6e74 726f 6c6c 6572 7212 0000  y_controllerr...
-00003c30: 005a 1b70 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
-00003c40: 732e 6361 6d65 7261 5f61 7272 6179 7213  s.camera_arrayr.
-00003c50: 0000 005a 4670 7978 7933 642e 6361 6c69  ...ZFpyxy3d.cali
-00003c60: 6272 6174 696f 6e2e 6361 7074 7572 655f  bration.capture_
-00003c70: 766f 6c75 6d65 2e68 656c 7065 725f 6675  volume.helper_fu
-00003c80: 6e63 7469 6f6e 732e 6765 745f 706f 696e  nctions.get_poin
-00003c90: 745f 6573 7469 6d61 7465 7372 1400 0000  t_estimatesr....
-00003ca0: da13 7079 7879 3364 2e63 6f6e 6669 6775  ..pyxy3d.configu
-00003cb0: 7261 746f 7272 1500 0000 5a1a 7079 7879  ratorr....Z.pyxy
-00003cc0: 3364 2e63 616d 6572 6173 2e6c 6976 655f  3d.cameras.live_
-00003cd0: 7374 7265 616d 7216 0000 005a 1f70 7978  streamr....Z.pyx
-00003ce0: 7933 642e 7265 636f 7264 696e 672e 7669  y3d.recording.vi
-00003cf0: 6465 6f5f 7265 636f 7264 6572 7217 0000  deo_recorderr...
-00003d00: 0072 7c00 0000 729c 0000 0072 1900 0000  .r|...r....r....
-00003d10: 7227 0000 0072 2500 0000 7225 0000 0072  r'...r%...r%...r
-00003d20: 2500 0000 7226 0000 00da 083c 6d6f 6475  %...r&.....<modu
-00003d30: 6c65 3e01 0000 0073 3400 0000 0801 0c02  le>....s4.......
-00003d40: 1002 0c01 0c01 0c01 1001 0c02 0c01 0c01  ................
-00003d50: 0c01 0c01 0c01 0c02 0c01 0c01 0c01 0c02  ................
-00003d60: 0c01 0c03 0c01 0c01 0403 0401 1003 140b  ................
+00001230: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00001240: 0500 0000 4300 0000 7346 0000 0064 017d  ....C...sF...d.}
+00001250: 017c 006a 00a0 01a1 0044 005d 197d 027c  .|.j.....D.].}.|
+00001260: 02a0 02a1 0072 2074 037c 02a0 0464 02a1  .....r t.|...d..
+00001270: 0183 017d 037c 0264 031b 007d 047c 0372  ...}.|.d...}.|.r
+00001280: 207c 04a0 05a1 0072 2064 047d 0171 077c   |.....r d.}.q.|
+00001290: 0153 0029 057a a60a 2020 2020 2020 2020  .S.).z..        
+000012a0: 506f 7374 2070 726f 6365 7373 696e 6720  Post processing 
+000012b0: 6361 6e20 6f6e 6c79 2062 6520 7065 7266  can only be perf
+000012c0: 6f72 6d65 6420 6966 2072 6563 6f72 6469  ormed if recordi
+000012d0: 6e67 7320 286d 7034 2066 696c 6573 2920  ngs (mp4 files) 
+000012e0: 6578 6973 7420 616e 6420 6578 7472 696e  exist and extrin
+000012f0: 7369 6373 200a 2020 2020 2020 2020 2863  sics .        (c
+00001300: 6f6e 6669 672e 746f 6d6c 2920 6172 6520  onfig.toml) are 
+00001310: 6361 6c69 6272 6174 6564 2069 6e20 7468  calibrated in th
+00001320: 6520 2772 6563 6f72 6427 2064 6972 6563  e 'record' direc
+00001330: 746f 7279 0a20 2020 2020 2020 2046 7a05  tory.        Fz.
+00001340: 2a2e 6d70 347a 0b63 6f6e 6669 672e 746f  *.mp4z.config.to
+00001350: 6d6c 5429 0672 2c00 0000 da07 6974 6572  mlT).r,.....iter
+00001360: 6469 72da 0669 735f 6469 72da 046c 6973  dir..is_dir..lis
+00001370: 74da 0467 6c6f 62da 0665 7869 7374 7329  t..glob..exists)
+00001380: 0572 3b00 0000 724a 0000 00da 0563 6869  .r;...rJ.....chi
+00001390: 6c64 5a09 6d70 345f 6669 6c65 735a 0b63  ldZ.mp4_filesZ.c
+000013a0: 6f6e 6669 675f 6669 6c65 7225 0000 0072  onfig_filer%...r
+000013b0: 2500 0000 7226 0000 00da 1b69 735f 706f  %...r&.....is_po
+000013c0: 7374 5f70 726f 6365 7373 696e 675f 656c  st_processing_el
+000013d0: 6967 6962 6c65 b900 0000 7312 0000 0004  igible....s.....
+000013e0: 060e 0108 010e 0108 010c 0104 0102 8004  ................
+000013f0: 027a 2353 6573 7369 6f6e 2e69 735f 706f  .z#Session.is_po
+00001400: 7374 5f70 726f 6365 7373 696e 675f 656c  st_processing_el
+00001410: 6967 6962 6c65 723a 0000 0063 0200 0000  igibler:...c....
+00001420: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001430: 4300 0000 73bc 0100 007c 017c 005f 007c  C...s....|.|._.|
+00001440: 00a0 01a1 0001 007c 006a 0004 0074 026a  .......|.j...t.j
+00001450: 036b 0272 1f01 007c 006a 0472 1d7c 006a  .k.r...|.j.r.|.j
+00001460: 05a0 06a1 0001 007c 00a0 07a1 0001 0064  .......|.......d
+00001470: 0953 0064 0953 0004 0074 026a 086b 0272  .S.d.S...t.j.k.r
+00001480: 3501 007c 006a 0472 337c 006a 05a0 06a1  5..|.j.r3|.j....
+00001490: 0001 007c 00a0 07a1 0001 0064 0953 0064  ...|.......d.S.d
+000014a0: 0953 0004 0074 026a 096b 0272 6201 0074  .S...t.j.k.rb..t
+000014b0: 0a7c 006a 0b83 017c 005f 0c7c 006a 0473  .|.j...|._.|.j.s
+000014c0: 487c 00a0 0da1 0001 007c 006a 05a0 06a1  H|.......|.j....
+000014d0: 0001 007c 00a0 07a1 0001 007c 00a0 0ea1  ...|.......|....
+000014e0: 0001 007c 00a0 0f64 01a1 0101 007c 00a0  ...|...d.....|..
+000014f0: 107c 006a 11a1 0101 0064 0953 0004 0074  .|.j.....d.S...t
+00001500: 026a 126b 0272 8901 0074 0a7c 006a 0b83  .j.k.r...t.|.j..
+00001510: 017c 005f 0c7c 006a 0473 757c 00a0 0da1  .|._.|.j.su|....
+00001520: 0001 007c 00a0 07a1 0001 007c 00a0 0ea1  ...|.......|....
+00001530: 0001 007c 00a0 0f64 01a1 0101 007c 006a  ...|...d.....|.j
+00001540: 05a0 13a1 0001 0064 0953 0004 0074 026a  .......d.S...t.j
+00001550: 146b 0272 9f01 007c 006a 0472 9d7c 00a0  .k.r...|.j.r.|..
+00001560: 07a1 0001 007c 006a 05a0 06a1 0001 0064  .....|.j.......d
+00001570: 0953 0064 0953 0074 026a 156b 0272 dc74  .S.d.S.t.j.k.r.t
+00001580: 16a0 1764 02a1 0101 007c 006a 0473 b474  ...d.....|.j.s.t
+00001590: 16a0 1764 03a1 0101 007c 00a0 0da1 0001  ...d.....|......
+000015a0: 0074 16a0 1764 04a1 0101 007c 00a0 07a1  .t...d.....|....
+000015b0: 0001 0074 16a0 1764 05a1 0101 007c 00a0  ...t...d.....|..
+000015c0: 0f64 06a1 0101 0074 16a0 1764 07a1 0101  .d.....t...d....
+000015d0: 007c 00a0 01a1 0001 0074 16a0 1764 08a1  .|.......t...d..
+000015e0: 0101 007c 006a 05a0 13a1 0001 0064 0953  ...|.j.......d.S
+000015f0: 0064 0953 0029 0a7a af0a 2020 2020 2020  .d.S.).z..      
+00001600: 2020 5669 6120 7468 6973 206d 6574 686f    Via this metho
+00001610: 642c 2074 6865 2066 7261 6d65 2072 6561  d, the frame rea
+00001620: 6469 6e67 2062 6568 6176 696f 7220 7769  ding behavior wi
+00001630: 6c6c 2062 6520 6368 616e 6765 6420 6279  ll be changed by
+00001640: 2074 6865 2047 5549 2e20 4966 2073 6f6d   the GUI. If som
+00001650: 6520 7072 6f70 6572 7469 6573 2061 7265  e properties are
+00001660: 0a20 2020 2020 2020 206e 6f74 2061 7661  .        not ava
+00001670: 696c 6162 6c65 2028 692e 652e 2073 796e  ilable (i.e. syn
+00001680: 6368 726f 6e69 7a65 7229 2074 6865 7920  chronizer) they 
+00001690: 7769 6c6c 2062 6520 6372 6561 7465 640a  will be created.
+000016a0: 2020 2020 2020 2020 547a 2041 7474 656d          Tz Attem
+000016b0: 7074 696e 6720 746f 2073 6574 2072 6563  pting to set rec
+000016c0: 6f72 6469 6e67 206d 6f64 657a 2e53 7472  ording modez.Str
+000016d0: 6561 6d20 746f 6f6c 7320 6e6f 7420 6c6f  eam tools not lo
+000016e0: 6164 6564 2c20 736f 206c 6f61 6469 6e67  aded, so loading
+000016f0: 2074 6865 6d20 7570 2e2e 2e7a 2850 6175   them up...z(Pau
+00001700: 7369 6e67 206d 6f6e 6f63 616c 7320 746f  sing monocals to
+00001710: 2065 6e74 6572 2072 6563 6f72 6469 6e67   enter recording
+00001720: 206d 6f64 657a 2053 746f 7020 7472 6163   modez Stop trac
+00001730: 6b69 6e67 2066 6f72 2072 6563 6f72 6469  king for recordi
+00001740: 6e67 206d 6f64 6546 7a22 5570 6461 7465  ng modeFz"Update
+00001750: 2073 7472 6561 6d20 6670 7320 746f 2072   stream fps to r
+00001760: 6563 6f72 6469 6e67 2066 7073 7a3e 5375  ecording fpsz>Su
+00001770: 6273 6372 6962 6520 7379 6e63 6872 6f6e  bscribe synchron
+00001780: 697a 6572 2074 6f20 7374 7265 616d 7320  izer to streams 
+00001790: 736f 2076 6964 656f 2072 6563 6f72 6465  so video recorde
+000017a0: 7220 6361 6e20 6d61 6e61 6765 4e29 1872  r can manageN).r
+000017b0: 3a00 0000 da12 7570 6461 7465 5f73 7472  :.....update_str
+000017c0: 6561 6d73 5f66 7073 7219 0000 0072 1f00  eams_fpsr....r..
+000017d0: 0000 7231 0000 0072 4100 0000 da18 756e  ..r1...rA.....un
+000017e0: 7375 6273 6372 6962 655f 6672 6f6d 5f73  subscribe_from_s
+000017f0: 7472 6561 6d73 da19 7061 7573 655f 616c  treams..pause_al
+00001800: 6c5f 6d6f 6e6f 6361 6c69 6272 6174 6f72  l_monocalibrator
+00001810: 7372 2400 0000 7220 0000 0072 0900 0000  sr$...r ...r....
+00001820: 7238 0000 0072 3900 0000 da11 6c6f 6164  r8...r9.....load
+00001830: 5f73 7472 6561 6d5f 746f 6f6c 73da 1373  _stream_tools..s
+00001840: 6574 5f73 7472 6561 6d73 5f63 6861 7275  et_streams_charu
+00001850: 636f da14 7365 745f 7374 7265 616d 735f  co..set_streams_
+00001860: 7472 6163 6b69 6e67 da17 6163 7469 7661  tracking..activa
+00001870: 7465 5f6d 6f6e 6f63 616c 6962 7261 746f  te_monocalibrato
+00001880: 7272 3300 0000 7221 0000 00da 1473 7562  rr3...r!.....sub
+00001890: 7363 7269 6265 5f74 6f5f 7374 7265 616d  scribe_to_stream
+000018a0: 7372 2200 0000 7223 0000 0072 5400 0000  sr"...r#...rT...
+000018b0: 7255 0000 0029 0272 3b00 0000 723a 0000  rU...).r;...r:..
+000018c0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+000018d0: da08 7365 745f 6d6f 6465 c900 0000 7362  ..set_mode....sb
+000018e0: 0000 0006 0508 0104 020c 0106 010a 010c  ................
+000018f0: 0104 fe0c 0406 010a 010c 0104 fe0c 040c  ................
+00001900: 0206 0208 010a 0108 0108 010a 0110 010c  ................
+00001910: 020c 0206 0108 0108 0208 010a 010e 020c  ................
+00001920: 0206 0108 010e 0104 fe08 040a 0106 010a  ................
+00001930: 0108 010a 0208 010a 020a 010a 0108 010a  ................
+00001940: 020e 0104 f17a 1053 6573 7369 6f6e 2e73  .....z.Session.s
+00001950: 6574 5f6d 6f64 65da 0a66 7073 5f74 6172  et_mode..fps_tar
+00001960: 6765 7463 0200 0000 0000 0000 0000 0000  getc............
+00001970: 0200 0000 0300 0000 4300 0000 7386 0000  ........C...s...
+00001980: 007c 006a 0004 0074 016a 026b 0272 0901  .|.j...t.j.k.r..
+00001990: 006e 3404 0074 016a 036b 0272 1001 006e  .n4..t.j.k.r...n
+000019a0: 2d04 0074 016a 046b 0272 2001 007c 017c  -..t.j.k.r ..|.|
+000019b0: 005f 057c 006a 06a0 077c 01a1 0101 006e  ._.|.j...|.....n
+000019c0: 1d04 0074 016a 086b 0272 3001 007c 017c  ...t.j.k.r0..|.|
+000019d0: 005f 097c 006a 06a0 0a7c 01a1 0101 006e  ._.|.j...|.....n
+000019e0: 0d74 016a 0b6b 0272 3d7c 017c 005f 0c7c  .t.j.k.r=|.|._.|
+000019f0: 006a 06a0 0d7c 01a1 0101 007c 00a0 0ea1  .j...|.....|....
+00001a00: 0001 0064 0153 0029 027a 780a 2020 2020  ...d.S.).zx.    
+00001a10: 2020 2020 5570 6461 7465 7320 7468 6520      Updates the 
+00001a20: 4650 5320 7573 6564 2062 7920 7468 6520  FPS used by the 
+00001a30: 6375 7272 656e 746c 7920 6163 7469 7665  currently active
+00001a40: 2073 6573 7369 6f6e 206d 6f64 650a 2020   session mode.  
+00001a50: 2020 2020 2020 5468 6973 2075 7064 6174        This updat
+00001a60: 6520 696e 636c 7564 6573 2074 6865 2063  e includes the c
+00001a70: 6f6e 6669 672e 746f 6d6c 0a20 2020 2020  onfig.toml.     
+00001a80: 2020 204e 290f 723a 0000 0072 1900 0000     N).r:...r....
+00001a90: 721f 0000 0072 2400 0000 7220 0000 0072  r....r$...r ...r
+00001aa0: 3600 0000 7228 0000 005a 1e73 6176 655f  6...r(...Z.save_
+00001ab0: 6670 735f 696e 7472 696e 7369 635f 6361  fps_intrinsic_ca
+00001ac0: 6c69 6272 6174 696f 6e72 2100 0000 7235  librationr!...r5
+00001ad0: 0000 005a 1e73 6176 655f 6670 735f 6578  ...Z.save_fps_ex
+00001ae0: 7472 696e 7369 635f 6361 6c69 6272 6174  trinsic_calibrat
+00001af0: 696f 6e72 2300 0000 7234 0000 005a 1273  ionr#...r4...Z.s
+00001b00: 6176 655f 6670 735f 7265 636f 7264 696e  ave_fps_recordin
+00001b10: 6772 6100 0000 2902 723b 0000 0072 6a00  gra...).r;...rj.
+00001b20: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
+00001b30: 00da 1373 6574 5f61 6374 6976 655f 6d6f  ...set_active_mo
+00001b40: 6465 5f66 7073 0a01 0000 731e 0000 0004  de_fps....s.....
+00001b50: 050c 0102 010c 0102 010c 0106 010e 010c  ................
+00001b60: 0106 010e 0108 0106 010c 010c 027a 1b53  .............z.S
+00001b70: 6573 7369 6f6e 2e73 6574 5f61 6374 6976  ession.set_activ
+00001b80: 655f 6d6f 6465 5f66 7073 da06 7265 7475  e_mode_fps..retu
+00001b90: 726e 6301 0000 0000 0000 0000 0000 0002  rnc.............
+00001ba0: 0000 0003 0000 0043 0000 0073 6e00 0000  .......C...sn...
+00001bb0: 6400 7d01 7c00 6a00 0400 7401 6a02 6b02  d.}.|.j...t.j.k.
+00001bc0: 720d 0100 0900 7c01 5300 0400 7401 6a03  r.....|.S...t.j.
+00001bd0: 6b02 7216 0100 0900 7c01 5300 0400 7401  k.r.....|.S...t.
+00001be0: 6a04 6b02 7221 0100 7c00 6a05 7d01 7c01  j.k.r!..|.j.}.|.
+00001bf0: 5300 0400 7401 6a06 6b02 722c 0100 7c00  S...t.j.k.r,..|.
+00001c00: 6a07 7d01 7c01 5300 7401 6a08 6b02 7235  j.}.|.S.t.j.k.r5
+00001c10: 7c00 6a09 7d01 7c01 5300 7c01 5300 a901  |.j.}.|.S.|.S...
+00001c20: 4e29 0a72 3a00 0000 7219 0000 0072 1f00  N).r:...r....r..
+00001c30: 0000 7224 0000 0072 2000 0000 7236 0000  ..r$...r ...r6..
+00001c40: 0072 2100 0000 7235 0000 0072 2300 0000  .r!...r5...r#...
+00001c50: 7234 0000 0029 0272 3b00 0000 5a03 6670  r4...).r;...Z.fp
+00001c60: 7372 2500 0000 7225 0000 0072 2600 0000  sr%...r%...r&...
+00001c70: da13 6765 745f 6163 7469 7665 5f6d 6f64  ..get_active_mod
+00001c80: 655f 6670 7320 0100 0073 2200 0000 0401  e_fps ...s".....
+00001c90: 0401 0c01 0201 0409 0cf8 0201 0407 0cfa  ................
+00001ca0: 0601 0405 0cfc 0601 0403 08fe 0601 0801  ................
+00001cb0: 7a1b 5365 7373 696f 6e2e 6765 745f 6163  z.Session.get_ac
+00001cc0: 7469 7665 5f6d 6f64 655f 6670 7363 0100  tive_mode_fpsc..
+00001cd0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00001ce0: 0000 4300 0000 7336 0000 007c 00a0 00a1  ..C...s6...|....
+00001cf0: 007d 017c 0164 0075 0172 177c 006a 01a0  .}.|.d.u.r.|.j..
+00001d00: 02a1 0044 005d 0b5c 027d 027d 037c 03a0  ...D.].\.}.}.|..
+00001d10: 037c 01a1 0101 0071 0d64 0053 0064 0053  .|.....q.d.S.d.S
+00001d20: 0072 6d00 0000 2904 726e 0000 0072 2f00  .rm...).rn...r/.
+00001d30: 0000 723e 0000 005a 0e73 6574 5f66 7073  ..r>...Z.set_fps
+00001d40: 5f74 6172 6765 7429 0472 3b00 0000 5a0f  _target).r;...Z.
+00001d50: 6163 7469 7665 5f6d 6f64 655f 6670 7372  active_mode_fpsr
+00001d60: 4400 0000 7245 0000 0072 2500 0000 7225  D...rE...r%...r%
+00001d70: 0000 0072 2600 0000 7261 0000 002f 0100  ...r&...ra.../..
+00001d80: 0073 0c00 0000 0801 0801 1201 0c01 04fe  .s..............
+00001d90: 0401 7a1a 5365 7373 696f 6e2e 7570 6461  ..z.Session.upda
+00001da0: 7465 5f73 7472 6561 6d73 5f66 7073 da0b  te_streams_fps..
+00001db0: 7472 6163 6b69 6e67 5f6f 6e63 0200 0000  tracking_onc....
+00001dc0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00001dd0: 4300 0000 7322 0000 007c 006a 00a0 01a1  C...s"...|.j....
+00001de0: 0044 005d 095c 027d 027d 037c 03a0 027c  .D.].\.}.}.|...|
+00001df0: 01a1 0101 0071 0564 0053 0072 6d00 0000  .....q.d.S.rm...
+00001e00: 2903 722f 0000 0072 3e00 0000 5a0f 7365  ).r/...r>...Z.se
+00001e10: 745f 7472 6163 6b69 6e67 5f6f 6e29 0472  t_tracking_on).r
+00001e20: 3b00 0000 726f 0000 0072 4400 0000 7245  ;...ro...rD...rE
+00001e30: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
+00001e40: 0000 7266 0000 0035 0100 0073 0600 0000  ..rf...5...s....
+00001e50: 1201 0c01 04ff 7a1c 5365 7373 696f 6e2e  ......z.Session.
+00001e60: 7365 745f 7374 7265 616d 735f 7472 6163  set_streams_trac
+00001e70: 6b69 6e67 6301 0000 0000 0000 0000 0000  kingc...........
+00001e80: 0003 0000 0004 0000 0043 0000 0073 3a00  .........C...s:.
+00001e90: 0000 7400 a001 6401 a101 0100 7402 7c00  ..t...d.....t.|.
+00001ea0: 6a03 8301 7c00 5f04 7c00 6a05 a006 a100  j...|._.|.j.....
+00001eb0: 4400 5d0a 5c02 7d01 7d02 7c02 a007 7c00  D.].\.}.}.|...|.
+00001ec0: 6a04 a101 0100 7110 6400 5300 2902 4e7a  j.....q.d.S.).Nz
+00001ed0: 2275 7064 6174 696e 6720 6368 6172 7563  "updating charuc
+00001ee0: 6f20 696e 2063 6173 6520 6e65 6365 7373  o in case necess
+00001ef0: 6172 7929 0872 5400 0000 7255 0000 0072  ary).rT...rU...r
+00001f00: 0900 0000 7238 0000 0072 3900 0000 722f  ....r8...r9...r/
+00001f10: 0000 0072 3e00 0000 5a0e 7570 6461 7465  ...r>...Z.update
+00001f20: 5f74 7261 636b 6572 2903 723b 0000 0072  _tracker).r;...r
+00001f30: 4400 0000 7245 0000 0072 2500 0000 7225  D...rE...r%...r%
+00001f40: 0000 0072 2600 0000 7265 0000 0039 0100  ...r&...re...9..
+00001f50: 0073 0a00 0000 0a01 0c01 1201 0e01 04ff  .s..............
+00001f60: 7a1b 5365 7373 696f 6e2e 7365 745f 7374  z.Session.set_st
+00001f70: 7265 616d 735f 6368 6172 7563 6f63 0100  reams_charucoc..
+00001f80: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00001f90: 0000 4300 0000 7318 0000 0074 00a0 0164  ..C...s....t...d
+00001fa0: 01a1 0101 007c 006a 02a0 03a1 0001 0064  .....|.j.......d
+00001fb0: 0053 0029 024e 7a14 7061 7573 696e 6720  .S.).Nz.pausing 
+00001fc0: 7379 6e63 6872 6f6e 697a 6572 2904 7254  synchronizer).rT
+00001fd0: 0000 0072 5500 0000 7241 0000 0072 6200  ...rU...rA...rb.
+00001fe0: 0000 a901 723b 0000 0072 2500 0000 7225  ....r;...r%...r%
+00001ff0: 0000 0072 2600 0000 da12 7061 7573 655f  ...r&.....pause_
+00002000: 7379 6e63 6872 6f6e 697a 6572 3f01 0000  synchronizer?...
+00002010: 7304 0000 000a 010e 017a 1a53 6573 7369  s........z.Sessi
+00002020: 6f6e 2e70 6175 7365 5f73 796e 6368 726f  on.pause_synchro
+00002030: 6e69 7a65 7263 0100 0000 0000 0000 0000  nizerc..........
+00002040: 0000 0100 0000 0300 0000 4300 0000 731e  ..........C...s.
+00002050: 0000 007c 006a 00a0 01a1 0001 007c 006a  ...|.j.......|.j
+00002060: 00a0 027c 006a 006a 03a1 0101 0064 0053  ...|.j.j.....d.S
+00002070: 0072 6d00 0000 2904 7241 0000 0072 6800  .rm...).rA...rh.
+00002080: 0000 5a0e 7365 745f 7374 7265 616d 5f66  ..Z.set_stream_f
+00002090: 7073 726a 0000 0072 7000 0000 7225 0000  psrj...rp...r%..
+000020a0: 0072 2500 0000 7226 0000 00da 1475 6e70  .r%...r&.....unp
+000020b0: 6175 7365 5f73 796e 6368 726f 6e69 7a65  ause_synchronize
+000020c0: 7243 0100 0073 0400 0000 0a01 1401 7a1c  rC...s........z.
+000020d0: 5365 7373 696f 6e2e 756e 7061 7573 655f  Session.unpause_
+000020e0: 7379 6e63 6872 6f6e 697a 6572 6301 0000  synchronizerc...
+000020f0: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00002100: 0043 0000 0073 3400 0000 6401 7d01 7c00  .C...s4...d.}.|.
+00002110: 6a00 6a01 a002 a100 a003 a100 4400 5d0d  j.j.........D.].
+00002120: 5c02 7d02 7d03 7c02 a004 6402 a101 7217  \.}.}.|...d...r.
+00002130: 7c01 6403 3700 7d01 710a 7c01 5300 2904  |.d.7.}.q.|.S.).
+00002140: 4e72 0100 0000 7246 0000 00e9 0100 0000  Nr....rF........
+00002150: 2905 7228 0000 00da 0464 6963 74da 0463  ).r(.....dict..c
+00002160: 6f70 7972 3e00 0000 da0a 7374 6172 7473  opyr>.....starts
+00002170: 7769 7468 2904 723b 0000 00da 0563 6f75  with).r;.....cou
+00002180: 6e74 da03 6b65 79da 0670 6172 616d 7372  nt..key..paramsr
+00002190: 2500 0000 7225 0000 0072 2600 0000 da1b  %...r%...r&.....
+000021a0: 6765 745f 636f 6e66 6967 7572 6564 5f63  get_configured_c
+000021b0: 616d 6572 615f 636f 756e 7447 0100 0073  amera_countG...s
+000021c0: 0c00 0000 0401 1801 0a01 0801 0280 0401  ................
+000021d0: 7a23 5365 7373 696f 6e2e 6765 745f 636f  z#Session.get_co
+000021e0: 6e66 6967 7572 6564 5f63 616d 6572 615f  nfigured_camera_
+000021f0: 636f 756e 7463 0100 0000 0000 0000 0000  countc..........
+00002200: 0000 0500 0000 0800 0000 0300 0000 738c  ..............s.
+00002210: 0000 0087 0066 0164 0164 0284 087d 0174  .....f.d.d...}.t
+00002220: 0083 008f 1e7d 0274 0164 0374 0283 0244  .....}.t.d.t...D
+00002230: 005d 107d 037c 0388 006a 03a0 04a1 0076  .].}.|...j.....v
+00002240: 0072 1971 0f7c 02a0 057c 017c 03a1 0201  .r.q.|...|.|....
+00002250: 0071 0f57 0064 0404 0004 0083 0301 006e  .q.W.d.........n
+00002260: 0831 0073 2a77 0101 0001 0001 0059 0001  .1.s*w.......Y..
+00002270: 0088 006a 066a 07a0 08a1 00a0 04a1 0044  ...j.j.........D
+00002280: 005d 0c7d 047c 04a0 0964 05a1 0172 4388  .].}.|...d...rC.
+00002290: 006a 066a 077c 043d 0071 3764 0453 0029  .j.j.|.=.q7d.S.)
+000022a0: 067a a30a 2020 2020 2020 2020 4361 6c6c  .z..        Call
+000022b0: 6564 2062 7920 6c6f 6164 5f73 7472 6561  ed by load_strea
+000022c0: 6d73 2069 6e20 7468 6520 6576 656e 7420  ms in the event 
+000022d0: 7468 6174 206e 6f20 6361 6d65 7261 7320  that no cameras 
+000022e0: 6172 6520 7265 7475 726e 6564 2062 7920  are returned by 
+000022f0: 7468 6520 636f 6e66 6967 7572 6174 6f72  the configurator
+00002300: 2e2e 2e0a 2020 2020 2020 2020 5769 6c6c  ....        Will
+00002310: 2070 6f70 756c 6174 6520 7365 6c66 2e63   populate self.c
+00002320: 616d 6572 6173 2075 7369 6e67 206d 756c  ameras using mul
+00002330: 7469 706c 6520 7468 7265 6164 730a 2020  tiple threads.  
+00002340: 2020 2020 2020 6301 0000 0000 0000 0000        c.........
+00002350: 0000 0002 0000 0007 0000 0013 0000 0073  ...............s
+00002360: 8c00 0000 7a37 7400 a001 6401 7c00 9b00  ....z7t...d.|...
+00002370: 9d02 a101 0100 7402 7c00 8301 7d01 7400  ......t.|...}.t.
+00002380: a001 6402 7c00 9b00 9d02 a101 0100 7c01  ..d.|.........|.
+00002390: 8800 6a03 7c00 3c00 8800 6a04 a005 7c01  ..j.|.<...j...|.
+000023a0: a101 0100 7400 a001 6403 7c00 9b00 6404  ....t...d.|...d.
+000023b0: 9d03 a101 0100 7406 7c01 7407 8800 6a08  ......t.|.t...j.
+000023c0: 8301 6405 8d02 8800 6a09 7c00 3c00 5700  ..d.....j.|.<.W.
+000023d0: 6400 5300 0100 0100 0100 7400 a001 6406  d.S.......t...d.
+000023e0: 7c00 9b00 9d02 a101 0100 5900 6400 5300  |.........Y.d.S.
+000023f0: 2907 4e7a 0c54 7279 696e 6720 706f 7274  ).Nz.Trying port
+00002400: 207a 1053 7563 6365 7373 2061 7420 706f   z.Success at po
+00002410: 7274 207a 174c 6f61 6469 6e67 2073 7472  rt z.Loading str
+00002420: 6561 6d20 6174 2070 6f72 7420 7a25 2077  eam at port z% w
+00002430: 6974 6820 6368 6172 7563 6f20 7472 6163  ith charuco trac
+00002440: 6b65 7220 666f 7220 6361 6c69 6272 6174  ker for calibrat
+00002450: 696f 6ea9 015a 0774 7261 636b 6572 7a12  ion..Z.trackerz.
+00002460: 4e6f 2063 616d 6572 6120 6174 2070 6f72  No camera at por
+00002470: 7420 290a 7254 0000 0072 5500 0000 720b  t ).rT...rU...r.
+00002480: 0000 0072 2e00 0000 7228 0000 005a 0b73  ...r....r(...Z.s
+00002490: 6176 655f 6361 6d65 7261 7216 0000 0072  ave_camerar....r
+000024a0: 0900 0000 7238 0000 0072 2f00 0000 2902  ....r8...r/...).
+000024b0: 7244 0000 0072 4600 0000 7270 0000 0072  rD...rF...rp...r
+000024c0: 2500 0000 7226 0000 00da 0761 6464 5f63  %...r&.....add_c
+000024d0: 616d 5401 0000 731c 0000 0002 0110 0108  amT...s.........
+000024e0: 0110 010a 010c 0104 010a 0104 ff02 030a  ................
+000024f0: 0112 ff06 0316 017a 2653 6573 7369 6f6e  .......z&Session
+00002500: 2e5f 6669 6e64 5f63 616d 6572 6173 2e3c  ._find_cameras.<
+00002510: 6c6f 6361 6c73 3e2e 6164 645f 6361 6d72  locals>.add_camr
+00002520: 0100 0000 4e5a 0673 7465 7265 6f29 0a72  ....NZ.stereo).r
+00002530: 0400 0000 da05 7261 6e67 65da 154d 4158  ......range..MAX
+00002540: 5f43 414d 4552 415f 504f 5254 5f43 4845  _CAMERA_PORT_CHE
+00002550: 434b 722e 0000 00da 046b 6579 73da 0673  CKr......keys..s
+00002560: 7562 6d69 7472 2800 0000 7274 0000 0072  ubmitr(...rt...r
+00002570: 7500 0000 7276 0000 0029 0572 3b00 0000  u...rv...).r;...
+00002580: 727c 0000 00da 0865 7865 6375 746f 72da  r|.....executor.
+00002590: 0169 7278 0000 0072 2500 0000 7270 0000  .irx...r%...rp..
+000025a0: 0072 2600 0000 da0d 5f66 696e 645f 6361  .r&....._find_ca
+000025b0: 6d65 7261 734e 0100 0073 1a00 0000 0c06  merasN...s......
+000025c0: 0810 0e01 0e01 0202 0e02 02fb 1cff 1409  ................
+000025d0: 0a01 0a01 0280 04fe 7a15 5365 7373 696f  ........z.Sessio
+000025e0: 6e2e 5f66 696e 645f 6361 6d65 7261 7363  n._find_camerasc
+000025f0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00002600: 0500 0000 4300 0000 73da 0000 0064 017c  ....C...s....d.|
+00002610: 005f 007c 006a 01a0 02a1 007c 005f 0374  ._.|.j.....|._.t
+00002620: 047c 006a 0383 0164 026b 0272 147c 00a0  .|.j...d.k.r.|..
+00002630: 05a1 0001 007c 006a 03a0 06a1 0044 005d  .....|.j.....D.]
+00002640: 1e5c 027d 017d 027c 017c 006a 07a0 08a1  .\.}.}.|.|.j....
+00002650: 0076 0072 2571 1974 09a0 0a64 037c 019b  .v.r%q.t...d.|..
+00002660: 009d 02a1 0101 0074 0b7c 027c 006a 0c64  .......t.|.|.j.d
+00002670: 048d 027c 006a 077c 013c 0071 197c 00a0  ...|.j.|.<.q.|..
+00002680: 0da1 0001 007c 00a0 0ea1 0001 0074 0f7c  .....|.......t.|
+00002690: 006a 10a0 08a1 0083 017c 005f 1174 127c  .j.......|._.t.|
+000026a0: 006a 0783 017c 005f 1364 017c 005f 1464  .j...|._.d.|._.d
+000026b0: 057c 005f 0074 09a0 0a64 06a1 0101 007c  .|._.t...d.....|
+000026c0: 00a0 15a1 0001 007c 00a0 16a1 0001 0074  .......|.......t
+000026d0: 09a0 0a64 07a1 0101 007c 006a 17a0 18a1  ...d.....|.j....
+000026e0: 0001 0064 0853 0029 097a ad0a 2020 2020  ...d.S.).z..    
+000026f0: 2020 2020 436f 6e6e 6563 7473 2074 6f20      Connects to 
+00002700: 7374 6f72 6564 2063 616d 6572 6173 2061  stored cameras a
+00002710: 6e64 2063 7265 6174 6573 2073 7472 6561  nd creates strea
+00002720: 6d73 2077 6974 6820 7072 6f76 6964 6564  ms with provided
+00002730: 2074 7261 636b 696e 670a 2020 2020 2020   tracking.      
+00002740: 2020 4265 6361 7573 6520 7468 6573 6520    Because these 
+00002750: 7374 7265 616d 7320 6172 6520 6176 6169  streams are avai
+00002760: 6c61 626c 652c 2074 6865 2073 796e 6368  lable, the synch
+00002770: 726f 6e69 7a65 7220 6361 6e20 7468 656e  ronizer can then
+00002780: 2062 6520 696e 6974 6961 6c69 7a65 640a   be initialized.
+00002790: 2020 2020 2020 2020 5472 0100 0000 7a18          Tr....z.
+000027a0: 4c6f 6164 696e 6720 5374 7265 616d 2066  Loading Stream f
+000027b0: 6f72 2070 6f72 7420 727b 0000 0046 7a33  or port r{...Fz3
+000027c0: 5061 7573 696e 6720 7374 7265 616d 2074  Pausing stream t
+000027d0: 6f6f 6c73 2073 696e 6365 2064 6566 6175  ools since defau
+000027e0: 6c74 206c 6f61 6473 2074 6f20 6368 6172  lt loads to char
+000027f0: 7563 6f7a 2d53 6967 6e61 6c6c 696e 6720  ucoz-Signalling 
+00002800: 7375 6363 6573 7366 756c 206c 6f61 6469  successful loadi
+00002810: 6e67 206f 6620 7374 7265 616d 2074 6f6f  ng of stream too
+00002820: 6c73 4e29 1972 3000 0000 7228 0000 005a  lsN).r0...r(...Z
+00002830: 0b67 6574 5f63 616d 6572 6173 722e 0000  .get_camerasr...
+00002840: 0072 4900 0000 7283 0000 0072 3e00 0000  .rI...r....r>...
+00002850: 722f 0000 0072 7f00 0000 7254 0000 0072  r/...r....rT...r
+00002860: 5500 0000 7216 0000 0072 3900 0000 da13  U...r....r9.....
+00002870: 5f61 646a 7573 745f 7265 736f 6c75 7469  _adjust_resoluti
+00002880: 6f6e 73da 155f 6c6f 6164 5f6d 6f6e 6f63  ons.._load_monoc
+00002890: 616c 6962 7261 746f 7273 da03 6d69 6e72  alibrators..minr
+000028a0: 3200 0000 7233 0000 0072 0c00 0000 7241  2...r3...r....rA
+000028b0: 0000 0072 3100 0000 7263 0000 0072 7100  ...r1...rc...rq.
+000028c0: 0000 da1a 7374 7265 616d 5f74 6f6f 6c73  ....stream_tools
+000028d0: 5f6c 6f61 6465 645f 7369 676e 616c 7243  _loaded_signalrC
+000028e0: 0000 00a9 0372 3b00 0000 7244 0000 0072  .....r;...rD...r
+000028f0: 4600 0000 7225 0000 0072 2500 0000 7226  F...r%...r%...r&
+00002900: 0000 0072 6400 0000 7101 0000 732c 0000  ...rd...q...s,..
+00002910: 0006 050c 020e 0208 0112 020e 0102 0110  ................
+00002920: 0216 0108 0208 0110 0302 0204 0106 ff06  ................
+00002930: 0506 010a 0208 0108 010a 020e 017a 1953  .............z.S
+00002940: 6573 7369 6f6e 2e6c 6f61 645f 7374 7265  ession.load_stre
+00002950: 616d 5f74 6f6f 6c73 6301 0000 0000 0000  am_toolsc.......
+00002960: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
+00002970: 0073 5e00 0000 7c00 6a00 a001 a100 4400  .s^...|.j.....D.
+00002980: 5d27 5c02 7d01 7d02 7c01 7c00 6a02 a003  ]'\.}.}.|.|.j...
+00002990: a100 7600 721a 7404 a005 6401 7c01 9b00  ..v.r.t...d.|...
+000029a0: 6402 9d03 a101 0100 7105 7404 a005 6403  d.......q.t...d.
+000029b0: 7c01 9b00 9d02 a101 0100 7406 7c00 6a07  |.........t.|.j.
+000029c0: 7c01 1900 8301 7c00 6a02 7c01 3c00 7105  |.....|.j.|.<.q.
+000029d0: 6400 5300 2904 4e7a 2f53 6b69 7070 696e  d.S.).Nz/Skippin
+000029e0: 6720 6f76 6572 206d 6f6e 6f63 616c 6962  g over monocalib
+000029f0: 7261 746f 7220 6372 6561 7469 6f6e 2066  rator creation f
+00002a00: 6f72 2070 6f72 7420 7a1b 2062 6563 6175  or port z. becau
+00002a10: 7365 2069 7420 616c 7265 6164 7920 6578  se it already ex
+00002a20: 6973 7473 2e7a 204c 6f61 6469 6e67 204d  ists.z Loading M
+00002a30: 6f6e 6f63 616c 6962 7261 746f 7220 666f  onocalibrator fo
+00002a40: 7220 706f 7274 2029 0872 2e00 0000 723e  r port ).r....r>
+00002a50: 0000 0072 3200 0000 727f 0000 0072 5400  ...r2...r....rT.
+00002a60: 0000 7255 0000 0072 0a00 0000 722f 0000  ..rU...r....r/..
+00002a70: 0072 8800 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+00002a80: 7226 0000 0072 8500 0000 9901 0000 7312  r&...r........s.
+00002a90: 0000 0012 010e 0104 010a 0104 ff02 0310  ................
+00002aa0: 0216 0104 f87a 1d53 6573 7369 6f6e 2e5f  .....z.Session._
+00002ab0: 6c6f 6164 5f6d 6f6e 6f63 616c 6962 7261  load_monocalibra
+00002ac0: 746f 7273 4eda 0b61 6374 6976 655f 706f  torsN..active_po
+00002ad0: 7274 6302 0000 0000 0000 0000 0000 0002  rtc.............
+00002ae0: 0000 0005 0000 0043 0000 0073 4600 0000  .......C...sF...
+00002af0: 7c01 6401 7501 720f 7400 a001 6402 7c01  |.d.u.r.t...d.|.
+00002b00: 9b00 9d02 a101 0100 7c01 7c00 5f02 7400  ........|.|._.t.
+00002b10: a001 6403 7c00 6a02 9b00 6404 9d03 a101  ..d.|.j...d.....
+00002b20: 0100 7c00 6a03 7c00 6a02 1900 a004 a100  ..|.j.|.j.......
+00002b30: 0100 6401 5300 2905 7a7e 0a20 2020 2020  ..d.S.).z~.     
+00002b40: 2020 2055 7365 6420 746f 206d 616b 6520     Used to make 
+00002b50: 7375 7265 2074 6861 7420 6f6e 6c79 2074  sure that only t
+00002b60: 6865 2061 6374 6976 6520 6361 6d65 7261  he active camera
+00002b70: 2074 6162 2069 7320 7265 6164 696e 6720   tab is reading 
+00002b80: 6672 616d 6573 2064 7572 696e 6720 7468  frames during th
+00002b90: 6520 696e 7472 696e 7369 6320 6361 6c69  e intrinsic cali
+00002ba0: 6272 6174 696f 6e20 7072 6f63 6573 730a  bration process.
+00002bb0: 2020 2020 2020 2020 4e7a 2953 6574 7469          Nz)Setti
+00002bc0: 6e67 2073 6573 7369 6f6e 2061 6374 6976  ng session activ
+00002bd0: 6520 6d6f 6e6f 6361 6c69 6272 6174 6f72  e monocalibrator
+00002be0: 2074 6f20 7a1a 4163 7469 7661 7465 2074   to z.Activate t
+00002bf0: 7261 636b 696e 6720 6f6e 2070 6f72 7420  racking on port 
+00002c00: 7a16 2061 6e64 2064 6561 6374 6976 6174  z. and deactivat
+00002c10: 6520 6f74 6865 7273 2905 7254 0000 0072  e others).rT...r
+00002c20: 5500 0000 7233 0000 0072 3200 0000 5a13  U...r3...r2...Z.
+00002c30: 7375 6273 6372 6962 655f 746f 5f73 7472  subscribe_to_str
+00002c40: 6561 6d29 0272 3b00 0000 7289 0000 0072  eam).r;...r....r
+00002c50: 2500 0000 7225 0000 0072 2600 0000 7267  %...r%...r&...rg
+00002c60: 0000 00a4 0100 0073 0e00 0000 0805 1001  .......s........
+00002c70: 0601 0401 0c01 04ff 1403 7a1f 5365 7373  ..........z.Sess
+00002c80: 696f 6e2e 6163 7469 7661 7465 5f6d 6f6e  ion.activate_mon
+00002c90: 6f63 616c 6962 7261 746f 7263 0100 0000  ocalibratorc....
+00002ca0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00002cb0: 4300 0000 732a 0000 0074 00a0 0164 01a1  C...s*...t...d..
+00002cc0: 0101 007c 006a 02a0 03a1 0044 005d 085c  ...|.j.....D.].\
+00002cd0: 027d 017d 027c 02a0 04a1 0001 0071 0a64  .}.}.|.......q.d
+00002ce0: 0253 0029 037a 8b0a 2020 2020 2020 2020  .S.).z..        
+00002cf0: 7573 6564 2077 6865 6e20 6e6f 7420 6163  used when not ac
+00002d00: 7469 7665 6c79 206f 6e20 7468 6520 6361  tively on the ca
+00002d10: 6d65 7261 2063 616c 6962 7261 7469 6f6e  mera calibration
+00002d20: 2074 6162 0a20 2020 2020 2020 206f 7220   tab.        or 
+00002d30: 7768 656e 2073 696c 656e 6369 6e67 2061  when silencing a
+00002d40: 6c6c 2069 6e20 7072 6570 6172 6174 696f  ll in preparatio
+00002d50: 6e20 666f 7220 6163 7469 7661 7469 6e67  n for activating
+00002d60: 206f 6e6c 7920 6f6e 650a 2020 2020 2020   only one.      
+00002d70: 2020 7a25 5061 7573 696e 6720 616c 6c20    z%Pausing all 
+00002d80: 6d6f 6e6f 6361 6c69 6272 6174 6f72 206c  monocalibrator l
+00002d90: 6f6f 7069 6e67 2e2e 2e4e 2905 7254 0000  ooping...N).rT..
+00002da0: 0072 5500 0000 7232 0000 0072 3e00 0000  .rU...r2...r>...
+00002db0: 5a15 756e 7375 6273 6372 6962 655f 746f  Z.unsubscribe_to
+00002dc0: 5f73 7472 6561 6d29 0372 3b00 0000 7244  _stream).r;...rD
+00002dd0: 0000 0072 4700 0000 7225 0000 0072 2500  ...rG...r%...r%.
+00002de0: 0000 7226 0000 0072 6300 0000 b101 0000  ..r&...rc.......
+00002df0: 7308 0000 000a 0512 010a 0104 ff7a 2153  s............z!S
+00002e00: 6573 7369 6f6e 2e70 6175 7365 5f61 6c6c  ession.pause_all
+00002e10: 5f6d 6f6e 6f63 616c 6962 7261 746f 7273  _monocalibrators
+00002e20: 46da 1564 6573 7469 6e61 7469 6f6e 5f64  F..destination_d
+00002e30: 6972 6563 746f 7279 da13 7374 6f72 655f  irectory..store_
+00002e40: 706f 696e 745f 6869 7374 6f72 7963 0300  point_historyc..
+00002e50: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00002e60: 0000 4300 0000 733e 0000 0074 00a0 0164  ..C...s>...t...d
+00002e70: 01a1 0101 007c 016a 0264 0264 0264 038d  .....|.j.d.d.d..
+00002e80: 0201 0074 037c 006a 0483 017c 005f 057c  ...t.|.j...|._.|
+00002e90: 006a 056a 067c 017c 0264 048d 0201 0064  .j.j.|.|.d.....d
+00002ea0: 027c 005f 0764 0053 0029 054e 7a17 496e  .|._.d.S.).Nz.In
+00002eb0: 6974 6961 7469 6e67 2072 6563 6f72 6469  itiating recordi
+00002ec0: 6e67 2e2e 2e54 2902 da07 7061 7265 6e74  ng...T)...parent
+00002ed0: 73da 0865 7869 7374 5f6f 6b29 0172 8b00  s..exist_ok).r..
+00002ee0: 0000 2908 7254 0000 0072 5500 0000 da05  ..).rT...rU.....
+00002ef0: 6d6b 6469 7272 1700 0000 7241 0000 00da  mkdirr....rA....
+00002f00: 0e76 6964 656f 5f72 6563 6f72 6465 72da  .video_recorder.
+00002f10: 0f73 7461 7274 5f72 6563 6f72 6469 6e67  .start_recording
+00002f20: 7237 0000 0029 0372 3b00 0000 728a 0000  r7...).r;...r...
+00002f30: 0072 8b00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+00002f40: 7226 0000 0072 9000 0000 ba01 0000 730e  r&...r........s.
+00002f50: 0000 000a 030e 010c 0206 0104 0106 ff0a  ................
+00002f60: 037a 1753 6573 7369 6f6e 2e73 7461 7274  .z.Session.start
+00002f70: 5f72 6563 6f72 6469 6e67 6301 0000 0000  _recordingc.....
+00002f80: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00002f90: 0000 0073 6a00 0000 7400 a001 6401 a101  ...sj...t...d...
+00002fa0: 0100 7c00 6a02 a003 a100 0100 7c00 6a02  ..|.j.......|.j.
+00002fb0: 6a04 721b 7400 a001 6402 a101 0100 7405  j.r.t...d.....t.
+00002fc0: 6403 8301 0100 7c00 6a02 6a04 730e 6404  d.....|.j.j.s.d.
+00002fd0: 7c00 5f06 7400 a001 6405 a101 0100 7c00  |._.t...d.....|.
+00002fe0: 6a07 a008 a100 0100 7c00 a009 a100 7233  j.......|.....r3
+00002ff0: 7c00 6a0a a008 a100 0100 6400 5300 6400  |.j.......d.S.d.
+00003000: 5300 2906 4e7a 1553 746f 7070 696e 6720  S.).Nz.Stopping 
+00003010: 7265 636f 7264 696e 672e 2e2e 7a2e 5761  recording...z.Wa
+00003020: 6974 696e 6720 666f 7220 7669 6465 6f20  iting for video 
+00003030: 7265 636f 7264 6572 2074 6f20 7361 7665  recorder to save
+00003040: 206f 7574 2064 6174 612e 2e2e 6700 0000   out data...g...
+00003050: 0000 00e0 3f46 7a3d 5265 636f 7264 696e  ....?Fz=Recordin
+00003060: 6720 6f66 2066 7261 6d65 7320 6973 2063  g of frames is c
+00003070: 6f6d 706c 6574 652e 2e2e 7369 676e 616c  omplete...signal
+00003080: 6c69 6e67 2063 6861 6e67 6520 696e 2073  ling change in s
+00003090: 7461 7475 7329 0b72 5400 0000 7255 0000  tatus).rT...rU..
+000030a0: 0072 8f00 0000 da0e 7374 6f70 5f72 6563  .r......stop_rec
+000030b0: 6f72 6469 6e67 5a09 7265 636f 7264 696e  ordingZ.recordin
+000030c0: 6772 0600 0000 7237 0000 00da 1972 6563  gr....r7.....rec
+000030d0: 6f72 6469 6e67 5f63 6f6d 706c 6574 655f  ording_complete_
+000030e0: 7369 676e 616c 7243 0000 0072 6000 0000  signalrC...r`...
+000030f0: da15 756e 6c6f 636b 5f70 6f73 7470 726f  ..unlock_postpro
+00003100: 6365 7373 696e 6772 7000 0000 7225 0000  cessingrp...r%..
+00003110: 0072 2500 0000 7226 0000 0072 9100 0000  .r%...r&...r....
+00003120: c601 0000 7318 0000 000a 010a 0108 010a  ....s...........
+00003130: 0108 0108 fe06 040a 020a 0108 020e 0104  ................
+00003140: ff7a 1653 6573 7369 6f6e 2e73 746f 705f  .z.Session.stop_
+00003150: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
+00003160: 0000 0000 0000 0400 0000 0800 0000 0300  ................
+00003170: 0000 7354 0000 0087 0066 0164 0164 0284  ..sT.....f.d.d..
+00003180: 087d 0174 0083 008f 177d 0288 006a 01a0  .}.t.....}...j..
+00003190: 02a1 0044 005d 087d 037c 02a0 037c 017c  ...D.].}.|...|.|
+000031a0: 03a1 0201 0071 0f57 0064 0304 0004 0083  .....q.W.d......
+000031b0: 0301 0064 0353 0031 0073 2377 0101 0001  ...d.S.1.s#w....
+000031c0: 0001 0059 0001 0064 0353 0029 047a 8243  ...Y...d.S.).z.C
+000031d0: 6861 6e67 6573 2074 6865 2063 616d 6572  hanges the camer
+000031e0: 6120 7265 736f 6c75 7469 6f6e 2074 6f20  a resolution to 
+000031f0: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
+00003200: 2063 6f6e 6669 6775 7261 7469 6f6e 2c20   configuration, 
+00003210: 6173 0a20 2020 2020 2020 206c 6f67 2061  as.        log a
+00003220: 7320 6974 2069 7320 6e6f 7420 636f 6e66  s it is not conf
+00003230: 6967 7572 6564 2066 6f72 2074 6865 2064  igured for the d
+00003240: 6566 6175 6c74 2072 6573 6f6c 7574 696f  efault resolutio
+00003250: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
+00003260: 0000 0a00 0000 1300 0000 73b6 0000 0088  ..........s.....
+00003270: 006a 007c 0019 007d 0188 006a 016a 0264  .j.|...}...j.j.d
+00003280: 017c 009b 009d 0219 0064 0219 007d 0288  .|.......d...}..
+00003290: 006a 037c 0019 006a 047d 037c 0264 0319  .j.|...j.}.|.d..
+000032a0: 007c 0364 0319 006b 0373 267c 0264 0419  .|.d...k.s&|.d..
+000032b0: 007c 0364 0419 006b 0372 5974 05a0 0664  .|.d...k.rYt...d
+000032c0: 057c 009b 0064 067c 0364 0364 0785 0219  .|...d.|.d.d....
+000032d0: 009b 0064 087c 0264 0364 0785 0219 009b  ...d.|.d.d......
+000032e0: 009d 06a1 0101 007c 01a0 077c 02a1 0101  .......|...|....
+000032f0: 0074 05a0 0664 097c 009b 0064 067c 0364  .t...d.|...d.|.d
+00003300: 0364 0785 0219 009b 0064 087c 0264 0364  .d.......d.|.d.d
+00003310: 0785 0219 009b 009d 06a1 0101 0064 0053  .............d.S
+00003320: 0064 0053 0029 0a4e 5a04 6361 6d5f da04  .d.S.).NZ.cam_..
+00003330: 7369 7a65 7201 0000 0072 7300 0000 7a27  sizer....rs...z'
+00003340: 4265 6769 6e6e 696e 6720 746f 2063 6861  Beginning to cha
+00003350: 6e67 6520 7265 736f 6c75 7469 6f6e 2061  nge resolution a
+00003360: 7420 706f 7274 207a 0620 6672 6f6d 2072  t port z. from r
+00003370: 5100 0000 7a04 2074 6f20 7a27 436f 6d70  Q...z. to z'Comp
+00003380: 6c65 7465 6420 6368 616e 6765 206f 6620  leted change of 
+00003390: 7265 736f 6c75 7469 6f6e 2061 7420 706f  resolution at po
+000033a0: 7274 2029 0872 2f00 0000 7228 0000 0072  rt ).r/...r(...r
+000033b0: 7400 0000 722e 0000 005a 1264 6566 6175  t...r....Z.defau
+000033c0: 6c74 5f72 6573 6f6c 7574 696f 6e72 5400  lt_resolutionrT.
+000033d0: 0000 7255 0000 005a 1163 6861 6e67 655f  ..rU...Z.change_
+000033e0: 7265 736f 6c75 7469 6f6e 2904 7244 0000  resolution).rD..
+000033f0: 0072 4500 0000 7294 0000 005a 0c64 6566  .rE...r....Z.def
+00003400: 6175 6c74 5f73 697a 6572 7000 0000 7225  ault_sizerp...r%
+00003410: 0000 0072 2600 0000 da11 6164 6a75 7374  ...r&.....adjust
+00003420: 5f72 6573 5f77 6f72 6b65 72d9 0100 0073  _res_worker....s
+00003430: 1800 0000 0a01 1601 0c01 2002 0401 2401  .......... ...$.
+00003440: 04ff 0a03 0401 2401 08ff 04fb 7a36 5365  ......$.....z6Se
+00003450: 7373 696f 6e2e 5f61 646a 7573 745f 7265  ssion._adjust_re
+00003460: 736f 6c75 7469 6f6e 732e 3c6c 6f63 616c  solutions.<local
+00003470: 733e 2e61 646a 7573 745f 7265 735f 776f  s>.adjust_res_wo
+00003480: 726b 6572 4e29 0472 0400 0000 722e 0000  rkerN).r....r...
+00003490: 0072 7f00 0000 7280 0000 0029 0472 3b00  .r....r....).r;.
+000034a0: 0000 7295 0000 0072 8100 0000 7244 0000  ..r....r....rD..
+000034b0: 0072 2500 0000 7270 0000 0072 2600 0000  .r%...rp...r&...
+000034c0: 7284 0000 00d5 0100 0073 0c00 0000 0c04  r........s......
+000034d0: 080e 0e01 0e01 02ff 22ff 7a1b 5365 7373  ........".z.Sess
+000034e0: 696f 6e2e 5f61 646a 7573 745f 7265 736f  ion._adjust_reso
+000034f0: 6c75 7469 6f6e 7363 0100 0000 0000 0000  lutionsc........
+00003500: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+00003510: 737a 0000 007c 006a 00a0 01a1 007c 005f  sz...|.j.....|._
+00003520: 027c 006a 00a0 03a1 007c 005f 0474 057c  .|.j.....|._.t.|
+00003530: 006a 047c 006a 0283 027c 005f 067c 006a  .j.|.j...|._.|.j
+00003540: 006a 0764 0119 0064 0219 007c 006a 065f  .j.d...d...|.j._
+00003550: 0864 037c 006a 006a 0764 0119 00a0 09a1  .d.|.j.j.d......
+00003560: 0076 0072 327c 006a 006a 0764 0119 0064  .v.r2|.j.j.d...d
+00003570: 0319 007c 006a 065f 0a74 0b7c 006a 067c  ...|.j._.t.|.j.|
+00003580: 006a 0c64 048d 027c 005f 0d64 0553 0029  .j.d...|._.d.S.)
+00003590: 067a f30a 2020 2020 2020 2020 466f 6c6c  .z..        Foll
+000035a0: 6f77 696e 6720 6361 7074 7572 6520 766f  owing capture vo
+000035b0: 6c75 6d65 206f 7074 696d 697a 6174 696f  lume optimizatio
+000035c0: 6e20 7669 6120 6275 6e64 6c65 2061 646a  n via bundle adj
+000035d0: 7573 746d 656e 742c 206f 7220 616c 7465  ustment, or alte
+000035e0: 7261 7469 6f6e 0a20 2020 2020 2020 2076  ration.        v
+000035f0: 6961 2061 2074 7261 6e73 666f 726d 206f  ia a transform o
+00003600: 6620 7468 6520 6f72 6967 696e 2c20 7468  f the origin, th
+00003610: 6520 656e 7469 7265 2063 6170 7475 7265  e entire capture
+00003620: 2076 6f6c 756d 6520 6361 6e20 6265 2072   volume can be r
+00003630: 656c 6f61 6465 640a 2020 2020 2020 2020  eloaded.        
+00003640: 6672 6f6d 2074 6865 2063 6f6e 6669 6720  from the config 
+00003650: 6461 7461 2077 6974 686f 7574 206e 6565  data without nee
+00003660: 6469 6e67 2074 6f20 676f 2074 6872 6f75  ding to go throu
+00003670: 6768 2074 6865 2073 7465 7073 0a0a 2020  gh the steps..  
+00003680: 2020 2020 2020 da0e 6361 7074 7572 655f        ..capture_
+00003690: 766f 6c75 6d65 da05 7374 6167 65da 116f  volume..stage..o
+000036a0: 7269 6769 6e5f 7379 6e63 5f69 6e64 6578  rigin_sync_index
+000036b0: 2901 7238 0000 004e 290e 7228 0000 0072  ).r8...N).r(...r
+000036c0: 1400 0000 da0f 706f 696e 745f 6573 7469  ......point_esti
+000036d0: 6d61 7465 7372 4d00 0000 724e 0000 0072  matesrM...rN...r
+000036e0: 1100 0000 7296 0000 0072 7400 0000 7297  ....r....rt...r.
+000036f0: 0000 0072 7f00 0000 7298 0000 0072 1200  ...r....r....r..
+00003700: 0000 7238 0000 00da 1271 7561 6c69 7479  ..r8.....quality
+00003710: 5f63 6f6e 7472 6f6c 6c65 7272 7000 0000  _controllerrp...
+00003720: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+00003730: 1d6c 6f61 645f 6573 7469 6d61 7465 645f  .load_estimated_
+00003740: 6361 7074 7572 655f 766f 6c75 6d65 eb01  capture_volume..
+00003750: 0000 7316 0000 000c 070c 0110 0114 0214  ..s.............
+00003760: 010a 0102 0108 ff02 0508 010c ff7a 2553  .............z%S
+00003770: 6573 7369 6f6e 2e6c 6f61 645f 6573 7469  ession.load_esti
+00003780: 6d61 7465 645f 6361 7074 7572 655f 766f  mated_capture_vo
+00003790: 6c75 6d65 6301 0000 0000 0000 0000 0000  lumec...........
+000037a0: 0002 0000 0005 0000 0043 0000 0073 a600  .........C...s..
+000037b0: 0000 7400 7c00 6a01 6a02 7c00 6a03 8302  ..t.|.j.j.|.j...
+000037c0: 7d01 7c01 6a04 6401 6402 8d01 0100 7405  }.|.j.d.d.....t.
+000037d0: 7c00 6a01 6a02 8301 a006 a100 7c00 5f07  |.j.j.......|._.
+000037e0: 7408 7c00 6a07 7c00 6a03 8302 7c00 5f09  t.|.j.|.j...|._.
+000037f0: 740a 7c00 6a07 7c00 6a09 8302 7c00 5f0b  t.|.j.|.j...|._.
+00003800: 7c00 6a0b a00c a100 0100 740d 7c00 6a0b  |.j.......t.|.j.
+00003810: 7c00 6a0e 8302 7c00 5f0f 7410 a011 6403  |.j...|._.t...d.
+00003820: 7412 6404 1400 9b00 6405 9d03 a101 0100  t.d.....d.......
+00003830: 7c00 6a0f a013 7412 a101 0100 7c00 6a0b  |.j...t.....|.j.
+00003840: a00c a100 0100 7c00 6a01 a014 7c00 6a0b  ......|.j...|.j.
+00003850: a101 0100 6406 5300 2907 7ad7 0a20 2020  ....d.S.).z..   
+00003860: 2020 2020 2054 6869 7320 6973 2077 6865       This is whe
+00003870: 7265 2074 6865 2063 616d 6572 6120 6172  re the camera ar
+00003880: 7261 7920 3620 446f 4620 6973 2073 6574  ray 6 DoF is set
+00003890: 2e20 4d61 6e79 2c20 6d61 6e79 2074 6869  . Many, many thi
+000038a0: 6e67 7320 6172 6520 6861 7070 656e 696e  ngs are happenin
+000038b0: 670a 2020 2020 2020 2020 6865 7265 2c20  g.        here, 
+000038c0: 6275 7420 7468 6579 2061 7265 2061 6c6c  but they are all
+000038d0: 206e 6563 6573 7361 7279 2073 7465 7073   necessary steps
+000038e0: 206f 6620 7468 6520 7072 6f63 6573 7320   of the process 
+000038f0: 736f 2049 2064 6964 6e27 7420 7761 6e74  so I didn't want
+00003900: 2074 6f0a 2020 2020 2020 2020 7472 7920   to.        try 
+00003910: 746f 2065 6e63 6170 7375 6c61 7465 2061  to encapsulate a
+00003920: 6e79 2066 7572 7468 6572 0a20 2020 2020  ny further.     
+00003930: 2020 2072 1800 0000 2901 5a0e 626f 6172     r....).Z.boar
+00003940: 6473 5f73 616d 706c 6564 7a1b 5265 6d6f  ds_sampledz.Remo
+00003950: 7669 6e67 2074 6865 2077 6f72 7374 2066  ving the worst f
+00003960: 6974 7469 6e67 20e9 6400 0000 7a21 2070  itting .d...z! p
+00003970: 6572 6365 6e74 206f 6620 706f 696e 7473  ercent of points
+00003980: 2066 726f 6d20 7468 6520 6d6f 6465 6c4e   from the modelN
+00003990: 2915 720f 0000 0072 2800 0000 5a09 746f  ).r....r(...Z.to
+000039a0: 6d6c 5f70 6174 6872 2d00 0000 5a14 7374  ml_pathr-...Z.st
+000039b0: 6572 656f 5f63 616c 6962 7261 7465 5f61  ereo_calibrate_a
+000039c0: 6c6c 720d 0000 005a 1567 6574 5f62 6573  llr....Z.get_bes
+000039d0: 745f 6361 6d65 7261 5f61 7272 6179 724e  t_camera_arrayrN
+000039e0: 0000 0072 1400 0000 7299 0000 0072 1100  ...r....r....r..
+000039f0: 0000 7296 0000 00da 086f 7074 696d 697a  ..r......optimiz
+00003a00: 6572 1200 0000 7238 0000 0072 9a00 0000  er....r8...r....
+00003a10: 7254 0000 0072 5500 0000 da11 4649 4c54  rT...rU.....FILT
+00003a20: 4552 4544 5f46 5241 4354 494f 4e5a 1666  ERED_FRACTIONZ.f
+00003a30: 696c 7465 725f 706f 696e 745f 6573 7469  ilter_point_esti
+00003a40: 6d61 7465 735a 1373 6176 655f 6361 7074  matesZ.save_capt
+00003a50: 7572 655f 766f 6c75 6d65 2902 723b 0000  ure_volume).r;..
+00003a60: 005a 1073 7465 7265 6f63 616c 6962 7261  .Z.stereocalibra
+00003a70: 746f 7272 2500 0000 7225 0000 0072 2600  torr%...r%...r&.
+00003a80: 0000 da13 6573 7469 6d61 7465 5f65 7874  ....estimate_ext
+00003a90: 7269 6e73 6963 7301 0200 0073 2a00 0000  rinsics....s*...
+00003aa0: 0206 0a01 04ff 0c03 0202 0601 02ff 0402  ................
+00003ab0: 04fe 0204 0801 06ff 1004 0a01 1002 0402  ................
+00003ac0: 0e01 04ff 0c03 0a01 1202 7a1b 5365 7373  ..........z.Sess
+00003ad0: 696f 6e2e 6573 7469 6d61 7465 5f65 7874  ion.estimate_ext
+00003ae0: 7269 6e73 6963 7372 6d00 0000 2901 4629  rinsicsrm...).F)
+00003af0: 2972 1b00 0000 721c 0000 0072 1d00 0000  )r....r....r....
+00003b00: 7203 0000 0072 8700 0000 7242 0000 0072  r....r....rB...r
+00003b10: 9300 0000 7292 0000 0072 1900 0000 5a13  ....r....r....Z.
+00003b20: 6d6f 6465 5f63 6861 6e67 655f 7375 6363  mode_change_succ
+00003b30: 6573 7372 1500 0000 722a 0000 0072 4800  essr....r*...rH.
+00003b40: 0000 724b 0000 0072 5000 0000 7257 0000  ..rK...rP...rW..
+00003b50: 0072 5900 0000 7260 0000 0072 6900 0000  .rY...r`...ri...
+00003b60: da03 696e 7472 6b00 0000 726e 0000 0072  ..intrk...rn...r
+00003b70: 6100 0000 da04 626f 6f6c 7266 0000 0072  a.....boolrf...r
+00003b80: 6500 0000 7271 0000 0072 7200 0000 727a  e...rq...rr...rz
+00003b90: 0000 0072 8300 0000 7264 0000 0072 8500  ...r....rd...r..
+00003ba0: 0000 7267 0000 0072 6300 0000 7205 0000  ..rg...rc...r...
+00003bb0: 0072 9000 0000 7291 0000 0072 8400 0000  .r....r....r....
+00003bc0: 729b 0000 0072 9f00 0000 da0d 5f5f 636c  r....r......__cl
+00003bd0: 6173 7363 656c 6c5f 5f72 2500 0000 7225  asscell__r%...r%
+00003be0: 0000 0072 3c00 0000 7226 0000 0072 2700  ...r<...r&...r'.
+00003bf0: 0000 3000 0000 734a 0000 0008 0006 0106  ..0...sJ........
+00003c00: 0106 0106 0108 0212 0208 2208 1208 0708  ..........".....
+00003c10: 0b08 1d08 1e0e 100e 410e 1608 0f0e 0608  ........A.......
+00003c20: 0408 0608 0408 0408 0708 2308 2810 0b08  ..........#.(...
+00003c30: 0d02 0a04 ff02 0102 ff02 010a ff08 0c08  ................
+00003c40: 0f08 1610 1672 2700 0000 2933 da0d 7079  .....r'...)3..py
+00003c50: 7879 3364 2e6c 6f67 6765 72da 0670 7978  xy3d.logger..pyx
+00003c60: 7933 6472 5400 0000 da03 6765 7472 1b00  y3drT.....getr..
+00003c70: 0000 da0c 5079 5174 362e 5174 436f 7265  ....PyQt6.QtCore
+00003c80: 7202 0000 0072 0300 0000 5a12 636f 6e63  r....r....Z.conc
+00003c90: 7572 7265 6e74 2e66 7574 7572 6573 7204  urrent.futuresr.
+00003ca0: 0000 00da 0770 6174 686c 6962 7205 0000  .....pathlibr...
+00003cb0: 00da 0474 696d 6572 0600 0000 da04 656e  ...timer......en
+00003cc0: 756d 7207 0000 0072 0800 0000 da1f 7079  umr....r......py
+00003cd0: 7879 3364 2e74 7261 636b 6572 732e 6368  xy3d.trackers.ch
+00003ce0: 6172 7563 6f5f 7472 6163 6b65 7272 0900  aruco_trackerr..
+00003cf0: 0000 5a21 7079 7879 3364 2e63 616c 6962  ..Z!pyxy3d.calib
+00003d00: 7261 7469 6f6e 2e6d 6f6e 6f63 616c 6962  ration.monocalib
+00003d10: 7261 746f 7272 0a00 0000 5a15 7079 7879  ratorr....Z.pyxy
+00003d20: 3364 2e63 616d 6572 6173 2e63 616d 6572  3d.cameras.camer
+00003d30: 6172 0b00 0000 5a1b 7079 7879 3364 2e63  ar....Z.pyxy3d.c
+00003d40: 616d 6572 6173 2e73 796e 6368 726f 6e69  ameras.synchroni
+00003d50: 7a65 7272 0c00 0000 5a27 7079 7879 3364  zerr....Z'pyxy3d
+00003d60: 2e63 616d 6572 6173 2e63 616d 6572 615f  .cameras.camera_
+00003d70: 6172 7261 795f 696e 6974 6961 6c69 7a65  array_initialize
+00003d80: 7272 0d00 0000 5a10 7079 7879 3364 2e69  rr....Z.pyxy3d.i
+00003d90: 6e74 6572 6661 6365 720e 0000 005a 2370  nterfacer....Z#p
+00003da0: 7978 7933 642e 6361 6c69 6272 6174 696f  yxy3d.calibratio
+00003db0: 6e2e 7374 6572 656f 6361 6c69 6272 6174  n.stereocalibrat
+00003dc0: 6f72 720f 0000 005a 3170 7978 7933 642e  orr....Z1pyxy3d.
+00003dd0: 6361 6c69 6272 6174 696f 6e2e 6361 7074  calibration.capt
+00003de0: 7572 655f 766f 6c75 6d65 2e70 6f69 6e74  ure_volume.point
+00003df0: 5f65 7374 696d 6174 6573 7210 0000 005a  _estimatesr....Z
+00003e00: 3070 7978 7933 642e 6361 6c69 6272 6174  0pyxy3d.calibrat
+00003e10: 696f 6e2e 6361 7074 7572 655f 766f 6c75  ion.capture_volu
+00003e20: 6d65 2e63 6170 7475 7265 5f76 6f6c 756d  me.capture_volum
+00003e30: 6572 1100 0000 5a34 7079 7879 3364 2e63  er....Z4pyxy3d.c
+00003e40: 616c 6962 7261 7469 6f6e 2e63 6170 7475  alibration.captu
+00003e50: 7265 5f76 6f6c 756d 652e 7175 616c 6974  re_volume.qualit
+00003e60: 795f 636f 6e74 726f 6c6c 6572 7212 0000  y_controllerr...
+00003e70: 005a 1b70 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
+00003e80: 732e 6361 6d65 7261 5f61 7272 6179 7213  s.camera_arrayr.
+00003e90: 0000 005a 4670 7978 7933 642e 6361 6c69  ...ZFpyxy3d.cali
+00003ea0: 6272 6174 696f 6e2e 6361 7074 7572 655f  bration.capture_
+00003eb0: 766f 6c75 6d65 2e68 656c 7065 725f 6675  volume.helper_fu
+00003ec0: 6e63 7469 6f6e 732e 6765 745f 706f 696e  nctions.get_poin
+00003ed0: 745f 6573 7469 6d61 7465 7372 1400 0000  t_estimatesr....
+00003ee0: da13 7079 7879 3364 2e63 6f6e 6669 6775  ..pyxy3d.configu
+00003ef0: 7261 746f 7272 1500 0000 5a1a 7079 7879  ratorr....Z.pyxy
+00003f00: 3364 2e63 616d 6572 6173 2e6c 6976 655f  3d.cameras.live_
+00003f10: 7374 7265 616d 7216 0000 005a 1f70 7978  streamr....Z.pyx
+00003f20: 7933 642e 7265 636f 7264 696e 672e 7669  y3d.recording.vi
+00003f30: 6465 6f5f 7265 636f 7264 6572 7217 0000  deo_recorderr...
+00003f40: 0072 7e00 0000 729e 0000 0072 1900 0000  .r~...r....r....
+00003f50: 7227 0000 0072 2500 0000 7225 0000 0072  r'...r%...r%...r
+00003f60: 2500 0000 7226 0000 00da 083c 6d6f 6475  %...r&.....<modu
+00003f70: 6c65 3e01 0000 0073 3400 0000 0801 0c02  le>....s4.......
+00003f80: 1002 0c01 0c01 0c01 1001 0c02 0c01 0c01  ................
+00003f90: 0c01 0c01 0c01 0c02 0c01 0c01 0c01 0c02  ................
+00003fa0: 0c01 0c03 0c01 0c01 0403 0401 1003 140b  ................
```

### Comparing `pyxy3d-0.0.21/pyxy3d/session/session.py` & `pyxy3d-0.0.22/pyxy3d/session/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,28 +234,37 @@
                 self.charuco_tracker = CharucoTracker(self.charuco)
                 if not self.stream_tools_loaded:
                     self.load_stream_tools()
 
                 self.pause_all_monocalibrators()
                 self.set_streams_charuco()
                 self.set_streams_tracking(True)
+                
                 self.synchronizer.subscribe_to_streams()
 
             case SessionMode.CaptureVolumeOrigin:
                 if self.stream_tools_loaded:
                     self.pause_all_monocalibrators()
                     self.synchronizer.unsubscribe_from_streams()
 
             case SessionMode.Recording:
+                logger.info("Attempting to set recording mode")
                 if not self.stream_tools_loaded:
+                    logger.info("Stream tools not loaded, so loading them up...")
                     self.load_stream_tools()
 
+                logger.info("Pausing monocals to enter recording mode")
                 self.pause_all_monocalibrators()
+                
+                logger.info("Stop tracking for recording mode")
                 self.set_streams_tracking(False)
+                logger.info("Update stream fps to recording fps")
                 self.update_streams_fps()
+                
+                logger.info("Subscribe synchronizer to streams so video recorder can manage")
                 self.synchronizer.subscribe_to_streams()
 
     def set_active_mode_fps(self, fps_target: int):
         """
         Updates the FPS used by the currently active session mode
         This update includes the config.toml
         """
@@ -385,19 +394,21 @@
         self.synchronizer = Synchronizer(
             self.streams
         )  # defaults to stream default fps of 6
 
         # recording widget becomes available when synchronizer is created
         self.stream_tools_loaded = True
         self.stream_tools_in_process = False
-        logger.info(f"Signalling successful loading of stream tools")
-        self.stream_tools_loaded_signal.emit()
 
+        logger.info("Pausing stream tools since default loads to charuco")
         self.pause_all_monocalibrators()
         self.pause_synchronizer()
+        
+        logger.info(f"Signalling successful loading of stream tools")
+        self.stream_tools_loaded_signal.emit()
 
     def _load_monocalibrators(self):
         for port, cam in self.cameras.items():
             if port in self.monocalibrators.keys():
                 logger.info(
                     f"Skipping over monocalibrator creation for port {port} because it already exists."
                 )
```

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.0.22/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.0.22/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/helper.py` & `pyxy3d-0.0.22/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.0.22/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.0.22/pyxy3d/trackers/holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.0.22/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.0.22/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc` & `pyxy3d-0.0.22/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.0.22/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.0.22/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.0.22/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.21/README.md` & `pyxy3d-0.0.22/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
-## Description
+#### Table of Contents
 
-Pyxy3D is an open-source python tool for converting two-dimensional (x,y) coordinates obtained from multiple standard webcams into 3D point estimates. It provides an integrated system for camera calibration and point triangulation that enables the creation of cost-efficient small scale motion capture systems. When combined with markerless tracking algorithms such as Google's Mediapipe, it is possible to perform markerless 3D tracking with a standard computer and a couple webcams. 
+[Introduction](#introduction)
 
-## Video Walkthrough
+[Quick Start](#quick-start)
 
-### Installation
+[Key Features](#key-features)
 
+[Limitations](#limitations)
 
+[Known Issues](#known-issues)
 
-### A complete session
+---
+## About
+Pyxy3D is an open-source python package designed for two primary purposes: calibrating DIY motion capture systems and triangulating the 3D position of tracked landmarks where (x,y) coordinates have been identified across concurrent frames. 
 
 
+## Quick Start
 
+1. Create a new virtual environment with Python 3.10 or later
+2. Activate the virtual environment
+3. Install pyxy3d
+4. Launch pyxy3d
 
 ## Key Features
 
 The project leans heavily upon OpenCV, SciPy, and PyQt to provide the following **key features**:
 
 - User-friendly graphical user interface (GUI)
 - Easy creation and modification of the charuco calibration board
@@ -34,86 +43,25 @@
 - Visualization of triangulated points for quick confirmation of output quality
 - Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
 - MediaPipe is only configured to run on Windows
-    - while the camera calibration will likely work on other systems, the markerless tracking will not (currently)
-- It does not support anything other than standard webcams. 
-    - I currently have no intention of supporting mobile phones as cameras for the system
-- Based on recent testing, some webcams will deliver poor connection times/frame rates/calibrations. I'm currently using 4 EMEET SmartCam C960 cameras. These are inexpensive (~$25 each) and readily available. They deliver decent results at 30 fps and 720p. I welcome feedback about user experiences with other cameras
-- No real-time tracking
-    - the underlying data processing pipeline was designed to accommodate real-time tracking but I want to make sure that everything works well with the simpler and more stable post-processing workflow before trying to get that implemented in an integrated way
+    - while the camera calibration will likely work on other systems, the included sample markerless tracking will not (currently)
+- It does not support anything other than standard webcams at the moment 
+    - calibration in post-processing is on the development roadmap
+    - once calibration in post is implemented, a method of synchronize pre-recorded frames will still be needed
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
 ## Known Issues
 
+### Crashes in the main GUI 
 The main GUI allows for accessing of all of the package's functionality at once, though this imposes some additional processing overhead that can undermine recording, and switching between GUI modes can provoke crashes. Improvements are on the To Do list, but in the meantime can be sidestepped by launching individual widgets from the command line as [described below](#3-launch-from-the-command-line)
 
-## Installation
-
-Pyxy3D is installable via pip and the GUI can be launched from the command line. It is **strongly** advised that you do so within a virtual environment. The package requires [Python 3.10](https://www.python.org/downloads/release/python-3100/)  or higher. Because the Mediapipe implementation only works on Windows currently, these steps assume you are installing on Windows 10.
-
-### 1. Create a virtual environment
-
-Find the path to your python.exe file. You can install Python 3.10 from [here](https://www.python.org/downloads/release/python-3100/). For me the path is `C:\Python310\python.exe`
-
-Create a folder where you would like the code and virtual environment to live. This can be different from the folder where your motion capture calibration and recording data is stored. Open the folder and right click within it, select  ![Pasted image 20230608102647](https://github.com/mprib/pyxy3d/assets/31831778/5c0ad5a7-fa57-473b-a549-243d93628dd3)
- from the context menu to launch a terminal. 
-   
-Run the following at the command prompt. Substitute in the path to `python.exe` that is true for your machine
-```
-C:\Python310\python.exe -m venv .venv
-```
-
-This will create a fresh version of python within that folder which you will use to manage your project. Activate the environment using the following command (if this exact command doesn't work, then [some other variation will](https://docs.python.org/3/library/venv.html#how-venvs-work))
-```
-.\.venv\Scripts\activate
-```
-
-The terminal should now show the environment is activated with something like this green parenthetical:
-![Pasted image 20230608095719](https://github.com/mprib/pyxy3d/assets/31831778/10a91524-9a81-41d1-b27b-0b6ba723cb27)
-
-You can confirm that your python path is set by running
-
-```
-python -c "import sys; print(sys.executable)"
-```
-which should point to the file in the virtual environment you created:
-![Pasted image 20230608100059](https://github.com/mprib/pyxy3d/assets/31831778/e214ebae-692c-4b50-b6f4-f34dcb44df43)
-
-### 2. Install pyxy3D via pip
-
-You are now ready to install pyxy3D from the Python Package Index (PyPI) via pip:
-
-```
-pip install pyxy3d
-```
-
-Installation may take a moment...
-
-### 3. Launch from the command line
-With the package installed and the virtual environment activated, the main GUI can be launched by running the following command to launch the tool:
-
-```
-pyxy3d
-```
-
-A video walkthrough of a sample session is [here]()
-
-If you experience crashes after initializing the session folder, then you can launch the individual interface components one at a time as needed. **NAVIGATE TO THE FOLDER OF THE SESSION YOU WANT TO LAUNCH** and run one of the following as needed: `charuco`, `cameras`, `calibrate`, `record`, `process`
-
-For example, if you are getting crashes when trying to record, within the terminal navigate to the session folder you previously created and run:
-
-```
-pyxy3d record
-```
-
-A recording widget will open up that should be more efficient and stable than the complete GUI.
 
 
 ## Reporting Issues and Requesting Features
 
 To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
```

### Comparing `pyxy3d-0.0.21/PKG-INFO` & `pyxy3d-0.0.22/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.0.21
+Version: 0.0.22
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -22,28 +22,37 @@
 Project-URL: repository, https://github.com/mprib/pyxy3d
 Description-Content-Type: text/markdown
 
 
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
-## Description
+#### Table of Contents
 
-Pyxy3D is an open-source python tool for converting two-dimensional (x,y) coordinates obtained from multiple standard webcams into 3D point estimates. It provides an integrated system for camera calibration and point triangulation that enables the creation of cost-efficient small scale motion capture systems. When combined with markerless tracking algorithms such as Google's Mediapipe, it is possible to perform markerless 3D tracking with a standard computer and a couple webcams. 
+[Introduction](#introduction)
 
-## Video Walkthrough
+[Quick Start](#quick-start)
 
-### Installation
+[Key Features](#key-features)
 
+[Limitations](#limitations)
 
+[Known Issues](#known-issues)
 
-### A complete session
+---
+## About
+Pyxy3D is an open-source python package designed for two primary purposes: calibrating DIY motion capture systems and triangulating the 3D position of tracked landmarks where (x,y) coordinates have been identified across concurrent frames. 
 
 
+## Quick Start
 
+1. Create a new virtual environment with Python 3.10 or later
+2. Activate the virtual environment
+3. Install pyxy3d
+4. Launch pyxy3d
 
 ## Key Features
 
 The project leans heavily upon OpenCV, SciPy, and PyQt to provide the following **key features**:
 
 - User-friendly graphical user interface (GUI)
 - Easy creation and modification of the charuco calibration board
@@ -58,86 +67,25 @@
 - Visualization of triangulated points for quick confirmation of output quality
 - Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
 - MediaPipe is only configured to run on Windows
-    - while the camera calibration will likely work on other systems, the markerless tracking will not (currently)
-- It does not support anything other than standard webcams. 
-    - I currently have no intention of supporting mobile phones as cameras for the system
-- Based on recent testing, some webcams will deliver poor connection times/frame rates/calibrations. I'm currently using 4 EMEET SmartCam C960 cameras. These are inexpensive (~$25 each) and readily available. They deliver decent results at 30 fps and 720p. I welcome feedback about user experiences with other cameras
-- No real-time tracking
-    - the underlying data processing pipeline was designed to accommodate real-time tracking but I want to make sure that everything works well with the simpler and more stable post-processing workflow before trying to get that implemented in an integrated way
+    - while the camera calibration will likely work on other systems, the included sample markerless tracking will not (currently)
+- It does not support anything other than standard webcams at the moment 
+    - calibration in post-processing is on the development roadmap
+    - once calibration in post is implemented, a method of synchronize pre-recorded frames will still be needed
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
 ## Known Issues
 
+### Crashes in the main GUI 
 The main GUI allows for accessing of all of the package's functionality at once, though this imposes some additional processing overhead that can undermine recording, and switching between GUI modes can provoke crashes. Improvements are on the To Do list, but in the meantime can be sidestepped by launching individual widgets from the command line as [described below](#3-launch-from-the-command-line)
 
-## Installation
-
-Pyxy3D is installable via pip and the GUI can be launched from the command line. It is **strongly** advised that you do so within a virtual environment. The package requires [Python 3.10](https://www.python.org/downloads/release/python-3100/)  or higher. Because the Mediapipe implementation only works on Windows currently, these steps assume you are installing on Windows 10.
-
-### 1. Create a virtual environment
-
-Find the path to your python.exe file. You can install Python 3.10 from [here](https://www.python.org/downloads/release/python-3100/). For me the path is `C:\Python310\python.exe`
-
-Create a folder where you would like the code and virtual environment to live. This can be different from the folder where your motion capture calibration and recording data is stored. Open the folder and right click within it, select  ![Pasted image 20230608102647](https://github.com/mprib/pyxy3d/assets/31831778/5c0ad5a7-fa57-473b-a549-243d93628dd3)
- from the context menu to launch a terminal. 
-   
-Run the following at the command prompt. Substitute in the path to `python.exe` that is true for your machine
-```
-C:\Python310\python.exe -m venv .venv
-```
-
-This will create a fresh version of python within that folder which you will use to manage your project. Activate the environment using the following command (if this exact command doesn't work, then [some other variation will](https://docs.python.org/3/library/venv.html#how-venvs-work))
-```
-.\.venv\Scripts\activate
-```
-
-The terminal should now show the environment is activated with something like this green parenthetical:
-![Pasted image 20230608095719](https://github.com/mprib/pyxy3d/assets/31831778/10a91524-9a81-41d1-b27b-0b6ba723cb27)
-
-You can confirm that your python path is set by running
-
-```
-python -c "import sys; print(sys.executable)"
-```
-which should point to the file in the virtual environment you created:
-![Pasted image 20230608100059](https://github.com/mprib/pyxy3d/assets/31831778/e214ebae-692c-4b50-b6f4-f34dcb44df43)
-
-### 2. Install pyxy3D via pip
-
-You are now ready to install pyxy3D from the Python Package Index (PyPI) via pip:
-
-```
-pip install pyxy3d
-```
-
-Installation may take a moment...
-
-### 3. Launch from the command line
-With the package installed and the virtual environment activated, the main GUI can be launched by running the following command to launch the tool:
-
-```
-pyxy3d
-```
-
-A video walkthrough of a sample session is [here]()
-
-If you experience crashes after initializing the session folder, then you can launch the individual interface components one at a time as needed. **NAVIGATE TO THE FOLDER OF THE SESSION YOU WANT TO LAUNCH** and run one of the following as needed: `charuco`, `cameras`, `calibrate`, `record`, `process`
-
-For example, if you are getting crashes when trying to record, within the terminal navigate to the session folder you previously created and run:
-
-```
-pyxy3d record
-```
-
-A recording widget will open up that should be more efficient and stable than the complete GUI.
 
 
 ## Reporting Issues and Requesting Features
 
 To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
```

