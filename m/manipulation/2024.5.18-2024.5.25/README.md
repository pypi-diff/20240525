# Comparing `tmp/manipulation-2024.5.18.tar.gz` & `tmp/manipulation-2024.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manipulation-2024.5.18.tar", max compression
+gzip compressed data, was "manipulation-2024.5.25.tar", max compression
```

## Comparing `manipulation-2024.5.18.tar` & `manipulation-2024.5.25.tar`

### file list

```diff
@@ -1,146 +1,145 @@
--rw-r--r--   0        0        0     1561 2024-02-22 14:57:44.046800 manipulation-2024.5.18/LICENSE.TXT
--rw-r--r--   0        0        0      536 2024-05-21 02:06:24.674757 manipulation-2024.5.18/README.md
--rw-r--r--   0        0        0      167 2024-02-22 14:57:44.110801 manipulation-2024.5.18/manipulation/__init__.py
--rw-r--r--   0        0        0      846 2024-02-22 14:57:44.110801 manipulation-2024.5.18/manipulation/_static/custom.css
--rw-r--r--   0        0        0     6481 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/clutter.py
--rw-r--r--   0        0        0      891 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/conf.py
--rw-r--r--   0        0        0    16339 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/create_sdf_from_mesh.py
--rw-r--r--   0        0        0      211 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/drake_gym.py
--rw-r--r--   0        0        0     9221 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/envs/box_flipup.py
--rw-r--r--   0        0        0     8473 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/envs/planar_gripper_pushing_a_box.py
--rw-r--r--   0        0        0    32464 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/normal_solution.npy
--rw-r--r--   0        0        0     1724 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_analytic_grasp.py
--rw-r--r--   0        0        0     6751 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_grasp_candidate.py
--rw-r--r--   0        0        0     1768 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_normal.py
--rw-r--r--   0        0        0     3978 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_simulation_tuning.py
--rw-r--r--   0        0        0     3598 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/deep_perception/test_contrastive.py
--rw-r--r--   0        0        0     1563 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/force/test_hybrid.py
--rw-r--r--   0        0        0     4758 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/grader.py
--rw-r--r--   0        0        0     3934 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/mobile/test_mobile_base_ik.py
--rw-r--r--   0        0        0     1188 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/plot_planar_manipulator.py
--rw-r--r--   0        0        0    26806 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_differential_ik.py
--rw-r--r--   0        0        0     3585 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_planar_manipulator.py
--rw-r--r--   0        0        0     2874 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_rigid_transforms.py
--rw-r--r--   0        0        0     1881 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_robot_painter.py
--rw-r--r--   0        0        0     1139 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_simple_qp.py
--rw-r--r--   0        0        0     3642 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pose/test_icp.py
--rw-r--r--   0        0        0     1445 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pose/test_pose_estimation.py
--rw-r--r--   0        0        0     3240 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pose/test_ransac.py
--rw-r--r--   0        0        0     3380 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/rl/test_stochastic_optimization.py
--rw-r--r--   0        0        0     2825 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/rl/test_vpg.py
--rw-r--r--   0        0        0      870 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/robot/test_direct_joint_control.py
--rw-r--r--   0        0        0     1184 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/robot/test_hardware_station_io.py
--rw-r--r--   0        0        0     2261 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/robot/test_reflected_inertia.py
--rw-r--r--   0        0        0      672 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/robot/test_survey.py
--rw-r--r--   0        0        0     1372 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/segmentation/test_mask.py
--rw-r--r--   0        0        0     2271 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
--rw-r--r--   0        0        0        0 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/__init__.py
--rw-r--r--   0        0        0    23490 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/geometry.py
--rw-r--r--   0        0        0     3711 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
--rw-r--r--   0        0        0     6529 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/robot.py
--rw-r--r--   0        0        0    14614 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
--rw-r--r--   0        0        0     1464 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/test_door_opening.py
--rw-r--r--   0        0        0     2391 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/test_rrt_planning.py
--rw-r--r--   0        0        0     5489 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/test_taskspace_iris.py
--rw-r--r--   0        0        0     3764 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/icp.py
--rw-r--r--   0        0        0      243 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/index.md
--rw-r--r--   0        0        0      256 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/meshcat_cpp_utils.py
--rw-r--r--   0        0        0      102 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/meshcat_utils.md
--rw-r--r--   0        0        0    17872 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/meshcat_utils.py
--rw-r--r--   0        0        0     5938 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
--rw-r--r--   0        0        0     1656 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/models/book.sdf
--rw-r--r--   0        0        0     1280 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/models/bunny/README
--rw-r--r--   0        0        0   658744 2024-02-22 14:57:44.122801 manipulation-2024.5.18/manipulation/models/bunny/bun_zipper_res2.ply
--rw-r--r--   0        0        0   196232 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/bunny/bunny.npy
--rw-r--r--   0        0        0     1496 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/camera_box.sdf
--rw-r--r--   0        0        0      155 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter.dmd.yaml
--rw-r--r--   0        0        0     1544 2024-04-08 12:21:31.612057 manipulation-2024.5.18/manipulation/models/clutter.scenarios.yaml
--rw-r--r--   0        0        0      367 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter_mustard.dmd.yaml
--rw-r--r--   0        0        0      183 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter_planning.dmd.yaml
--rw-r--r--   0        0        0      165 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter_w_cameras.dmd.yaml
--rw-r--r--   0        0        0     1976 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/cupboard.scenario.yaml
--rw-r--r--   0        0        0     2485 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/double_pendulum.urdf
--rw-r--r--   0        0        0      215 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/floating_joint.urdf
--rw-r--r--   0        0        0     1407 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/floor.sdf
--rw-r--r--   0        0        0     1472 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/003_cracker_box.sdf
--rw-r--r--   0        0        0     1470 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/004_sugar_box.sdf
--rw-r--r--   0        0        0     1631 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/005_tomato_soup_can.sdf
--rw-r--r--   0        0        0     4991 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/006_mustard_bottle.sdf
--rw-r--r--   0        0        0     1480 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/009_gelatin_box.sdf
--rw-r--r--   0        0        0     1476 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/010_potted_meat_can.sdf
--rw-r--r--   0        0        0     1104 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/061_foam_brick.sdf
--rw-r--r--   0        0        0      246 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/README.md
--rw-r--r--   0        0        0     4709 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/bin.sdf
--rw-r--r--   0        0        0     9110 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/cupboard.sdf
--rw-r--r--   0        0        0     6069 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf
--rw-r--r--   0        0        0     5708 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf
--rw-r--r--   0        0        0    21069 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj
--rw-r--r--   0        0        0    21659 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj
--rw-r--r--   0        0        0    23842 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj
--rw-r--r--   0        0        0    24252 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj
--rw-r--r--   0        0        0    26183 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj
--rw-r--r--   0        0        0    15215 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj
--rw-r--r--   0        0        0    18773 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj
--rw-r--r--   0        0        0    23818 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj
--rw-r--r--   0        0        0    24964 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj
--rw-r--r--   0        0        0      643 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/iiwa_and_wsg.dmd.yaml
--rw-r--r--   0        0        0      943 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/README.md
--rw-r--r--   0        0        0     1126 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/drake_obstacles.dmd.yaml
--rw-r--r--   0        0        0     3138 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/ground.sdf
--rw-r--r--   0        0        0    61205 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/mecanum_base.urdf
--rw-r--r--   0        0        0      673 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/obstacle_boxes.sdf
--rw-r--r--   0        0        0      663 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/obstacles.sdf
--rw-r--r--   0        0        0    19606 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/mobile_iiwa14_primitive_collision.urdf
--rw-r--r--   0        0        0     1645 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/mustard_w_cameras.dmd.yaml
--rw-r--r--   0        0        0      374 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/package.xml
--rw-r--r--   0        0        0     2574 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/planar_bin.sdf
--rw-r--r--   0        0        0     3716 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/planar_foam_brick_collision_as_visual.sdf
--rw-r--r--   0        0        0    12699 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/planar_iiwa14_no_collision.urdf
--rw-r--r--   0        0        0     1185 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/planar_joint.sdf
--rw-r--r--   0        0        0     1114 2024-04-08 12:21:31.612057 manipulation-2024.5.18/manipulation/models/planar_manipulation_station.scenario.yaml
--rw-r--r--   0        0        0   140342 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/pr2_collision_fixed.urdf
--rw-r--r--   0        0        0     1791 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/pr2_shelves.dmd.yaml
--rw-r--r--   0        0        0    49209 2024-03-17 12:35:12.475299 manipulation-2024.5.18/manipulation/models/rubiks_cube.sdf
--rw-r--r--   0        0        0    15864 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/rubiks_cube_2_by_2.sdf
--rw-r--r--   0        0        0      111 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
--rw-r--r--   0        0        0     2963 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers.sdf
--rw-r--r--   0        0        0     2660 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
--rw-r--r--   0        0        0     2299 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/segmentation_and_grasp_scene.dmd.yaml
--rw-r--r--   0        0        0     2784 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/shelves.sdf
--rw-r--r--   0        0        0     2876 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/shelves_w_ellipsoid_collision.sdf
--rw-r--r--   0        0        0     1388 2024-03-27 11:26:12.916327 manipulation-2024.5.18/manipulation/models/simple_2d_cspace.xml
--rw-r--r--   0        0        0      462 2024-03-27 10:57:46.553239 manipulation-2024.5.18/manipulation/models/simple_2d_obstacle.obj
--rw-r--r--   0        0        0      778 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/README.md
--rw-r--r--   0        0        0     4816 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/read_spot_camera_intrinsics.py
--rw-r--r--   0        0        0       21 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/requirements.txt
--rw-r--r--   0        0        0    27982 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/spot_with_arm.urdf
--rw-r--r--   0        0        0     3866 2024-05-21 02:06:24.674757 manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml
--rw-r--r--   0        0        0    30003 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf
--rw-r--r--   0        0        0      390 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/README.md
--rw-r--r--   0        0        0     6386 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/base.obj
--rw-r--r--   0        0        0     6203 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/head.obj
--rw-r--r--   0        0        0    40367 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/mid.obj
--rw-r--r--   0        0        0     1382 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/suction-base.urdf
--rw-r--r--   0        0        0     3060 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/suction-head.urdf
--rw-r--r--   0        0        0    82673 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/tip.obj
--rw-r--r--   0        0        0      642 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/two_bins.dmd.yaml
--rw-r--r--   0        0        0      668 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/two_bins.sdf
--rw-r--r--   0        0        0     1915 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.dmd.yaml
--rw-r--r--   0        0        0     2441 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.sdf
--rw-r--r--   0        0        0    16346 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/two_link_iiwa14.urdf
--rw-r--r--   0        0        0     2148 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/mustard_depth_camera_example.py
--rw-r--r--   0        0        0     4190 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/pick.py
--rw-r--r--   0        0        0    26538 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/scenarios.py
--rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/station.md
--rw-r--r--   0        0        0    51887 2024-05-21 02:06:24.674757 manipulation-2024.5.18/manipulation/station.py
--rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/systems.md
--rw-r--r--   0        0        0     4801 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/systems.py
--rw-r--r--   0        0        0     1547 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_create_sdf_from_mesh.py
--rw-r--r--   0        0        0     2292 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_gym.py
--rw-r--r--   0        0        0      425 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_meshcat_utils.py
--rw-r--r--   0        0        0      561 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_model_directives.py
--rw-r--r--   0        0        0      314 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_utils.py
--rw-r--r--   0        0        0       86 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/utils.md
--rw-r--r--   0        0        0     7226 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/utils.py
--rw-r--r--   0        0        0     3284 2024-05-21 02:06:24.674757 manipulation-2024.5.18/pyproject.toml
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 manipulation-2024.5.18/PKG-INFO
+-rw-r--r--   0        0        0     1561 2024-02-22 14:57:44.046800 manipulation-2024.5.25/LICENSE.TXT
+-rw-r--r--   0        0        0      536 2024-05-21 02:06:24.674757 manipulation-2024.5.25/README.md
+-rw-r--r--   0        0        0      167 2024-02-22 14:57:44.110801 manipulation-2024.5.25/manipulation/__init__.py
+-rw-r--r--   0        0        0      846 2024-02-22 14:57:44.110801 manipulation-2024.5.25/manipulation/_static/custom.css
+-rw-r--r--   0        0        0     6481 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/clutter.py
+-rw-r--r--   0        0        0      891 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/conf.py
+-rw-r--r--   0        0        0    16339 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/create_sdf_from_mesh.py
+-rw-r--r--   0        0        0      211 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/drake_gym.py
+-rw-r--r--   0        0        0     9221 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/envs/box_flipup.py
+-rw-r--r--   0        0        0     8473 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/envs/planar_gripper_pushing_a_box.py
+-rw-r--r--   0        0        0    32464 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/clutter/normal_solution.npy
+-rw-r--r--   0        0        0     1724 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/clutter/test_analytic_grasp.py
+-rw-r--r--   0        0        0     6751 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/clutter/test_grasp_candidate.py
+-rw-r--r--   0        0        0     1768 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/clutter/test_normal.py
+-rw-r--r--   0        0        0     3978 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/clutter/test_simulation_tuning.py
+-rw-r--r--   0        0        0     3598 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/deep_perception/test_contrastive.py
+-rw-r--r--   0        0        0     1563 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/force/test_hybrid.py
+-rw-r--r--   0        0        0     4758 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/grader.py
+-rw-r--r--   0        0        0     3850 2024-05-25 09:53:14.578332 manipulation-2024.5.25/manipulation/exercises/mobile/test_mobile_base_ik.py
+-rw-r--r--   0        0        0     1188 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pick/plot_planar_manipulator.py
+-rw-r--r--   0        0        0    26806 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pick/test_differential_ik.py
+-rw-r--r--   0        0        0     3585 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pick/test_planar_manipulator.py
+-rw-r--r--   0        0        0     2874 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pick/test_rigid_transforms.py
+-rw-r--r--   0        0        0     1881 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pick/test_robot_painter.py
+-rw-r--r--   0        0        0     1139 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pick/test_simple_qp.py
+-rw-r--r--   0        0        0     3642 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pose/test_icp.py
+-rw-r--r--   0        0        0     1445 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pose/test_pose_estimation.py
+-rw-r--r--   0        0        0     3240 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/pose/test_ransac.py
+-rw-r--r--   0        0        0     3380 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/rl/test_stochastic_optimization.py
+-rw-r--r--   0        0        0     2825 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/rl/test_vpg.py
+-rw-r--r--   0        0        0      870 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/robot/test_direct_joint_control.py
+-rw-r--r--   0        0        0     1184 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/robot/test_hardware_station_io.py
+-rw-r--r--   0        0        0     2261 2024-02-22 14:57:44.114801 manipulation-2024.5.25/manipulation/exercises/robot/test_reflected_inertia.py
+-rw-r--r--   0        0        0      672 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/robot/test_survey.py
+-rw-r--r--   0        0        0     1372 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/segmentation/test_mask.py
+-rw-r--r--   0        0        0     2271 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/__init__.py
+-rw-r--r--   0        0        0    23490 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/geometry.py
+-rw-r--r--   0        0        0     3711 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
+-rw-r--r--   0        0        0     6529 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/robot.py
+-rw-r--r--   0        0        0    14614 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
+-rw-r--r--   0        0        0     1464 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/test_door_opening.py
+-rw-r--r--   0        0        0     2391 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/test_rrt_planning.py
+-rw-r--r--   0        0        0     5489 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/exercises/trajectories/test_taskspace_iris.py
+-rw-r--r--   0        0        0     3764 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/icp.py
+-rw-r--r--   0        0        0      243 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/index.md
+-rw-r--r--   0        0        0      256 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/meshcat_cpp_utils.py
+-rw-r--r--   0        0        0      102 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/meshcat_utils.md
+-rw-r--r--   0        0        0    17872 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/meshcat_utils.py
+-rw-r--r--   0        0        0     5938 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
+-rw-r--r--   0        0        0     1656 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/models/book.sdf
+-rw-r--r--   0        0        0     1280 2024-02-22 14:57:44.118801 manipulation-2024.5.25/manipulation/models/bunny/README
+-rw-r--r--   0        0        0   658744 2024-02-22 14:57:44.122801 manipulation-2024.5.25/manipulation/models/bunny/bun_zipper_res2.ply
+-rw-r--r--   0        0        0   196232 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/bunny/bunny.npy
+-rw-r--r--   0        0        0     1496 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/camera_box.sdf
+-rw-r--r--   0        0        0      155 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/clutter.dmd.yaml
+-rw-r--r--   0        0        0     1544 2024-04-08 12:21:31.612057 manipulation-2024.5.25/manipulation/models/clutter.scenarios.yaml
+-rw-r--r--   0        0        0      367 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/clutter_mustard.dmd.yaml
+-rw-r--r--   0        0        0      183 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/clutter_planning.dmd.yaml
+-rw-r--r--   0        0        0      165 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/clutter_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0     1976 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/cupboard.scenario.yaml
+-rw-r--r--   0        0        0     2485 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/double_pendulum.urdf
+-rw-r--r--   0        0        0      215 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/floating_joint.urdf
+-rw-r--r--   0        0        0     1407 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/floor.sdf
+-rw-r--r--   0        0        0     1472 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/hydro/003_cracker_box.sdf
+-rw-r--r--   0        0        0     1470 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/hydro/004_sugar_box.sdf
+-rw-r--r--   0        0        0     1631 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/hydro/005_tomato_soup_can.sdf
+-rw-r--r--   0        0        0     4991 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/hydro/006_mustard_bottle.sdf
+-rw-r--r--   0        0        0     1480 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/hydro/009_gelatin_box.sdf
+-rw-r--r--   0        0        0     1476 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/hydro/010_potted_meat_can.sdf
+-rw-r--r--   0        0        0     1104 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/061_foam_brick.sdf
+-rw-r--r--   0        0        0      246 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/README.md
+-rw-r--r--   0        0        0     4709 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/bin.sdf
+-rw-r--r--   0        0        0     9110 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/cupboard.sdf
+-rw-r--r--   0        0        0     6069 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf
+-rw-r--r--   0        0        0     5711 2024-05-25 09:53:14.578332 manipulation-2024.5.25/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf
+-rw-r--r--   0        0        0    21069 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj
+-rw-r--r--   0        0        0    21659 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj
+-rw-r--r--   0        0        0    23842 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj
+-rw-r--r--   0        0        0    24252 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj
+-rw-r--r--   0        0        0    26183 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj
+-rw-r--r--   0        0        0    15215 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj
+-rw-r--r--   0        0        0    18773 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj
+-rw-r--r--   0        0        0    23818 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj
+-rw-r--r--   0        0        0    24964 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj
+-rw-r--r--   0        0        0      643 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/iiwa_and_wsg.dmd.yaml
+-rw-r--r--   0        0        0      943 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/mecanum/README.md
+-rw-r--r--   0        0        0     1126 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/mecanum/drake_obstacles.dmd.yaml
+-rw-r--r--   0        0        0     3138 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/mecanum/ground.sdf
+-rw-r--r--   0        0        0    61205 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/mecanum/mecanum_base.urdf
+-rw-r--r--   0        0        0      673 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/mecanum/obstacle_boxes.sdf
+-rw-r--r--   0        0        0      663 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/mecanum/obstacles.sdf
+-rw-r--r--   0        0        0    19606 2024-04-22 09:52:20.076913 manipulation-2024.5.25/manipulation/models/mobile_iiwa14_primitive_collision.urdf
+-rw-r--r--   0        0        0     1645 2024-04-22 09:52:20.080913 manipulation-2024.5.25/manipulation/models/mustard_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0      374 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/package.xml
+-rw-r--r--   0        0        0     2574 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/planar_bin.sdf
+-rw-r--r--   0        0        0     3716 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/planar_foam_brick_collision_as_visual.sdf
+-rw-r--r--   0        0        0    12699 2024-04-22 09:52:20.080913 manipulation-2024.5.25/manipulation/models/planar_iiwa14_no_collision.urdf
+-rw-r--r--   0        0        0     1185 2024-02-22 14:57:44.126801 manipulation-2024.5.25/manipulation/models/planar_joint.sdf
+-rw-r--r--   0        0        0     1114 2024-04-08 12:21:31.612057 manipulation-2024.5.25/manipulation/models/planar_manipulation_station.scenario.yaml
+-rw-r--r--   0        0        0     1807 2024-05-25 09:53:14.578332 manipulation-2024.5.25/manipulation/models/pr2_shelves.dmd.yaml
+-rw-r--r--   0        0        0    49209 2024-03-17 12:35:12.475299 manipulation-2024.5.25/manipulation/models/rubiks_cube.sdf
+-rw-r--r--   0        0        0    15864 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/rubiks_cube_2_by_2.sdf
+-rw-r--r--   0        0        0      111 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
+-rw-r--r--   0        0        0     2966 2024-05-25 09:53:14.578332 manipulation-2024.5.25/manipulation/models/schunk_wsg_50_welded_fingers.sdf
+-rw-r--r--   0        0        0     2663 2024-05-25 09:53:14.578332 manipulation-2024.5.25/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
+-rw-r--r--   0        0        0     2299 2024-04-22 09:52:20.080913 manipulation-2024.5.25/manipulation/models/segmentation_and_grasp_scene.dmd.yaml
+-rw-r--r--   0        0        0     2784 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/shelves.sdf
+-rw-r--r--   0        0        0     2876 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/shelves_w_ellipsoid_collision.sdf
+-rw-r--r--   0        0        0     1388 2024-03-27 11:26:12.916327 manipulation-2024.5.25/manipulation/models/simple_2d_cspace.xml
+-rw-r--r--   0        0        0      462 2024-03-27 10:57:46.553239 manipulation-2024.5.25/manipulation/models/simple_2d_obstacle.obj
+-rw-r--r--   0        0        0      778 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/spot/README.md
+-rw-r--r--   0        0        0     4816 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/spot/read_spot_camera_intrinsics.py
+-rw-r--r--   0        0        0       21 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/spot/requirements.txt
+-rw-r--r--   0        0        0    27982 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/spot/spot_with_arm.urdf
+-rw-r--r--   0        0        0     3866 2024-05-21 02:06:24.674757 manipulation-2024.5.25/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml
+-rw-r--r--   0        0        0    30003 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf
+-rw-r--r--   0        0        0      390 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/suction/README.md
+-rw-r--r--   0        0        0     6386 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/suction/base.obj
+-rw-r--r--   0        0        0     6203 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/suction/head.obj
+-rw-r--r--   0        0        0    40367 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/suction/mid.obj
+-rw-r--r--   0        0        0     1382 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/suction/suction-base.urdf
+-rw-r--r--   0        0        0     3060 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/suction/suction-head.urdf
+-rw-r--r--   0        0        0    82673 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/suction/tip.obj
+-rw-r--r--   0        0        0      642 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/two_bins.dmd.yaml
+-rw-r--r--   0        0        0      668 2024-04-22 09:52:20.080913 manipulation-2024.5.25/manipulation/models/two_bins.sdf
+-rw-r--r--   0        0        0     1915 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/models/two_bins_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0     2441 2024-04-22 09:52:20.080913 manipulation-2024.5.25/manipulation/models/two_bins_w_cameras.sdf
+-rw-r--r--   0        0        0    16346 2024-04-22 09:52:20.080913 manipulation-2024.5.25/manipulation/models/two_link_iiwa14.urdf
+-rw-r--r--   0        0        0     2148 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/mustard_depth_camera_example.py
+-rw-r--r--   0        0        0     4190 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/pick.py
+-rw-r--r--   0        0        0    26538 2024-04-22 09:52:20.080913 manipulation-2024.5.25/manipulation/scenarios.py
+-rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/station.md
+-rw-r--r--   0        0        0    51887 2024-05-21 02:06:24.674757 manipulation-2024.5.25/manipulation/station.py
+-rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/systems.md
+-rw-r--r--   0        0        0     4801 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/systems.py
+-rw-r--r--   0        0        0     1547 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/test/test_create_sdf_from_mesh.py
+-rw-r--r--   0        0        0     2292 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/test/test_gym.py
+-rw-r--r--   0        0        0      425 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/test/test_meshcat_utils.py
+-rw-r--r--   0        0        0      561 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/test/test_model_directives.py
+-rw-r--r--   0        0        0      314 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/test/test_utils.py
+-rw-r--r--   0        0        0       86 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/utils.md
+-rw-r--r--   0        0        0     7226 2024-02-22 14:57:44.130802 manipulation-2024.5.25/manipulation/utils.py
+-rw-r--r--   0        0        0     3284 2024-05-25 11:10:34.637052 manipulation-2024.5.25/pyproject.toml
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 manipulation-2024.5.25/PKG-INFO
```

### Comparing `manipulation-2024.5.18/LICENSE.TXT` & `manipulation-2024.5.25/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/README.md` & `manipulation-2024.5.25/README.md`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/_static/custom.css` & `manipulation-2024.5.25/manipulation/_static/custom.css`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/clutter.py` & `manipulation-2024.5.25/manipulation/clutter.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/conf.py` & `manipulation-2024.5.25/manipulation/conf.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/create_sdf_from_mesh.py` & `manipulation-2024.5.25/manipulation/create_sdf_from_mesh.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/envs/box_flipup.py` & `manipulation-2024.5.25/manipulation/envs/box_flipup.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/envs/planar_gripper_pushing_a_box.py` & `manipulation-2024.5.25/manipulation/envs/planar_gripper_pushing_a_box.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/clutter/normal_solution.npy` & `manipulation-2024.5.25/manipulation/exercises/clutter/normal_solution.npy`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/clutter/test_analytic_grasp.py` & `manipulation-2024.5.25/manipulation/exercises/clutter/test_analytic_grasp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/clutter/test_grasp_candidate.py` & `manipulation-2024.5.25/manipulation/exercises/clutter/test_grasp_candidate.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/clutter/test_normal.py` & `manipulation-2024.5.25/manipulation/exercises/clutter/test_normal.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/clutter/test_simulation_tuning.py` & `manipulation-2024.5.25/manipulation/exercises/clutter/test_simulation_tuning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/deep_perception/test_contrastive.py` & `manipulation-2024.5.25/manipulation/exercises/deep_perception/test_contrastive.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/force/test_hybrid.py` & `manipulation-2024.5.25/manipulation/exercises/force/test_hybrid.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/grader.py` & `manipulation-2024.5.25/manipulation/exercises/grader.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/mobile/test_mobile_base_ik.py` & `manipulation-2024.5.25/manipulation/exercises/mobile/test_mobile_base_ik.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             self.assertTrue(q is not None, "IK failed, no configuration returned!")
 
             diagram, plant, scene_graph = self.notebook_locals["build_env"]()
 
             context = diagram.CreateDefaultContext()
             plant_context = plant.GetMyContextFromRoot(context)
             sg_context = scene_graph.GetMyContextFromRoot(context)
-            self.notebook_locals["filterCollsionGeometry"](scene_graph, sg_context)
 
             plant.SetPositions(plant_context, q)
 
             query_object = plant.get_geometry_query_input_port().Eval(plant_context)
             inspector = query_object.inspector()
 
             pairs = (
```

