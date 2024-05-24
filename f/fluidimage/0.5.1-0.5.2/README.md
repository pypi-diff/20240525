# Comparing `tmp/fluidimage-0.5.1.tar.gz` & `tmp/fluidimage-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidimage-0.5.1.tar", last modified: Mon May  6 09:04:16 2024, max compression
+gzip compressed data, was "fluidimage-0.5.2.tar", last modified: Fri May 24 21:35:17 2024, max compression
```

## Comparing `fluidimage-0.5.1.tar` & `fluidimage-0.5.2.tar`

### file list

```diff
@@ -1,263 +1,270 @@
--rw-r--r--   0        0        0       58 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.flake8
--rw-r--r--   0        0        0     1166 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.github/workflows/ci-linux.yml
--rw-r--r--   0        0        0      554 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.github/workflows/ci-pixi.yml
--rw-r--r--   0        0        0     3919 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     3223 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     1151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.hgtags
--rw-r--r--   0        0        0       43 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.mdformat.toml
--rw-r--r--   0        0        0      376 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.readthedocs.yml
--rw-r--r--   0        0        0      210 2024-05-06 08:54:34.000000 fluidimage-0.5.1/AUTHORS.md
--rw-r--r--   0        0        0     7668 2024-05-06 08:54:34.000000 fluidimage-0.5.1/CHANGES.md
--rw-r--r--   0        0        0     1266 2024-05-06 08:54:34.000000 fluidimage-0.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    21781 2024-05-06 08:54:34.000000 fluidimage-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0      205 2024-05-06 08:54:34.000000 fluidimage-0.5.1/MANIFEST.in
--rw-r--r--   0        0        0      309 2024-05-06 08:54:34.000000 fluidimage-0.5.1/Makefile
--rw-r--r--   0        0        0     3151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/README.md
--rw-r--r--   0        0        0     1266 2024-05-06 09:04:15.958915 fluidimage-0.5.1/doc/CONTRIBUTING.md
--rw-r--r--   0        0        0     5780 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/Makefile
--rw-r--r--   0        0        0      210 2024-05-06 09:04:15.958915 fluidimage-0.5.1/doc/authors.md
--rw-r--r--   0        0        0      748 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/autosum.rst
--rw-r--r--   0        0        0     8443 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/build-from-source.md
--rw-r--r--   0        0        0     7668 2024-05-06 09:04:15.958915 fluidimage-0.5.1/doc/changes.md
--rw-r--r--   0        0        0     9545 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/conf.py
--rw-r--r--   0        0        0       36 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/Makefile
--rw-r--r--   0        0        0      275 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/bos_parallel.md
--rw-r--r--   0        0        0      708 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/bos_parallel.py
--rw-r--r--   0        0        0      914 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/im2im_parallel.py
--rw-r--r--   0        0        0      442 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/im2im_try_params.py
--rw-r--r--   0        0        0      217 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/my_example_im2im.py
--rw-r--r--   0        0        0      370 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/my_example_im2im_class.py
--rw-r--r--   0        0        0      375 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_parallel.md
--rw-r--r--   0        0        0      864 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_parallel.py
--rw-r--r--   0        0        0      645 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_try_params.md
--rw-r--r--   0        0        0      675 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_try_params.py
--rw-r--r--   0        0        0     2124 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/README.md
--rw-r--r--   0        0        0        0 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/__init__.py
--rw-r--r--   0        0        0     1386 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/args.py
--rwxr-xr-x   0        0        0      779 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/job_piv.py
--rwxr-xr-x   0        0        0     1095 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/job_pre.py
--rwxr-xr-x   0        0        0     2086 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/params_piv.py
--rwxr-xr-x   0        0        0     1811 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/params_pre.py
--rwxr-xr-x   0        0        0      672 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/submit_piv.py
--rwxr-xr-x   0        0        0      787 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/submit_pre.py
--rw-r--r--   0        0        0      896 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/test_piv_as_real.py
--rwxr-xr-x   0        0        0      724 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/try_piv.py
--rwxr-xr-x   0        0        0      538 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/try_pre.py
--rw-r--r--   0        0        0      457 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_cluster.md
--rw-r--r--   0        0        0      918 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel.md
--rw-r--r--   0        0        0      827 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel.py
--rw-r--r--   0        0        0      536 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel_complete.py
--rw-r--r--   0        0        0      953 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel_im2im.py
--rw-r--r--   0        0        0      989 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel_im2im_class.py
--rw-r--r--   0        0        0      863 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params.md
--rw-r--r--   0        0        0      614 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params.py
--rw-r--r--   0        0        0      747 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params_Karman.py
--rw-r--r--   0        0        0      814 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params_with_im2im_preproc.py
--rw-r--r--   0        0        0      380 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/README.md
--rw-r--r--   0        0        0      908 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/bench_piv_2005C.py
--rw-r--r--   0        0        0     1419 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/download.py
--rw-r--r--   0        0        0      744 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/path_images.py
--rw-r--r--   0        0        0      437 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2001A_topology.py
--rw-r--r--   0        0        0      496 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2001A_work.py
--rw-r--r--   0        0        0      622 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_topology.py
--rw-r--r--   0        0        0      682 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_work.py
--rw-r--r--   0        0        0      117 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/possible_paths.txt
--rw-r--r--   0        0        0     1413 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc.md
--rw-r--r--   0        0        0     1061 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_parallel.py
--rw-r--r--   0        0        0      816 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_sback1_filter.py
--rw-r--r--   0        0        0     1037 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_sback2_rescale.py
--rw-r--r--   0        0        0      544 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_try_params.py
--rw-r--r--   0        0        0      364 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_try_params_opencv.py
--rw-r--r--   0        0        0     1552 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/profile_piv_work.py
--rw-r--r--   0        0        0      448 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/submit_job_legi.py
--rw-r--r--   0        0        0      711 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/surface_tracking.py
--rw-r--r--   0        0        0     1201 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/test_run_examples.py
--rw-r--r--   0        0        0      357 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples.md
--rw-r--r--   0        0        0      238 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/for_dev.md
--rw-r--r--   0        0        0      673 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/index.md
--rw-r--r--   0        0        0     1686 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/install.md
--rw-r--r--   0        0        0      405 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/ipynbslides/README.txt
--rw-r--r--   0        0        0   493343 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/ipynbslides/fluidimage_legi_20170403.ipynb
--rw-r--r--   0        0        0     2094 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/overview.md
--rw-r--r--   0        0        0     1424 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/overview_orga_package.md
--rw-r--r--   0        0        0     1857 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/related_codes.md
--rw-r--r--   0        0        0       77 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/to_do.md
--rw-r--r--   0        0        0      432 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorial.md
--rw-r--r--   0        0        0     3116 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_calibration2dsimple.md
--rw-r--r--   0        0        0     2412 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_direct_calibration.md
--rw-r--r--   0        0        0     7352 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_opencv_calibration.md
--rw-r--r--   0        0        0     4407 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_opencv_tomo_reconstruct.md
--rw-r--r--   0        0        0     8785 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_piv.md
--rw-r--r--   0        0        0     2950 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_stereo_reconstruction.md
--rw-r--r--   0        0        0     1367 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_tsai_calibration.md
--rw-r--r--   0        0        0     8971 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/uvmat.md
--rw-r--r--   0        0        0     1252 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/Dockerfile
--rw-r--r--   0        0        0     1147 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/Makefile
--rw-r--r--   0        0        0      618 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/hgrc
--rw-r--r--   0        0        0       77 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/pythranrc
--rw-r--r--   0        0        0     1803 2024-05-06 08:54:34.000000 fluidimage-0.5.1/meson.build
--rw-r--r--   0        0        0      655 2024-05-06 08:54:34.000000 fluidimage-0.5.1/meson.options
--rw-r--r--   0        0        0     4888 2024-05-06 08:54:34.000000 fluidimage-0.5.1/noxfile.py
--rw-r--r--   0        0        0   310844 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pdm.lock
--rw-r--r--   0        0        0   782153 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pixi.lock
--rw-r--r--   0        0        0     1009 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pixi.toml
--rw-r--r--   0        0        0    21630 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pylintrc
--rw-r--r--   0        0        0     4483 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3311 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/__init__.py
--rw-r--r--   0        0        0      534 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/_opencv.py
--rw-r--r--   0        0        0      162 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/_version.py
--rw-r--r--   0        0        0      278 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/bos.py
--rw-r--r--   0        0        0      263 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/__init__.py
--rw-r--r--   0        0        0     2858 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/_evaluate_subpix.py
--rw-r--r--   0        0        0      878 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/correl.cu
--rw-r--r--   0        0        0    21039 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/correl.py
--rw-r--r--   0        0        0    10794 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/correl_pycuda.py
--rw-r--r--   0        0        0      333 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/errors.py
--rw-r--r--   0        0        0     7467 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/fft.py
--rw-r--r--   0        0        0      132 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/__init__.py
--rw-r--r--   0        0        0      613 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/griddata.py
--rw-r--r--   0        0        0      388 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/meson.build
--rw-r--r--   0        0        0      867 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py
--rw-r--r--   0        0        0     8006 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline.py
--rw-r--r--   0        0        0    10312 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py
--rw-r--r--   0        0        0     4807 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/mean_neighbors.py
--rw-r--r--   0        0        0      489 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/meson.build
--rw-r--r--   0        0        0    39595 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    37615 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    36317 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    35832 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    37828 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    38146 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    36451 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    34562 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0     1188 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/reduction_kernel.cu
--rw-r--r--   0        0        0     6180 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/subpix.py
--rw-r--r--   0        0        0     6544 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/test_correl.py
--rw-r--r--   0        0        0     2519 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/test_fft.py
--rw-r--r--   0        0        0      465 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/__init__.py
--rw-r--r--   0        0        0     3587 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib2d_simple.py
--rw-r--r--   0        0        0     9318 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib_cv.py
--rw-r--r--   0        0        0    23798 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib_direct.py
--rw-r--r--   0        0        0     7528 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib_tsai.py
--rw-r--r--   0        0        0      302 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/meson.build
--rw-r--r--   0        0        0     2033 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/test_calib_cv.py
--rw-r--r--   0        0        0     2609 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/test_direct_stereo_reconstruction.py
--rw-r--r--   0        0        0     1302 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/test_tsai_calibration.py
--rw-r--r--   0        0        0     4272 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/util.py
--rw-r--r--   0        0        0      739 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/config.py
--rw-r--r--   0        0        0     1434 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/conftest.py
--rw-r--r--   0        0        0      274 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/__init__.py
--rw-r--r--   0        0        0    13511 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/display_piv.py
--rw-r--r--   0        0        0     4822 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/display_pre.py
--rw-r--r--   0        0        0      214 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/meson.build
--rw-r--r--   0        0        0    26293 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/piv.py
--rw-r--r--   0        0        0     4457 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/preproc.py
--rw-r--r--   0        0        0      425 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/test_piv.py
--rw-r--r--   0        0        0     9009 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/tomo.py
--rw-r--r--   0        0        0     3376 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/__init__.py
--rw-r--r--   0        0        0    17837 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/base.py
--rw-r--r--   0        0        0    10536 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async.py
--rw-r--r--   0        0        0     4054 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_multiproc.py
--rw-r--r--   0        0        0     3892 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_seq_for_multi.py
--rw-r--r--   0        0        0     2106 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_sequential.py
--rw-r--r--   0        0        0     8058 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_servers.py
--rw-r--r--   0        0        0      396 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_servers_threading.py
--rw-r--r--   0        0        0     2210 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_sequential.py
--rw-r--r--   0        0        0      393 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/meson.build
--rw-r--r--   0        0        0     7358 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/multi_exec_async.py
--rw-r--r--   0        0        0     3668 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/multi_exec_subproc.py
--rw-r--r--   0        0        0     7661 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/servers.py
--rw-r--r--   0        0        0      338 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/__init__.py
--rw-r--r--   0        0        0      769 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/base_matplotlib.py
--rw-r--r--   0        0        0     8981 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/imviewer.py
--rw-r--r--   0        0        0      228 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/Makefile
--rw-r--r--   0        0        0      153 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/__init__.py
--rw-r--r--   0        0        0     2659 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/main.py
--rw-r--r--   0        0        0     3750 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.py
--rw-r--r--   0        0        0     1671 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.ui
--rw-r--r--   0        0        0      170 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/meson.build
--rw-r--r--   0        0        0      568 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/test_launcher.py
--rw-r--r--   0        0        0      348 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/meson.build
--rw-r--r--   0        0        0    10703 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/monitor.py
--rw-r--r--   0        0        0       67 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/monitor.tcss
--rw-r--r--   0        0        0     2459 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/pg_main.py
--rw-r--r--   0        0        0     5903 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/pg_wrapper.py
--rw-r--r--   0        0        0     6018 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/piv_viewer.py
--rw-r--r--   0        0        0     1093 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_imviewer.py
--rw-r--r--   0        0        0      965 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_imviewer_pg.py
--rw-r--r--   0        0        0     2727 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_monitor.py
--rw-r--r--   0        0        0     1132 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_piv_viewer.py
--rw-r--r--   0        0        0     2612 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/image2image.py
--rw-r--r--   0        0        0      543 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/meson.build
--rw-r--r--   0        0        0      337 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/optical_flow.py
--rw-r--r--   0        0        0      278 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/piv.py
--rw-r--r--   0        0        0      104 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/__init__.py
--rw-r--r--   0        0        0      210 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/meson.build
--rw-r--r--   0        0        0     2412 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/piv.py
--rw-r--r--   0        0        0    14134 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/postproc.py
--rw-r--r--   0        0        0     2927 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/test_piv.py
--rw-r--r--   0        0        0     3771 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/test_util.py
--rw-r--r--   0        0        0     4070 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/util.py
--rw-r--r--   0        0        0    24145 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/vector_field.py
--rw-r--r--   0        0        0      580 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/preproc.py
--rw-r--r--   0        0        0      351 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/__init__.py
--rw-r--r--   0        0        0      131 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/meson.build
--rw-r--r--   0        0        0      230 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/__init__.py
--rw-r--r--   0        0        0      151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/meson.build
--rw-r--r--   0        0        0     7578 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/mlos.py
--rw-r--r--   0        0        0     1362 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/test_mlos.py
--rw-r--r--   0        0        0     2730 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/run_from_xml.py
--rw-r--r--   0        0        0     1605 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/synthetic.py
--rw-r--r--   0        0        0      521 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/test_image2image.py
--rw-r--r--   0        0        0     2259 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/test_run_from_xml.py
--rw-r--r--   0        0        0     2874 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/__init__.py
--rw-r--r--   0        0        0    17551 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/base.py
--rw-r--r--   0        0        0     6355 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/bos.py
--rw-r--r--   0        0        0     5706 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/example.py
--rw-r--r--   0        0        0     3999 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/image2image.py
--rw-r--r--   0        0        0     2497 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/launcher.py
--rw-r--r--   0        0        0    10341 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/log.py
--rw-r--r--   0        0        0      642 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/meson.build
--rw-r--r--   0        0        0     1422 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/nb_cpu_cores.py
--rw-r--r--   0        0        0     1020 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/optical_flow.py
--rw-r--r--   0        0        0     8851 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/piv.py
--rw-r--r--   0        0        0    10337 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/preproc.py
--rw-r--r--   0        0        0     8772 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/splitters.py
--rw-r--r--   0        0        0    10745 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/surface_tracking.py
--rw-r--r--   0        0        0     1347 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_bos.py
--rw-r--r--   0        0        0     1993 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_example.py
--rw-r--r--   0        0        0     1628 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_image2image.py
--rw-r--r--   0        0        0     1220 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_optical_flow.py
--rw-r--r--   0        0        0     2578 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_piv.py
--rw-r--r--   0        0        0     1773 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_preproc.py
--rw-r--r--   0        0        0     1919 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_splitters.py
--rw-r--r--   0        0        0     2251 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_surftracking.py
--rw-r--r--   0        0        0      741 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/__init__.py
--rw-r--r--   0        0        0     1318 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/log.py
--rw-r--r--   0        0        0      151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/meson.build
--rw-r--r--   0        0        0      398 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/test_util.py
--rw-r--r--   0        0        0     3154 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/util.py
--rw-r--r--   0        0        0     7306 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/uvmat.py
--rw-r--r--   0        0        0     6699 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/__init__.py
--rw-r--r--   0        0        0     2662 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/bos.py
--rw-r--r--   0        0        0     2687 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/image2image.py
--rw-r--r--   0        0        0      301 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/meson.build
--rw-r--r--   0        0        0     6651 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/optical_flow.py
--rw-r--r--   0        0        0      198 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/__init__.py
--rw-r--r--   0        0        0     7836 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/fix.py
--rw-r--r--   0        0        0      179 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/meson.build
--rw-r--r--   0        0        0     6418 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/multipass.py
--rw-r--r--   0        0        0    26467 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/singlepass.py
--rw-r--r--   0        0        0     2492 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/test_piv.py
--rw-r--r--   0        0        0     4587 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/__init__.py
--rw-r--r--   0        0        0     3844 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_cv.py
--rw-r--r--   0        0        0    14387 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_py.py
--rw-r--r--   0        0        0     2213 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/io.py
--rw-r--r--   0        0        0      184 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/meson.build
--rw-r--r--   0        0        0     3977 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/toolbox.py
--rw-r--r--   0        0        0    22183 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/surface_tracking.py
--rw-r--r--   0        0        0      776 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/test_bos.py
--rw-r--r--   0        0        0      542 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/test_image2image.py
--rw-r--r--   0        0        0     1815 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/test_preproc.py
--rw-r--r--   0        0        0     1307 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/with_mask.py
--rw-r--r--   0        0        0     4742 2024-05-06 09:04:16.440784 fluidimage-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.flake8
+-rw-r--r--   0        0        0     1166 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.github/workflows/ci-linux.yml
+-rw-r--r--   0        0        0      554 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.github/workflows/ci-pixi.yml
+-rw-r--r--   0        0        0     3919 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     3223 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1198 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.hgtags
+-rw-r--r--   0        0        0       43 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.mdformat.toml
+-rw-r--r--   0        0        0      376 2024-05-24 21:29:17.000000 fluidimage-0.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0      210 2024-05-24 21:29:17.000000 fluidimage-0.5.2/AUTHORS.md
+-rw-r--r--   0        0        0     8196 2024-05-24 21:29:17.000000 fluidimage-0.5.2/CHANGES.md
+-rw-r--r--   0        0        0     1266 2024-05-24 21:29:17.000000 fluidimage-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    21781 2024-05-24 21:29:17.000000 fluidimage-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0      205 2024-05-24 21:29:17.000000 fluidimage-0.5.2/MANIFEST.in
+-rw-r--r--   0        0        0      309 2024-05-24 21:29:17.000000 fluidimage-0.5.2/Makefile
+-rw-r--r--   0        0        0     3151 2024-05-24 21:29:17.000000 fluidimage-0.5.2/README.md
+-rw-r--r--   0        0        0     1266 2024-05-24 21:35:17.118528 fluidimage-0.5.2/doc/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5780 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/Makefile
+-rw-r--r--   0        0        0      210 2024-05-24 21:35:17.118528 fluidimage-0.5.2/doc/authors.md
+-rw-r--r--   0        0        0      748 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/autosum.rst
+-rw-r--r--   0        0        0     8443 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/build-from-source.md
+-rw-r--r--   0        0        0     8196 2024-05-24 21:35:17.118528 fluidimage-0.5.2/doc/changes.md
+-rw-r--r--   0        0        0      239 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/commands.md
+-rw-r--r--   0        0        0     9545 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/conf.py
+-rw-r--r--   0        0        0       36 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/Makefile
+-rw-r--r--   0        0        0      275 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/bos_parallel.md
+-rw-r--r--   0        0        0      708 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/bos_parallel.py
+-rw-r--r--   0        0        0      914 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/im2im_parallel.py
+-rw-r--r--   0        0        0      442 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/im2im_try_params.py
+-rw-r--r--   0        0        0      217 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/my_example_im2im.py
+-rw-r--r--   0        0        0      370 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/my_example_im2im_class.py
+-rw-r--r--   0        0        0      375 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/optflow_parallel.md
+-rw-r--r--   0        0        0      864 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/optflow_parallel.py
+-rw-r--r--   0        0        0      645 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/optflow_try_params.md
+-rw-r--r--   0        0        0      675 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/optflow_try_params.py
+-rw-r--r--   0        0        0     2124 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/__init__.py
+-rw-r--r--   0        0        0     1386 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/args.py
+-rwxr-xr-x   0        0        0      779 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/job_piv.py
+-rwxr-xr-x   0        0        0     1095 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/job_pre.py
+-rwxr-xr-x   0        0        0     2086 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/params_piv.py
+-rwxr-xr-x   0        0        0     1811 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/params_pre.py
+-rwxr-xr-x   0        0        0      672 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/submit_piv.py
+-rwxr-xr-x   0        0        0      787 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/submit_pre.py
+-rw-r--r--   0        0        0      896 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/test_piv_as_real.py
+-rwxr-xr-x   0        0        0      724 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/try_piv.py
+-rwxr-xr-x   0        0        0      538 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_as_real/try_pre.py
+-rw-r--r--   0        0        0      457 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_cluster.md
+-rw-r--r--   0        0        0      918 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_parallel.md
+-rw-r--r--   0        0        0      827 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_parallel.py
+-rw-r--r--   0        0        0      536 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_parallel_complete.py
+-rw-r--r--   0        0        0      953 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_parallel_im2im.py
+-rw-r--r--   0        0        0      989 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_parallel_im2im_class.py
+-rw-r--r--   0        0        0      863 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_try_params.md
+-rw-r--r--   0        0        0      614 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_try_params.py
+-rw-r--r--   0        0        0      747 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_try_params_Karman.py
+-rw-r--r--   0        0        0      814 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/piv_try_params_with_im2im_preproc.py
+-rw-r--r--   0        0        0      380 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/README.md
+-rw-r--r--   0        0        0      908 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/bench_piv_2005C.py
+-rw-r--r--   0        0        0     1419 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/download.py
+-rw-r--r--   0        0        0      744 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/path_images.py
+-rw-r--r--   0        0        0      437 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/piv_2001A_topology.py
+-rw-r--r--   0        0        0      496 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/piv_2001A_work.py
+-rw-r--r--   0        0        0      622 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/piv_2005C_topology.py
+-rw-r--r--   0        0        0      682 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/piv_2005C_work.py
+-rw-r--r--   0        0        0      137 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/possible_paths.txt
+-rw-r--r--   0        0        0      905 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/pivchallenge/profile_mean.py
+-rw-r--r--   0        0        0     1413 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/preproc.md
+-rw-r--r--   0        0        0     1061 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/preproc_parallel.py
+-rw-r--r--   0        0        0      816 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/preproc_sback1_filter.py
+-rw-r--r--   0        0        0     1037 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/preproc_sback2_rescale.py
+-rw-r--r--   0        0        0      544 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/preproc_try_params.py
+-rw-r--r--   0        0        0      364 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/preproc_try_params_opencv.py
+-rw-r--r--   0        0        0     1552 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/profile_piv_work.py
+-rw-r--r--   0        0        0      448 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/submit_job_legi.py
+-rw-r--r--   0        0        0      711 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/surface_tracking.py
+-rw-r--r--   0        0        0     1201 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples/test_run_examples.py
+-rw-r--r--   0        0        0      357 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/examples.md
+-rw-r--r--   0        0        0      238 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/for_dev.md
+-rw-r--r--   0        0        0      682 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/index.md
+-rw-r--r--   0        0        0     1686 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/install.md
+-rw-r--r--   0        0        0      405 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/ipynbslides/README.txt
+-rw-r--r--   0        0        0   493343 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/ipynbslides/fluidimage_legi_20170403.ipynb
+-rw-r--r--   0        0        0     2094 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/overview.md
+-rw-r--r--   0        0        0     1424 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/overview_orga_package.md
+-rw-r--r--   0        0        0     1857 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/related_codes.md
+-rw-r--r--   0        0        0       77 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/to_do.md
+-rw-r--r--   0        0        0      432 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorial.md
+-rw-r--r--   0        0        0     3116 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorials/tuto_calibration2dsimple.md
+-rw-r--r--   0        0        0     2412 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorials/tuto_direct_calibration.md
+-rw-r--r--   0        0        0     7352 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorials/tuto_opencv_calibration.md
+-rw-r--r--   0        0        0     4407 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorials/tuto_opencv_tomo_reconstruct.md
+-rw-r--r--   0        0        0     8785 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorials/tuto_piv.md
+-rw-r--r--   0        0        0     2950 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorials/tuto_stereo_reconstruction.md
+-rw-r--r--   0        0        0     1367 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/tutorials/tuto_tsai_calibration.md
+-rw-r--r--   0        0        0     8971 2024-05-24 21:29:17.000000 fluidimage-0.5.2/doc/uvmat.md
+-rw-r--r--   0        0        0     1252 2024-05-24 21:29:17.000000 fluidimage-0.5.2/docker/Dockerfile
+-rw-r--r--   0        0        0     1147 2024-05-24 21:29:17.000000 fluidimage-0.5.2/docker/Makefile
+-rw-r--r--   0        0        0      618 2024-05-24 21:29:17.000000 fluidimage-0.5.2/docker/hgrc
+-rw-r--r--   0        0        0       77 2024-05-24 21:29:17.000000 fluidimage-0.5.2/docker/pythranrc
+-rw-r--r--   0        0        0     1803 2024-05-24 21:29:17.000000 fluidimage-0.5.2/meson.build
+-rw-r--r--   0        0        0      655 2024-05-24 21:29:17.000000 fluidimage-0.5.2/meson.options
+-rw-r--r--   0        0        0     4888 2024-05-24 21:29:17.000000 fluidimage-0.5.2/noxfile.py
+-rw-r--r--   0        0        0   310844 2024-05-24 21:29:17.000000 fluidimage-0.5.2/pdm.lock
+-rw-r--r--   0        0        0   782153 2024-05-24 21:29:17.000000 fluidimage-0.5.2/pixi.lock
+-rw-r--r--   0        0        0     1009 2024-05-24 21:29:17.000000 fluidimage-0.5.2/pixi.toml
+-rw-r--r--   0        0        0    21630 2024-05-24 21:29:17.000000 fluidimage-0.5.2/pylintrc
+-rw-r--r--   0        0        0     4729 2024-05-24 21:29:17.000000 fluidimage-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3311 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/_opencv.py
+-rw-r--r--   0        0        0      162 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/_version.py
+-rw-r--r--   0        0        0      278 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/bos.py
+-rw-r--r--   0        0        0      263 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/__init__.py
+-rw-r--r--   0        0        0     2858 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/_evaluate_subpix.py
+-rw-r--r--   0        0        0      878 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/correl.cu
+-rw-r--r--   0        0        0    21039 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/correl.py
+-rw-r--r--   0        0        0    10794 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/correl_pycuda.py
+-rw-r--r--   0        0        0      333 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/errors.py
+-rw-r--r--   0        0        0     7467 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/fft.py
+-rw-r--r--   0        0        0      132 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/interpolate/__init__.py
+-rw-r--r--   0        0        0      613 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/interpolate/griddata.py
+-rw-r--r--   0        0        0      388 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/interpolate/meson.build
+-rw-r--r--   0        0        0      867 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py
+-rw-r--r--   0        0        0     8006 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/interpolate/thin_plate_spline.py
+-rw-r--r--   0        0        0    10312 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py
+-rw-r--r--   0        0        0     4807 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/mean_neighbors.py
+-rw-r--r--   0        0        0      489 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/meson.build
+-rw-r--r--   0        0        0    39595 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    37615 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    36317 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    35832 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    37828 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    38146 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    36451 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    34562 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0     1188 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/reduction_kernel.cu
+-rw-r--r--   0        0        0     6180 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/subpix.py
+-rw-r--r--   0        0        0     6419 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/test_correl.py
+-rw-r--r--   0        0        0     2519 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calcul/test_fft.py
+-rw-r--r--   0        0        0      465 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/__init__.py
+-rw-r--r--   0        0        0     3587 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/calib2d_simple.py
+-rw-r--r--   0        0        0     9318 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/calib_cv.py
+-rw-r--r--   0        0        0    23798 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/calib_direct.py
+-rw-r--r--   0        0        0     7528 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/calib_tsai.py
+-rw-r--r--   0        0        0      302 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/meson.build
+-rw-r--r--   0        0        0     2033 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/test_calib_cv.py
+-rw-r--r--   0        0        0     2609 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/test_direct_stereo_reconstruction.py
+-rw-r--r--   0        0        0     1302 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/test_tsai_calibration.py
+-rw-r--r--   0        0        0     4272 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/calibration/util.py
+-rw-r--r--   0        0        0      739 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/config.py
+-rw-r--r--   0        0        0     1434 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/conftest.py
+-rw-r--r--   0        0        0      274 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/__init__.py
+-rw-r--r--   0        0        0    13511 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/display_piv.py
+-rw-r--r--   0        0        0     4822 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/display_pre.py
+-rw-r--r--   0        0        0      214 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/meson.build
+-rw-r--r--   0        0        0    27168 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/piv.py
+-rw-r--r--   0        0        0     4457 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/preproc.py
+-rw-r--r--   0        0        0      425 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/test_piv.py
+-rw-r--r--   0        0        0     9009 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/data_objects/tomo.py
+-rw-r--r--   0        0        0     3530 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/__init__.py
+-rw-r--r--   0        0        0    19680 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/base.py
+-rw-r--r--   0        0        0    10684 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_async.py
+-rw-r--r--   0        0        0     4054 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_async_multiproc.py
+-rw-r--r--   0        0        0     2816 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_async_seq_for_multi.py
+-rw-r--r--   0        0        0     2106 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_async_sequential.py
+-rw-r--r--   0        0        0     8015 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_async_servers.py
+-rw-r--r--   0        0        0      396 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_async_servers_threading.py
+-rw-r--r--   0        0        0      436 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_seq_for_multi.py
+-rw-r--r--   0        0        0     2762 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/exec_sequential.py
+-rw-r--r--   0        0        0      476 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/meson.build
+-rw-r--r--   0        0        0     7002 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/multi_exec_async.py
+-rw-r--r--   0        0        0     3716 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/multi_exec_subproc.py
+-rw-r--r--   0        0        0      359 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/multi_exec_subproc_sync.py
+-rw-r--r--   0        0        0      383 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/multi_exec_sync.py
+-rw-r--r--   0        0        0     7858 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/executors/servers.py
+-rw-r--r--   0        0        0      338 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/base_matplotlib.py
+-rw-r--r--   0        0        0     8981 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/imviewer.py
+-rw-r--r--   0        0        0      228 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/launcher/Makefile
+-rw-r--r--   0        0        0      153 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/launcher/__init__.py
+-rw-r--r--   0        0        0     2659 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/launcher/main.py
+-rw-r--r--   0        0        0     3750 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/launcher/mainwindow.py
+-rw-r--r--   0        0        0     1671 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/launcher/mainwindow.ui
+-rw-r--r--   0        0        0      170 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/launcher/meson.build
+-rw-r--r--   0        0        0      568 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/launcher/test_launcher.py
+-rw-r--r--   0        0        0      348 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/meson.build
+-rw-r--r--   0        0        0    10702 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/monitor.py
+-rw-r--r--   0        0        0       67 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/monitor.tcss
+-rw-r--r--   0        0        0     2459 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/pg_main.py
+-rw-r--r--   0        0        0     5903 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/pg_wrapper.py
+-rw-r--r--   0        0        0     6018 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/piv_viewer.py
+-rw-r--r--   0        0        0     1093 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/test_imviewer.py
+-rw-r--r--   0        0        0      965 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/test_imviewer_pg.py
+-rw-r--r--   0        0        0     2727 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/test_monitor.py
+-rw-r--r--   0        0        0     1132 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/gui/test_piv_viewer.py
+-rw-r--r--   0        0        0     2612 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/image2image.py
+-rw-r--r--   0        0        0      543 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/meson.build
+-rw-r--r--   0        0        0      337 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/optical_flow.py
+-rw-r--r--   0        0        0      278 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/piv.py
+-rw-r--r--   0        0        0      104 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/__init__.py
+-rw-r--r--   0        0        0      210 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/meson.build
+-rw-r--r--   0        0        0     2412 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/piv.py
+-rw-r--r--   0        0        0    14134 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/postproc.py
+-rw-r--r--   0        0        0     2927 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/test_piv.py
+-rw-r--r--   0        0        0     3771 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/test_util.py
+-rw-r--r--   0        0        0     4070 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/util.py
+-rw-r--r--   0        0        0    24145 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/postproc/vector_field.py
+-rw-r--r--   0        0        0      580 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/preproc.py
+-rw-r--r--   0        0        0      351 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/reconstruct/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/reconstruct/meson.build
+-rw-r--r--   0        0        0      230 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/reconstruct/tomo/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/reconstruct/tomo/meson.build
+-rw-r--r--   0        0        0     7578 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/reconstruct/tomo/mlos.py
+-rw-r--r--   0        0        0     1362 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/reconstruct/tomo/test_mlos.py
+-rw-r--r--   0        0        0     2730 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/run_from_xml.py
+-rw-r--r--   0        0        0     1605 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/synthetic.py
+-rw-r--r--   0        0        0      521 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/test_image2image.py
+-rw-r--r--   0        0        0     2264 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/test_run_from_xml.py
+-rw-r--r--   0        0        0     1060 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/__init__.py
+-rw-r--r--   0        0        0    20150 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/base.py
+-rw-r--r--   0        0        0     5997 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/bos.py
+-rw-r--r--   0        0        0     5689 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/example.py
+-rw-r--r--   0        0        0     3648 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/image2image.py
+-rw-r--r--   0        0        0     2497 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/launcher.py
+-rw-r--r--   0        0        0    10341 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/log.py
+-rw-r--r--   0        0        0     7829 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/mean.py
+-rw-r--r--   0        0        0      673 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/meson.build
+-rw-r--r--   0        0        0     1422 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/nb_cpu_cores.py
+-rw-r--r--   0        0        0     1020 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/optical_flow.py
+-rw-r--r--   0        0        0     8653 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/piv.py
+-rw-r--r--   0        0        0    10035 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/preproc.py
+-rw-r--r--   0        0        0     8772 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/splitters.py
+-rw-r--r--   0        0        0    10456 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/surface_tracking.py
+-rw-r--r--   0        0        0     1347 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_bos.py
+-rw-r--r--   0        0        0     2281 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_example.py
+-rw-r--r--   0        0        0     1628 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_image2image.py
+-rw-r--r--   0        0        0     1996 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_mean.py
+-rw-r--r--   0        0        0     1220 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_optical_flow.py
+-rw-r--r--   0        0        0     2578 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_piv.py
+-rw-r--r--   0        0        0     1773 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_preproc.py
+-rw-r--r--   0        0        0     1919 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_splitters.py
+-rw-r--r--   0        0        0     2251 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/topologies/test_surftracking.py
+-rw-r--r--   0        0        0      741 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/util/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/util/log.py
+-rw-r--r--   0        0        0      151 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/util/meson.build
+-rw-r--r--   0        0        0      398 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/util/test_util.py
+-rw-r--r--   0        0        0     3154 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/util/util.py
+-rw-r--r--   0        0        0     7306 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/uvmat.py
+-rw-r--r--   0        0        0     6699 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/__init__.py
+-rw-r--r--   0        0        0     2662 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/bos.py
+-rw-r--r--   0        0        0     2687 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/image2image.py
+-rw-r--r--   0        0        0      301 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/meson.build
+-rw-r--r--   0        0        0     6651 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/optical_flow.py
+-rw-r--r--   0        0        0      198 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/piv/__init__.py
+-rw-r--r--   0        0        0     7836 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/piv/fix.py
+-rw-r--r--   0        0        0      179 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/piv/meson.build
+-rw-r--r--   0        0        0     6418 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/piv/multipass.py
+-rw-r--r--   0        0        0    26467 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/piv/singlepass.py
+-rw-r--r--   0        0        0     2492 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/piv/test_piv.py
+-rw-r--r--   0        0        0     4587 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/preproc/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/preproc/_toolbox_cv.py
+-rw-r--r--   0        0        0    14387 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/preproc/_toolbox_py.py
+-rw-r--r--   0        0        0     2213 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/preproc/io.py
+-rw-r--r--   0        0        0      184 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/preproc/meson.build
+-rw-r--r--   0        0        0     3977 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/preproc/toolbox.py
+-rw-r--r--   0        0        0    22183 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/surface_tracking.py
+-rw-r--r--   0        0        0      776 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/test_bos.py
+-rw-r--r--   0        0        0      542 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/test_image2image.py
+-rw-r--r--   0        0        0     1815 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/test_preproc.py
+-rw-r--r--   0        0        0     1307 2024-05-24 21:29:17.000000 fluidimage-0.5.2/src/fluidimage/works/with_mask.py
+-rw-r--r--   0        0        0     4742 2024-05-24 21:35:17.609399 fluidimage-0.5.2/PKG-INFO
```

### Comparing `fluidimage-0.5.1/.github/workflows/ci-linux.yml` & `fluidimage-0.5.2/.github/workflows/ci-linux.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/.github/workflows/ci-pixi.yml` & `fluidimage-0.5.2/.github/workflows/ci-pixi.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/.github/workflows/wheels.yml` & `fluidimage-0.5.2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/.gitlab-ci.yml` & `fluidimage-0.5.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/.hgtags` & `fluidimage-0.5.2/.hgtags`

 * *Files 14% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 bb6f0ccc21452f0e1aa5caa5e058c8a163556c0d 0.4.2
 d1026b6b03c5e9ef8d0f23b60158684ed3d9e936 0.4.3
 f615cec0efdc3377cb9c7dfa96926fc2100d8c02 0.4.3.post0
 e66f70954560bbccdde36c76eac0a12f82ada45d 0.4.4
 80b7c7a51553b4ff08206a336e3e5d4795ffe306 0.4.5
 15eedfa330603df0403c6d8d6fc49ec468536e9b 0.4.6
 2c46b012bb330adfdac0d3c636af579e6b22426f 0.5.0
+56d3b6c261b4b41bbf5bc0d2f10e76733ab3859e 0.5.1
```

