# Comparing `tmp/domainlab-0.1.2.tar.gz` & `tmp/domainlab-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domainlab-0.1.2.tar", max compression
+gzip compressed data, was "domainlab-0.1.3.tar", max compression
```

## Comparing `domainlab-0.1.2.tar` & `domainlab-0.1.3.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0     1067 2023-03-26 11:30:13.727342 domainlab-0.1.2/LICENSE
--rw-r--r--   0        0        0       27 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/.gitignore
--rw-r--r--   0        0        0      178 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/.pylintrc
--rw-r--r--   0        0        0      730 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/__init__.py
--rw-r--r--   0        0        0        0 2023-02-12 17:14:36.932061 domainlab-0.1.2/domainlab/algos/__init__.py
--rw-r--r--   0        0        0     1139 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/a_algo_builder.py
--rw-r--r--   0        0        0     4689 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_custom.py
--rw-r--r--   0        0        0     2955 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_dann.py
--rw-r--r--   0        0        0     1612 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_deepall.py
--rw-r--r--   0        0        0     1547 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_deepall_mldg.py
--rw-r--r--   0        0        0     1633 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_dial.py
--rw-r--r--   0        0        0     2304 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_diva.py
--rw-r--r--   0        0        0     2095 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_hduva.py
--rw-r--r--   0        0        0     3275 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_jigen1.py
--rw-r--r--   0        0        0     3212 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_match_hduva.py
--rw-r--r--   0        0        0     2814 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/algos/builder_matchdg.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/compos/__init__.py
--rw-r--r--   0        0        0      621 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_args.py
--rw-r--r--   0        0        0     3905 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_base.py
--rw-r--r--   0        0        0    12409 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_ctr_erm.py
--rw-r--r--   0        0        0    16853 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/compos/matchdg_match.py
--rw-r--r--   0        0        0     3961 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/compos/matchdg_utils.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/msels/__init__.py
--rw-r--r--   0        0        0      602 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/msels/a_model_sel.py
--rw-r--r--   0        0        0     1092 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/msels/c_msel.py
--rw-r--r--   0        0        0     1233 2023-01-29 12:41:05.994218 domainlab-0.1.2/domainlab/algos/msels/c_msel_oracle.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/observers/__init__.py
--rw-r--r--   0        0        0      647 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/observers/a_observer.py
--rw-r--r--   0        0        0     4562 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/observers/b_obvisitor.py
--rw-r--r--   0        0        0      501 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/algos/observers/c_obvisitor_cleanup.py
--rw-r--r--   0        0        0     1186 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/observers/c_obvisitor_gen.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/algos/trainers/__init__.py
--rw-r--r--   0        0        0     3286 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/a_trainer.py
--rw-r--r--   0        0        0      782 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/algos/trainers/args_dial.py
--rw-r--r--   0        0        0     1775 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/train_basic.py
--rw-r--r--   0        0        0     2833 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/algos/trainers/train_dial.py
--rw-r--r--   0        0        0     1741 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/train_matchdg.py
--rw-r--r--   0        0        0     3661 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/algos/trainers/train_mldg.py
--rw-r--r--   0        0        0     3302 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/algos/trainers/train_visitor.py
--rw-r--r--   0        0        0     1608 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/algos/trainers/zoo_trainer.py
--rw-r--r--   0        0        0     1945 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/algos/zoo_algos.py
--rw-r--r--   0        0        0     9237 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/arg_parser.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/__init__.py
--rw-r--r--   0        0        0     1474 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/a_nn_builder.py
--rw-r--r--   0        0        0     1485 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/builder_nn_alex.py
--rw-r--r--   0        0        0     1582 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/builder_nn_conv_bn_relu_2.py
--rw-r--r--   0        0        0     1505 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/builder_nn_external_from_file.py
--rw-r--r--   0        0        0      750 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/exp/exp_cuda_seed.py
--rwxr-xr-x   0        0        0     2396 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/compos/exp/exp_main.py
--rw-r--r--   0        0        0     8124 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/compos/exp/exp_utils.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/__init__.py
--rw-r--r--   0        0        0      853 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_adversarial.py
--rw-r--r--   0        0        0      739 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_classif.py
--rw-r--r--   0        0        0     2799 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py
--rw-r--r--   0        0        0     1888 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/net_gated.py
--rw-r--r--   0        0        0     1061 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/nn.py
--rw-r--r--   0        0        0     2743 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/nn_alex.py
--rw-r--r--   0        0        0      764 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/nn_zoo/nn_torchvision.py
--rw-r--r--   0        0        0     4637 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/pcr/p_chain_handler.py
--rw-r--r--   0        0        0      794 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/pcr/request.py
--rw-r--r--   0        0        0      617 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/utils_conv_get_flat_dim.py
--rw-r--r--   0        0        0      799 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/a_model_builder.py
--rw-r--r--   0        0        0     1326 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/a_vae_builder.py
--rw-r--r--   0        0        0     1886 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/c_vae_adaptor_model_recon.py
--rw-r--r--   0        0        0     1343 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/c_vae_builder_classif.py
--rw-r--r--   0        0        0     3441 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/c_vae_recon.py
--rw-r--r--   0        0        0     2195 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py
--rw-r--r--   0        0        0     2244 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py
--rw-r--r--   0        0        0     1484 2023-01-23 10:37:17.607822 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_cond_prior.py
--rw-r--r--   0        0        0     1598 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/compos/vae/compos/decoder_losses.py
--rw-r--r--   0        0        0     3398 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder.py
--rw-r--r--   0        0        0      671 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_dirichlet.py
--rw-r--r--   0        0        0     1917 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic.py
--rw-r--r--   0        0        0     2111 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py
--rw-r--r--   0        0        0     2279 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py
--rw-r--r--   0        0        0     5204 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xyd_parallel.py
--rw-r--r--   0        0        0     5016 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xydt_elevator.py
--rw-r--r--   0        0        0     1891 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/compos/encoder_zy.py
--rw-r--r--   0        0        0     1207 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/utils_request_chain_builder.py
--rw-r--r--   0        0        0     3203 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif.py
--rw-r--r--   0        0        0     1562 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif_topic.py
--rw-r--r--   0        0        0     1581 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/compos/zoo_nn.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/__init__.py
--rw-r--r--   0        0        0     6116 2023-02-05 10:55:35.735388 domainlab-0.1.2/domainlab/dsets/a_dset_mnist_color_rgb_solo.py
--rw-r--r--   0        0        0     1314 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/dset_img_path_list.py
--rw-r--r--   0        0        0      843 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/dset_mnist_color_solo_default.py
--rw-r--r--   0        0        0     1487 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/dset_poly_domains_mnist_color_default.py
--rw-r--r--   0        0        0     5759 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/dsets/dset_subfolder.py
--rw-r--r--   0        0        0      449 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/dsets/utils_color_palette.py
--rw-r--r--   0        0        0     2278 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/dsets/utils_data.py
--rw-r--r--   0        0        0     5958 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/dsets/utils_wrapdset_patches.py
--rw-r--r--   0        0        0        0 2023-02-24 09:24:49.305369 domainlab-0.1.2/domainlab/exp_protocol/__init__.py
--rw-r--r--   0        0        0     1711 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/exp_protocol/aggregate_results.py
--rw-r--r--   0        0        0     5731 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/exp_protocol/benchmark.smk
--rw-r--r--   0        0        0     4511 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/exp_protocol/run_experiment.py
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/models/__init__.py
--rw-r--r--   0        0        0     1108 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/a_model.py
--rw-r--r--   0        0        0     7623 2023-03-26 11:36:12.379054 domainlab-0.1.2/domainlab/models/a_model_classif.py
--rw-r--r--   0        0        0      855 2023-03-26 11:30:13.751344 domainlab-0.1.2/domainlab/models/args_jigen.py
--rw-r--r--   0        0        0     2482 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/models/args_vae.py
--rw-r--r--   0        0        0     1402 2023-04-04 08:28:24.062639 domainlab-0.1.2/domainlab/models/interface_vae_xyd.py
--rw-r--r--   0        0        0     1458 2023-02-23 11:55:38.957077 domainlab-0.1.2/domainlab/models/model_custom.py
--rw-r--r--   0        0        0     1951 2023-02-23 11:55:38.961078 domainlab-0.1.2/domainlab/models/model_dann.py
--rw-r--r--   0        0        0     1209 2023-02-23 11:55:38.961078 domainlab-0.1.2/domainlab/models/model_deep_all.py
--rw-r--r--   0        0        0     3543 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/models/model_diva.py
--rw-r--r--   0        0        0     4870 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/model_hduva.py
--rw-r--r--   0        0        0     2335 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/models/model_jigen.py
--rw-r--r--   0        0        0     1082 2023-04-04 08:28:24.062639 domainlab-0.1.2/domainlab/models/model_vae_xyd_classif.py
--rw-r--r--   0        0        0      714 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/model_wrapper_matchdg4net.py
--rw-r--r--   0        0        0      752 2023-04-04 10:43:25.421862 domainlab-0.1.2/domainlab/models/model_wrapper_matchdg4vae.py
--rw-r--r--   0        0        0     1508 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/models/wrapper_matchdg.py
--rw-r--r--   0        0        0       58 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/tasks/__init__.py
--rw-r--r--   0        0        0     4879 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/tasks/a_task.py
--rw-r--r--   0        0        0     1453 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/a_task_classif.py
--rw-r--r--   0        0        0     2982 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/b_task.py
--rw-r--r--   0        0        0     1474 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/b_task_classif.py
--rw-r--r--   0        0        0     1826 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/tasks/task_dset.py
--rw-r--r--   0        0        0     4057 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_folder.py
--rw-r--r--   0        0        0     2748 2023-01-26 17:13:55.056713 domainlab-0.1.2/domainlab/tasks/task_folder_mk.py
--rw-r--r--   0        0        0     2349 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_mnist_color.py
--rw-r--r--   0        0        0     5085 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_pathlist.py
--rw-r--r--   0        0        0      897 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/task_utils.py
--rw-r--r--   0        0        0     8773 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/utils_task.py
--rw-r--r--   0        0        0     1828 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/tasks/utils_task_dset.py
--rw-r--r--   0        0        0     3733 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/tasks/zoo_tasks.py
--rw-r--r--   0        0        0     3060 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/uml/libDG.uml
--rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/__init__.py
--rw-r--r--   0        0        0     4713 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/flows_gen_img_model.py
--rw-r--r--   0        0        0    20727 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/utils/generate_benchmark_plots.py
--rw-r--r--   0        0        0     1057 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/get_git_tag.py
--rw-r--r--   0        0        0     9420 2023-05-08 09:57:19.628046 domainlab-0.1.2/domainlab/utils/hyperparameter_sampling.py
--rw-r--r--   0        0        0      801 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/override_interface.py
--rw-r--r--   0        0        0     2168 2023-03-26 11:30:13.755344 domainlab-0.1.2/domainlab/utils/perf.py
--rw-r--r--   0        0        0     3847 2023-03-26 11:36:42.932263 domainlab-0.1.2/domainlab/utils/perf_metrics.py
--rw-r--r--   0        0        0     3131 2023-05-08 09:56:58.704046 domainlab-0.1.2/domainlab/utils/sanity_check.py
--rw-r--r--   0        0        0      899 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/test_img.py
--rw-r--r--   0        0        0      336 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/u_import.py
--rw-r--r--   0        0        0     1949 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/u_import_net_module.py
--rw-r--r--   0        0        0      901 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/utils_class.py
--rw-r--r--   0        0        0     1303 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/utils_classif.py
--rw-r--r--   0        0        0      446 2023-05-08 09:57:19.632046 domainlab-0.1.2/domainlab/utils/utils_cuda.py
--rw-r--r--   0        0        0     1098 2023-01-23 10:37:17.611822 domainlab-0.1.2/domainlab/utils/utils_img_sav.py
--rw-r--r--   0        0        0      695 2023-05-08 10:14:38.024078 domainlab-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 domainlab-0.1.2/setup.py
--rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 domainlab-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-03-26 11:30:13.727342 domainlab-0.1.3/LICENSE
+-rw-r--r--   0        0        0       27 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/.gitignore
+-rw-r--r--   0        0        0      178 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/.pylintrc
+-rw-r--r--   0        0        0      372 2023-06-15 08:02:10.360084 domainlab-0.1.3/domainlab/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-12 17:14:36.932061 domainlab-0.1.3/domainlab/algos/__init__.py
+-rw-r--r--   0        0        0     1139 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/algos/a_algo_builder.py
+-rw-r--r--   0        0        0     4689 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_custom.py
+-rw-r--r--   0        0        0     2979 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_dann.py
+-rw-r--r--   0        0        0     1612 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_deepall.py
+-rw-r--r--   0        0        0     1547 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_deepall_mldg.py
+-rw-r--r--   0        0        0     1633 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_dial.py
+-rw-r--r--   0        0        0     2304 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_diva.py
+-rw-r--r--   0        0        0     2087 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_hduva.py
+-rw-r--r--   0        0        0     3299 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_jigen1.py
+-rw-r--r--   0        0        0     3212 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_match_hduva.py
+-rw-r--r--   0        0        0     2814 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/builder_matchdg.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/algos/compos/__init__.py
+-rw-r--r--   0        0        0      621 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/algos/compos/matchdg_args.py
+-rw-r--r--   0        0        0     3905 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/algos/compos/matchdg_base.py
+-rw-r--r--   0        0        0    12409 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/algos/compos/matchdg_ctr_erm.py
+-rw-r--r--   0        0        0    16853 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/algos/compos/matchdg_match.py
+-rw-r--r--   0        0        0     3961 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/algos/compos/matchdg_utils.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/algos/msels/__init__.py
+-rw-r--r--   0        0        0      787 2023-06-15 08:02:10.364084 domainlab-0.1.3/domainlab/algos/msels/a_model_sel.py
+-rw-r--r--   0        0        0     1092 2023-06-12 14:17:55.228036 domainlab-0.1.3/domainlab/algos/msels/c_msel.py
+-rw-r--r--   0        0        0     1244 2023-06-15 08:02:10.364084 domainlab-0.1.3/domainlab/algos/msels/c_msel_oracle.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/algos/observers/__init__.py
+-rw-r--r--   0        0        0      647 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/algos/observers/a_observer.py
+-rw-r--r--   0        0        0     4844 2023-06-15 12:46:32.736605 domainlab-0.1.3/domainlab/algos/observers/b_obvisitor.py
+-rw-r--r--   0        0        0      501 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/algos/observers/c_obvisitor_cleanup.py
+-rw-r--r--   0        0        0     1186 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/algos/observers/c_obvisitor_gen.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/algos/trainers/__init__.py
+-rw-r--r--   0        0        0     3286 2023-06-07 14:57:05.214196 domainlab-0.1.3/domainlab/algos/trainers/a_trainer.py
+-rw-r--r--   0        0        0      782 2023-02-23 11:55:38.957077 domainlab-0.1.3/domainlab/algos/trainers/args_dial.py
+-rw-r--r--   0        0        0     1775 2023-06-15 12:46:32.744604 domainlab-0.1.3/domainlab/algos/trainers/train_basic.py
+-rw-r--r--   0        0        0     2597 2023-06-15 08:02:10.364084 domainlab-0.1.3/domainlab/algos/trainers/train_dial.py
+-rw-r--r--   0        0        0     1741 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/algos/trainers/train_matchdg.py
+-rw-r--r--   0        0        0     3661 2023-06-09 15:11:19.592532 domainlab-0.1.3/domainlab/algos/trainers/train_mldg.py
+-rw-r--r--   0        0        0     3455 2023-06-15 08:02:10.364084 domainlab-0.1.3/domainlab/algos/trainers/train_visitor.py
+-rw-r--r--   0        0        0     1608 2023-04-04 10:43:25.421862 domainlab-0.1.3/domainlab/algos/trainers/zoo_trainer.py
+-rw-r--r--   0        0        0     1945 2023-04-04 10:43:25.421862 domainlab-0.1.3/domainlab/algos/zoo_algos.py
+-rw-r--r--   0        0        0     9237 2023-05-08 09:57:19.628046 domainlab-0.1.3/domainlab/arg_parser.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/__init__.py
+-rw-r--r--   0        0        0     1474 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/a_nn_builder.py
+-rw-r--r--   0        0        0     1485 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/builder_nn_alex.py
+-rw-r--r--   0        0        0     1582 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/builder_nn_conv_bn_relu_2.py
+-rw-r--r--   0        0        0     1505 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/builder_nn_external_from_file.py
+-rw-r--r--   0        0        0      750 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/exp/exp_cuda_seed.py
+-rwxr-xr-x   0        0        0     2396 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/compos/exp/exp_main.py
+-rw-r--r--   0        0        0     8124 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/compos/exp/exp_utils.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/__init__.py
+-rw-r--r--   0        0        0      853 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/net_adversarial.py
+-rw-r--r--   0        0        0      739 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/net_classif.py
+-rw-r--r--   0        0        0     2799 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py
+-rw-r--r--   0        0        0     1888 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/net_gated.py
+-rw-r--r--   0        0        0     1061 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/nn.py
+-rw-r--r--   0        0        0     2743 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/nn_alex.py
+-rw-r--r--   0        0        0      764 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/nn_zoo/nn_torchvision.py
+-rw-r--r--   0        0        0     4637 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/pcr/p_chain_handler.py
+-rw-r--r--   0        0        0      794 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/pcr/request.py
+-rw-r--r--   0        0        0      617 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/utils_conv_get_flat_dim.py
+-rw-r--r--   0        0        0      799 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/a_model_builder.py
+-rw-r--r--   0        0        0     1326 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/a_vae_builder.py
+-rw-r--r--   0        0        0     1886 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/c_vae_adaptor_model_recon.py
+-rw-r--r--   0        0        0     1343 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/c_vae_builder_classif.py
+-rw-r--r--   0        0        0     3441 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/c_vae_recon.py
+-rw-r--r--   0        0        0     2195 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py
+-rw-r--r--   0        0        0     2244 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py
+-rw-r--r--   0        0        0     1484 2023-01-23 10:37:17.607822 domainlab-0.1.3/domainlab/compos/vae/compos/decoder_cond_prior.py
+-rw-r--r--   0        0        0     1598 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/compos/vae/compos/decoder_losses.py
+-rw-r--r--   0        0        0     3398 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder.py
+-rw-r--r--   0        0        0      671 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder_dirichlet.py
+-rw-r--r--   0        0        0     1917 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder_domain_topic.py
+-rw-r--r--   0        0        0     2111 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py
+-rw-r--r--   0        0        0     2279 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py
+-rw-r--r--   0        0        0     5204 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder_xyd_parallel.py
+-rw-r--r--   0        0        0     5016 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder_xydt_elevator.py
+-rw-r--r--   0        0        0     1891 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/compos/encoder_zy.py
+-rw-r--r--   0        0        0     1207 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/utils_request_chain_builder.py
+-rw-r--r--   0        0        0     3203 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/zoo_vae_builders_classif.py
+-rw-r--r--   0        0        0     1562 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/compos/vae/zoo_vae_builders_classif_topic.py
+-rw-r--r--   0        0        0     1581 2023-04-04 10:43:25.421862 domainlab-0.1.3/domainlab/compos/zoo_nn.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/dsets/__init__.py
+-rw-r--r--   0        0        0     6116 2023-02-05 10:55:35.735388 domainlab-0.1.3/domainlab/dsets/a_dset_mnist_color_rgb_solo.py
+-rw-r--r--   0        0        0     1314 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/dsets/dset_img_path_list.py
+-rw-r--r--   0        0        0      843 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/dsets/dset_mnist_color_solo_default.py
+-rw-r--r--   0        0        0     1487 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/dsets/dset_poly_domains_mnist_color_default.py
+-rw-r--r--   0        0        0     5759 2023-02-23 11:55:38.957077 domainlab-0.1.3/domainlab/dsets/dset_subfolder.py
+-rw-r--r--   0        0        0      449 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/dsets/utils_color_palette.py
+-rw-r--r--   0        0        0     2278 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/dsets/utils_data.py
+-rw-r--r--   0        0        0     5958 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/dsets/utils_wrapdset_patches.py
+-rw-r--r--   0        0        0        0 2023-02-24 09:24:49.305369 domainlab-0.1.3/domainlab/exp_protocol/__init__.py
+-rw-r--r--   0        0        0     1711 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/exp_protocol/aggregate_results.py
+-rw-r--r--   0        0        0     5731 2023-05-08 09:57:19.628046 domainlab-0.1.3/domainlab/exp_protocol/benchmark.smk
+-rw-r--r--   0        0        0     4511 2023-05-31 11:59:04.132023 domainlab-0.1.3/domainlab/exp_protocol/run_experiment.py
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/models/__init__.py
+-rw-r--r--   0        0        0     1108 2023-04-04 10:43:25.421862 domainlab-0.1.3/domainlab/models/a_model.py
+-rw-r--r--   0        0        0     7709 2023-06-15 12:46:32.744604 domainlab-0.1.3/domainlab/models/a_model_classif.py
+-rw-r--r--   0        0        0      855 2023-03-26 11:30:13.751344 domainlab-0.1.3/domainlab/models/args_jigen.py
+-rw-r--r--   0        0        0     2482 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/models/args_vae.py
+-rw-r--r--   0        0        0     1402 2023-04-04 08:28:24.062639 domainlab-0.1.3/domainlab/models/interface_vae_xyd.py
+-rw-r--r--   0        0        0     1458 2023-02-23 11:55:38.957077 domainlab-0.1.3/domainlab/models/model_custom.py
+-rw-r--r--   0        0        0     2194 2023-06-15 08:02:10.368084 domainlab-0.1.3/domainlab/models/model_dann.py
+-rw-r--r--   0        0        0     1209 2023-02-23 11:55:38.961078 domainlab-0.1.3/domainlab/models/model_deep_all.py
+-rw-r--r--   0        0        0     3543 2023-06-09 15:14:49.856538 domainlab-0.1.3/domainlab/models/model_diva.py
+-rw-r--r--   0        0        0     5180 2023-06-15 08:02:10.368084 domainlab-0.1.3/domainlab/models/model_hduva.py
+-rw-r--r--   0        0        0     2335 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/models/model_jigen.py
+-rw-r--r--   0        0        0     1227 2023-06-15 08:02:10.368084 domainlab-0.1.3/domainlab/models/model_vae_xyd_classif.py
+-rw-r--r--   0        0        0      714 2023-04-04 10:43:25.421862 domainlab-0.1.3/domainlab/models/model_wrapper_matchdg4net.py
+-rw-r--r--   0        0        0      752 2023-04-04 10:43:25.421862 domainlab-0.1.3/domainlab/models/model_wrapper_matchdg4vae.py
+-rw-r--r--   0        0        0     1508 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/models/wrapper_matchdg.py
+-rw-r--r--   0        0        0       58 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/tasks/__init__.py
+-rw-r--r--   0        0        0     4879 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/tasks/a_task.py
+-rw-r--r--   0        0        0     1453 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/a_task_classif.py
+-rw-r--r--   0        0        0     2982 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/b_task.py
+-rw-r--r--   0        0        0     1474 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/b_task_classif.py
+-rw-r--r--   0        0        0     1826 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/tasks/task_dset.py
+-rw-r--r--   0        0        0     4057 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/task_folder.py
+-rw-r--r--   0        0        0     2748 2023-01-26 17:13:55.056713 domainlab-0.1.3/domainlab/tasks/task_folder_mk.py
+-rw-r--r--   0        0        0     2349 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/task_mnist_color.py
+-rw-r--r--   0        0        0     5085 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/task_pathlist.py
+-rw-r--r--   0        0        0      897 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/task_utils.py
+-rw-r--r--   0        0        0     8773 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/utils_task.py
+-rw-r--r--   0        0        0     1828 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/tasks/utils_task_dset.py
+-rw-r--r--   0        0        0     3733 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/tasks/zoo_tasks.py
+-rw-r--r--   0        0        0     3060 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/uml/libDG.uml
+-rw-r--r--   0        0        0        0 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/__init__.py
+-rw-r--r--   0        0        0     4713 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/flows_gen_img_model.py
+-rw-r--r--   0        0        0    20727 2023-05-08 09:57:19.628046 domainlab-0.1.3/domainlab/utils/generate_benchmark_plots.py
+-rw-r--r--   0        0        0     1057 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/get_git_tag.py
+-rw-r--r--   0        0        0     9420 2023-05-08 09:57:19.628046 domainlab-0.1.3/domainlab/utils/hyperparameter_sampling.py
+-rw-r--r--   0        0        0      801 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/override_interface.py
+-rw-r--r--   0        0        0     2168 2023-03-26 11:30:13.755344 domainlab-0.1.3/domainlab/utils/perf.py
+-rw-r--r--   0        0        0     3847 2023-03-26 11:36:42.932263 domainlab-0.1.3/domainlab/utils/perf_metrics.py
+-rw-r--r--   0        0        0     3131 2023-05-08 09:56:58.704046 domainlab-0.1.3/domainlab/utils/sanity_check.py
+-rw-r--r--   0        0        0      899 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/test_img.py
+-rw-r--r--   0        0        0      336 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/u_import.py
+-rw-r--r--   0        0        0     1949 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/u_import_net_module.py
+-rw-r--r--   0        0        0      901 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/utils_class.py
+-rw-r--r--   0        0        0     1303 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/utils_classif.py
+-rw-r--r--   0        0        0      446 2023-05-08 09:57:19.632046 domainlab-0.1.3/domainlab/utils/utils_cuda.py
+-rw-r--r--   0        0        0     1098 2023-01-23 10:37:17.611822 domainlab-0.1.3/domainlab/utils/utils_img_sav.py
+-rw-r--r--   0        0        0      695 2023-06-15 13:04:40.052638 domainlab-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 domainlab-0.1.3/setup.py
+-rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 domainlab-0.1.3/PKG-INFO
```

### Comparing `domainlab-0.1.2/LICENSE` & `domainlab-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/a_algo_builder.py` & `domainlab-0.1.3/domainlab/algos/a_algo_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/builder_custom.py` & `domainlab-0.1.3/domainlab/algos/builder_custom.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/builder_dann.py` & `domainlab-0.1.3/domainlab/algos/builder_dann.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
 from domainlab.algos.observers.c_obvisitor_cleanup import ObVisitorCleanUp
 from domainlab.algos.trainers.train_visitor import TrainerVisitor