### Comparing `manipulation-2024.5.18/manipulation/exercises/pick/plot_planar_manipulator.py` & `manipulation-2024.5.25/manipulation/exercises/pick/plot_planar_manipulator.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pick/test_differential_ik.py` & `manipulation-2024.5.25/manipulation/exercises/pick/test_differential_ik.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pick/test_planar_manipulator.py` & `manipulation-2024.5.25/manipulation/exercises/pick/test_planar_manipulator.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pick/test_rigid_transforms.py` & `manipulation-2024.5.25/manipulation/exercises/pick/test_rigid_transforms.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pick/test_robot_painter.py` & `manipulation-2024.5.25/manipulation/exercises/pick/test_robot_painter.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pick/test_simple_qp.py` & `manipulation-2024.5.25/manipulation/exercises/pick/test_simple_qp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pose/test_icp.py` & `manipulation-2024.5.25/manipulation/exercises/pose/test_icp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pose/test_pose_estimation.py` & `manipulation-2024.5.25/manipulation/exercises/pose/test_pose_estimation.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/pose/test_ransac.py` & `manipulation-2024.5.25/manipulation/exercises/pose/test_ransac.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/rl/test_stochastic_optimization.py` & `manipulation-2024.5.25/manipulation/exercises/rl/test_stochastic_optimization.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/rl/test_vpg.py` & `manipulation-2024.5.25/manipulation/exercises/rl/test_vpg.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/robot/test_direct_joint_control.py` & `manipulation-2024.5.25/manipulation/exercises/robot/test_direct_joint_control.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/robot/test_hardware_station_io.py` & `manipulation-2024.5.25/manipulation/exercises/robot/test_hardware_station_io.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/robot/test_reflected_inertia.py` & `manipulation-2024.5.25/manipulation/exercises/robot/test_reflected_inertia.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/robot/test_survey.py` & `manipulation-2024.5.25/manipulation/exercises/robot/test_survey.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/segmentation/test_mask.py` & `manipulation-2024.5.25/manipulation/exercises/segmentation/test_mask.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/segmentation/test_segmentation_and_grasp.py` & `manipulation-2024.5.25/manipulation/exercises/segmentation/test_segmentation_and_grasp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/geometry.py` & `manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/geometry.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py` & `manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/robot.py` & `manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/robot.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py` & `manipulation-2024.5.25/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/trajectories/test_door_opening.py` & `manipulation-2024.5.25/manipulation/exercises/trajectories/test_door_opening.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/trajectories/test_rrt_planning.py` & `manipulation-2024.5.25/manipulation/exercises/trajectories/test_rrt_planning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/exercises/trajectories/test_taskspace_iris.py` & `manipulation-2024.5.25/manipulation/exercises/trajectories/test_taskspace_iris.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/icp.py` & `manipulation-2024.5.25/manipulation/icp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/meshcat_utils.py` & `manipulation-2024.5.25/manipulation/meshcat_utils.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf` & `manipulation-2024.5.25/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/book.sdf` & `manipulation-2024.5.25/manipulation/models/book.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/bunny/README` & `manipulation-2024.5.25/manipulation/models/bunny/README`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/bunny/bun_zipper_res2.ply` & `manipulation-2024.5.25/manipulation/models/bunny/bun_zipper_res2.ply`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/bunny/bunny.npy` & `manipulation-2024.5.25/manipulation/models/bunny/bunny.npy`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/camera_box.sdf` & `manipulation-2024.5.25/manipulation/models/camera_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/clutter.scenarios.yaml` & `manipulation-2024.5.25/manipulation/models/clutter.scenarios.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/cupboard.scenario.yaml` & `manipulation-2024.5.25/manipulation/models/cupboard.scenario.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/double_pendulum.urdf` & `manipulation-2024.5.25/manipulation/models/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/floor.sdf` & `manipulation-2024.5.25/manipulation/models/floor.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/003_cracker_box.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/003_cracker_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/004_sugar_box.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/004_sugar_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/005_tomato_soup_can.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/005_tomato_soup_can.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/006_mustard_bottle.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/006_mustard_bottle.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/009_gelatin_box.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/009_gelatin_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/010_potted_meat_can.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/010_potted_meat_can.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/061_foam_brick.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/061_foam_brick.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/bin.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/bin.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/cupboard.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/cupboard.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf` & `manipulation-2024.5.25/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         </inertia>
       </inertial>
       <kinematic>0</kinematic>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/wsg_body.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/wsg_body.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.7 0.7 0.7 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