### Comparing `fluidimage-0.5.1/CHANGES.md` & `fluidimage-0.5.2/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Release notes
 
 See also the
-[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.1...branch%2Fdefault).
+[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.2...branch%2Fdefault).
+
+## [0.5.2] (2024-05-24)
+
+- New command `fluidimage-mean` to compute mean of images with the new topology
+  {class}`fluidimage.topologies.mean.TopologyMeanImage`.
+
+- New executors `multi_exec_sync` ({mod}`fluidimage.executors.multi_exec_sync`) and
+  `multi_exec_subproc_sync` ({mod}`fluidimage.executors.multi_exec_subproc_sync`).
+
+- [!108](https://foss.heptapod.net/fluiddyn/fluidimage/-/merge_requests/108): save UVmat
+  error codes in PIV files.
 
 ## [0.5.1] (2024-05-06)
 
 - Follow UVmat: change defaults and exact meaning for parameter
   `params.multipass.smoothing_coef` (=2).
 
 ## [0.5.0] (2024-05-02)
@@ -213,7 +224,8 @@
 [0.4.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.1...0.4.2
 [0.4.3]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.2...0.4.3
 [0.4.4]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.3...0.4.4
 [0.4.5]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.4...0.4.5
 [0.4.6]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...0.4.6
 [0.5.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.6...0.5.0
 [0.5.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...0.5.1
+[0.5.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.1...0.5.2
```

### Comparing `fluidimage-0.5.1/CONTRIBUTING.md` & `fluidimage-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/LICENSE.txt` & `fluidimage-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/README.md` & `fluidimage-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/CONTRIBUTING.md` & `fluidimage-0.5.2/doc/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/Makefile` & `fluidimage-0.5.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/autosum.rst` & `fluidimage-0.5.2/doc/autosum.rst`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/build-from-source.md` & `fluidimage-0.5.2/doc/build-from-source.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/changes.md` & `fluidimage-0.5.2/doc/changes.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Release notes
 
 See also the
-[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.1...branch%2Fdefault).
+[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.2...branch%2Fdefault).
+
+## [0.5.2] (2024-05-24)
+
+- New command `fluidimage-mean` to compute mean of images with the new topology
+  {class}`fluidimage.topologies.mean.TopologyMeanImage`.
+
+- New executors `multi_exec_sync` ({mod}`fluidimage.executors.multi_exec_sync`) and
+  `multi_exec_subproc_sync` ({mod}`fluidimage.executors.multi_exec_subproc_sync`).
+
+- [!108](https://foss.heptapod.net/fluiddyn/fluidimage/-/merge_requests/108): save UVmat
+  error codes in PIV files.
 
 ## [0.5.1] (2024-05-06)
 
 - Follow UVmat: change defaults and exact meaning for parameter
   `params.multipass.smoothing_coef` (=2).
 
 ## [0.5.0] (2024-05-02)
@@ -213,7 +224,8 @@
 [0.4.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.1...0.4.2
 [0.4.3]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.2...0.4.3
 [0.4.4]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.3...0.4.4
 [0.4.5]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.4...0.4.5
 [0.4.6]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...0.4.6
 [0.5.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.6...0.5.0
 [0.5.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...0.5.1
+[0.5.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.1...0.5.2
```

### Comparing `fluidimage-0.5.1/doc/conf.py` & `fluidimage-0.5.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/bos_parallel.py` & `fluidimage-0.5.2/doc/examples/bos_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/im2im_parallel.py` & `fluidimage-0.5.2/doc/examples/im2im_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/optflow_parallel.py` & `fluidimage-0.5.2/doc/examples/optflow_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/optflow_try_params.md` & `fluidimage-0.5.2/doc/examples/optflow_try_params.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/optflow_try_params.py` & `fluidimage-0.5.2/doc/examples/optflow_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/README.md` & `fluidimage-0.5.2/doc/examples/piv_as_real/README.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/args.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/args.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/job_piv.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/job_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/job_pre.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/job_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/params_piv.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/params_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/params_pre.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/params_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/submit_piv.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/submit_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/submit_pre.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/submit_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/test_piv_as_real.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/test_piv_as_real.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/try_piv.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/try_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_as_real/try_pre.py` & `fluidimage-0.5.2/doc/examples/piv_as_real/try_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_parallel.md` & `fluidimage-0.5.2/doc/examples/piv_parallel.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_parallel.py` & `fluidimage-0.5.2/doc/examples/piv_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_parallel_complete.py` & `fluidimage-0.5.2/doc/examples/piv_parallel_complete.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_parallel_im2im.py` & `fluidimage-0.5.2/doc/examples/piv_parallel_im2im.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_parallel_im2im_class.py` & `fluidimage-0.5.2/doc/examples/piv_parallel_im2im_class.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_try_params.md` & `fluidimage-0.5.2/doc/examples/piv_try_params.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_try_params.py` & `fluidimage-0.5.2/doc/examples/piv_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_try_params_Karman.py` & `fluidimage-0.5.2/doc/examples/piv_try_params_Karman.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/piv_try_params_with_im2im_preproc.py` & `fluidimage-0.5.2/doc/examples/piv_try_params_with_im2im_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/pivchallenge/bench_piv_2005C.py` & `fluidimage-0.5.2/doc/examples/pivchallenge/bench_piv_2005C.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/pivchallenge/download.py` & `fluidimage-0.5.2/doc/examples/pivchallenge/download.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/pivchallenge/path_images.py` & `fluidimage-0.5.2/doc/examples/pivchallenge/path_images.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_topology.py` & `fluidimage-0.5.2/doc/examples/pivchallenge/piv_2005C_topology.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_work.py` & `fluidimage-0.5.2/doc/examples/pivchallenge/piv_2005C_work.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/preproc.md` & `fluidimage-0.5.2/doc/examples/preproc.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/preproc_parallel.py` & `fluidimage-0.5.2/doc/examples/preproc_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/preproc_sback1_filter.py` & `fluidimage-0.5.2/doc/examples/preproc_sback1_filter.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/preproc_sback2_rescale.py` & `fluidimage-0.5.2/doc/examples/preproc_sback2_rescale.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/preproc_try_params.py` & `fluidimage-0.5.2/doc/examples/preproc_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/profile_piv_work.py` & `fluidimage-0.5.2/doc/examples/profile_piv_work.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/surface_tracking.py` & `fluidimage-0.5.2/doc/examples/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/examples/test_run_examples.py` & `fluidimage-0.5.2/doc/examples/test_run_examples.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/index.md` & `fluidimage-0.5.2/doc/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 caption: User guide
 maxdepth: 1
 ---
 overview
 install
 tutorial
 examples
+commands
 build-from-source
 ```
 
 ```{toctree}
 ---
 caption: Python API
 maxdepth: 1
```

### Comparing `fluidimage-0.5.1/doc/install.md` & `fluidimage-0.5.2/doc/install.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/ipynbslides/fluidimage_legi_20170403.ipynb` & `fluidimage-0.5.2/doc/ipynbslides/fluidimage_legi_20170403.ipynb`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/overview.md` & `fluidimage-0.5.2/doc/overview.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/overview_orga_package.md` & `fluidimage-0.5.2/doc/overview_orga_package.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/related_codes.md` & `fluidimage-0.5.2/doc/related_codes.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/tutorials/tuto_calibration2dsimple.md` & `fluidimage-0.5.2/doc/tutorials/tuto_calibration2dsimple.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/tutorials/tuto_direct_calibration.md` & `fluidimage-0.5.2/doc/tutorials/tuto_direct_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/tutorials/tuto_opencv_calibration.md` & `fluidimage-0.5.2/doc/tutorials/tuto_opencv_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/tutorials/tuto_opencv_tomo_reconstruct.md` & `fluidimage-0.5.2/doc/tutorials/tuto_opencv_tomo_reconstruct.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/tutorials/tuto_piv.md` & `fluidimage-0.5.2/doc/tutorials/tuto_piv.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/tutorials/tuto_stereo_reconstruction.md` & `fluidimage-0.5.2/doc/tutorials/tuto_stereo_reconstruction.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/tutorials/tuto_tsai_calibration.md` & `fluidimage-0.5.2/doc/tutorials/tuto_tsai_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/doc/uvmat.md` & `fluidimage-0.5.2/doc/uvmat.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/docker/Dockerfile` & `fluidimage-0.5.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/docker/Makefile` & `fluidimage-0.5.2/docker/Makefile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/docker/hgrc` & `fluidimage-0.5.2/docker/hgrc`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/meson.build` & `fluidimage-0.5.2/meson.build`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/meson.options` & `fluidimage-0.5.2/meson.options`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/noxfile.py` & `fluidimage-0.5.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/pdm.lock` & `fluidimage-0.5.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/pixi.lock` & `fluidimage-0.5.2/pixi.lock`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/pixi.toml` & `fluidimage-0.5.2/pixi.toml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/pylintrc` & `fluidimage-0.5.2/pylintrc`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/pyproject.toml` & `fluidimage-0.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "transonic>=0.6.2",
     "pythran>=0.9.7",
 ]
 build-backend = 'mesonpy'
 
 [project]
 name = "fluidimage"
-version = "0.5.1"
+version = "0.5.2"
 description = "Fluid image processing with Python."
 authors = [
     {name = "Pierre Augier", email = "pierre.augier@legi.cnrs.fr"},
 ]
 dependencies = [
     "numpy >= 1.8",
     "matplotlib >= 3.5",
@@ -54,30 +54,34 @@
 
 [project.scripts]
 fluidimlauncher = "fluidimage.gui.launcher.main:main"
 fluidimage-monitor = "fluidimage.gui.monitor:main"
 fluidimviewer = "fluidimage.gui.imviewer:main"
 fluidimviewer-pg = "fluidimage.gui.pg_main:main"
 fluidpivviewer = "fluidimage.gui.piv_viewer:main"
+fluidimage-mean = "fluidimage.topologies.mean:main"
 
 [project.optional-dependencies]
 pims = ["pims"]
 opencv = ["opencv-python"]
 graph = ["gprof2dot"]
 pytest = ["pytest", "pytest-asyncio"]
 all = ["fluidimage[pims, opencv, graph, pytest]"]
 # qt = ["PySide6"]
 
 [project.entry-points."fluidimage.executors"]
 exec_sequential = "fluidimage.executors.exec_sequential"
 exec_async = "fluidimage.executors.exec_async"
 exec_async_sequential =  "fluidimage.executors.exec_async_sequential"
 exec_async_seq_for_multi = "fluidimage.executors.exec_async_seq_for_multi"
+exec_seq_for_multi = "fluidimage.executors.exec_seq_for_multi"
 multi_exec_async =  "fluidimage.executors.multi_exec_async"
+multi_exec_sync =  "fluidimage.executors.multi_exec_sync"
 multi_exec_subproc = "fluidimage.executors.multi_exec_subproc"
+multi_exec_subproc_sync = "fluidimage.executors.multi_exec_subproc_sync"
 exec_async_multi =  "fluidimage.executors.exec_async_multiproc"
 exec_async_servers =  "fluidimage.executors.exec_async_servers"
 exec_async_servers_threading =  "fluidimage.executors.exec_async_servers_threading"
 
 
 [tool.pdm]
 distribution = true
```

### Comparing `fluidimage-0.5.1/src/fluidimage/__init__.py` & `fluidimage-0.5.2/src/fluidimage/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/_opencv.py` & `fluidimage-0.5.2/src/fluidimage/_opencv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/_evaluate_subpix.py` & `fluidimage-0.5.2/src/fluidimage/calcul/_evaluate_subpix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/correl.cu` & `fluidimage-0.5.2/src/fluidimage/calcul/correl.cu`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/correl.py` & `fluidimage-0.5.2/src/fluidimage/calcul/correl.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/correl_pycuda.py` & `fluidimage-0.5.2/src/fluidimage/calcul/correl_pycuda.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/fft.py` & `fluidimage-0.5.2/src/fluidimage/calcul/fft.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/griddata.py` & `fluidimage-0.5.2/src/fluidimage/calcul/interpolate/griddata.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py` & `fluidimage-0.5.2/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline.py` & `fluidimage-0.5.2/src/fluidimage/calcul/interpolate/thin_plate_spline.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py` & `fluidimage-0.5.2/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/mean_neighbors.py` & `fluidimage-0.5.2/src/fluidimage/calcul/mean_neighbors.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png` & `fluidimage-0.5.2/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/reduction_kernel.cu` & `fluidimage-0.5.2/src/fluidimage/calcul/reduction_kernel.cu`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/subpix.py` & `fluidimage-0.5.2/src/fluidimage/calcul/subpix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/test_correl.py` & `fluidimage-0.5.2/src/fluidimage/calcul/test_correl.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,17 +60,17 @@
         nb_particles = (nx // 4) ** 2
 
         cls.im0, cls.im1 = make_synthetic_images(
             cls.displacements, nb_particles, shape_im0=(ny, nx), epsilon=0.0
         )
 
 
-for k, cls in classes.items():
+for method, cls in classes.items():
 
-    def _test(self, cls=cls, k=k):
+    def _test(self, cls=cls, name=method):
         if issubclass(cls, CorrelFFTBase):
             displacement_max = "50%"
         else:
             displacement_max = None
 
         correl = cls(
             self.im0.shape, self.im1.shape, displacement_max=displacement_max
@@ -82,40 +82,37 @@
             dx,
             dy,
             correl_max,
             other_peaks,
         ) = correl.compute_displacements_from_correl(c, norm=norm)
         displacement_computed = np.array([dx, dy])
 
-        print(f"{k}, displacement = [0, 0]\t error= {abs(displacement_computed)}")
+        print(f"{name}, displacement = [0, 0]\t{abs(displacement_computed) = }")
 
         assert np.allclose([0, 0], displacement_computed, atol=1e-03)
         assert np.allclose(correl_max, 1.0), correl_max
 
         # then, with the 2 figures with displacements
         c, norm = correl(self.im0, self.im1)
         dx, dy, correl_max, _ = correl.compute_displacements_from_correl(
             c, norm=norm
         )
 
         displacement_computed = np.array([dx, dy])
 
-        logger.debug(
-            k
-            + ", displacement = {}\t error= {}\n".format(
-                self.displacements,
-                abs(displacement_computed - self.displacements),
-            )
+        print(
+            f"{name}, displacement = {self.displacements}\t"
+            f"error = {abs(displacement_computed - self.displacements)}"
         )
 
         self.assertTrue(
             np.allclose(self.displacements, displacement_computed, atol=0.8)
         )
 
-    exec("TestCorrel.test_correl_square_image_" + k + " = _test")
+    exec("TestCorrel.test_correl_square_image_" + method + " = _test")
 
 
 class TestCorrel1(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         nx = 32
         ny = 64
@@ -132,28 +129,28 @@
         nb_particles = (max(nx, ny) // 4) ** 2
 
         cls.im0, cls.im1 = make_synthetic_images(
             cls.displacements, nb_particles, shape_im0=(ny, nx), epsilon=0.0
         )
 
 
-for k, cls in classes.items():
+for method, cls in classes.items():
 
-    def _test1(self, cls=cls, k=k):
+    def _test1(self, cls=cls, name=method):
         correl = cls(self.im0.shape, self.im1.shape)
 
         # first, no displacement
         c, norm = correl(self.im0, self.im0)
         dx, dy, correl_max, _ = correl.compute_displacements_from_correl(
             c, norm=norm
         )
         displacement_computed = np.array([dx, dy])
 
         logger.debug(
-            k
+            name
             + ", displacement = [0, 0]\t error= {}\n".format(
                 abs(displacement_computed)
             )
         )
 
         assert np.allclose(correl_max, 1.0), correl_max
         assert np.allclose([0, 0], displacement_computed, atol=1e-03)
@@ -162,27 +159,24 @@
         c, norm = correl(self.im0, self.im1)
         dx, dy, correl_max, _ = correl.compute_displacements_from_correl(
             c, norm=norm
         )
 
         displacement_computed = np.array([dx, dy])
 
-        logger.debug(
-            k
-            + ", displacement = {}\t error= {}\n".format(
-                self.displacements,
-                abs(displacement_computed - self.displacements),
-            )
+        print(
+            f"{name}, displacement = {self.displacements}\t"
+            f"error = {abs(displacement_computed - self.displacements)}"
         )
 
         self.assertTrue(
             np.allclose(self.displacements, displacement_computed, atol=0.8)
         )
 
-    exec("TestCorrel1.test_correl_rectangular_image_" + k + " = _test1")
+    exec("TestCorrel1.test_correl_rectangular_image_" + method + " = _test1")
 
 
 class TestCorrel2(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         nx0 = 48
         ny0 = 96
@@ -207,40 +201,37 @@
             shape_im1=(ny1, nx1),
             epsilon=0.0,
         )
 
         cls.im1 = cls.im1.astype("float32")
 
 
-for k, cls in classes_real_space.items():
+for method, cls in classes_real_space.items():
 
-    def _test2(self, cls=cls, k=k):
+    def _test2(self, cls=cls, name=method):
         correl = cls(self.im0.shape, self.im1.shape, mode="valid")
 
         # with the 2 figures with displacements
         c, norm = correl(self.im0, self.im1)
         dx, dy, correl_max, _ = correl.compute_displacements_from_correl(
             c, norm=norm
         )
 
         displacement_computed = np.array([dx, dy])
 
-        logger.debug(
-            k
-            + ", displacement = {}\t error= {}\n".format(
-                self.displacements,
-                abs(displacement_computed - self.displacements),
-            )
+        print(
+            f"{name}, displacement = {self.displacements}\t"
+            f"error = {abs(displacement_computed - self.displacements)}"
         )
 
         self.assertTrue(
             np.allclose(self.displacements, displacement_computed, atol=0.8)
         )
 
-    exec("TestCorrel2.test_correl_images_diff_sizes_" + k + " = _test2")
+    exec("TestCorrel2.test_correl_images_diff_sizes_" + method + " = _test2")
 
 
 def _test_like_fftshift(n0, n1):
     correl = np.reshape(np.arange(n0 * n1, dtype=np.float32), (n0, n1))
     assert np.allclose(
         _like_fftshift(correl),
         np.ascontiguousarray(np.fft.fftshift(correl[::-1, ::-1])),
```

### Comparing `fluidimage-0.5.1/src/fluidimage/calcul/test_fft.py` & `fluidimage-0.5.2/src/fluidimage/calcul/test_fft.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/calib2d_simple.py` & `fluidimage-0.5.2/src/fluidimage/calibration/calib2d_simple.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/calib_cv.py` & `fluidimage-0.5.2/src/fluidimage/calibration/calib_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/calib_direct.py` & `fluidimage-0.5.2/src/fluidimage/calibration/calib_direct.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/calib_tsai.py` & `fluidimage-0.5.2/src/fluidimage/calibration/calib_tsai.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/test_calib_cv.py` & `fluidimage-0.5.2/src/fluidimage/calibration/test_calib_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/test_direct_stereo_reconstruction.py` & `fluidimage-0.5.2/src/fluidimage/calibration/test_direct_stereo_reconstruction.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/test_tsai_calibration.py` & `fluidimage-0.5.2/src/fluidimage/calibration/test_tsai_calibration.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/calibration/util.py` & `fluidimage-0.5.2/src/fluidimage/calibration/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/config.py` & `fluidimage-0.5.2/src/fluidimage/config.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/conftest.py` & `fluidimage-0.5.2/src/fluidimage/conftest.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/data_objects/display_piv.py` & `fluidimage-0.5.2/src/fluidimage/data_objects/display_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/data_objects/display_pre.py` & `fluidimage-0.5.2/src/fluidimage/data_objects/display_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/data_objects/piv.py` & `fluidimage-0.5.2/src/fluidimage/data_objects/piv.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,14 +422,31 @@
                         values[i] = k.encode()
                 except AttributeError:
                     pass
 
                 g.create_dataset("keys", data=keys)
                 g.create_dataset("values", data=values)
 
+                if name_dict == "errors":
+                    error_codes = np.empty(len(values), dtype=np.uint8)
+                    code_unknow = np.iinfo(error_codes.dtype).max
+                    for idx, error in enumerate(values):
+                        if error.startswith(b"Correlation peak touching"):
+                            code = 1
+                        elif error.startswith(b"correl < correl_min"):
+                            code = 2
+                        elif error.startswith(b"delta2 < displacement_max2"):
+                            code = 3
+                        elif error.startswith(b"diff neighbour too large"):
+                            code = 4
+                        else:
+                            code = code_unknow
+                        error_codes[idx] = code
+                    g.create_dataset("codes", data=error_codes)
+
         if "deltaxs_tps" in self.__dict__:
             g = g_piv.create_group("deltaxs_tps")
             for i, arr in enumerate(self.deltaxs_tps):
                 g.create_dataset(f"subdom{i}", data=arr)
 
             g = g_piv.create_group("deltays_tps")
             for i, arr in enumerate(self.deltays_tps):
```

### Comparing `fluidimage-0.5.1/src/fluidimage/data_objects/preproc.py` & `fluidimage-0.5.2/src/fluidimage/data_objects/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/data_objects/tomo.py` & `fluidimage-0.5.2/src/fluidimage/data_objects/tomo.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/__init__.py` & `fluidimage-0.5.2/src/fluidimage/executors/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,19 @@
    :toctree:
 
    base
    exec_sequential
    exec_async
    exec_async_sequential
    multi_exec_async
+   multi_exec_sync
    multi_exec_subproc
+   multi_exec_subproc_sync
    exec_async_seq_for_multi
+   exec_seq_for_multi
    exec_async_multiproc
    exec_async_servers
    servers
 
 .. autofunction:: get_entry_points
 
 .. autofunction:: get_executor_names
@@ -54,16 +57,17 @@
 
 from .base import ExecutorBase
 
 # on Windows (and MacOS), one cannot use "multi_exec_async"
 # because the OS does not support forks (or not fully) and
 # multiprocessing works differently than on Linux
 # see https://docs.python.org/3/library/multiprocessing.html#contexts-and-start-methods
-supported_multi_executors = ["multi_exec_subproc"]
+supported_multi_executors = ["multi_exec_subproc", "multi_exec_subproc_sync"]
 if sys.platform == "linux":
+    supported_multi_executors.insert(0, "multi_exec_sync")
     supported_multi_executors.insert(0, "multi_exec_async")
 
 
 _entry_points = None
 
 
 def get_entry_points(reload=False):
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/base.py` & `fluidimage-0.5.2/src/fluidimage/executors/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,20 @@
     """
 
     info_job: dict
     path_job_data: Path
     _path_lockfile: Path
     num_expected_results: int
     time_start: str
+    _final_seq_work_run: bool
+
+    # for results log
+    _path_results: Path
+    _path_num_results: Path
+    _len_saved_results: int
 
     def _init_log_path(self):
         self.time_start_str = time_as_str()
         unique_postfix = f"{self.time_start_str}_{os.getpid()}"
         path_job_data = self.path_dir_result / f"job_{unique_postfix}"
 
         if path_job_data.exists():
@@ -198,14 +204,15 @@
         # to avoid a pylint warning
         self.t_start = None
 
     def _get_file_object_for_logger(self):
         return sys.stdout
 
     def _init_compute(self):
+        self._final_seq_work_run = False
         self.t_start = time()
         self._init_num_expected_results()
         if self.num_expected_results == 0:
             return
         self._init_compute_log()
         self._save_job_data()
 
@@ -214,15 +221,15 @@
 
         topology_name = str_short(type(self.topology))
         executor_name = str_short(type(self))
         print("  topology:", topology_name)
         print("  executor:", executor_name)
         print("  nb_cpus_allowed =", nb_cores)
         print("  nb_max_workers =", self.nb_max_workers)
-        print("  num_expected_results", self.num_expected_results)
+        print("  num_expected_results =", self.num_expected_results)
         print("  path_dir_result =", self.path_dir_result)
         print(
             "Monitoring app can be launched with:\n"
             f"fluidimage-monitor {self.path_dir_result}"
         )
         self.info_job = {
             "topology": topology_name,
@@ -272,15 +279,24 @@
 
     def _reset_std_as_default(self):
         sys.stdout = self._old_stdout
         sys.stderr = self._old_stderr
         reset_logger()
         self._log_file.close()
 
+    def _run_final_seq_work(self):
+        if (
+            hasattr(self.topology, "final_seq_work")
+            and not self._final_seq_work_run
+        ):
+            self.topology.final_seq_work()
+            self._final_seq_work_run = True
+
     def _finalize_compute(self):
+        self._run_final_seq_work()
         log_memory_usage(time_as_str(2) + ": end of `compute`. mem usage")
         self.topology.print_at_exit(time() - self.t_start)
         self._reset_std_as_default()
         self._release_lock()
 
     def log_in_file(self, *args, sep=" ", end="\n"):
         """Simple write in the log file (without print)"""
@@ -357,14 +373,50 @@
             input_queue=None, output_queue=first_work.output_queue
         )
         self._first_queue = copy.copy(first_work.output_queue)
         # split the first queue
         self._keys_first_queue = list(self._first_queue.keys())
         self.num_expected_results = len(self._keys_first_queue)
 
+    def _init_results_log(self, path_job_data):
+
+        if hasattr(self, "index_process"):
+            str_index_process = f"_{self.index_process:03}"
+        else:
+            str_index_process = ""
+
+        self._path_results = path_job_data / f"results{str_index_process}.txt"
+        self._path_num_results = (
+            self._path_results.parent / f"len_results{str_index_process}.txt"
+        )
+        self._len_saved_results = 0
+
+    def _save_results_names(self):
+
+        new_results = self.topology.results[self._len_saved_results :]
+        self._len_saved_results = len(self.topology.results)
+
+        with open(self._path_num_results, "w", encoding="utf-8") as file:
+            file.write(f"{self._len_saved_results}\n")
+
+        if new_results:
+            if isinstance(new_results[0], str):
+                new_results = [Path(path).name for path in new_results]
+            elif hasattr(new_results[0], "name"):
+                new_results = [_r.name for _r in new_results]
+            else:
+                new_results = [str(_r) for _r in new_results]
+            new_results = "\n".join(new_results) + "\n"
+
+            with open(self._path_results, "a", encoding="utf-8") as file:
+                file.write(new_results)
+
+        if not self._log_file.closed:
+            self._log_file.flush()
+
 
 class MultiExecutorBase(ExecutorBase):
     """Manage the multi-executor mode
 
      This class is not the one whose really compute the topology. The topology is
      split and each slice is computed with an ExecutorAsync
 
@@ -450,24 +502,14 @@
                 for process in self.processes:
                     os.kill(process.pid, signal_number)
 
             signal.signal(12, handler_signals)
 
         self._start_processes()
         self.nb_processes = len(self.processes)
-        self._wait_for_all_processes()
-        self._finalize_compute()
-
-    def _poll_return_code(self, process):
-        return process.poll()
-
-    def _join_processes(self):
-        """Join the processes"""
-
-    def _wait_for_all_processes(self):
 
         running_processes = {
             idx: process for idx, process in enumerate(self.processes)
         }
         running_processes_updated = {}
         return_codes = {}
         self.errors = {}
@@ -519,21 +561,34 @@
                     progress.update(progress_task, completed=num_results)
                 running_processes, running_processes_updated = (
                     running_processes_updated,
                     running_processes,
                 )
                 running_processes_updated.clear()
 
-        self._join_processes()
+            self._join_processes()
+
+            self.topology.results = results = []
+            for path in self.path_job_data.glob("results_*.txt"):
+                with open(path, encoding="utf-8") as file:
+                    results.extend(line.strip() for line in file.readlines())
+
+            self._run_final_seq_work()
+
+            progress.update(progress_task, completed=len(self.topology.results))
+
+        self._finalize_compute()
+
+    def _poll_return_code(self, process):
+        return process.poll()
+
+    def _join_processes(self):
+        """Join the processes"""
 
     def _finalize_compute(self):
-        self.topology.results = results = []
-        for path in self.path_job_data.glob("results_*.txt"):
-            with open(path, encoding="utf-8") as file:
-                results.extend(line.strip() for line in file.readlines())
 
         if self.errors:
             text_error = (
                 f"{len(self.errors)} sub-executors failed "
                 f"(over {len(self.processes)} processes)."
             )
             for idx_process, error in self.errors.items():
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/exec_async.py` & `fluidimage-0.5.2/src/fluidimage/executors/exec_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,19 @@
         and process the items as soon as they are available.
 
         """
         for work in self.works:
             # global functions
             if work.kind is not None and "global" in work.kind:
 
+                try:
+                    work.func_or_cls.__self__.executor = self
+                except AttributeError:
+                    pass
+
                 async def func(work=work):
                     while True:
                         while (
                             isinstance(work.input_queue, tuple)
                             and all(not q for q in work.input_queue)
                         ) or not work.input_queue:
                             await trio.sleep(self.sleep_time)
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/exec_async_multiproc.py` & `fluidimage-0.5.2/src/fluidimage/executors/exec_async_multiproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/exec_async_seq_for_multi.py` & `fluidimage-0.5.2/src/fluidimage/executors/exec_async_seq_for_multi.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     ):
         if stop_if_error:
             raise NotImplementedError(
                 "stop_if_error not implemented for ExecutorAsyncForMulti"
             )
 
         self._log_path = path_log
+        topology.executor = self
         super().__init__(
             topology,
             path_dir_result,
             nb_max_workers=nb_max_workers,
             nb_items_queue_max=8,
             sleep_time=sleep_time,
             logging_level=logging_level,
@@ -55,25 +56,18 @@
         self.num_expected_results = None
 
         if hasattr(self.topology, "results"):
             self.async_funcs["_save_topology_results"] = (
                 self._save_topology_results
             )
             path_log_dir = Path(self._log_path).parent
-            path_job_data = path_log_dir.with_name("job" + path_log_dir.name[3:])
-            self._path_results = (
-                path_job_data / f"results_{self.index_process:03}.txt"
+            self.path_job_data = path_log_dir.with_name(
+                "job" + path_log_dir.name[3:]
             )
-
-            self._path_num_results = (
-                self._path_results.parent
-                / f"len_results_{self.index_process:03}.txt"
-            )
-
-            self._len_saved_results = 0
+            self._init_results_log(self.path_job_data)
 
             sys.stdout = self._log_file
 
     def _get_file_object_for_logger(self):
         return self._log_file
 
     def _init_log_path(self):
@@ -96,37 +90,14 @@
         txt = self.topology.make_text_at_exit(time() - self.t_start)
         with open(self._log_path, "a", encoding="utf-8") as file:
             file.write(txt)
 
         if hasattr(self.topology, "results"):
             self._save_results_names()
 
-    def _save_results_names(self):
-
-        new_results = self.topology.results[self._len_saved_results :]
-        self._len_saved_results = len(self.topology.results)
-
-        with open(self._path_num_results, "w", encoding="utf-8") as file:
-            file.write(f"{self._len_saved_results}\n")
-
-        if new_results:
-            if isinstance(new_results[0], str):
-                new_results = [Path(path).name for path in new_results]
-            elif hasattr(new_results[0], "name"):
-                new_results = [_r.name for _r in new_results]
-            else:
-                new_results = [str(_r) for _r in new_results]
-            new_results = "\n".join(new_results) + "\n"
-
-            with open(self._path_results, "a", encoding="utf-8") as file:
-                file.write(new_results)
-
-        if not self._log_file.closed:
-            self._log_file.flush()
-
     async def _save_topology_results(self):
         while not self._has_to_stop:
             self._save_results_names()
             await trio.sleep(1.0)
 
 
 Executor = ExecutorAsyncSeqForMulti
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/exec_async_sequential.py` & `fluidimage-0.5.2/src/fluidimage/executors/exec_async_sequential.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/exec_async_servers.py` & `fluidimage-0.5.2/src/fluidimage/executors/exec_async_servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 
 .. autoclass:: ExecutorAsyncServers
    :members:
    :private-members:
 
 """
 
-import os
 import signal
 
 import numpy as np
 import trio
 
-from fluiddyn import time_as_str
 from fluidimage.util import log_debug, logger
 
 from .exec_async import ExecutorAsync
 from .servers import launch_server
 
 max_items_in_server = 4
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/exec_sequential.py` & `fluidimage-0.5.2/src/fluidimage/executors/exec_sequential.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,26 @@
 
     def compute(self):
         """Compute the whole topology."""
         self._init_compute()
         self.exec_one_shot_works()
         self._run_works()
         self._finalize_compute()
+        if hasattr(self.topology, "results"):
+            self._save_results_names()
 
     def _run_works(self):
         while not all([len(queue) == 0 for queue in self.topology.queues]):
             for work in self.works:
                 # global functions
                 if work.kind is not None and "global" in work.kind:
-                    if len(work.output_queue) > self.nb_items_queue_max:
+                    if (
+                        work.output_queue is not None
+                        and len(work.output_queue) > self.nb_items_queue_max
+                    ):
                         continue
 
                     work.func_or_cls(work.input_queue, work.output_queue)
 
                 else:
                     if not work.input_queue:
                         continue
@@ -63,9 +68,21 @@
                             f"work {work.name_no_space} ({key}) "
                             f"done in {time.time() - t_start:.3f} s"
                         )
 
                     if work.output_queue is not None:
                         work.output_queue[key] = ret
 
+            if hasattr(self.topology, "results"):
+                self._save_results_names()
+
+    def _init_compute_log(self):
+        self.nb_max_workers = 1
+        super()._init_compute_log()
+
+    def _save_job_data(self):
+        super()._save_job_data()
+        if hasattr(self.topology, "results"):
+            self._init_results_log(self.path_job_data)
+
 
 Executor = ExecutorSequential
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/multi_exec_async.py` & `fluidimage-0.5.2/src/fluidimage/executors/multi_exec_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,25 @@
 Multi executors async
 =====================
 
 .. autoclass:: MultiExecutorAsync
    :members:
    :private-members:
 
-.. autoclass:: ExecutorAsyncForMulti
-   :members:
-   :private-members:
-
 """
 
 import copy
 from multiprocessing import Process
 
+from fluidimage.topologies.splitters import split_list
+
 from .base import MultiExecutorBase
 from .exec_async_seq_for_multi import ExecutorAsyncSeqForMulti
 
 
-class ExecutorAsyncForMulti(ExecutorAsyncSeqForMulti):
-    """Slightly modified ExecutorAsync"""
-
-
 class MultiExecutorAsync(MultiExecutorBase):
     """Manage the multi-executor mode
 
      This class is not the one whose really compute the topology. The topology is
      split and each slice is computed with an ExecutorAsync
 
     Parameters
@@ -44,14 +38,16 @@
 
       Defines the waiting time (from trio.sleep) of a function. Async functions
       await `trio.sleep(sleep_time)` when they have done a work on an item, and
       when there is nothing in their input_queue.
 
     """
 
+    ExecutorForMulti = ExecutorAsyncSeqForMulti
+
     def _start_processes(self):
         """
         There are two ways to split self.topology work:
 
         - If first self.topology has "series" attribute (from seriesOfArray), it
           creates "self.nb_max_workers" topologies and changes "ind_start" and
           "ind_stop" of topology.series. The split considers series.ind_step.
@@ -68,24 +64,15 @@
             self._start_multiprocess_series()
         else:
             self._start_multiprocess_first_queue()
 
     def _start_multiprocess_first_queue(self):
         """Start the processes spitting the work with the first queue"""
 
-        nb_keys_per_process = max(
-            1, int(len(self._keys_first_queue) / self.nb_processes)
-        )
-
-        keys_for_processes = []
-        for iproc in range(self.nb_processes):
-            istart = iproc * nb_keys_per_process
-            keys_for_processes.append(
-                self._keys_first_queue[istart : istart + nb_keys_per_process]
-            )
+        keys_for_processes = split_list(self._keys_first_queue, self.nb_processes)
 
         # change topology
         self.topology.first_queue = self.topology.works[0].output_queue
         topology = copy.copy(self.topology)
         topology.first_queue.clear()
         del topology.works[0]
         old_queue = topology.first_queue
@@ -168,15 +155,15 @@
                 series.ind_start, series.ind_stop, series.ind_step = (
                     start_stop_step
                 )
                 self.launch_process(new_topology, idx_process)
 
     def init_and_compute(self, topology_this_process, log_path, idx_process):
         """Create an executor and start it in a process"""
-        executor = ExecutorAsyncForMulti(
+        executor = self.ExecutorForMulti(
             topology_this_process,
             self.path_dir_result,
             sleep_time=self.sleep_time,
             path_log=log_path,
             logging_level=self.logging_level,
             t_start=self.t_start,
             index_process=idx_process,
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/multi_exec_subproc.py` & `fluidimage-0.5.2/src/fluidimage/executors/multi_exec_subproc.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,37 +18,38 @@
 from .base import MultiExecutorBase
 
 
 class MultiExecutorSubproc(MultiExecutorBase):
     """Multi executor based on subprocesses and splitters"""
 
     splitter: Splitter
+    executor_for_multi = "exec_async_seq_for_multi"
 
     def _init_num_expected_results(self):
 
         try:
             splitter_cls = self.topology.Splitter
         except AttributeError as error:
             raise ValueError(
-                "MultiExecutorSubproc can only execute "
+                f"{type(self).__name__} can only execute "
                 "topologies with a Splitter."
             ) from error
 
         params = deepcopy(self.topology.params)
 
         try:
             params._set_child(
                 "compute_kwargs",
                 attribs={
-                    "executor": "exec_async_seq_for_multi",
+                    "executor": self.executor_for_multi,
                     "nb_max_workers": 1,
                 },
             )
         except ValueError:
-            params.compute_kwargs.executor = "exec_async_seq_for_multi"
+            params.compute_kwargs.executor = self.executor_for_multi
             params.compute_kwargs.nb_max_workers = 1
 
         try:
             params.compute_kwargs._set_child(
                 "kwargs_executor",
                 attribs={
                     "path_log": None,
```

### Comparing `fluidimage-0.5.1/src/fluidimage/executors/servers.py` & `fluidimage-0.5.2/src/fluidimage/executors/servers.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,14 +173,23 @@
                 except AttributeError:
                     pass
 
             signal.signal(signal.SIGINT, signal_handler)
 
         self.conn = conn
         self.event_has_to_stop = event_has_to_stop
+
+        try:
+            params.saving.how
+        except AttributeError:
+            pass
+        else:
+            if params.saving.how == "ask":
+                params.saving.how = "complete"
+
         self.topology = topology_cls(params)
 
         self._log_file = open(log_path, "w", encoding="utf-8")
 
         stdout = sys.stdout
         if isinstance(stdout, MultiFile):
             stdout = sys.__stdout__
```

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/base_matplotlib.py` & `fluidimage-0.5.2/src/fluidimage/gui/base_matplotlib.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/imviewer.py` & `fluidimage-0.5.2/src/fluidimage/gui/imviewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/launcher/main.py` & `fluidimage-0.5.2/src/fluidimage/gui/launcher/main.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.py` & `fluidimage-0.5.2/src/fluidimage/gui/launcher/mainwindow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.ui` & `fluidimage-0.5.2/src/fluidimage/gui/launcher/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/launcher/test_launcher.py` & `fluidimage-0.5.2/src/fluidimage/gui/launcher/test_launcher.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/monitor.py` & `fluidimage-0.5.2/src/fluidimage/gui/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         module_name, class_name = self.info_job["topology"].rsplit(".", 1)
         mod = import_module(module_name)
         class_topology = getattr(mod, class_name)
         params_default = class_topology.create_default_params()
         copy_doc(self.params, params_default)
 
         self.paths_len_results = sorted(
-            self.path_job_info.glob("len_results_*.txt")
+            self.path_job_info.glob("len_results*.txt")
         )
         assert self.paths_len_results
 
         self.num_results = 0
         self.detect_results()
 
     def detect_results(self):
```

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/pg_main.py` & `fluidimage-0.5.2/src/fluidimage/gui/pg_main.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/pg_wrapper.py` & `fluidimage-0.5.2/src/fluidimage/gui/pg_wrapper.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/piv_viewer.py` & `fluidimage-0.5.2/src/fluidimage/gui/piv_viewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/test_imviewer.py` & `fluidimage-0.5.2/src/fluidimage/gui/test_imviewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/test_imviewer_pg.py` & `fluidimage-0.5.2/src/fluidimage/gui/test_imviewer_pg.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/test_monitor.py` & `fluidimage-0.5.2/src/fluidimage/gui/test_monitor.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/gui/test_piv_viewer.py` & `fluidimage-0.5.2/src/fluidimage/gui/test_piv_viewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/image2image.py` & `fluidimage-0.5.2/src/fluidimage/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/meson.build` & `fluidimage-0.5.2/src/fluidimage/meson.build`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/postproc/piv.py` & `fluidimage-0.5.2/src/fluidimage/postproc/piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/postproc/postproc.py` & `fluidimage-0.5.2/src/fluidimage/postproc/postproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/postproc/test_piv.py` & `fluidimage-0.5.2/src/fluidimage/postproc/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/postproc/test_util.py` & `fluidimage-0.5.2/src/fluidimage/postproc/test_util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/postproc/util.py` & `fluidimage-0.5.2/src/fluidimage/postproc/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/postproc/vector_field.py` & `fluidimage-0.5.2/src/fluidimage/postproc/vector_field.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/preproc.py` & `fluidimage-0.5.2/src/fluidimage/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/mlos.py` & `fluidimage-0.5.2/src/fluidimage/reconstruct/tomo/mlos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/test_mlos.py` & `fluidimage-0.5.2/src/fluidimage/reconstruct/tomo/test_mlos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/run_from_xml.py` & `fluidimage-0.5.2/src/fluidimage/run_from_xml.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/synthetic.py` & `fluidimage-0.5.2/src/fluidimage/synthetic.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/test_image2image.py` & `fluidimage-0.5.2/src/fluidimage/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/test_run_from_xml.py` & `fluidimage-0.5.2/src/fluidimage/test_run_from_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     command = f"run {path_uvmat_xml} --mode recompute"
 
     with monkeypatch.context() as ctx:
         ctx.setattr(sys, "argv", command.split())
         action = main()
 
     path_results = tmp_path / "Images.civ"
-    assert action.params.saving.path == str(path_results)
+    assert str(action.params.saving.path) == str(path_results)
 
     paths_piv = sorted(p.name for p in path_results.glob("piv*.h5"))
 
     if name == "Karman":
         assert paths_piv == ["piv_01-02.h5", "piv_03-04.h5"]
     elif name == "Jet":
         assert paths_piv == ["piv_060ab.h5", "piv_061ab.h5"]
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/base.py` & `fluidimage-0.5.2/src/fluidimage/topologies/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,30 +20,93 @@
 .. autoclass:: TopologyBaseFromImages
    :members:
    :private-members:
 
 """
 
 import json
+import os
+import sys
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from pathlib import Path
 from typing import Sequence, Union
 from warnings import warn
 
+from fluiddyn.io.query import query
 from fluidimage import ParamContainer, SerieOfArraysFromFiles, SeriesOfArrays
 from fluidimage.util import DEBUG, cstring, logger
 
 from ..executors import (
     ExecutorBase,
     get_executor_names,
     import_executor_class,
     supported_multi_executors,
 )
 
+how_values = ("ask", "new_dir", "complete", "recompute", "from_path_indices")
+
+
+def prepare_path_dir_result(
+    path_dir_input, path_saving, postfix_saving, how_saving
+):
+    """Makes new directory for results, if required, and returns its path."""
+
+    if how_saving not in how_values:
+        raise ValueError(
+            f"how_saving (here equal to '{how_saving}') "
+            f"should be in {how_values}"
+        )
+
+    path_dir_input = str(path_dir_input)
+
+    if path_saving is not None:
+        path_dir_result = path_saving
+    else:
+        path_dir_result = path_dir_input + "." + postfix_saving
+
+    how = how_saving
+    if not os.path.exists(path_dir_result):
+        if how == "ask":
+            how = "recompute"
+    else:
+        if how == "ask":
+            answer = query(
+                f"The directory {path_dir_result} "
+                + "already exists. What do you want to do?\n"
+                "New dir, Complete, Recompute or Stop?\n"
+            )
+
+            while answer.lower() not in ["n", "c", "r", "s"]:
+                answer = query(
+                    "The answer should be in ['n', 'c', 'r', 's']\n"
+                    "Please type your answer again...\n"
+                )
+
+            if answer == "s":
+                print("Stopped by the user.")
+                sys.exit()
+
+            elif answer == "n":
+                how = "new_dir"
+            elif answer == "c":
+                how = "complete"
+            elif answer == "r":
+                how = "recompute"
+
+        if how == "new_dir":
+            i = 0
+            while os.path.exists(path_dir_result + str(i)):
+                i += 1
+            path_dir_result += str(i)
+
+    path_dir_result = Path(path_dir_result)
+    path_dir_result.mkdir(exist_ok=True)
+    return path_dir_result, how
+
 
 class Work:
     """Represent a work
 
     Work are treated differently by executors depending of the ``kind``
     argument. Work can be:
 
@@ -142,14 +205,21 @@
         """Check if a name is in the queue"""
         for names in self.values():
             if image_name in names:
                 return True
         return False
 
 
+class QueueList(list):
+
+    def __init__(self, name):
+        self.name = name
+        super().__init__()
+
+
 class TopologyBase:
     """Base class for topologies of processing.
 
     This class is meant to be subclassed, not instantiated directly.
 
     Parameters
     ----------
@@ -195,28 +265,48 @@
                     "module": cls.__module__,
                     "class": cls.__name__,
                 }
             ),
         )
 
     def __init__(
-        self, path_dir_result=None, logging_level="info", nb_max_workers=None
+        self,
+        params=None,
+        path_dir_src=None,
+        path_dir_result=None,
+        logging_level="info",
+        nb_max_workers=None,
     ):
-        self.path_dir_result = path_dir_result
+        self.params = params
+        self.path_dir_src = Path(path_dir_src)
+        if path_dir_result is None:
+            self._init_path_dir_result(path_dir_src)
+        else:
+            self.path_dir_result = path_dir_result
         self.logging_level = logging_level
         self.nb_max_workers = nb_max_workers
 
         self.queues = []
         self.works = []
         self.works_dict = {}
         self.executor = None
 
+    def _init_path_dir_result(self, path_dir_src):
+        p_saving = self.params.saving
+        self.path_dir_result, self.how_saving = prepare_path_dir_result(
+            path_dir_src, p_saving.path, p_saving.postfix, p_saving.how
+        )
+        p_saving.path = self.path_dir_result
+
     def add_queue(self, name: str, kind: str = None):
         """Create a new queue."""
-        queue = Queue(name=name, kind=kind)
+        if kind == "list":
+            queue = QueueList(name)
+        else:
+            queue = Queue(name=name, kind=kind)
         self.queues.append(queue)
         return queue
 
     def add_work(
         self,
         name: str,
         func_or_cls,
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/bos.py` & `fluidimage-0.5.2/src/fluidimage/topologies/bos.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 """
 
 import sys
 from pathlib import Path
 
 from fluidimage import ParamContainer
 from fluidimage.data_objects.piv import get_name_bos
-from fluidimage.topologies import prepare_path_dir_result
 from fluidimage.topologies.base import TopologyBaseFromImages
 from fluidimage.topologies.splitters import SplitterFromImages
 from fluidimage.util import imread
 from fluidimage.works import image2image
 from fluidimage.works.bos import WorkBOS
 
 
@@ -90,30 +89,21 @@
 
         params._set_child("preproc")
         image2image.complete_im2im_params_with_default(params.preproc)
 
         return params
 
     def __init__(self, params, logging_level="info", nb_max_workers=None):
-        self.params = params
-
         self.main_work = WorkBOS(params)
         self.serie = self.main_work.serie
         self.path_reference = self.main_work.path_reference
 
-        path_dir = Path(self.serie.path_dir)
-        path_dir_result, self.how_saving = prepare_path_dir_result(
-            path_dir, params.saving.path, params.saving.postfix, params.saving.how
-        )
-
-        self.path_dir_result = path_dir_result
-        self.path_dir_src = Path(path_dir)
-
         super().__init__(
-            path_dir_result=path_dir_result,
+            params=params,
+            path_dir_src=self.serie.path_dir,
             logging_level=logging_level,
             nb_max_workers=nb_max_workers,
         )
 
         queue_paths = self.add_queue("paths")
         queue_arrays = queue_arrays1 = self.add_queue("arrays")
         queue_bos = self.add_queue("bos")
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/example.py` & `fluidimage-0.5.2/src/fluidimage/topologies/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,31 +88,29 @@
             path_dir_result=None,
             nloops=1,
             multiplicator_nb_images=1,
         )
         return params
 
     def __init__(self, params, logging_level="info", nb_max_workers=None):
-        self.params = params
 
-        path_input = params["path_input"]
         path_dir_result = params["path_dir_result"]
         nloops = params["nloops"]
         self.multiplicator_nb_images = params["multiplicator_nb_images"]
 
-        self.path_input = path_input
-
         super().__init__(
+            params=params,
+            path_dir_src=params["path_input"],
             path_dir_result=path_dir_result,
             logging_level=logging_level,
             nb_max_workers=nb_max_workers,
         )
 
-        if not self.path_dir_result.exists():
-            self.path_dir_result.mkdir()
+        if not path_dir_result.exists():
+            path_dir_result.mkdir()
 
         self.img_counter = 0
 
         func1 = partial(func1_for_partial, nloops)
         func2 = partial(func2_for_partial, nloops)
 
         queue_names = self.add_queue("names images")
@@ -163,28 +161,29 @@
             output_queue=queue_cpu2,
         )
         self.add_work(
             "save", func_or_cls=self.save, input_queue=queue_cpu2, kind="io"
         )
 
     def fill_names(self, input_queue, output_queue):
+        del input_queue
         for ind in range(self.multiplicator_nb_images):
-            for name in sorted(os.listdir(self.path_input)):
+            for name in sorted(os.listdir(self.path_dir_src)):
                 key = name.split(".bmp")[0] + f"_{ind:02}"
                 output_queue[key] = name
 
     def fill_couples_names(self, input_queue, output_queue):
         for key, name in list(input_queue.items()):
             output_queue[key] = [key, (name, name)]
 
     def read_array(self, name):
         if name == "Karman_03.bmp":
             raise ValueError("For testing")
 
-        image = imread(self.path_input / name)
+        image = imread(self.path_dir_src / name)
         return image
 
     def fill_couples_arrays(self, input_queues, output_queue):
         queue_couples_names, queue_arrays = input_queues
         queue_couples_arrays = output_queue
 
         for key, array in list(queue_arrays.items()):
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/image2image.py` & `fluidimage-0.5.2/src/fluidimage/topologies/image2image.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 """
 
 import sys
 from pathlib import Path
 
 from fluiddyn.io.image import imsave
 from fluidimage import ParamContainer
-from fluidimage.topologies import prepare_path_dir_result
 from fluidimage.topologies.splitters import SplitterFromImages
 from fluidimage.util import imread
 from fluidimage.works.image2image import WorkImage2Image
 
 from .base import TopologyBaseFromImages
 
 
@@ -67,33 +66,25 @@
 
         super()._add_default_params_saving(params)
         WorkImage2Image._complete_params_with_default(params)
 
         return params
 
     def __init__(self, params, logging_level="info", nb_max_workers=None):
-        self.params = params
 
         if params.im2im is None:
             raise ValueError("params.im2im has to be set.")
 
         self.work = WorkImage2Image(params)
         self.serie = self.work.serie
         im2im_func = self.work.im2im_func
 
-        path_dir = self.serie.path_dir
-        path_dir_result, self.how_saving = prepare_path_dir_result(
-            path_dir, params.saving.path, params.saving.postfix, params.saving.how
-        )
-
-        self.path_dir_result = path_dir_result
-        self.path_dir_src = Path(path_dir)
-
         super().__init__(
-            path_dir_result=path_dir_result,
+            params=params,
+            path_dir_src=self.serie.path_dir,
             logging_level=logging_level,
             nb_max_workers=nb_max_workers,
         )
 
         self.queue_paths = self.add_queue("paths")
         self.queue_arrays = self.add_queue("arrays")
         self.queue_results = self.add_queue("results")
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/launcher.py` & `fluidimage-0.5.2/src/fluidimage/topologies/launcher.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/log.py` & `fluidimage-0.5.2/src/fluidimage/topologies/log.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/nb_cpu_cores.py` & `fluidimage-0.5.2/src/fluidimage/topologies/nb_cpu_cores.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/optical_flow.py` & `fluidimage-0.5.2/src/fluidimage/topologies/optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/piv.py` & `fluidimage-0.5.2/src/fluidimage/topologies/piv.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import copy
 import sys
 from pathlib import Path
 
 from fluidimage import ParamContainer, SeriesOfArrays
 from fluidimage.data_objects.piv import ArrayCouple, get_name_piv
-from fluidimage.topologies import TopologyBaseFromSeries, prepare_path_dir_result
+from fluidimage.topologies import TopologyBaseFromSeries
 from fluidimage.topologies.nb_cpu_cores import nb_cores
 from fluidimage.topologies.splitters import SplitterFromSeries
 from fluidimage.util import imread, logger
 from fluidimage.works import image2image
 from fluidimage.works.piv import WorkPIV
 
 
@@ -84,21 +84,17 @@
             params.series.path,
             params.series.str_subset,
             ind_start=params.series.ind_start,
             ind_stop=params.series.ind_stop,
             ind_step=params.series.ind_step,
         )
 
-        path_dir = self.series.serie.path_dir
-        path_dir_result, self.how_saving = prepare_path_dir_result(
-            path_dir, params.saving.path, params.saving.postfix, params.saving.how
-        )
-
         super().__init__(
-            path_dir_result=path_dir_result,
+            params=params,
+            path_dir_src=self.series.serie.path_dir,
             logging_level=logging_level,
             nb_max_workers=nb_max_workers,
         )
 
         queue_couples_of_names = self.add_queue("couples of names")
         queue_paths = self.add_queue("paths")
         queue_arrays = queue_arrays1 = self.add_queue("arrays")
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/preproc.py` & `fluidimage-0.5.2/src/fluidimage/topologies/preproc.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import sys
 from typing import Dict, Tuple
 
 from fluiddyn.util.paramcontainer import ParamContainer
 from fluidimage import SeriesOfArrays
 from fluidimage.data_objects.preproc import ArraySerie as ArraySubset
 from fluidimage.data_objects.preproc import PreprocResults, get_name_preproc
-from fluidimage.topologies import TopologyBaseFromSeries, prepare_path_dir_result
+from fluidimage.topologies import TopologyBaseFromSeries
 from fluidimage.topologies.splitters import SplitterFromSeries
 from fluidimage.util import imread
 from fluidimage.works import image2image
 from fluidimage.works.preproc import (
     WorkPreproc,
     _make_doc_with_filtered_params_doc,
 )
@@ -187,31 +187,22 @@
         subset = self.series.get_serie_from_index(0)
         self.nb_items_per_serie = subset.get_nb_arrays()
 
         if os.path.isdir(params.series.path):
             path_dir = params.series.path
         else:
             path_dir = os.path.dirname(params.series.path)
-        self.path_dir_input = path_dir
-
-        path_dir_result, self.how_saving = prepare_path_dir_result(
-            path_dir,
-            params.saving.path,
-            params.saving.postfix,
-            params.saving.how,
-        )
 
         super().__init__(
-            path_dir_result=path_dir_result,
+            params=params,
+            path_dir_src=path_dir,
             logging_level=logging_level,
             nb_max_workers=nb_max_workers,
         )
 
-        self.params.saving.path = self.path_dir_result
-
         # Define waiting queues
         queue_subsets_of_names = self.add_queue("subsets of filenames")
         queue_paths = self.add_queue("image paths")
         queue_arrays = queue_arrays1 = self.add_queue("arrays")
         queue_subsets_of_arrays = self.add_queue("subsets of arrays")
         queue_preproc_objects = self.add_queue("preproc results")
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/splitters.py` & `fluidimage-0.5.2/src/fluidimage/topologies/splitters.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/surface_tracking.py` & `fluidimage-0.5.2/src/fluidimage/topologies/surface_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 import sys
 from pathlib import Path
 
 from fluiddyn.io.image import imsave_h5
 from fluidimage import ParamContainer, SerieOfArraysFromFiles, SeriesOfArrays
-from fluidimage.topologies import TopologyBase, prepare_path_dir_result
+from fluidimage.topologies import TopologyBase
 from fluidimage.util import imread, logger
 from fluidimage.works import image2image
 from fluidimage.works.surface_tracking import WorkSurfaceTracking
 
 
 class TopologySurfaceTracking(TopologyBase):
     """Topology for SurfaceTracking.
@@ -119,26 +119,19 @@
             + str(self.serie.get_slicing_tuples()[0][2] + 1)
             + ":"
             + str(self.serie.get_slicing_tuples()[0][2]),
             ind_start=self.serie.get_slicing_tuples()[0][0],
             ind_stop=self.serie.get_slicing_tuples()[0][1] - 1,
             ind_step=self.serie.get_slicing_tuples()[0][2],
         )
-        path_dir = self.serie.path_dir
-        path_dir_result, self.how_saving = prepare_path_dir_result(
-            path_dir, params.saving.path, params.saving.postfix, params.saving.how
-        )
-
-        self.path_dir_result = path_dir_result
-        self.path_dir_src = Path(path_dir)
-
         self.surface_tracking_work = WorkSurfaceTracking(params)
 
         super().__init__(
-            path_dir_result=path_dir_result,
+            params=params,
+            path_dir_src=self.serie.path_dir,
             logging_level=logging_level,
             nb_max_workers=nb_max_workers,
         )
 
         queue_paths = self.add_queue("paths")
         queue_couples_of_names = self.add_queue("couples of names")
         queue_arrays = queue_arrays1 = self.add_queue("arrays")
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_bos.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_example.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+import sys
+
 import pytest
 
 from fluidimage.executors import supported_multi_executors
 from fluidimage.topologies.example import TopologyExample
 
 executors = [
     "exec_sequential",
     "exec_async_sequential",
     "exec_async",
     "exec_async_multi",
-    "exec_async_servers",
     "exec_async_servers_threading",
 ]
 
+if sys.platform != "darwin":
+    # too much ConnectionRefusedError on Github Actions
+    executors.extend(
+        [
+            "exec_async_servers",
+        ]
+    )
+
 executors.extend(supported_multi_executors)
 
 # tmp: TopologyExample doesn't have a Splitter
 executors.remove("multi_exec_subproc")
+executors.remove("multi_exec_subproc_sync")
 
 
+@pytest.mark.usefixtures("close_plt_figs")
 @pytest.mark.parametrize("executor", executors)
 def test_topo_example(tmp_path_karman, executor):
 
     path_input = tmp_path_karman
 
     params = TopologyExample.create_default_params()
     params["path_input"] = path_input
@@ -34,15 +45,17 @@
 
     # there is a logging problem with this class but we don't mind.
     if executor != "exec_async_servers_threading":
         log = topology.read_log_data()
         assert (
             log.topology_name == "fluidimage.topologies.example.TopologyExample"
         )
-        assert log.nb_max_workers == 2
+
+        if executor != "exec_sequential":
+            assert log.nb_max_workers == 2
 
         if [
             len(log.durations[key])
             for key in ("read_array", "cpu1", "cpu2", "save")
         ] != [4, 3, 2, 2]:
             print("Issue with this log file:")
             print(log.path_log_file.read_text())
```

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_image2image.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_optical_flow.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_piv.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_preproc.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_splitters.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_splitters.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/topologies/test_surftracking.py` & `fluidimage-0.5.2/src/fluidimage/topologies/test_surftracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/util/__init__.py` & `fluidimage-0.5.2/src/fluidimage/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/util/log.py` & `fluidimage-0.5.2/src/fluidimage/util/log.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/util/util.py` & `fluidimage-0.5.2/src/fluidimage/util/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/uvmat.py` & `fluidimage-0.5.2/src/fluidimage/uvmat.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/__init__.py` & `fluidimage-0.5.2/src/fluidimage/works/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/bos.py` & `fluidimage-0.5.2/src/fluidimage/works/bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/image2image.py` & `fluidimage-0.5.2/src/fluidimage/works/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/optical_flow.py` & `fluidimage-0.5.2/src/fluidimage/works/optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/piv/fix.py` & `fluidimage-0.5.2/src/fluidimage/works/piv/fix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/piv/multipass.py` & `fluidimage-0.5.2/src/fluidimage/works/piv/multipass.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/piv/singlepass.py` & `fluidimage-0.5.2/src/fluidimage/works/piv/singlepass.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/piv/test_piv.py` & `fluidimage-0.5.2/src/fluidimage/works/piv/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/preproc/__init__.py` & `fluidimage-0.5.2/src/fluidimage/works/preproc/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_cv.py` & `fluidimage-0.5.2/src/fluidimage/works/preproc/_toolbox_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_py.py` & `fluidimage-0.5.2/src/fluidimage/works/preproc/_toolbox_py.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/preproc/io.py` & `fluidimage-0.5.2/src/fluidimage/works/preproc/io.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/preproc/toolbox.py` & `fluidimage-0.5.2/src/fluidimage/works/preproc/toolbox.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/surface_tracking.py` & `fluidimage-0.5.2/src/fluidimage/works/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/test_bos.py` & `fluidimage-0.5.2/src/fluidimage/works/test_bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/test_image2image.py` & `fluidimage-0.5.2/src/fluidimage/works/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/test_preproc.py` & `fluidimage-0.5.2/src/fluidimage/works/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/src/fluidimage/works/with_mask.py` & `fluidimage-0.5.2/src/fluidimage/works/with_mask.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.1/PKG-INFO` & `fluidimage-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidimage
-Version: 0.5.1
+Version: 0.5.2
 Summary: Fluid image processing with Python.
 Keywords: PIV
 Author-Email: Pierre Augier <pierre.augier@legi.cnrs.fr>
 License: CeCILL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