-from domainlab.algos.trainers.train_visitor import HyperSchedulerAneal
+from domainlab.algos.trainers.train_visitor import HyperSchedulerWarmupExponential
 from domainlab.algos.trainers.train_dial import TrainerDIAL
 from domainlab.algos.trainers.zoo_trainer import TrainerChainNodeGetter
 from domainlab.compos.nn_zoo.net_classif import ClassifDropoutReluLinear
 from domainlab.compos.utils_conv_get_flat_dim import get_flat_dim
 from domainlab.compos.zoo_nn import FeatExtractNNBuilderChainNodeGetter
 from domainlab.models.model_dann import mk_dann
 from domainlab.utils.utils_cuda import get_device
@@ -57,12 +57,12 @@
                           alpha=args.gamma_reg,
                           net_encoder=net_encoder,
                           net_classifier=net_classifier,
                           net_discriminator=net_discriminator)
         trainer = TrainerChainNodeGetter(args)(default="visitor")
         trainer.init_business(model, task, observer, device, args)
         if trainer.name == "visitor":
-            trainer.set_scheduler(HyperSchedulerAneal,
+            trainer.set_scheduler(HyperSchedulerWarmupExponential,
                                   total_steps=trainer.num_batches*args.epos,
                                   flag_update_epoch=False,
                                   flag_update_batch=True)
         return trainer
```

### Comparing `domainlab-0.1.2/domainlab/algos/builder_deepall.py` & `domainlab-0.1.3/domainlab/algos/builder_deepall.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/builder_deepall_mldg.py` & `domainlab-0.1.3/domainlab/algos/builder_deepall_mldg.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/builder_dial.py` & `domainlab-0.1.3/domainlab/algos/builder_dial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/builder_diva.py` & `domainlab-0.1.3/domainlab/algos/builder_diva.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/builder_hduva.py` & `domainlab-0.1.3/domainlab/algos/builder_hduva.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+"""
+build hduva model, get trainer from cmd arguments
+"""
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
 from domainlab.algos.observers.c_obvisitor_cleanup import ObVisitorCleanUp
-from domainlab.algos.trainers.train_visitor import TrainerVisitor
 from domainlab.algos.trainers.zoo_trainer import TrainerChainNodeGetter
 from domainlab.compos.pcr.request import RequestVAEBuilderCHW
 from domainlab.compos.vae.utils_request_chain_builder import VAEChainNodeGetter
 from domainlab.models.model_hduva import mk_hduva
 from domainlab.utils.utils_cuda import get_device
```

### Comparing `domainlab-0.1.2/domainlab/algos/builder_jigen1.py` & `domainlab-0.1.3/domainlab/algos/builder_jigen1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from domainlab.algos.a_algo_builder import NodeAlgoBuilder
 from domainlab.algos.msels.c_msel import MSelTrLoss
 from domainlab.algos.msels.c_msel_oracle import MSelOracleVisitor
 from domainlab.algos.observers.b_obvisitor import ObVisitor
 from domainlab.algos.observers.c_obvisitor_cleanup import ObVisitorCleanUp
 from domainlab.algos.trainers.train_visitor import TrainerVisitor
-from domainlab.algos.trainers.train_visitor import HyperSchedulerAneal
+from domainlab.algos.trainers.train_visitor import HyperSchedulerWarmupExponential
 from domainlab.compos.nn_zoo.net_classif import ClassifDropoutReluLinear
 from domainlab.compos.utils_conv_get_flat_dim import get_flat_dim
 from domainlab.compos.zoo_nn import FeatExtractNNBuilderChainNodeGetter
 from domainlab.models.model_jigen import mk_jigen
 from domainlab.utils.utils_cuda import get_device
 from domainlab.dsets.utils_wrapdset_patches import WrapDsetPatches
 
@@ -68,12 +68,12 @@
                            coeff_reg=args.gamma_reg,
                            net_encoder=net_encoder,
                            net_classifier_class=net_classifier,
                            net_classifier_permutation=net_classifier_perm)
 
         trainer = TrainerVisitor()
         trainer.init_business(model, task, observer, device, args)