@@ -56,15 +56,15 @@
         </inertia>
       </inertial>
       <kinematic>0</kinematic>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/finger_with_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_with_tip.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
       <collision name="left_tip">
@@ -107,15 +107,15 @@
         </inertia>
       </inertial>
       <kinematic>0</kinematic>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/finger_with_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_with_tip.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
       <collision name="right_tip">
```

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj` & `manipulation-2024.5.25/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/iiwa_and_wsg.dmd.yaml` & `manipulation-2024.5.25/manipulation/models/iiwa_and_wsg.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mecanum/README.md` & `manipulation-2024.5.25/manipulation/models/mecanum/README.md`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mecanum/drake_obstacles.dmd.yaml` & `manipulation-2024.5.25/manipulation/models/mecanum/drake_obstacles.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mecanum/ground.sdf` & `manipulation-2024.5.25/manipulation/models/mecanum/ground.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mecanum/mecanum_base.urdf` & `manipulation-2024.5.25/manipulation/models/mecanum/mecanum_base.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mecanum/obstacle_boxes.sdf` & `manipulation-2024.5.25/manipulation/models/mecanum/obstacle_boxes.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mecanum/obstacles.sdf` & `manipulation-2024.5.25/manipulation/models/mecanum/obstacles.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mobile_iiwa14_primitive_collision.urdf` & `manipulation-2024.5.25/manipulation/models/mobile_iiwa14_primitive_collision.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/mustard_w_cameras.dmd.yaml` & `manipulation-2024.5.25/manipulation/models/mustard_w_cameras.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/planar_bin.sdf` & `manipulation-2024.5.25/manipulation/models/planar_bin.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/planar_foam_brick_collision_as_visual.sdf` & `manipulation-2024.5.25/manipulation/models/planar_foam_brick_collision_as_visual.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/planar_iiwa14_no_collision.urdf` & `manipulation-2024.5.25/manipulation/models/planar_iiwa14_no_collision.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/planar_joint.sdf` & `manipulation-2024.5.25/manipulation/models/planar_joint.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/planar_manipulation_station.scenario.yaml` & `manipulation-2024.5.25/manipulation/models/planar_manipulation_station.scenario.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/pr2_shelves.dmd.yaml` & `manipulation-2024.5.25/manipulation/models/pr2_shelves.dmd.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Model directive for iiwa with sphere collision and welded gripper
 directives:
 
 # Add iiwa
 - add_model:
     name: pr2