-        trainer.set_scheduler(HyperSchedulerAneal,
+        trainer.set_scheduler(HyperSchedulerWarmupExponential,
                               total_steps=trainer.num_batches*args.epos,
                               flag_update_epoch=False,
                               flag_update_batch=True)
         return trainer
```

### Comparing `domainlab-0.1.2/domainlab/algos/builder_match_hduva.py` & `domainlab-0.1.3/domainlab/algos/builder_match_hduva.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/builder_matchdg.py` & `domainlab-0.1.3/domainlab/algos/builder_matchdg.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/compos/matchdg_args.py` & `domainlab-0.1.3/domainlab/algos/compos/matchdg_args.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/compos/matchdg_base.py` & `domainlab-0.1.3/domainlab/algos/compos/matchdg_base.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/compos/matchdg_ctr_erm.py` & `domainlab-0.1.3/domainlab/algos/compos/matchdg_ctr_erm.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/compos/matchdg_match.py` & `domainlab-0.1.3/domainlab/algos/compos/matchdg_match.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/compos/matchdg_utils.py` & `domainlab-0.1.3/domainlab/algos/compos/matchdg_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/msels/c_msel.py` & `domainlab-0.1.3/domainlab/algos/msels/c_msel.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/msels/c_msel_oracle.py` & `domainlab-0.1.3/domainlab/algos/msels/c_msel_oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
     def update(self):
         """
         if the best model should be updated
         """
         self.tr_obs.exp.visitor.save(self.trainer.model, "epoch")
         if self.tr_obs.metric_te["acc"] > self.best_oracle_acc:
-            self.best_oracle_acc = self.tr_obs.metric_te["acc"]  # FIXME: only works for classification
+            self.best_oracle_acc = self.tr_obs.metric_te["acc"]
+            # FIXME: only works for classification
             self.tr_obs.exp.visitor.save(self.trainer.model, "oracle")
             print("oracle model saved")
         return self.msel.update()
 
     def if_stop(self):
         """
         if should early stop
```

### Comparing `domainlab-0.1.2/domainlab/algos/observers/a_observer.py` & `domainlab-0.1.3/domainlab/algos/observers/a_observer.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/observers/b_obvisitor.py` & `domainlab-0.1.3/domainlab/algos/observers/b_obvisitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,16 +55,20 @@
     def after_all(self):
         """
         After training is done
         """
         model_ld = None
         try:
             model_ld = self.exp.visitor.load()
-        except FileNotFoundError:
+        except FileNotFoundError as err:  # if other errors/exceptions occur, we do not catch them
+            # other exceptions will terminate the python script
             # this can happen if loss is increasing, model never get selected
+            print(err)
+            print("this error can occur if model selection criteria is worsening, \
+                  model never get persisted")
             return
 
         model_ld = model_ld.to(self.device)
         model_ld.eval()
         print("persisted model performance metric: \n")
         metric_te = model_ld.cal_perf_metric(self.loader_tr, self.device, self.loader_te)
         self.dump_prediction(model_ld, metric_te)
```

### Comparing `domainlab-0.1.2/domainlab/algos/observers/c_obvisitor_gen.py` & `domainlab-0.1.3/domainlab/algos/observers/c_obvisitor_gen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/a_trainer.py` & `domainlab-0.1.3/domainlab/algos/trainers/a_trainer.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/args_dial.py` & `domainlab-0.1.3/domainlab/algos/trainers/args_dial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/train_basic.py` & `domainlab-0.1.3/domainlab/algos/trainers/train_basic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/train_dial.py` & `domainlab-0.1.3/domainlab/algos/trainers/train_dial.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,21 +32,14 @@
             grad = torch.autograd.grad(loss_gen_adv, [img_adv])[0]
             # instead of gradient descent, we gradient ascent here
             img_adv = img_adv_ini.detach() + step_size * torch.sign(grad.detach())
             img_adv = torch.min(torch.max(img_adv, img_natural - epsilon), img_natural + epsilon)
             img_adv = torch.clamp(img_adv, 0.0, 1.0)
         return img_adv
 
-    def tr_batch(self, epoch, ind_batch):
-        """
-        anneal parameter for each batch
-        """
-        self.model.hyper_update(epoch*self.num_batches + ind_batch, self.hyper_scheduler)
-        return super().tr_epoch(epoch)
-
     def tr_epoch(self, epoch):
         self.model.train()
         self.epo_loss_tr = 0
         for ind_batch, (tensor_x, vec_y, vec_d, *_) in enumerate(self.loader_tr):
             tensor_x, vec_y, vec_d = \
                 tensor_x.to(self.device), vec_y.to(self.device), vec_d.to(self.device)
             self.optimizer.zero_grad()
```

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/train_matchdg.py` & `domainlab-0.1.3/domainlab/algos/trainers/train_matchdg.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/train_mldg.py` & `domainlab-0.1.3/domainlab/algos/trainers/train_mldg.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/train_visitor.py` & `domainlab-0.1.3/domainlab/algos/trainers/train_visitor.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,24 +10,29 @@
     """
     TrainerVisitor
     """
     def set_scheduler(self, scheduler, total_steps,
                       flag_update_epoch=False,
                       flag_update_batch=False):
         """
-        set the warmup or anealing strategy
+        set the warmup strategy from objective scheduler
+        set wheter the hyper-parameter scheduling happens per epoch or per batch
         """
         self.hyper_scheduler = self.model.hyper_init(scheduler)
         self.flag_update_hyper_per_epoch = flag_update_epoch
         self.flag_update_hyper_per_batch = flag_update_batch
         self.hyper_scheduler.set_steps(total_steps=total_steps)
 
     def after_batch(self, epoch, ind_batch):
+        """
+        if hyper-parameters should be updated per batch, then step
+        should be set to epoch*self.num_batches + ind_batch
+        """
         if self.flag_update_hyper_per_batch:
-            self.model.hyper_update(epoch, self.hyper_scheduler)
+            self.model.hyper_update(epoch*self.num_batches + ind_batch, self.hyper_scheduler)
         return super().after_batch(epoch, ind_batch)
 
     def before_tr(self):
         if self.hyper_scheduler is None:
             warnings.warn("hyper-parameter scheduler not set, \
                           going to use default Warmpup and epoch update")
             self.set_scheduler(HyperSchedulerWarmup,
@@ -38,21 +43,14 @@
         """
         update hyper-parameters only per epoch
         """
         if self.flag_update_hyper_per_epoch:
             self.model.hyper_update(epoch, self.hyper_scheduler)
         return super().tr_epoch(epoch)
 
-    def tr_batch(self, epoch, ind_batch):
-        """
-        anneal hyper-parameter for each batch
-        """
-        self.model.hyper_update(epoch*self.num_batches + ind_batch, self.hyper_scheduler)
-        return super().tr_epoch(epoch)
-
 
 class HyperSchedulerWarmup():
     """
     HyperSchedulerWarmup
     """
     def __init__(self, **kwargs):
         self.dict_par_setpoint = kwargs
@@ -73,31 +71,29 @@
         ratio = ((epoch+1) * 1.) / self.total_steps
         list_par = [par_setpoint, par_setpoint * ratio]
         par = min(list_par)
         return par
 
     def __call__(self, epoch):
         dict_rst = {}
-        for key, _ in self.dict_par_setpoint.items():
-            dict_rst[key] = self.warmup(self.dict_par_setpoint[key], epoch)
+        for key, val_setpoint in self.dict_par_setpoint.items():
+            dict_rst[key] = self.warmup(val_setpoint, epoch)
         return dict_rst
 
 
-class HyperSchedulerAneal(HyperSchedulerWarmup):
+class HyperSchedulerWarmupExponential(HyperSchedulerWarmup):
     """
-    HyperSchedulerAneal
+    HyperScheduler Exponential
     """
-    def aneal(self, epoch, alpha):
+    def aneal(self, par_setpoint, epoch):
         """
         start from a small value of par to ramp up the steady state value using
         number of total_steps
         :param epoch:
         """
         ratio = ((epoch+1) * 1.) / self.total_steps
         denominator = (1. + np.exp(-10 * ratio))
-        return float((2. / denominator - 1) * alpha)
-
-    def __call__(self, epoch):
-        dict_rst = {}
-        for key, val in self.dict_par_setpoint.items():
-            dict_rst[key] = self.aneal(epoch, val)
-        return dict_rst
+        # ratio is 0, denom is 2, 2/denom is 1, return is 0
+        # ratio is 1, denom is 1+exp(-10), 2/denom is 2/(1+exp(-10))=2, return is 1
+        # exp(-10)=4.5e-5 is approximately 0
+        # slowly increase the regularization weight from 0 to 1*alpha as epochs goes on
+        return float((2. / denominator - 1) * par_setpoint)
```

### Comparing `domainlab-0.1.2/domainlab/algos/trainers/zoo_trainer.py` & `domainlab-0.1.3/domainlab/algos/trainers/zoo_trainer.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/algos/zoo_algos.py` & `domainlab-0.1.3/domainlab/algos/zoo_algos.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/arg_parser.py` & `domainlab-0.1.3/domainlab/arg_parser.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/a_nn_builder.py` & `domainlab-0.1.3/domainlab/compos/a_nn_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/builder_nn_alex.py` & `domainlab-0.1.3/domainlab/compos/builder_nn_alex.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/builder_nn_conv_bn_relu_2.py` & `domainlab-0.1.3/domainlab/compos/builder_nn_conv_bn_relu_2.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/builder_nn_external_from_file.py` & `domainlab-0.1.3/domainlab/compos/builder_nn_external_from_file.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/exp/exp_cuda_seed.py` & `domainlab-0.1.3/domainlab/compos/exp/exp_cuda_seed.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/exp/exp_main.py` & `domainlab-0.1.3/domainlab/compos/exp/exp_main.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/exp/exp_utils.py` & `domainlab-0.1.3/domainlab/compos/exp/exp_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/nn_zoo/net_adversarial.py` & `domainlab-0.1.3/domainlab/compos/nn_zoo/net_adversarial.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/nn_zoo/net_classif.py` & `domainlab-0.1.3/domainlab/compos/nn_zoo/net_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py` & `domainlab-0.1.3/domainlab/compos/nn_zoo/net_conv_conv_bn_pool_2.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/nn_zoo/net_gated.py` & `domainlab-0.1.3/domainlab/compos/nn_zoo/net_gated.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/nn_zoo/nn.py` & `domainlab-0.1.3/domainlab/compos/nn_zoo/nn.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/nn_zoo/nn_alex.py` & `domainlab-0.1.3/domainlab/compos/nn_zoo/nn_alex.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/nn_zoo/nn_torchvision.py` & `domainlab-0.1.3/domainlab/compos/nn_zoo/nn_torchvision.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/pcr/p_chain_handler.py` & `domainlab-0.1.3/domainlab/compos/pcr/p_chain_handler.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/pcr/request.py` & `domainlab-0.1.3/domainlab/compos/pcr/request.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/utils_conv_get_flat_dim.py` & `domainlab-0.1.3/domainlab/compos/utils_conv_get_flat_dim.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/a_model_builder.py` & `domainlab-0.1.3/domainlab/compos/vae/a_model_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/a_vae_builder.py` & `domainlab-0.1.3/domainlab/compos/vae/a_vae_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/c_vae_adaptor_model_recon.py` & `domainlab-0.1.3/domainlab/compos/vae/c_vae_adaptor_model_recon.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/c_vae_builder_classif.py` & `domainlab-0.1.3/domainlab/compos/vae/c_vae_builder_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/c_vae_recon.py` & `domainlab-0.1.3/domainlab/compos/vae/c_vae_recon.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/decoder_concat_vec_reshape_conv_gated_conv.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_cond_prior.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/decoder_cond_prior.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/decoder_losses.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/decoder_losses.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_dirichlet.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder_dirichlet.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder_domain_topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder_domain_topic_img2topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder_domain_topic_img_topic2zd.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xyd_parallel.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder_xyd_parallel.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_xydt_elevator.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder_xydt_elevator.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/compos/encoder_zy.py` & `domainlab-0.1.3/domainlab/compos/vae/compos/encoder_zy.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/utils_request_chain_builder.py` & `domainlab-0.1.3/domainlab/compos/vae/utils_request_chain_builder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif.py` & `domainlab-0.1.3/domainlab/compos/vae/zoo_vae_builders_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/vae/zoo_vae_builders_classif_topic.py` & `domainlab-0.1.3/domainlab/compos/vae/zoo_vae_builders_classif_topic.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/compos/zoo_nn.py` & `domainlab-0.1.3/domainlab/compos/zoo_nn.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/dsets/a_dset_mnist_color_rgb_solo.py` & `domainlab-0.1.3/domainlab/dsets/a_dset_mnist_color_rgb_solo.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/dsets/dset_img_path_list.py` & `domainlab-0.1.3/domainlab/dsets/dset_img_path_list.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/dsets/dset_mnist_color_solo_default.py` & `domainlab-0.1.3/domainlab/dsets/dset_mnist_color_solo_default.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/dsets/dset_poly_domains_mnist_color_default.py` & `domainlab-0.1.3/domainlab/dsets/dset_poly_domains_mnist_color_default.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/dsets/dset_subfolder.py` & `domainlab-0.1.3/domainlab/dsets/dset_subfolder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/dsets/utils_data.py` & `domainlab-0.1.3/domainlab/dsets/utils_data.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/dsets/utils_wrapdset_patches.py` & `domainlab-0.1.3/domainlab/dsets/utils_wrapdset_patches.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/exp_protocol/aggregate_results.py` & `domainlab-0.1.3/domainlab/exp_protocol/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/exp_protocol/benchmark.smk` & `domainlab-0.1.3/domainlab/exp_protocol/benchmark.smk`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/exp_protocol/run_experiment.py` & `domainlab-0.1.3/domainlab/exp_protocol/run_experiment.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/a_model.py` & `domainlab-0.1.3/domainlab/models/a_model.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/a_model_classif.py` & `domainlab-0.1.3/domainlab/models/a_model_classif.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         """
         logit_y = self.cal_logit_y(tensor_x)
         if (tensor_y.shape[-1] == 1) | (len(tensor_y.shape) == 1):
             y_target = tensor_y
         else:
             _, y_target = tensor_y.max(dim=1)
         lc_y = F.cross_entropy(logit_y, y_target, reduction="none")
+        # cross entropy always return a scalar, no need for inside instance reduction
         return lc_y
 
     def pred2file(self, loader_te, device, filename,
                   metric_te,
                   spliter="#"):
         """
         pred2file dump predicted label to file as sanity check
```

### Comparing `domainlab-0.1.2/domainlab/models/args_jigen.py` & `domainlab-0.1.3/domainlab/models/args_jigen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/args_vae.py` & `domainlab-0.1.3/domainlab/models/args_vae.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/interface_vae_xyd.py` & `domainlab-0.1.3/domainlab/models/interface_vae_xyd.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/model_custom.py` & `domainlab-0.1.3/domainlab/models/model_custom.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/model_dann.py` & `domainlab-0.1.3/domainlab/models/model_dann.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+"""
+construct feature extractor, task neural network (e.g. classification) and domain classification network
+"""
 from torch.nn import functional as F
 
 from domainlab.compos.nn_zoo.net_adversarial import AutoGradFunReverseMultiply
 from domainlab.models.a_model_classif import AModelClassif
 
+
 def mk_dann(parent_class=AModelClassif):
     """Instantiate a Deep Adversarial Net (DAN) model
 
     Args:
         parent_class (AModel, optional): Class object determining the task
         type. Defaults to AModelClassif.
 
@@ -24,26 +28,26 @@
             self.net_encoder = net_encoder
             self.net_classifier = net_classifier
             self.net_discriminator = net_discriminator
 
         def hyper_update(self, epoch, fun_scheduler):
             """hyper_update.
             :param epoch:
-            :param fun_scheduler:
+            :param fun_scheduler: the hyperparameter scheduler object
             """
-            dict_rst = fun_scheduler(epoch)
+            dict_rst = fun_scheduler(epoch)  # the __call__ method of hyperparameter scheduler
             self.alpha = dict_rst["alpha"]
 
         def hyper_init(self, functor_scheduler):
             """hyper_init.
             :param functor_scheduler:
             """
             return functor_scheduler(alpha=self.alpha)
 
-        def cal_logit_y(self, tensor_x):
+        def cal_logit_y(self, tensor_x):  # FIXME: this is only for classification
             """
             calculate the logit for softmax classification
             """
             return self.net_classifier(self.net_encoder(tensor_x))
 
         def cal_reg_loss(self, tensor_x, tensor_y, tensor_d, others=None):
             feat = self.net_encoder(tensor_x)
```

### Comparing `domainlab-0.1.2/domainlab/models/model_deep_all.py` & `domainlab-0.1.3/domainlab/models/model_deep_all.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/model_diva.py` & `domainlab-0.1.3/domainlab/models/model_diva.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/model_hduva.py` & `domainlab-0.1.3/domainlab/models/model_hduva.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,27 @@
         """
         def hyper_update(self, epoch, fun_scheduler):
             """hyper_update.
 
             :param epoch:
             :param fun_scheduler:
             """
-            dict_rst = fun_scheduler(epoch)
+            dict_rst = fun_scheduler(epoch)  # the __call__ function of hyper-para-scheduler object
             self.beta_d = dict_rst["beta_d"]
             self.beta_y = dict_rst["beta_y"]
             self.beta_x = dict_rst["beta_x"]
             self.beta_t = dict_rst["beta_t"]
 
         def hyper_init(self, functor_scheduler):
             """hyper_init.
             :param functor_scheduler:
             """
+            # calling the constructor of the hyper-parameter-scheduler class, so that this scheduler
+            # class build a dictionary {"beta_d":self.beta_d, "beta_y":self.beta_y}
+            # constructor signature is def __init__(self, **kwargs):
             return functor_scheduler(
                 beta_d=self.beta_d, beta_y=self.beta_y, beta_x=self.beta_x,
                 beta_t=self.beta_t)
 
         @store_args
         def __init__(self, chain_node_builder,
                      zy_dim, zd_dim,
```

### Comparing `domainlab-0.1.2/domainlab/models/model_jigen.py` & `domainlab-0.1.3/domainlab/models/model_jigen.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/model_vae_xyd_classif.py` & `domainlab-0.1.3/domainlab/models/model_vae_xyd_classif.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,12 +24,17 @@
         """
         calculate the logit for softmax classification
         """
         zy_q_loc = self.encoder.infer_zy_loc(tensor_x)
         logit_y = self.net_classif_y(zy_q_loc)
         return logit_y
 
+
+    def cal_task_loss(self, tensor_x, tensor_y):
+        tloss = super().cal_task_loss(tensor_x, tensor_y)
+        return self.gamma_y * tloss
+
     def _init_components(self):
         super()._init_components()
         self.add_module("net_classif_y",
                         self.chain_node_builder.construct_classifier(
                             self.zy_dim, self.dim_y))
```

### Comparing `domainlab-0.1.2/domainlab/models/model_wrapper_matchdg4net.py` & `domainlab-0.1.3/domainlab/models/model_wrapper_matchdg4net.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/model_wrapper_matchdg4vae.py` & `domainlab-0.1.3/domainlab/models/model_wrapper_matchdg4vae.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/models/wrapper_matchdg.py` & `domainlab-0.1.3/domainlab/models/wrapper_matchdg.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/a_task.py` & `domainlab-0.1.3/domainlab/tasks/a_task.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/a_task_classif.py` & `domainlab-0.1.3/domainlab/tasks/a_task_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/b_task.py` & `domainlab-0.1.3/domainlab/tasks/b_task.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/b_task_classif.py` & `domainlab-0.1.3/domainlab/tasks/b_task_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/task_dset.py` & `domainlab-0.1.3/domainlab/tasks/task_dset.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/task_folder.py` & `domainlab-0.1.3/domainlab/tasks/task_folder.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/task_folder_mk.py` & `domainlab-0.1.3/domainlab/tasks/task_folder_mk.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/task_mnist_color.py` & `domainlab-0.1.3/domainlab/tasks/task_mnist_color.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/task_pathlist.py` & `domainlab-0.1.3/domainlab/tasks/task_pathlist.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/task_utils.py` & `domainlab-0.1.3/domainlab/tasks/task_utils.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/utils_task.py` & `domainlab-0.1.3/domainlab/tasks/utils_task.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/utils_task_dset.py` & `domainlab-0.1.3/domainlab/tasks/utils_task_dset.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/tasks/zoo_tasks.py` & `domainlab-0.1.3/domainlab/tasks/zoo_tasks.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/uml/libDG.uml` & `domainlab-0.1.3/domainlab/uml/libDG.uml`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/flows_gen_img_model.py` & `domainlab-0.1.3/domainlab/utils/flows_gen_img_model.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/generate_benchmark_plots.py` & `domainlab-0.1.3/domainlab/utils/generate_benchmark_plots.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/get_git_tag.py` & `domainlab-0.1.3/domainlab/utils/get_git_tag.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/hyperparameter_sampling.py` & `domainlab-0.1.3/domainlab/utils/hyperparameter_sampling.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/override_interface.py` & `domainlab-0.1.3/domainlab/utils/override_interface.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/perf.py` & `domainlab-0.1.3/domainlab/utils/perf.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/perf_metrics.py` & `domainlab-0.1.3/domainlab/utils/perf_metrics.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/sanity_check.py` & `domainlab-0.1.3/domainlab/utils/sanity_check.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/test_img.py` & `domainlab-0.1.3/domainlab/utils/test_img.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/u_import_net_module.py` & `domainlab-0.1.3/domainlab/utils/u_import_net_module.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/utils_class.py` & `domainlab-0.1.3/domainlab/utils/utils_class.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/utils_classif.py` & `domainlab-0.1.3/domainlab/utils/utils_classif.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/domainlab/utils/utils_img_sav.py` & `domainlab-0.1.3/domainlab/utils/utils_img_sav.py`

 * *Files identical despite different names*

### Comparing `domainlab-0.1.2/pyproject.toml` & `domainlab-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domainlab"
-version = "0.1.2"
+version = "0.1.3"
 description = "Library of Domain Generalization"
 authors = ["Xudong Sun <smilesun.east@gmail.com>", "Alexej Gossmann <alexej.gossmann@fda.hhs.gov>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.4"
 matplotlib = "^3.6.1"
```

### Comparing `domainlab-0.1.2/setup.py` & `domainlab-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'snakemake==7.21.0',
  'torch>=1.12.0,<2.0.0',
  'torchmetrics>=0.10.0,<0.11.0',
  'torchvision>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'domainlab',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Library of Domain Generalization',
     'long_description': 'None',
     'author': 'Xudong Sun',
     'author_email': 'smilesun.east@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `domainlab-0.1.2/PKG-INFO` & `domainlab-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domainlab
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library of Domain Generalization
 Author: Xudong Sun
 Author-email: smilesun.east@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