-    file: package://manipulation/pr2_collision_fixed.urdf
+    file: package://drake_models/pr2_description/urdf/pr2_simplified.urdf
 
 # Add shelves
 - add_model:
     name: shelves_1
     file: package://drake_models/manipulation_station/shelves.sdf
 
 - add_frame:
```

### Comparing `manipulation-2024.5.18/manipulation/models/rubiks_cube.sdf` & `manipulation-2024.5.25/manipulation/models/rubiks_cube.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/rubiks_cube_2_by_2.sdf` & `manipulation-2024.5.25/manipulation/models/rubiks_cube_2_by_2.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers.sdf` & `manipulation-2024.5.25/manipulation/models/schunk_wsg_50_welded_fingers.sdf`

 * *Files 9% similar despite different names*

#### Comparing `manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers.sdf` & `manipulation-2024.5.25/manipulation/models/schunk_wsg_50_welded_fingers.sdf`

```diff
@@ -15,15 +15,15 @@
           <izz>0.164814</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/wsg_body.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/wsg_body.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.7 0.7 0.7 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
@@ -50,15 +50,15 @@
           <izz>0.16</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
@@ -82,15 +82,15 @@
           <izz>0.16</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
```

### Comparing `manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf` & `manipulation-2024.5.25/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf`

 * *Files 2% similar despite different names*

#### Comparing `manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf` & `manipulation-2024.5.25/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf`

```diff
@@ -15,15 +15,15 @@
           <izz>0.164814</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/wsg_body.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/wsg_body.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.7 0.7 0.7 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
@@ -51,15 +51,15 @@
           <izz>0.16</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
     </link>
@@ -76,15 +76,15 @@
           <izz>0.16</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.gltf</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
     </link>
```

### Comparing `manipulation-2024.5.18/manipulation/models/segmentation_and_grasp_scene.dmd.yaml` & `manipulation-2024.5.25/manipulation/models/segmentation_and_grasp_scene.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/shelves.sdf` & `manipulation-2024.5.25/manipulation/models/shelves.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/shelves_w_ellipsoid_collision.sdf` & `manipulation-2024.5.25/manipulation/models/shelves_w_ellipsoid_collision.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/simple_2d_cspace.xml` & `manipulation-2024.5.25/manipulation/models/simple_2d_cspace.xml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/spot/README.md` & `manipulation-2024.5.25/manipulation/models/spot/README.md`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/spot/read_spot_camera_intrinsics.py` & `manipulation-2024.5.25/manipulation/models/spot/read_spot_camera_intrinsics.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/spot/spot_with_arm.urdf` & `manipulation-2024.5.25/manipulation/models/spot/spot_with_arm.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml` & `manipulation-2024.5.25/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf` & `manipulation-2024.5.25/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/suction/base.obj` & `manipulation-2024.5.25/manipulation/models/suction/base.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/suction/head.obj` & `manipulation-2024.5.25/manipulation/models/suction/head.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/suction/mid.obj` & `manipulation-2024.5.25/manipulation/models/suction/mid.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/suction/suction-base.urdf` & `manipulation-2024.5.25/manipulation/models/suction/suction-base.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/suction/suction-head.urdf` & `manipulation-2024.5.25/manipulation/models/suction/suction-head.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/suction/tip.obj` & `manipulation-2024.5.25/manipulation/models/suction/tip.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/two_bins.dmd.yaml` & `manipulation-2024.5.25/manipulation/models/two_bins.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/two_bins.sdf` & `manipulation-2024.5.25/manipulation/models/two_bins.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.dmd.yaml` & `manipulation-2024.5.25/manipulation/models/two_bins_w_cameras.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.sdf` & `manipulation-2024.5.25/manipulation/models/two_bins_w_cameras.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/models/two_link_iiwa14.urdf` & `manipulation-2024.5.25/manipulation/models/two_link_iiwa14.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/mustard_depth_camera_example.py` & `manipulation-2024.5.25/manipulation/mustard_depth_camera_example.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/pick.py` & `manipulation-2024.5.25/manipulation/pick.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/scenarios.py` & `manipulation-2024.5.25/manipulation/scenarios.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/station.py` & `manipulation-2024.5.25/manipulation/station.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/systems.py` & `manipulation-2024.5.25/manipulation/systems.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/test/test_create_sdf_from_mesh.py` & `manipulation-2024.5.25/manipulation/test/test_create_sdf_from_mesh.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/test/test_gym.py` & `manipulation-2024.5.25/manipulation/test/test_gym.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/test/test_model_directives.py` & `manipulation-2024.5.25/manipulation/test/test_model_directives.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/manipulation/utils.py` & `manipulation-2024.5.25/manipulation/utils.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.5.18/pyproject.toml` & `manipulation-2024.5.25/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "manipulation"
 # Use e.g. 2023.10.4.rc0 if I need to release a release candidate.
 # Use e.g. 2023.10.4.post1 if I need to rerelease on the same day.
-version = "2024.05.18"
+version = "2024.05.25"
 description = "MIT 6.421 - Robotic Manipulation"
 authors = ["Russ Tedrake <russt@mit.edu>"]
 license = "BSD License"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License"
@@ -42,16 +42,16 @@
 name = "drake-nightly"
 url = "https://drake-packages.csail.mit.edu/whl/nightly/"
 priority = "explicit"
 
 [tool.poetry.dependencies]
 python = "<4.0,>=3.10"
 cloudpickle = "2.2.1"  # needs to be pinned for stored files to remain compatible.
-#drake = { version = "==0.0.20240302", source = "drake-nightly" }
-drake = ">=1.28.0"
+#drake = { version = ">=0.0.20240524", source = "drake-nightly" }
+drake = ">=1.29.0"
 gradescope-utils = ">=0.4.0"
 mpld3  = ">=0.5.6"
 nevergrad = ">=0.4.3"  # TODO: avoid expensive bayesian optimization dep
 psutil = ">=5.9.*"
 #pymcubes = ">=0.0.9"
 pyzmq = ">=25.0.0" # seems to be needed on python 3.11
 scipy = ">=1.10.0"  # From github dependabot
@@ -64,16 +64,16 @@
 #wandb = ">=0.14.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 # Must include all dependencies required to build the docs with sphinx + autodoc.
 [tool.poetry.group.docs.dependencies]
-#drake = { version = ">=0.0.20240302", source = "drake-nightly" }
-drake = ">=1.28.0"
+#drake = { version = ">=0.0.20240524", source = "drake-nightly" }
+drake = ">=1.29.0"
 ipython = ">=7.8.0"
 sphinx = ">=7.2.6"
 myst-parser = ">=2.0.0"
 sphinx_rtd_theme = ">=2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 beautifulsoup4 = ">=4.6.3"
```

### Comparing `manipulation-2024.5.18/PKG-INFO` & `manipulation-2024.5.25/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: manipulation
-Version: 2024.5.18
+Version: 2024.5.25
 Summary: MIT 6.421 - Robotic Manipulation
 License: BSD License
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cloudpickle (==2.2.1)
-Requires-Dist: drake (>=1.28.0)
+Requires-Dist: drake (>=1.29.0)
 Requires-Dist: gradescope-utils (>=0.4.0)
 Requires-Dist: mpld3 (>=0.5.6)
 Requires-Dist: nevergrad (>=0.4.3)
 Requires-Dist: psutil (>=5.9)
 Requires-Dist: pyzmq (>=25.0.0)
 Requires-Dist: scipy (>=1.10.0)
 Requires-Dist: stable-baselines3 (>=2.0.0)
```

