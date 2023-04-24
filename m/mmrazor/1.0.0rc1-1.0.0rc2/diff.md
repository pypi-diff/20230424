# Comparing `tmp/mmrazor-1.0.0rc1.tar.gz` & `tmp/mmrazor-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmrazor-1.0.0rc1.tar", last modified: Tue Nov  1 14:55:12 2022, max compression
+gzip compressed data, was "dist/mmrazor-1.0.0rc2.tar", last modified: Fri Jan  6 11:15:49 2023, max compression
```

## Comparing `mmrazor-1.0.0rc1.tar` & `mmrazor-1.0.0rc2.tar`

### file list

```diff
@@ -1,485 +1,627 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10732 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8130 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/datasets/mmcls/
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/datasets/mmcls/cifar100_bs16_auto_aug.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/datasets/mmcls/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/datasets/mmcls/pipelines/auto_aug_cifar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/darts_supernet.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/dsnas_shufflenet_supernet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/spos_mobilenet_supernet.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/spos_shufflenet_supernet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/cifar10_darts_subnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2583 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/cifar10_darts_supernet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2887 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_dsnas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_spos.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_autoslim.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_autoslim_pil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/vanilla_models/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/vanilla_models/wrn16_2_cifar10.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/abloss/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_logits_resnet50_resnet18_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_pretrain_backbone_resnet50_resnet18_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/abloss/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/byot/
--rw-r--r--   0 runner    (1001) docker     (121)     6264 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/byot/byot_resnet18_8xb16_cifar100.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/byot/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/crd/
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/crd/crd_neck_r50_r18_8xb16_cifar10.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/crd/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/crd/datasets/crd_cifar10_bs16.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dafl/
--rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dafl/dafl_logits_resnet34_resnet18_8xb256_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dafl/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/deit/
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/deit/deit-base_regnety160_pt-16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/deit/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dfad/
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dfad/dfad_logits_resnet34_resnet18_8xb32_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dfad/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dkd/
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dkd/dkd_resnet34_resnet18_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dkd/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/factor_transfer/
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_pretrain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_train.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/factor_transfer/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/fitnets/
--rw-r--r--   0 runner    (1001) docker     (121)     2979 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/fitnets/fitnets_backbone_logits_resnet50_resnet18_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/fitnets/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet34_resnet18_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_mobilenet-v2_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_shufflenet-v2-1x_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/ofd/
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/ofd/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/ofd/ofd_backbone_resnet50_resnet18_8xb16_cifar10.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/rkd/
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/rkd/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/rkd/rkd_neck_resnet34_resnet18_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/wsld/
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/wsld/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/wsld/wsld_logits_resnet34_resnet18_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/zskt/
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/zskt/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/zskt/zskt_backbone_logits_resnet34_resnet18_8xb16_cifar10.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_frcnn_r101_frcnn_r50_1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/fbkd/
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/fbkd/fbkd_fpn_faster-rcnn_r101_faster-rcnn_r50_1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/fbkd/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_faster-rcnn_r101_faster-rcnn_r50_2x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_fcos_x101_retina_r50_1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_mask-rcnn_swin_retina_r50_2x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_reppoints_x101-dcn_reppoints_r50_2x_coco.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_retina_x101_retina_r50_2x_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet3d/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet3d/pkd/
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet3d/pkd/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet3d/pkd/pkd_fpn_fcos3d_r101_fcos3d_r50_8xb2-1x_nus-mono3d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmseg/cwd/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmseg/cwd/cwd_logits_pspnet_r101-d8_pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmseg/cwd/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_slimmable_subnet_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-220M.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-320M.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-530M.py
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_supernet_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/darts/
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/darts/darts_supernet_unroll_1xb96_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/darts/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/dsnas/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_subnet_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_supernet_8xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_search_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_subnet_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_supernet_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_search_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_subnet_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_supernet_8xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_search_coco_1x.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_subnet_coco_1x.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_supernet_coco_1x.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_retina_shufflenet_supernet_coco_1x.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_shufflenet_subnet_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_shufflenet_supernet_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/pruning/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/pruning/mmcls/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/pruning/mmcls/l1-norm/
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/vanilla/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/vanilla/mmcls/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn16-w2_b16x8_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn22-w4_b16x8_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn28-w4_b16x8_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn40-w2_b16x8_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-11-01 14:55:11.000000 mmrazor-1.0.0rc1/mmrazor/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/dist_test.sh
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/dist_train.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/get_channel_units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/misc/print_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/model_converters/convert_kd_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/model_converters/publish_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/slurm_test.sh
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/
--rw-r--r--   0 runner    (1001) docker     (121)     6088 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/feature_diff_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/feature_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_configs/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_diff_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_diff_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)     8628 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/datasets/crd_dataset_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/datasets/transforms/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/engine/
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/hooks/dump_subnet_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/hooks/estimate_resources_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     8256 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/engine/optimizers/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/optimizers/optimizer_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/autoslim_val_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     6781 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/darts_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/distill_val_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)    12910 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/evolution_search_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/slimmable_val_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)    14521 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/subnet_sampler_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/engine/runner/utils/genetic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6764 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9905 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/datafree_distillation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/fpn_teacher_distill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/overhaul_feature_distillation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3616 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/self_distill.py
--rw-r--r--   0 runner    (1001) docker     (121)     5674 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/single_teacher_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9619 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/autoslim.py
--rw-r--r--   0 runner    (1001) docker     (121)    24465 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/darts.py
--rw-r--r--   0 runner    (1001) docker     (121)    15333 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/dsnas.py
--rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/spos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/pruning/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8334 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/pruning/ite_prune_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8458 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/algorithms/pruning/slimmable_network.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14014 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/darts_backbone.py
--rw-r--r--   0 runner    (1001) docker     (121)     8424 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/searchable_mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8575 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/searchable_shufflenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14338 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/wideresnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/base_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/byot_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/convmodule_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/crd_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/factor_transfer_connectors.py
--rw-r--r--   0 runner    (1001) docker     (121)    12309 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/fbkd_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/ofd_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/torch_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/bricks/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_conv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     6708 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15617 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/mixins/dynamic_conv_mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    14049 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/mixins/dynamic_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/base_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/dafl_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/zskt_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/heads/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/heads/darts_subnet_head.py
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/heads/deit_head.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5601 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/darts_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/efficientnet_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/gather_tensors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/mobilenet_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     8815 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/shufflenet_series.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/distillers/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/distillers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/distillers/base_distiller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/distillers/byot_distiller.py
--rw-r--r--   0 runner    (1001) docker     (121)    12451 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/distillers/configurable_distiller.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/distillers/ofd_distiller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/ab_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/at_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     9694 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/crd_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/cwd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/dafl_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     5605 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/decoupled_kd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/factor_transfer_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/fbkd_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/kd_soft_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/l2_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/ofd_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/pkd_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     5008 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/relational_kd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/losses/weighted_soft_label_distillation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/base_mutable.py
--rw-r--r--   0 runner    (1001) docker     (121)    14440 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/derived_mutable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/base_mutable_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4669 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/mutable_channel_container.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/oneshot_mutalbe_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4429 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/sequential_mutable_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/simple_mutable_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10472 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/l1_mutable_channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)    12095 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/mutable_channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5238 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/one_shot_mutable_channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5391 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/sequential_mutable_channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/slimmable_channel_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21644 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/diff_mutable_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/mutable_module.py
--rw-r--r--   0 runner    (1001) docker     (121)    10462 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/one_shot_mutable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_value/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7392 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_value/mutable_value.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/base_mutator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/channel_mutator/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/channel_mutator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13542 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/channel_mutator/channel_mutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/channel_mutator/one_shot_channel_mutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/channel_mutator/slimmable_channel_mutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9172 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/group_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4191 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/diff_module_mutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2977 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/module_mutator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/one_shot_module_mutator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/delivery_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/distill_delivery.py
--rw-r--r--   0 runner    (1001) docker     (121)     5797 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/function_outputs_delivery.py
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/method_outputs_delivery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/base_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22635 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/flops_params_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/latency_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/activation_layer_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/base_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/conv_layer_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/deconv_layer_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/linear_layer_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/norm_layer_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/pooling_layer_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/upsample_layer_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8636 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/resource_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4218 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/base_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/function_inputs_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/function_outputs_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/method_inputs_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5744 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/method_outputs_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/module_inputs_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/module_outputs_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/param_recorder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/recorder_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/backward_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/loss_calculator/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/loss_calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/loss_calculator/image_classifier_loss_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/loss_calculator/single_stage_detector_loss_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7451 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11552 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/models/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/utils/optim_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/models/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/registry/
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/structures/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/structures/graph/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7042 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/graph/channel_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    12173 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/graph/channel_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)    12414 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/graph/channel_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    17870 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/graph/module_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/structures/subnet/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/subnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/subnet/candidate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/structures/subnet/fix_subnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/testing/_fast_stop_training_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/utils/index_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/utils/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/mmrazor/visualization/local_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10732 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20517 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/mmrazor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7220 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17667 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/data/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_core/test_graph/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_core/test_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6346 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_core/test_graph/test_channel_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_core/test_graph/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_metafiles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6268 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_autoslim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_base_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8736 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_darts.py
--rw-r--r--   0 runner    (1001) docker     (121)     9645 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_datafree_distill.py
--rw-r--r--   0 runner    (1001) docker     (121)     7393 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_dsnas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_ofd_algo.py
--rw-r--r--   0 runner    (1001) docker     (121)     6885 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_prune_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_self_distill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_single_teacher_distill.py
--rw-r--r--   0 runner    (1001) docker     (121)     6166 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_slimmable_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_spos.py
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_algorithms/toy_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8219 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_derived_mutable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_diffchoiceroute.py
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_diffop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_gumbelchoiceroute.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_mutable_channels.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_sequential_mutable_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/test_l1_mutable_channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5571 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/test_mutable_channel_units.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/test_one_shot_mutable_channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/test_sequential_mutable_channel_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     6282 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_onehotop.py
--rw-r--r--   0 runner    (1001) docker     (121)     7873 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_oneshotop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutators/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5800 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutators/test_channel_mutator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:55:12.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutators/test_classical_models/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutators/test_classical_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8198 2022-11-01 14:55:09.000000 mmrazor-1.0.0rc1/tests/test_models/test_mutators/test_diff_mutator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/datasets/mmcls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/datasets/mmcls/cifar100_bs16_auto_aug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/datasets/mmcls/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/datasets/mmcls/pipelines/auto_aug_cifar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/attentive_mobilenetv3_supernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/darts_supernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/dsnas_shufflenet_supernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/ofa_mobilenetv3_supernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/spos_mobilenet_supernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/spos_shufflenet_supernet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/cifar10_darts_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/cifar10_darts_supernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_dsnas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_spos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_AdamW.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_autoslim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_autoslim_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_bignas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_ofa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/vanilla_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/vanilla_models/wrn16_2_cifar10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/abloss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_logits_resnet50_resnet18_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_pretrain_backbone_resnet50_resnet18_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/abloss/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/byot/
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/byot/byot_resnet18_8xb16_cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/byot/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/crd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/crd/crd_neck_r50_r18_8xb16_cifar10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/crd/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/crd/datasets/crd_cifar10_bs16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dafl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dafl/dafl_logits_resnet34_resnet18_8xb256_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dafl/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/deit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/deit/deit-base_regnety160_pt-16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/deit/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dfad/
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dfad/dfad_logits_resnet34_resnet18_8xb32_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dfad/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dkd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dkd/dkd_resnet34_resnet18_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dkd/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/factor_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/factor_transfer/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/fitnets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/fitnets/fitnets_backbone_logits_resnet50_resnet18_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/fitnets/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet34_resnet18_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_mobilenet-v2_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_shufflenet-v2-1x_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/ofd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/ofd/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/ofd/ofd_backbone_resnet50_resnet18_8xb16_cifar10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/rkd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/rkd/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/rkd/rkd_neck_resnet34_resnet18_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/wsld/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/wsld/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/wsld/wsld_logits_resnet34_resnet18_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/zskt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/zskt/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/zskt/zskt_backbone_logits_resnet34_resnet18_8xb16_cifar10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_frcnn_r101_frcnn_r50_1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/fbkd/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/fbkd/fbkd_fpn_faster-rcnn_r101_faster-rcnn_r50_1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/fbkd/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/mgd/
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/mgd/mgd_fpn_retina_x101_retina_r50_2x_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_faster-rcnn_r101_faster-rcnn_r50_2x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_fcos_x101_retina_r50_1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_mask-rcnn_swin_retina_r50_2x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_reppoints_x101-dcn_reppoints_r50_2x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_retina_x101_retina_r50_2x_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet3d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet3d/pkd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet3d/pkd/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet3d/pkd/pkd_fpn_fcos3d_r101_fcos3d_r50_8xb2-1x_nus-mono3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmseg/cwd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmseg/cwd/cwd_logits_pspnet_r101-d8_pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmseg/cwd/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoformer/autoformer_search_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoformer/autoformer_supernet_32xb256_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_search_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_slimmable_subnet_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-220M.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-320M.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-530M.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_supernet_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/bignas/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/bignas/attentive_mobilenet_search_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/bignas/attentive_mobilenet_subnet_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/bignas/attentive_mobilenet_supernet_32xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0_mmrazor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/darts_supernet_unroll_1xb96_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/dsnas/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_subnet_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_supernet_8xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/onceforall/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/onceforall/ofa_mobilenet_search_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/onceforall/ofa_mobilenet_subnet_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/onceforall/ofa_mobilenet_supernet_32xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/faster-rcnn_nas_backbone_fpn_1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_search_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_subnet_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_supernet_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_search_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_search_predictor_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_subnet_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_supernet_8xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_search_coco_1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_subnet_coco_1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_supernet_coco_1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_retina_shufflenet_supernet_coco_1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_shufflenet_subnet_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_shufflenet_supernet_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/dcff/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/dcff/dcff_compact_resnet_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/dcff/dcff_resnet_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/l1-norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k_c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmdet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmdet/dcff/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmdet/dcff/dcff_compact_faster_rcnn_resnet50_8xb4_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmdet/dcff/dcff_faster_rcnn_resnet50_8xb4_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmdet/dcff/dcff_faster_rcnn_resnet50_fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmpose/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmpose/dcff/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmpose/dcff/dcff_compact_topdown_heatmap_resnet50_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmpose/dcff/dcff_topdown_heatmap_resnet50_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmseg/dcff/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmseg/dcff/dcff_compact_pointrend_resnet50_8xb2_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmseg/dcff/dcff_pointrend_resnet50_8xb2_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmseg/dcff/pointrend_resnet50.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/vanilla/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/vanilla/mmcls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn16-w2_b16x8_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn22-w4_b16x8_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn28-w4_b16x8_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn40-w2_b16x8_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-01-06 11:15:48.000000 mmrazor-1.0.0rc2/mmrazor/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/dist_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/dist_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/misc/print_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/convert_attentivenas_nas_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/convert_bignas_gml_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/convert_kd_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/convert_kd_ckpt_to_student.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/convert_ofa_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/convert_supernet2subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/publish_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/pruning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/pruning/get_channel_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/pruning/get_l1_prune_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/slurm_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/slurm_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/feature_diff_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/feature_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_diff_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_diff_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/datasets/crd_dataset_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/datasets/transforms/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/datasets/transforms/auto_augmentv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/datasets/transforms/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/hooks/dump_subnet_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/hooks/estimate_resources_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/engine/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/optimizers/optimizer_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/autoslim_greedy_search_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/darts_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/distill_val_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19286 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/evolution_search_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/iteprune_val_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/slimmable_val_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/subnet_sampler_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/subnet_val_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/utils/calibrate_bn_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/engine/runner/utils/genetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/datafree_distillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/fpn_teacher_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/overhaul_feature_distillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/self_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/single_teacher_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/autoslim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/bignas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24468 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/darts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/dsnas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/spos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/pruning/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/pruning/dcff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/pruning/ite_prune_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/algorithms/pruning/slimmable_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/darts_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/searchable_autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/searchable_mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/searchable_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/searchable_shufflenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/wideresnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/classifiers/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/base_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/byot_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/convmodule_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/crd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/factor_transfer_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/fbkd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/mgd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/ofd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/torch_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_relative_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/head/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/head/dynamic_linear_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22096 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/mixins/dynamic_conv_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/mixins/dynamic_layernorm_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/mixins/dynamic_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/base_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/dafl_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/zskt_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/heads/darts_subnet_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/heads/deit_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/necks/squeezemean_with_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/darts_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/efficientnet_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/gather_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/mobilenet_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/shufflenet_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/transformer_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/utils/mutable_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/architectures/utils/set_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/distillers/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/distillers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/distillers/base_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/distillers/byot_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/distillers/configurable_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/distillers/ofd_distiller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/ab_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/at_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/crd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/dafl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/decoupled_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/factor_transfer_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/fbkd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/kd_soft_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/l2_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/mgd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/ofd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/pkd_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/relational_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/losses/weighted_soft_label_distillation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/base_mutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/derived_mutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/base_mutable_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/mutable_channel_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/oneshot_mutable_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/sequential_mutable_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/simple_mutable_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/dcff_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/l1_mutable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/mutable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/one_shot_mutable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/sequential_mutable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/slimmable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21644 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/diff_mutable_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/mutable_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/one_shot_mutable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_value/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_value/mutable_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/base_mutator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/channel_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/dcff_channel_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/one_shot_channel_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/slimmable_channel_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/group_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/diff_module_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/module_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/one_shot_module_mutator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/value_mutator/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/value_mutator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/value_mutator/dynamic_value_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/mutators/value_mutator/value_mutator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/delivery_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/distill_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/function_outputs_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/method_outputs_delivery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/demo_inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/demo_inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/demo_inputs/default_demo_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/demo_inputs/demo_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/demo_inputs/mmseg_demo_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/base_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/flops_params_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/latency_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/activation_layer_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/base_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/conv_layer_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/deconv_layer_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/linear_layer_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/norm_layer_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/pooling_layer_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/upsample_layer_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/resource_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/handler/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/handler/carts_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/handler/gp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/handler/mlp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/handler/rbf_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/predictor/metric_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/base_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/function_inputs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/function_outputs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/method_inputs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/method_outputs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/module_inputs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/module_outputs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/param_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/recorder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/backward_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/channel_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/fx_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/cascade_encoder_decoder_loss_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/image_classifier_loss_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/single_stage_detector_loss_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/sum_loss_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/top_down_pose_estimator_loss_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/two_stage_detector_loss_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/utils/optim_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/utils/parse_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/models/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/channel_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/channel_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/channel_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/module_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/graph/pseudo_fx_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/structures/subnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/subnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/subnet/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/structures/subnet/fix_subnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/testing/_fast_stop_training_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/utils/index_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/utils/log_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/utils/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/mmrazor/visualization/local_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-01-06 11:15:48.000000 mmrazor-1.0.0rc2/mmrazor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/mmrazor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 11:15:48.000000 mmrazor-1.0.0rc2/mmrazor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 11:15:48.000000 mmrazor-1.0.0rc2/mmrazor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-06 11:15:48.000000 mmrazor-1.0.0rc2/mmrazor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-06 11:15:48.000000 mmrazor-1.0.0rc2/mmrazor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/data/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31300 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/data/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/data/tracer_passed_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_core/test_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_graph/test_channel_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_graph/test_channel_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_graph/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_graph/test_prune_tracer_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_core/test_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_tracer/test_backward_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_tracer/test_fx_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_tracer/test_loss_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_core/test_tracer/test_prune_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_autoslim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_base_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_bignas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_darts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_datafree_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_dcff_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_dsnas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_ofd_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_prune_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_self_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_single_teacher_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_slimmable_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_spos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_algorithms/toy_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_derived_mutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_diffchoiceroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_diffop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_gumbelchoiceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_mutable_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_sequential_mutable_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_dcff_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_l1_mutable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_mutable_channel_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_one_shot_mutable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_sequential_mutable_channel_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_onehotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_oneshotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_sequential_mutable_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_channel_mutator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_classical_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_classical_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_dcff_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_diff_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_value_mutator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_task_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_task_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_models/test_task_modules/test_demo_inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_task_modules/test_demo_inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_models/test_task_modules/test_demo_inputs/test_demo_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/test_tools/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 11:15:49.000000 mmrazor-1.0.0rc2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/utils/set_dist_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-01-06 11:15:46.000000 mmrazor-1.0.0rc2/tests/utils/set_torch_thread.py
```

### Comparing `mmrazor-1.0.0rc1/PKG-INFO` & `mmrazor-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmrazor
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: OpenMMLab Model Compression Toolbox and Benchmark
 Home-page: https://github.com/open-mmlab/mmrazor
 Author: MMRazor Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmrazor-logo.png" width="600"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmrazor Version: 1.0.0rc1 Summary: OpenMMLab Model
+Metadata-Version: 2.1 Name: mmrazor Version: 1.0.0rc2 Summary: OpenMMLab Model
 Compression Toolbox and Benchmark Home-page: https://github.com/open-mmlab/
 mmrazor Author: MMRazor Contributors Author-email: openmmlab@gmail.com License:
 Apache License 2.0 Description:
                          [resources/mmrazor-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
```

### Comparing `mmrazor-1.0.0rc1/README.md` & `mmrazor-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/datasets/mmcls/cifar100_bs16_auto_aug.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/datasets/mmcls/cifar100_bs16_auto_aug.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/datasets/mmcls/pipelines/auto_aug_cifar.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/datasets/mmcls/pipelines/auto_aug_cifar.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/darts_supernet.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/darts_supernet.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/dsnas_shufflenet_supernet.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/dsnas_shufflenet_supernet.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/spos_mobilenet_supernet.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/spos_mobilenet_supernet.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,24 +42,24 @@
             type='MBBlock',
             kernel_size=3,
             expand_ratio=1,
             act_cfg=dict(type='ReLU6'))))
 
 arch_setting = [
     # Parameters to build layers. 3 parameters are needed to construct a
-    # layer, from left to right: channel, num_blocks, mutable_cfg.
+    # layer, from left to right: channel, num_blocks, stride, mutable_cfg.
     [24, 1, 1, _FIRST_MUTABLE],
     [32, 4, 2, _STAGE_MUTABLE],
     [56, 4, 2, _STAGE_MUTABLE],
     [112, 4, 2, _STAGE_MUTABLE],
     [128, 4, 1, _STAGE_MUTABLE],
     [256, 4, 2, _STAGE_MUTABLE],
     [432, 1, 1, _STAGE_MUTABLE]
 ]
 
 nas_backbone = dict(
     _scope_='mmrazor',
-    type='SearchableMobileNet',
+    type='SearchableMobileNetV2',
     first_channels=40,
     last_channels=1728,
     widen_factor=1.0,
     arch_setting=arch_setting)
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/nas_backbones/spos_shufflenet_supernet.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/nas_backbones/spos_shufflenet_supernet.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/cifar10_darts_subnet.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/cifar10_darts_subnet.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/cifar10_darts_supernet.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/cifar10_darts_supernet.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_dsnas.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_dsnas.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_logits_resnet50_resnet18_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_logits_resnet50_resnet18_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_pretrain_backbone_resnet50_resnet18_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/abloss/abloss_pretrain_backbone_resnet50_resnet18_8xb32_in1k.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,33 +38,33 @@
         distill_losses=dict(
             loss_s4=dict(type='ABLoss', loss_weight=1.0),
             loss_s3=dict(type='ABLoss', loss_weight=0.5),
             loss_s2=dict(type='ABLoss', loss_weight=0.25),
             loss_s1=dict(type='ABLoss', loss_weight=0.125)),
         connectors=dict(
             loss_s4_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=512,
                 out_channel=2048,
                 norm_cfg=dict(type='BN'),
                 act_cfg=None),
             loss_s3_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=256,
                 out_channel=1024,
                 norm_cfg=dict(type='BN'),
                 act_cfg=None),
             loss_s2_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=128,
                 out_channel=512,
                 norm_cfg=dict(type='BN'),
                 act_cfg=None),
             loss_s1_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=64,
                 out_channel=256,
                 norm_cfg=dict(type='BN'),
                 act_cfg=None)),
         loss_forward_mappings=dict(
             loss_s4=dict(
                 s_feature=dict(
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/abloss/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/abloss/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/byot/byot_resnet18_8xb16_cifar100.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/byot/byot_resnet18_8xb16_cifar100.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/byot/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/byot/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/crd/crd_neck_r50_r18_8xb16_cifar10.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/crd/crd_neck_r50_r18_8xb16_cifar10.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/crd/datasets/crd_cifar10_bs16.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/crd/datasets/crd_cifar10_bs16.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dafl/dafl_logits_resnet34_resnet18_8xb256_cifar10.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dafl/dafl_logits_resnet34_resnet18_8xb256_cifar10.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dafl/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dafl/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/deit/deit-base_regnety160_pt-16xb64_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/deit/deit-base_regnety160_pt-16xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/deit/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/deit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dfad/dfad_logits_resnet34_resnet18_8xb32_cifar10.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dfad/dfad_logits_resnet34_resnet18_8xb32_cifar10.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dfad/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dfad/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dkd/dkd_resnet34_resnet18_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dkd/dkd_resnet34_resnet18_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/dkd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/dkd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_pretrain.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_pretrain.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_train.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_train.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/factor_transfer/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/factor_transfer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/fitnets/fitnets_backbone_logits_resnet50_resnet18_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/fitnets/fitnets_backbone_logits_resnet50_resnet18_8xb32_in1k.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,20 +33,20 @@
         distill_losses=dict(
             loss_s4=dict(type='L2Loss', loss_weight=10),
             loss_s3=dict(type='L2Loss', loss_weight=10),
             loss_kl=dict(
                 type='KLDivergence', tau=6, loss_weight=10, reduction='mean')),
         connectors=dict(
             loss_s4_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=512,
                 out_channel=2048,
                 norm_cfg=dict(type='BN')),
             loss_s3_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=256,
                 out_channel=1024,
                 norm_cfg=dict(type='BN'))),
         loss_forward_mappings=dict(
             loss_s4=dict(
                 s_feature=dict(
                     from_student=True,
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/fitnets/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/fitnets/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet34_resnet18_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet34_resnet18_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_mobilenet-v2_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_mobilenet-v2_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_shufflenet-v2-1x_16xb64_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/kd_logits_resnet50_shufflenet-v2-1x_16xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/kd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/kd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/ofd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/ofd/metafile.yml`

 * *Files 4% similar despite different names*

```diff
@@ -31,8 +31,8 @@
           Top 5 Accuracy: 99.8200
     Results:
       - Task: Image Classification
         Dataset: CIFAR-10
         Metrics:
           Top 1 Accuracy: 95.4400
     Config: configs/distill/mmcls/ofd/ofd_backbone_resnet50_resnet18_8xb16_cifar10.py
-    Weights: https://download.openmmlab.com/mmrazor/v1/factor_transfer/factor-transfer_backbone_resnet50_resnet18_8xb16_cifar10_train_20220831_201322-943df33f.pth
+    Weights: https://download.openmmlab.com/mmrazor/v1/overhaul/ofd_backbone_resnet50_resnet18_8xb16_cifar10_20220831_220553-f5d12e61.pth
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/ofd/ofd_backbone_resnet50_resnet18_8xb16_cifar10.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/ofd/ofd_backbone_resnet50_resnet18_8xb16_cifar10.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 model = dict(
     _scope_='mmrazor',
     type='OverhaulFeatureDistillation',
     data_preprocessor=dict(
         type='ImgDataPreprocessor',
         # RGB format normalization parameters
-        mean=[123.675, 116.28, 103.53],
-        std=[58.395, 57.12, 57.375],
+        mean=[125.307, 122.961, 113.8575],
+        std=[51.5865, 50.847, 51.255],
         # convert image from BGR to RGB
-        bgr_to_rgb=True),
+        bgr_to_rgb=False),
     architecture=dict(
         cfg_path=  # noqa: E251
         'mmrazor::vanilla/mmcls/wide-resnet/wrn16-w2_b16x8_cifar10.py',
         pretrained=False),
     teacher=dict(
         cfg_path=  # noqa: E251
         'mmrazor::vanilla/mmcls/wide-resnet/wrn28-w4_b16x8_cifar10.py',
@@ -38,29 +38,29 @@
             bb_3=dict(type='ModuleOutputs', source='backbone.bn1')),
         distill_losses=dict(
             loss_1=dict(type='OFDLoss', loss_weight=0.25),
             loss_2=dict(type='OFDLoss', loss_weight=0.5),
             loss_3=dict(type='OFDLoss', loss_weight=1.0)),
         connectors=dict(
             loss_1_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=32,
                 out_channel=64,
                 norm_cfg=dict(type='BN'),
                 act_cfg=None),
             loss_1_tfeat=dict(type='OFDTeacherConnector'),
             loss_2_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=64,
                 out_channel=128,
                 norm_cfg=dict(type='BN'),
                 act_cfg=None),
             loss_2_tfeat=dict(type='OFDTeacherConnector'),
             loss_3_sfeat=dict(
-                type='ConvModuleConncetor',
+                type='ConvModuleConnector',
                 in_channel=128,
                 out_channel=256,
                 norm_cfg=dict(type='BN'),
                 act_cfg=None),
             loss_3_tfeat=dict(type='OFDTeacherConnector')),
         loss_forward_mappings=dict(
             loss_1=dict(
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/rkd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/rkd/metafile.yml`

 * *Files 3% similar despite different names*

```diff
@@ -31,8 +31,8 @@
           Top 5 Accuracy: 91.59
     Results:
       - Task: Image Classification
         Dataset: ImageNet-1k
         Metrics:
           Top 1 Accuracy: 70.23
     Config: configs/distill/mmcls/rkd/rkd_neck_resnet34_resnet18_8xb32_in1k.py
-    Weights: https://download.openmmlab.com/mmrazor/v0.3/distill/rkd/rkd_neck_resnet34_resnet18_8xb32_in1k_acc-70.23_20220401-f25700ac.pth
+    Weights: https://download.openmmlab.com/mmrazor/v1/rkd/rkd_neck_resnet34_resnet18_8xb32_in1k_acc-70.23_20220401-a91e223f.pth
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/rkd/rkd_neck_resnet34_resnet18_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/rkd/rkd_neck_resnet34_resnet18_8xb32_in1k.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         std=[58.395, 57.12, 57.375],
         # convert image from BGR to RGB
         bgr_to_rgb=True),
     architecture=dict(
         cfg_path='mmcls::resnet/resnet18_8xb32_in1k.py', pretrained=False),
     teacher=dict(
         cfg_path='mmcls::resnet/resnet34_8xb32_in1k.py', pretrained=True),
-    teacher_ckpt='resnet34_8xb32_in1k_20210831-f257d4e6.pth',
+    teacher_ckpt=  # noqa
+    'https://download.openmmlab.com/mmclassification/v0/resnet/resnet34_8xb32_in1k_20210831-f257d4e6.pth',  # noqa
     distiller=dict(
         type='ConfigurableDistiller',
         student_recorders=dict(
             feat=dict(type='ModuleOutputs', source='neck.gap')),
         teacher_recorders=dict(
             feat=dict(type='ModuleOutputs', source='neck.gap')),
         distill_losses=dict(
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/wsld/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/wsld/metafile.yml`

 * *Files 8% similar despite different names*

```diff
@@ -31,8 +31,8 @@
           Top 5 Accuracy: 91.59
     Results:
       - Task: Image Classification
         Dataset: ImageNet-1k
         Metrics:
           Top 1 Accuracy: 71.54
     Config: configs/distill/mmcls/wsld/wsld_logits_resnet34_resnet18_8xb32_in1k.py
-    Weights: https://download.openmmlab.com/mmrazor/v0.1/distill/wsld/wsld_cls_head_resnet34_resnet18_8xb32_in1k/wsld_cls_head_resnet34_resnet18_8xb32_in1k_acc-71.54_20211222-91f28cf6.pth
+    Weights: https://download.openmmlab.com/mmrazor/v1/wsld/wsld_cls_head_resnet34_resnet18_8xb32_in1k/wsld_cls_head_resnet34_resnet18_8xb32_in1k_acc-71.54_20211222-57925cbf.pth
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/wsld/wsld_logits_resnet34_resnet18_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/wsld/wsld_logits_resnet34_resnet18_8xb32_in1k.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         std=[58.395, 57.12, 57.375],
         # convert image from BGR to RGB
         bgr_to_rgb=True),
     architecture=dict(
         cfg_path='mmcls::resnet/resnet18_8xb32_in1k.py', pretrained=False),
     teacher=dict(
         cfg_path='mmcls::resnet/resnet34_8xb32_in1k.py', pretrained=True),
-    teacher_ckpt='resnet34_8xb32_in1k_20210831-f257d4e6.pth',
+    teacher_ckpt=  # noqa
+    'https://download.openmmlab.com/mmclassification/v0/resnet/resnet34_8xb32_in1k_20210831-f257d4e6.pth',  # noqa
     distiller=dict(
         type='ConfigurableDistiller',
         student_recorders=dict(
             fc=dict(type='ModuleOutputs', source='head.fc'),
             gt_labels=dict(type='ModuleInputs', source='head.loss_module')),
         teacher_recorders=dict(
             fc=dict(type='ModuleOutputs', source='head.fc')),
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/zskt/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/zskt/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmcls/zskt/zskt_backbone_logits_resnet34_resnet18_8xb16_cifar10.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmcls/zskt/zskt_backbone_logits_resnet34_resnet18_8xb16_cifar10.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_frcnn_r101_frcnn_r50_1x_coco.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_frcnn_r101_frcnn_r50_1x_coco.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco_visualization.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco_visualization.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/cwd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/cwd/metafile.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,8 +16,8 @@
         Weights: https://download.openmmlab.com/mmdetection/v2.0/gfl/gfl_r101_fpn_mstrain_2x_coco/gfl_r101_fpn_mstrain_2x_coco_20200629_200126-dd12f847.pth
     Results:
       - Task: Object Detection
         Dataset: COCO
         Metrics:
           box AP: 41.9
     Config: configs/distill/mmdet/cwd/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco.py
-    Weights: https://download.openmmlab.com/mmrazor/v0.1/distill/cwd/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco_20211222-655dff39.pth
+    Weights: https://download.openmmlab.com/mmrazor/v1/cwd/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco_20211222-c134bb21.pth
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/fbkd/fbkd_fpn_faster-rcnn_r101_faster-rcnn_r50_1x_coco.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/fbkd/fbkd_fpn_faster-rcnn_r101_faster-rcnn_r50_1x_coco.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/fbkd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/fbkd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_faster-rcnn_r101_faster-rcnn_r50_2x_coco.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_faster-rcnn_r101_faster-rcnn_r50_2x_coco.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_fcos_x101_retina_r50_1x_coco.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_fcos_x101_retina_r50_1x_coco.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_mask-rcnn_swin_retina_r50_2x_coco.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_mask-rcnn_swin_retina_r50_2x_coco.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_reppoints_x101-dcn_reppoints_r50_2x_coco.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_reppoints_x101-dcn_reppoints_r50_2x_coco.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_retina_x101_retina_r50_2x_coco.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_retina_x101_retina_r50_2x_coco.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_base_ = ['./pkd_fpn_frcnn_r101_frcnn_r50_2x_coco.py']
+_base_ = ['./pkd_fpn_faster-rcnn_r101_faster-rcnn_r50_2x_coco.py']
 
 teacher_ckpt = 'https://download.openmmlab.com/mmdetection/v2.0/retinanet/retinanet_x101_64x4d_fpn_1x_coco/retinanet_x101_64x4d_fpn_1x_coco_20200130-366f5af1.pth'  # noqa: E501
 
 model = dict(
     architecture=dict(
         cfg_path='mmdet::retinanet/retinanet_r50_fpn_2x_coco.py'),
     teacher=dict(
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet3d/pkd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet3d/pkd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmdet3d/pkd/pkd_fpn_fcos3d_r101_fcos3d_r50_8xb2-1x_nus-mono3d.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmdet3d/pkd/pkd_fpn_fcos3d_r101_fcos3d_r50_8xb2-1x_nus-mono3d.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmseg/cwd/cwd_logits_pspnet_r101-d8_pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmseg/cwd/cwd_logits_pspnet_r101-d8_pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/distill/mmseg/cwd/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/distill/mmseg/cwd/metafile.yml`

 * *Files 14% similar despite different names*

```diff
@@ -34,8 +34,8 @@
         Weights: https://download.openmmlab.com/mmsegmentation/v0.5/pspnet/pspnet_r101-d8_512x1024_80k_cityscapes/pspnet_r101-d8_512x1024_80k_cityscapes_20200606_112211-e1e1100f.pth
     Results:
       - Task: Semantic Segmentation
         Dataset: Cityscapes
         Metrics:
           mIoU: 75.54
     Config: configs/distill/mmseg/cwd/cwd_logits_pspnet_r101-d8_pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
-    Weights: https://download.openmmlab.com/mmrazor/v0.1/distill/cwd/cwd_cls_head_pspnet_r101_d8_pspnet_r18_d8_512x1024_cityscapes_80k/cwd_cls_head_pspnet_r101_d8_pspnet_r18_d8_512x1024_cityscapes_80k_mIoU-75.54_20211222-3a26ee1c.pth
+    Weights: https://download.openmmlab.com/mmrazor/v1/cwd/cwd_cls_head_pspnet_r101_d8_pspnet_r18_d8_512x1024_cityscapes_80k/cwd_cls_head_pspnet_r101_d8_pspnet_r18_d8_512x1024_cityscapes_80k_mIoU-75.54_20211222-3e643f6f.pth
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_slimmable_subnet_8xb256_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_slimmable_subnet_8xb256_in1k.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,18 +30,17 @@
     data_preprocessor=data_preprocessor,
     mutator=dict(
         type='SlimmableChannelMutator',
         channel_unit_cfg=dict(
             type='SlimmableChannelUnit',
             units='tests/data/MBV2_slimmable_config.json'),
         parse_cfg=dict(
-            type='BackwardTracer',
-            loss_calculator=dict(type='ImageClassifierPseudoLoss'))))
+            type='ChannelAnalyzer',
+            demo_input=(1, 3, 224, 224),
+            tracer_type='BackwardTracer')))
 
 model_wrapper_cfg = dict(
     type='mmrazor.SlimmableNetworkDDP',
     broadcast_buffers=False,
     find_unused_parameters=True)
 
-optim_wrapper = dict(accumulative_counts=3)
-
 val_cfg = dict(type='mmrazor.SlimmableValLoop')
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_supernet_8xb256_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_supernet_8xb256_in1k.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 _base_ = [
-    'mmrazor::_base_/settings/imagenet_bs2048_autoslim_pil.py',
+    '../../../_base_/settings/imagenet_bs2048_autoslim_pil.py',
     'mmcls::_base_/models/mobilenet_v2_1x.py',
     'mmcls::_base_/default_runtime.py',
 ]
 
 supernet = _base_.model
 supernet.backbone.widen_factor = 1.5
 supernet.head.in_channels = 1920
@@ -17,20 +17,20 @@
     mean=[123.675, 116.28, 103.53],
     std=[58.395, 57.12, 57.375],
     # convert image from BGR to RGB
     bgr_to_rgb=True,
 )
 
 # !autoslim algorithm config
-num_samples = 2
+num_random_samples = 2
 model = dict(
     _delete_=True,
     _scope_='mmrazor',
     type='AutoSlim',
-    num_samples=num_samples,
+    num_random_samples=num_random_samples,
     architecture=supernet,
     data_preprocessor=data_preprocessor,
     distiller=dict(
         type='ConfigurableDistiller',
         teacher_recorders=dict(
             fc=dict(type='ModuleOutputs', source='head.fc')),
         student_recorders=dict(
@@ -46,24 +46,23 @@
         channel_unit_cfg=dict(
             type='OneShotMutableChannelUnit',
             default_args=dict(
                 candidate_choices=list(i / 12 for i in range(2, 13)),
                 choice_mode='ratio',
                 divisor=8)),
         parse_cfg=dict(
-            type='BackwardTracer',
-            loss_calculator=dict(type='ImageClassifierPseudoLoss'))))
+            type='ChannelAnalyzer',
+            demo_input=(1, 3, 224, 224),
+            tracer_type='BackwardTracer')))
 
 model_wrapper_cfg = dict(
     type='mmrazor.AutoSlimDDP',
     broadcast_buffers=False,
     find_unused_parameters=False)
 
-optim_wrapper = dict(accumulative_counts=num_samples + 2)
-
 # learning policy
 max_epochs = 50
 param_scheduler = dict(end=max_epochs)
 
 # train, val, test setting
 train_cfg = dict(max_epochs=max_epochs)
-val_cfg = dict(type='mmrazor.AutoSlimValLoop')
+val_cfg = dict(type='mmrazor.SubnetValLoop')
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/autoslim/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/autoslim/metafile.yml`

 * *Files 3% similar despite different names*

```diff
@@ -22,39 +22,39 @@
       Channel: https://download.openmmlab.com/mmrazor/v1/autoslim/autoslim_mbv2_subnet_8xb256_in1k_flops-530M_acc-74.23_20220715-aa8754fe_subnet_cfg.yaml
     Results:
       - Task: Image Classification
         Dataset: ImageNet-1k
         Metrics:
           Top 1 Accuracy: 74.23
           Top 5 Accuracy: 91.73
-    Config: configs/pruning/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-530M.py
+    Config: configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-530M.py
     Weights: https://download.openmmlab.com/mmrazor/v1/autoslim/autoslim_mbv2_subnet_8xb256_in1k_flops-530M_acc-74.23_20220715-aa8754fe.pth
   - Name: autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-320M
     In Collection: AutoSlim
     Metadata:
       Flops(G): 0.32
       Params(M): 5.77
       Supernet: MobileNet v2(x1.5)
       Channel: https://download.openmmlab.com/mmrazor/v1/autoslim/autoslim_mbv2_subnet_8xb256_in1k_flops-320M_acc-72.73_20220715-9aa8f8ae_subnet_cfg.yaml
     Results:
       - Task: Image Classification
         Dataset: ImageNet-1k
         Metrics:
           Top 1 Accuracy: 72.73
           Top 5 Accuracy: 90.84
-    Config: configs/pruning/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-320M.py
+    Config: configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-320M.py
     Weights: https://download.openmmlab.com/mmrazor/v1/autoslim/autoslim_mbv2_subnet_8xb256_in1k_flops-320M_acc-72.73_20220715-9aa8f8ae.pth
   - Name: autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-220M
     In Collection: AutoSlim
     Metadata:
       Flops(G): 0.22
       Params(M): 4.13
       Supernet: MobileNet v2(x1.5)
       Channel: https://download.openmmlab.com/mmrazor/v1/autoslim/autoslim_mbv2_subnet_8xb256_in1k_flops-220M_acc-71.4_20220715-9c288f3b_subnet_cfg.yaml
     Results:
       - Task: Image Classification
         Dataset: ImageNet-1k
         Metrics:
           Top 1 Accuracy: 71.4
           Top 5 Accuracy: 90.08
-    Config: configs/pruning/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-220M.py
+    Config: configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-220M.py
     Weights: https://download.openmmlab.com/mmrazor/v1/autoslim/autoslim_mbv2_subnet_8xb256_in1k_flops-220M_acc-71.4_20220715-9c288f3b.pth
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/darts/darts_supernet_unroll_1xb96_cifar10.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/darts_supernet_unroll_1xb96_cifar10.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/darts/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/darts/metafile.yml`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     Converted From:
       Code: https://github.com/quark0/darts
 Models:
   - Name: darts_subnet_1xb96_cifar10_2.0
     In Collection: Darts
     Metadata:
       Params(M): 3.42
-      Mutable: https://download.openmmlab.com/mmrazor/v0.1/nas/darts/darts_subnetnet_1xb96_cifar10/darts_subnetnet_1xb96_cifar10_acc-97.32_20211222-e5727921_mutable_cfg.yaml
+      Mutable: https://download.openmmlab.com/mmrazor/v1/darts/darts_subnetnet_1xb96_cifar10_acc-97.32_20211222-e5727921_mutable_cfg.yaml
     Results:
       - Task: Image Classification
         Dataset: CIFAR-10
         Metrics:
           Top 1 Accuracy: 97.32
           Top 5 Accuracy: 99.94
-    Config: configs/nas/darts/darts_subnet_1xb96_cifar10_2.0.py
-    Weights: https://download.openmmlab.com/mmrazor/v0.1/nas/darts/darts_subnetnet_1xb96_cifar10/darts_subnetnet_1xb96_cifar10_acc-97.32_20211222-e5727921.pth
+    Config: configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0.py
+    Weights: https://download.openmmlab.com/mmrazor/v1/darts/darts_subnetnet_1xb96_cifar10_acc-97.32_20211222-23ca1e10.pth
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_supernet_8xb128_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_supernet_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_supernet_8xb128_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_supernet_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_supernet_8xb128_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_supernet_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_supernet_coco_1x.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_supernet_coco_1x.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_retina_shufflenet_supernet_coco_1x.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/detnas_retina_shufflenet_supernet_coco_1x.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/nas/mmdet/detnas/metafile.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/nas/mmdet/detnas/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k_b.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,38 @@
-_base_ = ['mmcls::resnet/resnet34_8xb32_in1k.py']
+_base_ = ['./l1-norm_resnet34_8xb32_in1k_a.py']
 
-stage_ratio_1 = 0.7
-stage_ratio_2 = 0.7
-stage_ratio_3 = 0.7
-stage_ratio_4 = 1.0
+un_prune = 1.0
+stage_ratio_1 = 0.5
+stage_ratio_2 = 0.4
+stage_ratio_3 = 0.6
+stage_ratio_4 = un_prune
 
 # the config template of target_pruning_ratio can be got by
 # python ./tools/get_channel_units.py {config_file} --choice
 target_pruning_ratio = {
-    'backbone.layer1.2.conv2_(0, 64)_64': stage_ratio_1,
+    # stage 1
+    'backbone.conv1_(0, 64)_64': un_prune,  # short cut layers
     'backbone.layer1.0.conv1_(0, 64)_64': stage_ratio_1,
     'backbone.layer1.1.conv1_(0, 64)_64': stage_ratio_1,
-    'backbone.layer1.2.conv1_(0, 64)_64': stage_ratio_1,
-    'backbone.layer2.0.conv1_(0, 128)_128': stage_ratio_2,
-    'backbone.layer2.3.conv2_(0, 128)_128': stage_ratio_2,
+    'backbone.layer1.2.conv1_(0, 64)_64': un_prune,
+    # stage 2
+    'backbone.layer2.0.conv1_(0, 128)_128': un_prune,
+    'backbone.layer2.0.conv2_(0, 128)_128': un_prune,  # short cut layers
     'backbone.layer2.1.conv1_(0, 128)_128': stage_ratio_2,
     'backbone.layer2.2.conv1_(0, 128)_128': stage_ratio_2,
-    'backbone.layer2.3.conv1_(0, 128)_128': stage_ratio_2,
-    'backbone.layer3.0.conv1_(0, 256)_256': stage_ratio_3,
-    'backbone.layer3.5.conv2_(0, 256)_256': stage_ratio_3,
+    'backbone.layer2.3.conv1_(0, 128)_128': un_prune,
+    # stage 3
+    'backbone.layer3.0.conv1_(0, 256)_256': un_prune,
+    'backbone.layer3.0.conv2_(0, 256)_256': un_prune,  # short cut layers
     'backbone.layer3.1.conv1_(0, 256)_256': stage_ratio_3,
     'backbone.layer3.2.conv1_(0, 256)_256': stage_ratio_3,
     'backbone.layer3.3.conv1_(0, 256)_256': stage_ratio_3,
     'backbone.layer3.4.conv1_(0, 256)_256': stage_ratio_3,
-    'backbone.layer3.5.conv1_(0, 256)_256': stage_ratio_3,
+    'backbone.layer3.5.conv1_(0, 256)_256': un_prune,
+    # stage 4
     'backbone.layer4.0.conv1_(0, 512)_512': stage_ratio_4,
-    'backbone.layer4.2.conv2_(0, 512)_512': stage_ratio_4,
+    'backbone.layer4.0.conv2_(0, 512)_512': un_prune,  # short cut layers
     'backbone.layer4.1.conv1_(0, 512)_512': stage_ratio_4,
     'backbone.layer4.2.conv1_(0, 512)_512': stage_ratio_4
 }
-data_preprocessor = {'type': 'mmcls.ClsDataPreprocessor'}
-architecture = _base_.model
-architecture.update({
-    'init_cfg': {
-        'type':
-        'Pretrained',
-        'checkpoint':
-        'https://download.openmmlab.com/mmclassification/v0/resnet/resnet34_8xb32_in1k_20210831-f257d4e6.pth'  # noqa
-    }
-})
 
-model = dict(
-    _delete_=True,
-    _scope_='mmrazor',
-    type='ItePruneAlgorithm',
-    architecture=architecture,
-    mutator_cfg=dict(
-        type='ChannelMutator',
-        channel_unit_cfg=dict(
-            type='L1MutableChannelUnit',
-            default_args=dict(choice_mode='ratio'))),
-    target_pruning_ratio=target_pruning_ratio,
-    step_epoch=1,
-    prune_times=1,
-)
+model = dict(target_pruning_ratio=target_pruning_ratio, )
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/model-index.yml` & `mmrazor-1.0.0rc2/mmrazor/.mim/model-index.yml`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/get_channel_units.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/pruning/get_channel_units.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import argparse
 import json
+import sys
 
 import torch.nn as nn
 from mmengine import MODELS
 from mmengine.config import Config
 
 from mmrazor.models import BaseAlgorithm
 from mmrazor.models.mutators import ChannelMutator
 
+sys.setrecursionlimit(int(pow(2, 20)))
+
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='Get channel unit of a model.')
     parser.add_argument('config', help='config of the model')
     parser.add_argument(
         '-c',
@@ -36,19 +39,33 @@
         help='the file path to store channel unit info')
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     config = Config.fromfile(args.config)
+    default_scope = config['default_scope']
+
     model = MODELS.build(config['model'])
     if isinstance(model, BaseAlgorithm):
         mutator = model.mutator
     elif isinstance(model, nn.Module):
-        mutator = ChannelMutator()
+        mutator: ChannelMutator = ChannelMutator(
+            channel_unit_cfg=dict(
+                type='L1MutableChannelUnit',
+                default_args=dict(choice_mode='ratio'),
+            ),
+            parse_cfg={
+                'type': 'ChannelAnalyzer',
+                'demo_input': {
+                    'type': 'DefaultDemoInput',
+                    'scope': default_scope
+                },
+                'tracer_type': 'FxTracer'
+            })
         mutator.prepare_from_supernet(model)
     if args.choice:
         config = mutator.choice_template
     else:
         config = mutator.config_template(
             with_channels=args.with_channel,
             with_unit_init_args=args.with_init_args)
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/misc/print_config.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/misc/print_config.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/model_converters/convert_kd_ckpt.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/convert_kd_ckpt.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/model_converters/publish_model.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/model_converters/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/slurm_test.sh` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/slurm_train.sh` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/test.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/test.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/train.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/train.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/feature_diff_visualization.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/feature_diff_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def parse_args():
     parser = argparse.ArgumentParser(description='Feature map visualization')
     parser.add_argument('img', help='Image file')
     parser.add_argument(
         'config1', help='train config file path for the first model')
     parser.add_argument(
         'config2', help='train config file path for the second model')
-    parser.add_argument('vis-config', help='visualization config file path')
+    parser.add_argument('vis_config', help='visualization config file path')
     parser.add_argument(
         'checkpoint1', help='Checkpoint file for the first model')
     parser.add_argument(
         'checkpoint2', help='Checkpoint file for the second model')
     parser.add_argument('--out-file', default=None, help='Path to output file')
     parser.add_argument(
         '--device', default='cpu', help='Device used for inference')
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/feature_visualization.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/feature_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from mmrazor.visualization.local_visualizer import modify
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Feature map visualization')
     parser.add_argument('img', help='Image file')
     parser.add_argument('config', help='train config file path')
-    parser.add_argument('vis-config', help='visualization config file path')
+    parser.add_argument('vis_config', help='visualization config file path')
     parser.add_argument('checkpoint', help='Checkpoint file')
     parser.add_argument('--out-file', default=None, help='Path to output file')
     parser.add_argument(
         '--device', default='cpu', help='Device used for inference')
     parser.add_argument('--repo', help='the corresponding repo name')
     parser.add_argument(
         '--use-norm',
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_diff_visualization.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_diff_visualization.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_diff_visualization.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_diff_visualization.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/.mim/tools/visualizations/vis_scheduler.py` & `mmrazor-1.0.0rc2/mmrazor/.mim/tools/visualizations/vis_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             else:
                 val = mapping[version.pre[0]]
             release.extend([val, version.pre[-1]])
         else:
             release.extend([val, 0])
 
     elif version.is_postrelease:
-        release.extend([1, version.post])
+        release.extend([1, version.post])  # type: ignore
     else:
         release.extend([0, 0])
     return tuple(release)
 
 
 mmcv_minimum_version = '2.0.0rc1'
 mmcv_maximum_version = '2.0.0'
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/datasets/crd_dataset_wrapper.py` & `mmrazor-1.0.0rc2/mmrazor/datasets/crd_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/datasets/transforms/formatting.py` & `mmrazor-1.0.0rc2/mmrazor/datasets/transforms/formatting.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/engine/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .hooks import DumpSubnetHook, EstimateResourcesHook
 from .optimizers import SeparateOptimWrapperConstructor
-from .runner import (AutoSlimValLoop, DartsEpochBasedTrainLoop,
+from .runner import (AutoSlimGreedySearchLoop, DartsEpochBasedTrainLoop,
                      DartsIterBasedTrainLoop, EvolutionSearchLoop,
                      GreedySamplerTrainLoop, SelfDistillValLoop,
-                     SingleTeacherDistillValLoop, SlimmableValLoop)
+                     SingleTeacherDistillValLoop, SlimmableValLoop,
+                     SubnetValLoop)
 
 __all__ = [
     'SeparateOptimWrapperConstructor', 'DumpSubnetHook',
     'SingleTeacherDistillValLoop', 'DartsEpochBasedTrainLoop',
     'DartsIterBasedTrainLoop', 'SlimmableValLoop', 'EvolutionSearchLoop',
-    'GreedySamplerTrainLoop', 'AutoSlimValLoop', 'EstimateResourcesHook',
-    'SelfDistillValLoop'
+    'GreedySamplerTrainLoop', 'EstimateResourcesHook', 'SelfDistillValLoop',
+    'AutoSlimGreedySearchLoop', 'SubnetValLoop'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/hooks/dump_subnet_hook.py` & `mmrazor-1.0.0rc2/mmrazor/engine/hooks/dump_subnet_hook.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/hooks/estimate_resources_hook.py` & `mmrazor-1.0.0rc2/mmrazor/engine/hooks/estimate_resources_hook.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Dict, Optional, Sequence
 
 import torch
 from mmengine.hooks import Hook
 from mmengine.registry import HOOKS
 from mmengine.structures import BaseDataElement
 
-from mmrazor.models.task_modules import ResourceEstimator
+from mmrazor.registry import TASK_UTILS
 
 DATA_BATCH = Optional[Sequence[dict]]
 
 
 @HOOKS.register_module()
 class EstimateResourcesHook(Hook):
     """Estimate model resources periodically.
@@ -19,15 +19,15 @@
     Args:
         interval (int): The saving period. If ``by_epoch=True``, interval
             indicates epochs, otherwise it indicates iterations.
             Defaults to -1, which means "never".
         by_epoch (bool): Saving checkpoints by epoch or by iteration.
             Default to True.
         estimator_cfg (Dict[str, Any]): Used for building a resource estimator.
-            Default to dict().
+            Default to None.
 
     Example:
     >>> add the `EstimatorResourcesHook` in custom_hooks as follows:
         custom_hooks = [
             dict(type='mmrazor.EstimateResourcesHook',
                  interval=1,
                  by_epoch=True,
@@ -37,19 +37,22 @@
     out_dir: str
 
     priority = 'VERY_LOW'
 
     def __init__(self,
                  interval: int = -1,
                  by_epoch: bool = True,
-                 estimator_cfg: Dict[str, Any] = dict(),
+                 estimator_cfg: Dict[str, Any] = None,
                  **kwargs) -> None:
         self.interval = interval
         self.by_epoch = by_epoch
-        self.estimator = ResourceEstimator(**estimator_cfg)
+        estimator_cfg = dict() if estimator_cfg is None else estimator_cfg
+        if 'type' not in estimator_cfg:
+            estimator_cfg['type'] = 'mmrazor.ResourceEstimator'
+        self.estimator = TASK_UTILS.build(estimator_cfg)
 
     def after_val_epoch(self,
                         runner,
                         metrics: Optional[Dict[str, float]] = None) -> None:
         """Estimate model resources after every n val epochs.
 
         Args:
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/hooks/visualization_hook.py` & `mmrazor-1.0.0rc2/mmrazor/engine/hooks/visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/optimizers/optimizer_constructor.py` & `mmrazor-1.0.0rc2/mmrazor/engine/optimizers/optimizer_constructor.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/runner/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/engine/runner/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from .autoslim_val_loop import AutoSlimValLoop
+from .autoslim_greedy_search_loop import AutoSlimGreedySearchLoop
 from .darts_loop import DartsEpochBasedTrainLoop, DartsIterBasedTrainLoop
 from .distill_val_loop import SelfDistillValLoop, SingleTeacherDistillValLoop
 from .evolution_search_loop import EvolutionSearchLoop
+from .iteprune_val_loop import ItePruneValLoop
 from .slimmable_val_loop import SlimmableValLoop
 from .subnet_sampler_loop import GreedySamplerTrainLoop
+from .subnet_val_loop import SubnetValLoop
 
 __all__ = [
     'SingleTeacherDistillValLoop', 'DartsEpochBasedTrainLoop',
     'DartsIterBasedTrainLoop', 'SlimmableValLoop', 'EvolutionSearchLoop',
-    'GreedySamplerTrainLoop', 'AutoSlimValLoop', 'SelfDistillValLoop'
+    'GreedySamplerTrainLoop', 'SubnetValLoop', 'SelfDistillValLoop',
+    'ItePruneValLoop', 'AutoSlimGreedySearchLoop'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/runner/autoslim_val_loop.py` & `mmrazor-1.0.0rc2/mmrazor/engine/runner/slimmable_val_loop.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,26 @@
 from torch.utils.data import DataLoader
 
 from mmrazor.models.utils import add_prefix
 from mmrazor.registry import LOOPS
 
 
 @LOOPS.register_module()
-class AutoSlimValLoop(ValLoop):
+class SlimmableValLoop(ValLoop):
+    """Knowledge Distill loop for validation. It is not only validate student,
+    but also validate teacher with the same dataloader.
+
+    Args:
+        runner (Runner): A reference of runner.
+        dataloader (Dataloader or dict): A dataloader object or a dict to
+            build a dataloader.
+        evaluator (Evaluator or dict or list): Used for computing metrics.
+        fp16 (bool): Whether to enable fp16 validation. Defaults to
+            False.
+    """
 
     def __init__(self,
                  runner,
                  dataloader: Union[DataLoader, Dict],
                  evaluator: Union[Evaluator, Dict, List],
                  fp16: bool = False) -> None:
         super().__init__(runner, dataloader, evaluator, fp16)
@@ -28,34 +39,20 @@
         self._model = model
 
     def run(self):
         """Launch validation."""
         self.runner.call_hook('before_val')
 
         all_metrics = dict()
-
-        self._model.set_max_subnet()
-        metrics = self._evaluate_once()
-        all_metrics.update(add_prefix(metrics, 'max_subnet'))
-
-        self._model.set_min_subnet()
-        metrics = self._evaluate_once()
-        all_metrics.update(add_prefix(metrics, 'min_subnet'))
-
-        for subnet_idx in range(self._model.num_samples):
-            self._model.set_subnet(self._model.sample_subnet())
+        for subnet_idx, subnet in enumerate(self._model.mutator.subnets):
+            self.runner.call_hook('before_val_epoch')
+            self.runner.model.eval()
+            self._model.mutator.set_choices(subnet)
+            for idx, data_batch in enumerate(self.dataloader):
+                self.run_iter(idx, data_batch)
             # compute student metrics
-            metrics = self._evaluate_once()
-            all_metrics.update(
-                add_prefix(metrics, f'random_subnet_{subnet_idx}'))
+            metrics = self.evaluator.evaluate(len(self.dataloader.dataset))
+            all_metrics.update(add_prefix(metrics, f'subnet_{subnet_idx}'))
 
         self.runner.call_hook('after_val_epoch', metrics=all_metrics)
 
         self.runner.call_hook('after_val')
-
-    def _evaluate_once(self) -> Dict:
-        self.runner.call_hook('before_val_epoch')
-        self.runner.model.eval()
-        for idx, data_batch in enumerate(self.dataloader):
-            self.run_iter(idx, data_batch)
-
-        return self.evaluator.evaluate(len(self.dataloader.dataset))
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/runner/darts_loop.py` & `mmrazor-1.0.0rc2/mmrazor/engine/runner/darts_loop.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/runner/distill_val_loop.py` & `mmrazor-1.0.0rc2/mmrazor/engine/runner/distill_val_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
             self.teacher.data_preprocessor = data_preprocessor
 
     def run(self):
         """Launch validation."""
         self.runner.call_hook('before_val')
         self.runner.call_hook('before_val_epoch')
         self.runner.model.eval()
-
         for idx, data_batch in enumerate(self.dataloader):
             self.run_iter(idx, data_batch)
         # compute student metrics
         metrics = self.evaluator.evaluate(len(self.dataloader.dataset))
         student_metrics = dict()
         for key, value in metrics.items():
             student_key = 'student.' + key
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/runner/evolution_search_loop.py` & `mmrazor-1.0.0rc2/mmrazor/engine/runner/evolution_search_loop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import os
 import os.path as osp
 import random
+import time
 import warnings
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
+import numpy as np
 import torch
 from mmengine import fileio
 from mmengine.dist import broadcast_object_list
 from mmengine.evaluator import Evaluator
 from mmengine.runner import EpochBasedTrainLoop
 from mmengine.utils import is_list_of
 from torch.utils.data import DataLoader
 
-from mmrazor.models.task_modules import ResourceEstimator
-from mmrazor.registry import LOOPS
+from mmrazor.registry import LOOPS, TASK_UTILS
 from mmrazor.structures import Candidates, export_fix_subnet
 from mmrazor.utils import SupportRandomSubnet
-from .utils import check_subnet_flops, crossover
+from .utils import CalibrateBNMixin, check_subnet_resources, crossover
 
 
 @LOOPS.register_module()
-class EvolutionSearchLoop(EpochBasedTrainLoop):
+class EvolutionSearchLoop(EpochBasedTrainLoop, CalibrateBNMixin):
     """Loop for evolution searching.
 
     Args:
         runner (Runner): A reference of runner.
         dataloader (Dataloader or dict): A dataloader object or a dict to
             build a dataloader.
         evaluator (Evaluator or dict or list): Used for computing metrics.
@@ -37,18 +38,24 @@
         num_candidates (int): The length of candidate pool. Defaults to 50.
         top_k (int): Specify top k candidates based on scores. Defaults to 10.
         num_mutation (int): The number of candidates got by mutation.
             Defaults to 25.
         num_crossover (int): The number of candidates got by crossover.
             Defaults to 25.
         mutate_prob (float): The probability of mutation. Defaults to 0.1.
-        flops_range (tuple, optional): It is used for screening candidates.
-        resource_estimator_cfg (dict): The config for building estimator, which
-            is be used to estimate the flops of sampled subnet. Defaults to
-            None, which means default config is used.
+        crossover_prob (float): The probability of crossover. Defaults to 0.5.
+        calibrate_sample_num (int): The number of images to compute the true
+            average of per-batch mean/variance instead of the running average.
+            Defaults to -1.
+        constraints_range (Dict[str, Any]): Constraints to be used for
+            screening candidates. Defaults to dict(flops=(0, 330)).
+        estimator_cfg (dict, Optional): Used for building a resource estimator.
+            Defaults to None.
+        predictor_cfg (dict, Optional): Used for building a metric predictor.
+            Defaults to None.
         score_key (str): Specify one metric in evaluation results to score
             candidates. Defaults to 'accuracy_top-1'.
         init_candidates (str, optional): The candidates file path, which is
             used to init `self.candidates`. Its format is usually in .yaml
             format. Defaults to None.
     """
 
@@ -60,16 +67,19 @@
                  max_keep_ckpts: int = 3,
                  resume_from: Optional[str] = None,
                  num_candidates: int = 50,
                  top_k: int = 10,
                  num_mutation: int = 25,
                  num_crossover: int = 25,
                  mutate_prob: float = 0.1,
-                 flops_range: Optional[Tuple[float, float]] = (0., 330.),
-                 resource_estimator_cfg: Optional[dict] = None,
+                 crossover_prob: float = 0.5,
+                 calibrate_sample_num: int = -1,
+                 constraints_range: Dict[str, Any] = dict(flops=(0., 330.)),
+                 estimator_cfg: Optional[Dict] = None,
+                 predictor_cfg: Optional[Dict] = None,
                  score_key: str = 'accuracy/top1',
                  init_candidates: Optional[str] = None) -> None:
         super().__init__(runner, dataloader, max_epochs)
         if isinstance(evaluator, dict) or is_list_of(evaluator, dict):
             self.evaluator = runner.build_evaluator(evaluator)  # type: ignore
         else:
             self.evaluator = evaluator  # type: ignore
@@ -79,44 +89,61 @@
             warnings.warn(
                 f'Dataset {self.dataloader.dataset.__class__.__name__} has no '
                 'metainfo. ``dataset_meta`` in evaluator, metric and '
                 'visualizer will be None.')
 
         self.num_candidates = num_candidates
         self.top_k = top_k
-        self.flops_range = flops_range
+        self.constraints_range = constraints_range
+        self.calibrate_sample_num = calibrate_sample_num
         self.score_key = score_key
         self.num_mutation = num_mutation
         self.num_crossover = num_crossover
         self.mutate_prob = mutate_prob
+        self.crossover_prob = crossover_prob
         self.max_keep_ckpts = max_keep_ckpts
         self.resume_from = resume_from
+        self.fp16 = False
 
         if init_candidates is None:
             self.candidates = Candidates()
         else:
             self.candidates = fileio.load(init_candidates)
             assert isinstance(self.candidates, Candidates), 'please use the \
                 correct init candidates file'
 
         self.top_k_candidates = Candidates()
-        if resource_estimator_cfg is None:
-            self.estimator = ResourceEstimator()
-        else:
-            self.estimator = ResourceEstimator(**resource_estimator_cfg)
 
         if self.runner.distributed:
             self.model = runner.model.module
         else:
             self.model = runner.model
 
+        # initialize estimator
+        estimator_cfg = dict() if estimator_cfg is None else estimator_cfg
+        if 'type' not in estimator_cfg:
+            estimator_cfg['type'] = 'mmrazor.ResourceEstimator'
+        self.estimator = TASK_UTILS.build(estimator_cfg)
+
+        # initialize predictor
+        self.use_predictor = False
+        self.predictor_cfg = predictor_cfg
+        if self.predictor_cfg is not None:
+            self.predictor_cfg['score_key'] = self.score_key
+            self.predictor_cfg['search_groups'] = \
+                self.model.mutator.search_groups
+            self.predictor = TASK_UTILS.build(self.predictor_cfg)
+
     def run(self) -> None:
         """Launch searching."""
         self.runner.call_hook('before_train')
 
+        if self.predictor_cfg is not None:
+            self._init_predictor()
+
         if self.resume_from:
             self._resume()
 
         while self._epoch < self._max_epochs:
             self.run_epoch()
             self._save_searcher_ckpt()
 
@@ -124,15 +151,15 @@
 
         self.runner.call_hook('after_train')
 
     def run_epoch(self) -> None:
         """Iterate one epoch.
 
         Steps:
-            1. Sample some new candidates from the supernet.Then Append them
+            1. Sample some new candidates from the supernet. Then Append them
                 to the candidates, Thus make its number equal to the specified
                 number.
             2. Validate these candidates(step 1) and update their scores.
             3. Pick the top k candidates based on the scores(step 2), which
                 will be used in mutation and crossover.
             4. Implement Mutation and crossover, generate better candidates.
         """
@@ -140,100 +167,136 @@
         self.update_candidates_scores()
 
         scores_before = self.top_k_candidates.scores
         self.runner.logger.info(f'top k scores before update: '
                                 f'{scores_before}')
 
         self.candidates.extend(self.top_k_candidates)
-        self.candidates.sort(key=lambda x: x[1], reverse=True)
-        self.top_k_candidates = Candidates(self.candidates[:self.top_k])
+        self.candidates.sort_by(key_indicator='score', reverse=True)
+        self.top_k_candidates = Candidates(self.candidates.data[:self.top_k])
 
         scores_after = self.top_k_candidates.scores
         self.runner.logger.info(f'top k scores after update: '
                                 f'{scores_after}')
 
         mutation_candidates = self.gen_mutation_candidates()
+        self.candidates_mutator_crossover = Candidates(mutation_candidates)
         crossover_candidates = self.gen_crossover_candidates()
-        candidates = mutation_candidates + crossover_candidates
-        assert len(candidates) <= self.num_candidates, 'Total of mutation and \
-            crossover should be no more than the number of candidates.'
+        self.candidates_mutator_crossover.extend(crossover_candidates)
 
-        self.candidates = Candidates(candidates)
+        assert len(self.candidates_mutator_crossover
+                   ) <= self.num_candidates, 'Total of mutation and \
+            crossover should be less than the number of candidates.'
+
+        self.candidates = self.candidates_mutator_crossover
         self._epoch += 1
 
     def sample_candidates(self) -> None:
         """Update candidate pool contains specified number of candicates."""
+        candidates_resources = []
+        init_candidates = len(self.candidates)
         if self.runner.rank == 0:
             while len(self.candidates) < self.num_candidates:
                 candidate = self.model.sample_subnet()
-                if self._check_constraints(random_subnet=candidate):
+                is_pass, result = self._check_constraints(
+                    random_subnet=candidate)
+                if is_pass:
                     self.candidates.append(candidate)
+                    candidates_resources.append(result)
+            self.candidates = Candidates(self.candidates.data)
         else:
-            self.candidates = Candidates([None] * self.num_candidates)
+            self.candidates = Candidates([dict(a=0)] * self.num_candidates)
+
+        if len(candidates_resources) > 0:
+            self.candidates.update_resources(
+                candidates_resources,
+                start=len(self.candidates.data) - len(candidates_resources))
+            assert init_candidates + len(
+                candidates_resources) == self.num_candidates
+
         # broadcast candidates to val with multi-GPUs.
         broadcast_object_list(self.candidates.data)
 
     def update_candidates_scores(self) -> None:
         """Validate candicate one by one from the candicate pool, and update
         top-k candicates."""
         for i, candidate in enumerate(self.candidates.subnets):
             self.model.set_subnet(candidate)
-            metrics = self._val_candidate()
-            score = metrics[self.score_key] \
+            metrics = self._val_candidate(use_predictor=self.use_predictor)
+            score = round(metrics[self.score_key], 2) \
                 if len(metrics) != 0 else 0.
-            self.candidates.set_score(i, score)
+            self.candidates.set_resource(i, score, 'score')
             self.runner.logger.info(
                 f'Epoch:[{self._epoch}/{self._max_epochs}] '
                 f'Candidate:[{i + 1}/{self.num_candidates}] '
-                f'Score:{score}')
+                f'Flops: {self.candidates.resources("flops")[i]} '
+                f'Params: {self.candidates.resources("params")[i]} '
+                f'Latency: {self.candidates.resources("latency")[i]} '
+                f'Score: {self.candidates.scores[i]} ')
 
-    def gen_mutation_candidates(self) -> List:
+    def gen_mutation_candidates(self):
         """Generate specified number of mutation candicates."""
+        mutation_resources = []
         mutation_candidates: List = []
         max_mutate_iters = self.num_mutation * 10
         mutate_iter = 0
         while len(mutation_candidates) < self.num_mutation:
             mutate_iter += 1
             if mutate_iter > max_mutate_iters:
                 break
 
             mutation_candidate = self._mutation()
 
-            if self._check_constraints(random_subnet=mutation_candidate):
+            is_pass, result = self._check_constraints(
+                random_subnet=mutation_candidate)
+            if is_pass:
                 mutation_candidates.append(mutation_candidate)
+                mutation_resources.append(result)
+
+        mutation_candidates = Candidates(mutation_candidates)
+        mutation_candidates.update_resources(mutation_resources)
+
         return mutation_candidates
 
-    def gen_crossover_candidates(self) -> List:
+    def gen_crossover_candidates(self):
         """Generate specofied number of crossover candicates."""
+        crossover_resources = []
         crossover_candidates: List = []
         crossover_iter = 0
         max_crossover_iters = self.num_crossover * 10
         while len(crossover_candidates) < self.num_crossover:
             crossover_iter += 1
             if crossover_iter > max_crossover_iters:
                 break
 
             crossover_candidate = self._crossover()
 
-            if self._check_constraints(random_subnet=crossover_candidate):
+            is_pass, result = self._check_constraints(
+                random_subnet=crossover_candidate)
+            if is_pass:
                 crossover_candidates.append(crossover_candidate)
+                crossover_resources.append(result)
+
+        crossover_candidates = Candidates(crossover_candidates)
+        crossover_candidates.update_resources(crossover_resources)
+
         return crossover_candidates
 
     def _mutation(self) -> SupportRandomSubnet:
         """Mutate with the specified mutate_prob."""
         candidate1 = random.choice(self.top_k_candidates.subnets)
         candidate2 = self.model.sample_subnet()
         candidate = crossover(candidate1, candidate2, prob=self.mutate_prob)
         return candidate
 
     def _crossover(self) -> SupportRandomSubnet:
         """Crossover."""
         candidate1 = random.choice(self.top_k_candidates.subnets)
         candidate2 = random.choice(self.top_k_candidates.subnets)
-        candidate = crossover(candidate1, candidate2)
+        candidate = crossover(candidate1, candidate2, prob=self.crossover_prob)
         return candidate
 
     def _resume(self):
         """Resume searching."""
         if self.runner.rank == 0:
             searcher_resume = fileio.load(self.resume_from)
             for k in searcher_resume.keys():
@@ -245,30 +308,69 @@
             self.runner.logger.info('#' * 100)
 
     def _save_best_fix_subnet(self):
         """Save best subnet in searched top-k candidates."""
         if self.runner.rank == 0:
             best_random_subnet = self.top_k_candidates.subnets[0]
             self.model.set_subnet(best_random_subnet)
-            best_fix_subnet = export_fix_subnet(self.model)
+
+            best_fix_subnet, sliced_model = \
+                export_fix_subnet(self.model, slice_weight=True)
+
+            timestamp_subnet = time.strftime('%Y%m%d_%H%M', time.localtime())
+            model_name = f'subnet_{timestamp_subnet}.pth'
+            save_path = osp.join(self.runner.work_dir, model_name)
+            torch.save({
+                'state_dict': sliced_model.state_dict(),
+                'meta': {}
+            }, save_path)
+            self.runner.logger.info(f'Subnet checkpoint {model_name} saved in '
+                                    f'{self.runner.work_dir}')
+
             save_name = 'best_fix_subnet.yaml'
+            best_fix_subnet = self._convert_fix_subnet(best_fix_subnet)
             fileio.dump(best_fix_subnet,
                         osp.join(self.runner.work_dir, save_name))
             self.runner.logger.info(
-                'Search finished and '
-                f'{save_name} saved in {self.runner.work_dir}.')
+                f'Subnet config {save_name} saved in {self.runner.work_dir}.')
+
+            self.runner.logger.info('Search finished.')
+
+    def _convert_fix_subnet(self, fix_subnet: Dict[str, Any]):
+        """Convert the fixed subnet to avoid python typing error."""
+        from mmrazor.utils.typing import DumpChosen
+
+        converted_fix_subnet = dict()
+        for k, v in fix_subnet.items():
+            assert isinstance(v, DumpChosen)
+            converted_fix_subnet[k] = dict(chosen=v.chosen)
+
+        return converted_fix_subnet
 
     @torch.no_grad()
-    def _val_candidate(self) -> Dict:
-        """Run validation."""
-        self.runner.model.eval()
-        for data_batch in self.dataloader:
-            outputs = self.runner.model.val_step(data_batch)
-            self.evaluator.process(data_samples=outputs, data_batch=data_batch)
-        metrics = self.evaluator.evaluate(len(self.dataloader.dataset))
+    def _val_candidate(self, use_predictor: bool = False) -> Dict:
+        """Run validation.
+
+        Args:
+            use_predictor (bool): Whether to use predictor to get metrics.
+                Defaults to False.
+        """
+        if use_predictor:
+            assert self.predictor is not None
+            metrics = self.predictor.predict(self.model)
+        else:
+            if self.calibrate_sample_num > 0:
+                self.calibrate_bn_statistics(self.runner.train_dataloader,
+                                             self.calibrate_sample_num)
+            self.runner.model.eval()
+            for data_batch in self.dataloader:
+                outputs = self.runner.model.val_step(data_batch)
+                self.evaluator.process(
+                    data_samples=outputs, data_batch=data_batch)
+            metrics = self.evaluator.evaluate(len(self.dataloader.dataset))
         return metrics
 
     def _save_searcher_ckpt(self) -> None:
         """Save searcher ckpt, which is different from common ckpt.
 
         It mainly contains the candicate pool, the top-k candicates with scores
         and the current epoch.
@@ -291,20 +393,61 @@
                 redundant_ckpts = range(1, cur_ckpt - self.max_keep_ckpts)
                 for _step in redundant_ckpts:
                     ckpt_path = osp.join(self.runner.work_dir,
                                          f'search_epoch_{_step}.pkl')
                     if osp.isfile(ckpt_path):
                         os.remove(ckpt_path)
 
-    def _check_constraints(self, random_subnet: SupportRandomSubnet) -> bool:
+    def _check_constraints(
+            self, random_subnet: SupportRandomSubnet) -> Tuple[bool, Dict]:
         """Check whether is beyond constraints.
 
         Returns:
-            bool: The result of checking.
+            bool, result: The result of checking.
         """
-        is_pass = check_subnet_flops(
+        is_pass, results = check_subnet_resources(
             model=self.model,
             subnet=random_subnet,
             estimator=self.estimator,
-            flops_range=self.flops_range)
+            constraints_range=self.constraints_range)
+
+        return is_pass, results
 
-        return is_pass
+    def _init_predictor(self):
+        """Initialize predictor, training is required."""
+        if self.predictor.handler_ckpt:
+            self.predictor.load_checkpoint()
+            self.runner.logger.info(
+                f'Loaded Checkpoints from {self.predictor.handler_ckpt}')
+        else:
+            self.runner.logger.info('No predictor checkpoints found. '
+                                    'Start pre-training the predictor.')
+            if isinstance(self.predictor.train_samples, str):
+                self.runner.logger.info('Find specified samples in '
+                                        f'{self.predictor.train_samples}')
+                train_samples = fileio.load(self.predictor.train_samples)
+                self.candidates = train_samples['subnets']
+            else:
+                self.runner.logger.info(
+                    'Without specified samples. Start random sampling.')
+                temp_num_candidates = self.num_candidates
+                self.num_candidates = self.predictor.train_samples
+
+                assert self.use_predictor is False, (
+                    'Real evaluation is required when initializing predictor.')
+                self.sample_candidates()
+                self.update_candidates_scores()
+                self.num_candidates = temp_num_candidates
+
+            inputs = []
+            for candidate in self.candidates.subnets:
+                inputs.append(self.predictor.model2vector(candidate))
+            inputs = np.array(inputs)
+            labels = np.array(self.candidates.scores)
+            self.predictor.fit(inputs, labels)
+            if self.runner.rank == 0:
+                predictor_dir = self.predictor.save_checkpoint(
+                    osp.join(self.runner.work_dir, 'predictor'))
+                self.runner.logger.info(
+                    f'Predictor pre-trained, saved in {predictor_dir}.')
+            self.use_predictor = True
+            self.candidates = Candidates()
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/runner/subnet_sampler_loop.py` & `mmrazor-1.0.0rc2/mmrazor/engine/runner/subnet_sampler_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import math
 import os
 import random
 from abc import abstractmethod
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import torch
 from mmengine import fileio
 from mmengine.evaluator import Evaluator
 from mmengine.runner import IterBasedTrainLoop
 from mmengine.utils import is_list_of
 from torch.utils.data import DataLoader
 
-from mmrazor.models.task_modules import ResourceEstimator
-from mmrazor.registry import LOOPS
+from mmrazor.registry import LOOPS, TASK_UTILS
 from mmrazor.structures import Candidates
 from mmrazor.utils import SupportRandomSubnet
-from .utils import check_subnet_flops
+from .utils import check_subnet_resources
 
 
 class BaseSamplerTrainLoop(IterBasedTrainLoop):
     """IterBasedTrainLoop for base sampler.
 
     Args:
         runner (Runner): A reference of runner.
@@ -73,43 +72,40 @@
             outputs=outputs)
         self._iter += 1
 
 
 @LOOPS.register_module()
 class GreedySamplerTrainLoop(BaseSamplerTrainLoop):
     """IterBasedTrainLoop for greedy sampler.
-
     In GreedySamplerTrainLoop, `Greedy` means that only use some top
     sampled candidates to train the supernet. So GreedySamplerTrainLoop mainly
     picks the top candidates based on their val socres, then use them to train
     the supernet one by one.
-
     Steps:
         1. Sample from the supernet and the candidates.
         2. Validate these sampled candidates to get each candidate's score.
         3. Get top-k candidates based on their scores, then use them to train
         the supernet one by one.
-
     Args:
         runner (Runner): A reference of runner.
         dataloader (Dataloader or dict): A dataloader object or a dict to
             build a dataloader for training the model.
         dataloader_val (Dataloader or dict): A dataloader object or a dict to
             build a dataloader for evaluating the candidates.
         evaluator (Evaluator or dict or list): Used for computing metrics.
         max_iters (int): Total training iters.
         val_begin (int): The iteration that begins validating.
             Defaults to 1.
         val_interval (int): Validation interval. Defaults to 1000.
         score_key (str): Specify one metric in evaluation results to score
             candidates. Defaults to 'accuracy_top-1'.
-        flops_range (dict): Constraints to be used for screening candidates.
-        resource_estimator_cfg (dict): The config for building estimator, which
-            is be used to estimate the flops of sampled subnet. Defaults to
-            None, which means default config is used.
+        constraints_range (Dict[str, Any]): Constraints to be used for
+            screening candidates. Defaults to dict(flops=(0, 330)).
+        estimator_cfg (dict, Optional): Used for building a resource estimator.
+            Defaults to None.
         num_candidates (int): The number of the candidates consist of samples
             from supernet and itself. Defaults to 1000.
         num_samples (int): The number of sample in each sampling subnet.
             Defaults to 10.
         top_k (int): Choose top_k subnet from the candidates used to train
             the supernet. Defaults to 5.
         prob_schedule (str): The schedule to generate the probablity of
@@ -135,16 +131,16 @@
                  dataloader: Union[Dict, DataLoader],
                  dataloader_val: Union[Dict, DataLoader],
                  evaluator: Union[Evaluator, Dict, List],
                  max_iters: int,
                  val_begin: int = 1,
                  val_interval: int = 1000,
                  score_key: str = 'accuracy/top1',
-                 flops_range: Optional[Tuple[float, float]] = (0., 330),
-                 resource_estimator_cfg: Optional[dict] = None,
+                 constraints_range: Dict[str, Any] = dict(flops=(0, 330)),
+                 estimator_cfg: Optional[Dict] = None,
                  num_candidates: int = 1000,
                  num_samples: int = 10,
                  top_k: int = 5,
                  prob_schedule: str = 'linear',
                  schedule_start_iter: int = 10000,
                  schedule_end_iter: int = 144360,
                  init_prob: float = 0.,
@@ -159,32 +155,34 @@
 
         if isinstance(evaluator, dict) or is_list_of(evaluator, dict):
             self.evaluator = runner.build_evaluator(evaluator)
         else:
             self.evaluator = evaluator
 
         self.score_key = score_key
-        self.flops_range = flops_range
+        self.constraints_range = constraints_range
         self.num_candidates = num_candidates
         self.num_samples = num_samples
         self.top_k = top_k
         assert prob_schedule in ['linear', 'consine']
         self.prob_schedule = prob_schedule
         self.schedule_start_iter = schedule_start_iter
         self.schedule_end_iter = schedule_end_iter
         self.init_prob = init_prob
         self.max_prob = max_prob
         self.cur_prob: float = 0.
 
         self.candidates = Candidates()
         self.top_k_candidates = Candidates()
-        if resource_estimator_cfg is None:
-            self.estimator = ResourceEstimator()
-        else:
-            self.estimator = ResourceEstimator(**resource_estimator_cfg)
+
+        # initialize estimator
+        estimator_cfg = dict() if estimator_cfg is None else estimator_cfg
+        if 'type' not in estimator_cfg:
+            estimator_cfg['type'] = 'mmrazor.ResourceEstimator'
+        self.estimator = TASK_UTILS.build(estimator_cfg)
 
     def run(self) -> None:
         """Launch training."""
         self.runner.call_hook('before_train')
         # In iteration-based training loop, we treat the whole training process
         # as a big epoch and execute the corresponding hook.
         self.runner.call_hook('before_train_epoch')
@@ -226,28 +224,30 @@
             sampled_candidates, num_sample_from_supernet = \
                 self.get_candidates_with_sample(num_samples=self.num_samples)
 
             self.candidates.extend(sampled_candidates)
 
             self.update_candidates_scores()
 
-            self.candidates.sort(key=lambda x: x[1], reverse=True)
-            self.candidates = Candidates(self.candidates[:self.num_candidates])
-            self.top_k_candidates = Candidates(self.candidates[:self.top_k])
+            self.candidates.sort_by(key_indicator='score', reverse=True)
+            self.candidates = Candidates(
+                self.candidates.data[:self.num_candidates])
+            self.top_k_candidates = Candidates(
+                self.candidates.data[:self.top_k])
 
             top1_score = self.top_k_candidates.scores[0]
             if (self._iter % self.val_interval) < self.top_k:
                 self.runner.logger.info(
                     f'GreedySampler: [{self._iter:>6d}] '
                     f'prob {self.cur_prob:.3f} '
                     f'num_sample_from_supernet '
                     f'{num_sample_from_supernet}/{self.num_samples} '
                     f'top1_score {top1_score:.3f} '
                     f'cur_num_candidates: {len(self.candidates)}')
-        return self.top_k_candidates.pop(0)[0]
+        return self.top_k_candidates.subnets[0]
 
     def update_cur_prob(self, cur_iter: int) -> None:
         """update current probablity of sampling from the candidates, which is
         generated based on the probablity strategy and current iter."""
         if cur_iter > self.schedule_end_iter:
             self.cur_prob = self.max_prob
         elif cur_iter < self.schedule_start_iter:
@@ -274,29 +274,30 @@
         """Get candidates with sampling from supernet and the candidates based
         on the current probablity."""
         num_sample_from_supernet = 0
         sampled_candidates = Candidates()
         for _ in range(num_samples):
             if random.random() >= self.cur_prob or len(self.candidates) == 0:
                 subnet = self._sample_from_supernet()
-                if self._check_constraints(subnet):
+                is_pass, _ = self._check_constraints(subnet)
+                if is_pass:
                     sampled_candidates.append(subnet)
                 num_sample_from_supernet += 1
             else:
                 sampled_candidates.append(self._sample_from_candidates())
         return sampled_candidates, num_sample_from_supernet
 
     def update_candidates_scores(self) -> None:
         """Update candidates' scores, which are validated with the
         `dataloader_val`."""
         for i, candidate in enumerate(self.candidates.subnets):
             self.model.set_subnet(candidate)
             metrics = self._val_candidate()
             score = metrics[self.score_key] if len(metrics) != 0 else 0.
-            self.candidates.set_score(i, score)
+            self.candidates.set_resource(i, score, 'score')
 
     @torch.no_grad()
     def _val_candidate(self) -> Dict:
         """Run validation."""
         self.runner.model.eval()
         for data_batch in self.dataloader_val:
             outputs = self.runner.model.val_step(data_batch)
@@ -308,30 +309,30 @@
         """Sample from the supernet."""
         subnet = self.model.sample_subnet()
         return subnet
 
     def _sample_from_candidates(self) -> SupportRandomSubnet:
         """Sample from the candidates."""
         assert len(self.candidates) > 0
-        subnet = random.choice(self.candidates)
+        subnet = random.choice(self.candidates.data)
         return subnet
 
-    def _check_constraints(self, random_subnet: SupportRandomSubnet) -> bool:
+    def _check_constraints(self, random_subnet: SupportRandomSubnet):
         """Check whether is beyond constraints.
 
         Returns:
-            bool: The result of checking.
+            bool, result: The result of checking.
         """
-        is_pass = check_subnet_flops(
+        is_pass, results = check_subnet_resources(
             model=self.model,
             subnet=random_subnet,
             estimator=self.estimator,
-            flops_range=self.flops_range)
+            constraints_range=self.constraints_range)
 
-        return is_pass
+        return is_pass, results
 
     def _save_candidates(self) -> None:
         """Save the candidates to init the next searching."""
         save_path = os.path.join(self.runner.work_dir, 'candidates.pkl')
         fileio.dump(self.candidates, save_path)
         self.runner.logger.info(f'candidates.pkl saved in '
                                 f'{self.runner.work_dir}')
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/engine/runner/utils/genetic.py` & `mmrazor-1.0.0rc2/mmrazor/engine/runner/utils/genetic.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/base.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/datafree_distillation.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/datafree_distillation.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/fpn_teacher_distill.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/fpn_teacher_distill.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,24 @@
     ) -> LossResults:
         """Calculate losses from a batch of inputs and data samples."""
 
         losses = dict()
         # If the `override_data` of a delivery is False, the delivery will
         # record the origin data.
         self.distiller.set_deliveries_override(False)
+
+        # Unlike ``SingleTeacherDistill``, teacher will only execute
+        # back + neck, not head, so there will be no loss.
         if self.teacher_trainable:
-            # Unlike ``SingleTeacherDistill``, teacher will only execute
-            # back + neck, not head, so there will be no loss.
             with self.distiller.teacher_recorders, self.distiller.deliveries:
                 _ = self.teacher.extract_feat(batch_inputs)
         else:
             with self.distiller.teacher_recorders, self.distiller.deliveries:
                 with torch.no_grad():
-                    _ = self.teacher(batch_inputs, data_samples, mode='loss')
+                    _ = self.teacher.extract_feat(batch_inputs)
 
         # If the `override_data` of a delivery is True, the delivery will
         # override the origin data with the recorded data.
         self.distiller.set_deliveries_override(True)
         with self.distiller.student_recorders, self.distiller.deliveries:
             student_losses = self.student(
                 batch_inputs, data_samples, mode='loss')
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/overhaul_feature_distillation.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/overhaul_feature_distillation.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/self_distill.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/self_distill.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/distill/configurable/single_teacher_distill.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/distill/configurable/single_teacher_distill.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
         self.teacher = teacher
         if teacher_ckpt:
             # avoid loaded parameters be overwritten
             self.teacher.init_weights()
             _ = load_checkpoint(self.teacher, teacher_ckpt)
         self.teacher_trainable = teacher_trainable
+        if not self.teacher_trainable:
+            for param in self.teacher.parameters():
+                param.requires_grad = False
         self.teacher_norm_eval = teacher_norm_eval
 
         # The student model will not calculate gradients and update parameters
         # in some pretraining process.
         self.student_trainable = student_trainable
 
         # The student loss will not be updated into ``losses`` in some
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/autoslim.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/pruning/slimmable_network.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,229 +5,213 @@
 
 import torch
 from mmengine.model import BaseModel, MMDistributedDataParallel
 from mmengine.optim import OptimWrapper
 from mmengine.structures import BaseDataElement
 from torch import nn
 
-from mmrazor.models.distillers import ConfigurableDistiller
-from mmrazor.models.mutators import OneShotChannelMutator
+from mmrazor.models.mutables import BaseMutable
+from mmrazor.models.mutators import SlimmableChannelMutator
 from mmrazor.models.utils import (add_prefix,
                                   reinitialize_optim_wrapper_count_status)
 from mmrazor.registry import MODEL_WRAPPERS, MODELS
+from mmrazor.structures.subnet.fix_subnet import _dynamic_to_static
 from ..base import BaseAlgorithm
 
-VALID_MUTATOR_TYPE = Union[OneShotChannelMutator, Dict]
-VALID_DISTILLER_TYPE = Union[ConfigurableDistiller, Dict]
+VALID_MUTATOR_TYPE = Union[SlimmableChannelMutator, Dict]
 VALID_PATH_TYPE = Union[str, Path]
 VALID_CHANNEL_CFG_PATH_TYPE = Union[VALID_PATH_TYPE, List[VALID_PATH_TYPE]]
 
 
 @MODELS.register_module()
-class AutoSlim(BaseAlgorithm):
+class SlimmableNetwork(BaseAlgorithm):
+    """Slimmable Neural Networks.
+
+    Please refer to paper
+    [Slimmable Neural Networks](https://arxiv.org/abs/1812.08928) for details.
+
+    Args:
+        mutator (dict | :obj:`SlimmableChannelMutator`): The config of
+            :class:`SlimmableChannelMutator` or built mutator.
+            About the config of mutator, please refer to
+            SlimmableChannelMutator
+        architecture (dict | :obj:`BaseModel`): The config of
+            :class:`BaseModel` or built model.
+        deploy_index (int): index of subnet to be deployed.
+        data_preprocessor (dict | :obj:`torch.nn.Module` | None): The
+            pre-process config of :class:`BaseDataPreprocessor`.
+            Defaults to None.
+        init_cfg (dict | None): The weight initialized config for
+            :class:`BaseModule`. Default to None.
+    """
 
     def __init__(self,
                  mutator: VALID_MUTATOR_TYPE,
-                 distiller: VALID_DISTILLER_TYPE,
                  architecture: Union[BaseModel, Dict],
+                 deploy_index=-1,
                  data_preprocessor: Optional[Union[Dict, nn.Module]] = None,
-                 init_cfg: Optional[Dict] = None,
-                 num_samples: int = 2) -> None:
-        """Implementation of Autoslim algorithm. Please refer to
-        https://arxiv.org/abs/1903.11728 for more details.
-
-        Args:
-            mutator (VALID_MUTATOR_TYPE): config of mutator.
-            distiller (VALID_DISTILLER_TYPE): config of  distiller.
-            architecture (Union[BaseModel, Dict]): the model to be searched.
-            data_preprocessor (Optional[Union[Dict, nn.Module]], optional):
-                data prepocessor. Defaults to None.
-            init_cfg (Optional[Dict], optional): config of initialization.
-                Defaults to None.
-            num_samples (int, optional): number of sample subnets.
-                Defaults to 2.
-        """
+                 init_cfg: Optional[Dict] = None) -> None:
         super().__init__(architecture, data_preprocessor, init_cfg)
 
-        self.mutator: OneShotChannelMutator = MODELS.build(mutator)
-        # prepare_from_supernet` must be called before distiller initialized
+        if isinstance(mutator, dict):
+            self.mutator = MODELS.build(mutator)
+        else:
+            self.mutator = mutator
         self.mutator.prepare_from_supernet(self.architecture)
+        self.num_subnet = len(self.mutator.subnets)
 
-        self.distiller = self._build_distiller(distiller)
-        self.distiller.prepare_from_teacher(self.architecture)
-        self.distiller.prepare_from_student(self.architecture)
-
-        self.num_samples = num_samples
-
+        # must after `prepare_from_supernet`
+        if deploy_index != -1:
+            self._deploy(deploy_index)
+        else:
+            self.is_deployed = False
+
+        # HACK
+        # reinitialize count status of `OptimWrapper` since
+        # `optim_wrapper.update_params` will be called multiple times
+        # in our slimmable train step.
         self._optim_wrapper_count_status_reinitialized = False
 
-    def _build_mutator(self,
-                       mutator: VALID_MUTATOR_TYPE) -> OneShotChannelMutator:
-        """Build mutator."""
-        if isinstance(mutator, dict):
-            mutator = MODELS.build(mutator)
-        if not isinstance(mutator, OneShotChannelMutator):
-            raise TypeError('mutator should be a `dict` or '
-                            '`OneShotModuleMutator` instance, but got '
-                            f'{type(mutator)}')
-
-        return mutator
-
-    def _build_distiller(
-            self, distiller: VALID_DISTILLER_TYPE) -> ConfigurableDistiller:
-        """Build distiller."""
-        if isinstance(distiller, dict):
-            distiller = MODELS.build(distiller)
-        if not isinstance(distiller, ConfigurableDistiller):
-            raise TypeError('distiller should be a `dict` or '
-                            '`ConfigurableDistiller` instance, but got '
-                            f'{type(distiller)}')
-
-        return distiller
-
-    def sample_subnet(self) -> Dict:
-        """Sample a subnet."""
-        return self.mutator.sample_choices()
-
-    def set_subnet(self, subnet) -> None:
-        """Set a subnet."""
-        self.mutator.set_choices(subnet)
-
-    def set_max_subnet(self) -> None:
-        """Set max subnet."""
-        self.mutator.set_choices(self.mutator.max_choices())
-
-    def set_min_subnet(self) -> None:
-        """Set min subnet."""
-        self.mutator.set_choices(self.mutator.min_choices())
-
     def train_step(self, data: List[dict],
                    optim_wrapper: OptimWrapper) -> Dict[str, torch.Tensor]:
         """Train step."""
-
-        def distill_step(
-                batch_inputs: torch.Tensor, data_samples: List[BaseDataElement]
-        ) -> Dict[str, torch.Tensor]:
-            subnet_losses = dict()
-            with optim_wrapper.optim_context(
-                    self), self.distiller.student_recorders:  # type: ignore
-                hard_loss = self(batch_inputs, data_samples, mode='loss')
-                soft_loss = self.distiller.compute_distill_losses()
-
-                subnet_losses.update(hard_loss)
-                subnet_losses.update(soft_loss)
-
-                parsed_subnet_losses, _ = self.parse_losses(subnet_losses)
-                optim_wrapper.update_params(parsed_subnet_losses)
-
-            return subnet_losses
-
+        input_data = self.data_preprocessor(data, True)
+        batch_inputs = input_data['inputs']
+        data_samples = input_data['data_samples']
+        train_kwargs = dict(
+            batch_inputs=batch_inputs,
+            data_samples=data_samples,
+            optim_wrapper=optim_wrapper)
+        if self.is_deployed:
+            return self._fixed_train_step(**train_kwargs)
+        else:
+            return self._slimmable_train_step(**train_kwargs)
+
+    def _slimmable_train_step(
+        self,
+        batch_inputs: torch.Tensor,
+        data_samples: List[BaseDataElement],
+        optim_wrapper: OptimWrapper,
+    ) -> Dict[str, torch.Tensor]:
+        """Train step of Slimmable Network."""
         if not self._optim_wrapper_count_status_reinitialized:
             reinitialize_optim_wrapper_count_status(
                 model=self,
                 optim_wrapper=optim_wrapper,
-                accumulative_counts=self.num_samples + 2)
+                accumulative_counts=self.num_subnet)
             self._optim_wrapper_count_status_reinitialized = True
+        total_losses = dict()
 
-        input_data = self.data_preprocessor(data, True)
-        batch_inputs = input_data['inputs']
-        data_samples = input_data['data_samples']
+        for subnet_idx, subnet in enumerate(self.mutator.subnets):
+            self.mutator.set_choices(subnet)
+            with optim_wrapper.optim_context(self):
+                losses = self(batch_inputs, data_samples, mode='loss')
+            parsed_losses, _ = self.parse_losses(losses)
+            optim_wrapper.update_params(parsed_losses)
 
-        total_losses = dict()
-        self.set_max_subnet()
-        with optim_wrapper.optim_context(
-                self), self.distiller.teacher_recorders:  # type: ignore
-            max_subnet_losses = self(batch_inputs, data_samples, mode='loss')
-            parsed_max_subnet_losses, _ = self.parse_losses(max_subnet_losses)
-            optim_wrapper.update_params(parsed_max_subnet_losses)
-        total_losses.update(add_prefix(max_subnet_losses, 'max_subnet'))
-
-        self.set_min_subnet()
-        min_subnet_losses = distill_step(batch_inputs, data_samples)
-        total_losses.update(add_prefix(min_subnet_losses, 'min_subnet'))
-
-        for sample_idx in range(self.num_samples):
-            self.set_subnet(self.sample_subnet())
-            random_subnet_losses = distill_step(batch_inputs, data_samples)
-            total_losses.update(
-                add_prefix(random_subnet_losses,
-                           f'random_subnet_{sample_idx}'))
+            total_losses.update(add_prefix(losses, f'subnet_{subnet_idx}'))
 
         return total_losses
 
+    def _fixed_train_step(
+        self,
+        batch_inputs: torch.Tensor,
+        data_samples: List[BaseDataElement],
+        optim_wrapper: OptimWrapper,
+    ) -> Dict[str, torch.Tensor]:
+        """Train step of fixed network."""
+        with optim_wrapper.optim_context(self):
+            losses = self(batch_inputs, data_samples, mode='loss')
+        parsed_losses, _ = self.parse_losses(losses)
+        optim_wrapper.update_params(parsed_losses)
+
+        return losses
+
+    def _fix_archtecture(self):
+        for module in self.architecture.modules():
+            if isinstance(module, BaseMutable):
+                if not module.is_fixed:
+                    module.fix_chosen(None)
+
+    def _deploy(self, index: int):
+        self.mutator.set_choices(self.mutator.subnets[index])
+        self.mutator.fix_channel_mutables()
+        self._fix_archtecture()
+        _dynamic_to_static(self.architecture)
+        self.is_deployed = True
+
 
 @MODEL_WRAPPERS.register_module()
-class AutoSlimDDP(MMDistributedDataParallel):
-    """DDPwapper for autoslim."""
+class SlimmableNetworkDDP(MMDistributedDataParallel):
+    """DDP wrapper for Slimmable Neural Network."""
 
     def __init__(self,
                  *,
                  device_ids: Optional[Union[List, int, torch.device]] = None,
                  **kwargs) -> None:
         if device_ids is None:
             if os.environ.get('LOCAL_RANK') is not None:
                 device_ids = [int(os.environ['LOCAL_RANK'])]
         super().__init__(device_ids=device_ids, **kwargs)
 
     def train_step(self, data: List[dict],
                    optim_wrapper: OptimWrapper) -> Dict[str, torch.Tensor]:
-
-        def distill_step(
-                batch_inputs: torch.Tensor, data_samples: List[BaseDataElement]
-        ) -> Dict[str, torch.Tensor]:
-            subnet_losses = dict()
-            with optim_wrapper.optim_context(
-                    self
-            ), self.module.distiller.student_recorders:  # type: ignore
-                hard_loss = self(batch_inputs, data_samples, mode='loss')
-                soft_loss = self.module.distiller.compute_distill_losses()
-
-                subnet_losses.update(hard_loss)
-                subnet_losses.update(soft_loss)
-
-                parsed_subnet_losses, _ = self.module.parse_losses(
-                    subnet_losses)
-                optim_wrapper.update_params(parsed_subnet_losses)
-
-            return subnet_losses
-
+        """Train step."""
+        input_data = self.module.data_preprocessor(data, True)
+        batch_inputs = input_data['inputs']
+        data_samples = input_data['data_samples']
+        train_kwargs = dict(
+            batch_inputs=batch_inputs,
+            data_samples=data_samples,
+            optim_wrapper=optim_wrapper)
+        if self.module.is_deployed:
+            return self._fixed_train_step(**train_kwargs)
+        else:
+            return self._slimmable_train_step(**train_kwargs)
+
+    def _slimmable_train_step(
+        self,
+        batch_inputs: torch.Tensor,
+        data_samples: List[BaseDataElement],
+        optim_wrapper: OptimWrapper,
+    ) -> Dict[str, torch.Tensor]:
+        """Train step of Slimmable Network."""
         if not self._optim_wrapper_count_status_reinitialized:
             reinitialize_optim_wrapper_count_status(
                 model=self,
                 optim_wrapper=optim_wrapper,
-                accumulative_counts=self.module.num_samples + 2)
+                accumulative_counts=self.module.num_subnet)
             self._optim_wrapper_count_status_reinitialized = True
+        total_losses = dict()
 
-        input_data = self.module.data_preprocessor(data, True)
-        batch_inputs = input_data['inputs']
-        data_samples = input_data['data_samples']
+        for subnet_idx, subnet in enumerate(self.module.mutator.subnets):
+            self.module.mutator.set_choices(subnet)
+            with optim_wrapper.optim_context(self):
+                losses = self(batch_inputs, data_samples, mode='loss')
+            parsed_losses, _ = self.module.parse_losses(losses)
+            optim_wrapper.update_params(parsed_losses)
 
-        total_losses = dict()
-        self.module.set_max_subnet()
-        with optim_wrapper.optim_context(
-                self), self.module.distiller.teacher_recorders:  # type: ignore
-            max_subnet_losses = self(batch_inputs, data_samples, mode='loss')
-            parsed_max_subnet_losses, _ = self.module.parse_losses(
-                max_subnet_losses)
-            optim_wrapper.update_params(parsed_max_subnet_losses)
-        total_losses.update(add_prefix(max_subnet_losses, 'max_subnet'))
-
-        self.module.set_min_subnet()
-        min_subnet_losses = distill_step(batch_inputs, data_samples)
-        total_losses.update(add_prefix(min_subnet_losses, 'min_subnet'))
-
-        for sample_idx in range(self.module.num_samples):
-            self.module.set_subnet(self.module.sample_subnet())
-            random_subnet_losses = distill_step(batch_inputs, data_samples)
-            total_losses.update(
-                add_prefix(random_subnet_losses,
-                           f'random_subnet_{sample_idx}'))
+            total_losses.update(add_prefix(losses, f'subnet_{subnet_idx}'))
 
         return total_losses
 
+    def _fixed_train_step(
+        self,
+        batch_inputs: torch.Tensor,
+        data_samples: List[BaseDataElement],
+        optim_wrapper: OptimWrapper,
+    ) -> Dict[str, torch.Tensor]:
+        """Train step of fixed network."""
+        with optim_wrapper.optim_context(self):
+            losses = self(batch_inputs, data_samples, mode='loss')
+        parsed_losses, _ = self.module.parse_losses(losses)
+        optim_wrapper.update_params(parsed_losses)
+
+        return losses
+
     @property
     def _optim_wrapper_count_status_reinitialized(self) -> bool:
         return self.module._optim_wrapper_count_status_reinitialized
 
     @_optim_wrapper_count_status_reinitialized.setter
     def _optim_wrapper_count_status_reinitialized(self, val: bool) -> None:
         assert isinstance(val, bool)
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/darts.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/darts.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def search_subnet(self):
         """Search subnet by mutator."""
         # Avoid circular import
         from mmrazor.structures import export_fix_subnet
 
         subnet = self.mutator.sample_choices()
         self.mutator.set_choices(subnet)
-        return export_fix_subnet(self)
+        return export_fix_subnet(self)[0]
 
     def train(self, mode=True):
         """Convert the model into eval mode while keep normalization layer
         unfreezed."""
 
         super().train(mode)
         if self.norm_training and not mode:
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/dsnas.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/dsnas.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,18 @@
                  estimator_cfg: Dict[str, Any] = None,
                  norm_training: bool = False,
                  data_preprocessor: Optional[Union[dict, nn.Module]] = None,
                  init_cfg: Optional[dict] = None,
                  **kwargs):
         super().__init__(architecture, data_preprocessor, **kwargs)
 
-        if estimator_cfg is None:
-            estimator_cfg = dict(type='mmrazor.ResourceEstimator')
+        # initialize estimator
+        estimator_cfg = dict() if estimator_cfg is None else estimator_cfg
+        if 'type' not in estimator_cfg:
+            estimator_cfg['type'] = 'mmrazor.ResourceEstimator'
         self.estimator = TASK_UTILS.build(estimator_cfg)
         if fix_subnet:
             # Avoid circular import
             from mmrazor.structures import load_fix_subnet
 
             # According to fix_subnet, delete the unchosen part of supernet
             load_fix_subnet(self.architecture, fix_subnet)
@@ -116,15 +118,15 @@
         """Search subnet by mutator."""
 
         # Avoid circular import
         from mmrazor.structures import export_fix_subnet
 
         subnet = self.mutator.sample_choices()
         self.mutator.set_choices(subnet)
-        return export_fix_subnet(self)
+        return export_fix_subnet(self)[0]
 
     def fix_subnet(self):
         """Fix subnet when finetuning."""
         subnet = self.mutator.sample_choices()
         self.mutator.set_choices(subnet)
         for module in self.architecture.modules():
             if isinstance(module, BaseMutable):
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/algorithms/nas/spos.py` & `mmrazor-1.0.0rc2/mmrazor/models/algorithms/nas/spos.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/darts_backbone.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/darts_backbone.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/searchable_mobilenet.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/searchable_mobilenet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 except ImportError:
     from mmrazor.utils import get_placeholder
     BaseBackbone = get_placeholder('mmcls')
     make_divisible = get_placeholder('mmcls')
 
 
 @MODELS.register_module()
-class SearchableMobileNet(BaseBackbone):
-    """Searchable MobileNet backbone.
+class SearchableMobileNetV2(BaseBackbone):
+    """Searchable MobileNetV2 backbone.
 
     Args:
         arch_setting (list[list]): Architecture settings.
         first_channels (int): Channel width of first ConvModule. Default: 32.
         last_channels (int): Channel width of last ConvModule. Default: 1200.
         widen_factor (float): Width multiplier, multiply number of
             channels in each layer by this amount. Default: 1.0.
@@ -66,15 +66,15 @@
         ...     [24, 2, 2, mutable_cfg],
         ...     [32, 3, 2, mutable_cfg],
         ...     [64, 4, 2, mutable_cfg],
         ...     [96, 3, 1, mutable_cfg],
         ...     [160, 3, 2, mutable_cfg],
         ...     [320, 1, 1, mutable_cfg]
         ... ]
-        >>> model = SearchableMobileNet(arch_setting=arch_setting)
+        >>> model = SearchableMobileNetV2(arch_setting=arch_setting)
     """
 
     def __init__(
         self,
         arch_setting: List[List],
         first_channels: int = 32,
         last_channels: int = 1280,
@@ -154,15 +154,15 @@
             act_cfg=self.act_cfg)
 
         self.add_module('conv2', layer)
         self.layers.append('conv2')
 
     def _make_layer(self, out_channels: int, num_blocks: int, stride: int,
                     mutable_cfg: Dict) -> Sequential:
-        """Stack mutable blocks to build a layer for SearchableMobileNet.
+        """Stack mutable blocks to build a layer for SearchableMobileNetV2.
 
         Note:
             Here we use ``module_kwargs`` to pass dynamic parameters such as
             ``in_channels``, ``out_channels`` and ``stride``
             to build the mutable.
 
         Args:
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/searchable_shufflenet_v2.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/searchable_shufflenet_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         with_cp (bool): Use checkpoint or not. Using checkpoint will save some
             memory while slowing down the training speed. Default: False.
         init_cfg (dict | list[dict], optional): initialization configuration
             dict to define initializer. OpenMMLab has implemented
             6 initializers, including ``Constant``, ``Xavier``, ``Normal``,
             ``Uniform``, ``Kaiming``, and ``Pretrained``.
 
-    Excamples:
+    Examples:
         >>> mutable_cfg = dict(
         ...     type='OneShotMutableOP',
         ...     candidates=dict(
         ...         shuffle_3x3=dict(
         ...             type='ShuffleBlock',
         ...             kernel_size=3,
         ...             norm_cfg=dict(type='BN'))))
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/backbones/wideresnet.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/backbones/wideresnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         norm_cfg (dict): The config dict for norm layers.
         norm_eval (bool): Whether to set norm layers to eval mode, namely,
             freeze running stats (mean and var). Note: Effect on Batch Norm
             and its variants only. Default: False.
         zero_init_residual (bool): Whether to use zero init for last norm layer
             in resblocks to let them behave as identity. Default: True.
     """
-    arch_settings = {
+    arch_setting = {
         10: (BasicBlock, (1, 1, 1)),
         16: (BasicBlock, (2, 2, 2)),
         22: (BasicBlock, (3, 3, 3)),
         28: (BasicBlock, (4, 4, 4)),
         40: (BasicBlock, (6, 6, 6)),
     }
 
@@ -293,29 +293,29 @@
         if depth > 40:
             """MMClassication now supports WRN-50 and 101 officially.
 
             Refer to:
             https://github.com/open-mmlab/mmclassification/pull/715/files
             """
             warnings.warn('`WiderResNet` deep than 40 now is deprecated')
-        if depth not in self.arch_settings:
+        if depth not in self.arch_setting:
             raise KeyError(f'invalid depth {depth} for WideResNet')
         self.depth = depth
         self.widen_factor = widen_factor
         self.stem_channels = stem_channels
         self.base_channels = base_channels
         self.num_stages = num_stages
         self.strides = strides
         self.dilations = dilations
         self.frozen_stages = frozen_stages
         self.conv_cfg = conv_cfg
         self.norm_cfg = norm_cfg
         self.norm_eval = norm_eval
         self.zero_init_residual = zero_init_residual
-        self.block, stage_blocks = self.arch_settings[depth]
+        self.block, stage_blocks = self.arch_setting[depth]
         self.stage_blocks = stage_blocks[:num_stages]
         self.expansion = get_expansion(self.block, widen_factor, expansion)
 
         self._make_stem_layer(in_channels, stem_channels)
 
         self.res_layers = []
         _in_channels = stem_channels
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .byot_connector import BYOTConnector
-from .convmodule_connector import ConvModuleConncetor
+from .convmodule_connector import ConvModuleConnector
 from .crd_connector import CRDConnector
 from .factor_transfer_connectors import Paraphraser, Translator
 from .fbkd_connector import FBKDStudentConnector, FBKDTeacherConnector
+from .mgd_connector import MGDConnector
 from .ofd_connector import OFDTeacherConnector
 from .torch_connector import TorchFunctionalConnector, TorchNNConnector
 
 __all__ = [
-    'ConvModuleConncetor', 'Translator', 'Paraphraser', 'BYOTConnector',
+    'ConvModuleConnector', 'Translator', 'Paraphraser', 'BYOTConnector',
     'FBKDTeacherConnector', 'FBKDStudentConnector', 'TorchFunctionalConnector',
-    'CRDConnector', 'TorchNNConnector', 'OFDTeacherConnector'
+    'CRDConnector', 'TorchNNConnector', 'OFDTeacherConnector', 'MGDConnector'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/base_connector.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/base_connector.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/byot_connector.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/byot_connector.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/convmodule_connector.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/convmodule_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from mmcv.cnn import ConvModule
 
 from mmrazor.registry import MODELS
 from .base_connector import BaseConnector
 
 
 @MODELS.register_module()
-class ConvModuleConncetor(BaseConnector):
+class ConvModuleConnector(BaseConnector):
     """Convolution connector that bundles conv/norm/activation layers.
 
     Args:
         in_channel (int): The input channel of the connector.
         out_channel (int): The output channel of the connector.
         kernel_size (int | tuple[int, int]): Size of the convolving kernel.
             Same as that in ``nn._ConvNd``.
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/crd_connector.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/crd_connector.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/factor_transfer_connectors.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/factor_transfer_connectors.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/fbkd_connector.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/fbkd_connector.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/ofd_connector.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/ofd_connector.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/connectors/torch_connector.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/connectors/torch_connector.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_conv.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_conv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import math
 from typing import Callable, Dict
 
+import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 
 from mmrazor.models.mutables.base_mutable import BaseMutable
 from mmrazor.registry import MODELS
 from ..mixins.dynamic_conv_mixins import (BigNasConvMixin, DynamicConvMixin,
-                                          OFAConvMixin)
+                                          FuseConvMixin, OFAConvMixin)
 
 GroupWiseConvWarned = False
 
 
 @MODELS.register_module()
 class DynamicConv2d(nn.Conv2d, DynamicConvMixin):
     """Dynamic Conv2d OP.
@@ -22,52 +24,39 @@
         :obj:`torch.nn.Conv2d`.
 
     Attributes:
         mutable_attrs (ModuleDict[str, BaseMutable]): Mutable attributes,
             such as `in_channels`. The key of the dict must in
             ``accepted_mutable_attrs``.
     """
+    mutable_attrs: nn.ModuleDict
     accepted_mutable_attrs = {'in_channels', 'out_channels'}
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         # TODO
         # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv2d
         assert self.padding_mode == 'zeros'
         self.mutable_attrs: Dict[str, BaseMutable] = nn.ModuleDict()
 
     @classmethod
     def convert_from(cls, module: nn.Conv2d) -> 'DynamicConv2d':
         """Convert an instance of nn.Conv2d to a new instance of
         DynamicConv2d."""
-        # a group-wise conv will not be converted to dynamic conv
-        if module.groups > 1 and not (module.groups == module.out_channels ==
-                                      module.in_channels):
-            global GroupWiseConvWarned
-            if GroupWiseConvWarned is False:
-                from mmengine import MMLogger
-                logger = MMLogger.get_current_instance()
-                logger.warning(
-                    ('Group-wise convolutional layers are not supported to be'
-                     'pruned now, so they are not converted to new'
-                     'DynamicConvs.'))
-                GroupWiseConvWarned = True
-
-            return module
-        else:
-            return cls(
-                in_channels=module.in_channels,
-                out_channels=module.out_channels,
-                kernel_size=module.kernel_size,
-                stride=module.stride,
-                padding=module.padding,
-                dilation=module.dilation,
-                groups=module.groups,
-                bias=True if module.bias is not None else False,
-                padding_mode=module.padding_mode)
+
+        return cls(
+            in_channels=module.in_channels,
+            out_channels=module.out_channels,
+            kernel_size=module.kernel_size,
+            stride=module.stride,
+            padding=module.padding,
+            dilation=module.dilation,
+            groups=module.groups,
+            bias=True if module.bias is not None else False,
+            padding_mode=module.padding_mode)
 
     @property
     def conv_func(self) -> Callable:
         """The function that will be used in ``forward_mixin``."""
         return F.conv2d
 
     @property
@@ -89,14 +78,15 @@
         :obj:`torch.nn.Conv2d`.
 
     Attributes:
         mutable_attrs (ModuleDict[str, BaseMutable]): Mutable attributes,
             such as `in_channels`. The key of the dict must in
             ``accepted_mutable_attrs``.
     """
+    mutable_attrs: nn.ModuleDict
     accepted_mutable_attrs = {'in_channels', 'out_channels', 'kernel_size'}
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         # TODO
         # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv2d
         assert self.padding_mode == 'zeros'
@@ -146,14 +136,15 @@
         :obj:`torch.nn.Conv2d`.
 
     Attributes:
         mutable_attrs (ModuleDict[str, BaseMutable]): Mutable attributes,
             such as `in_channels`. The key of the dict must in
             ``accepted_mutable_attrs``.
     """
+    mutable_attrs: nn.ModuleDict
     accepted_mutable_attrs = {'in_channels', 'out_channels'}
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         # TODO
         # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv2d
         assert self.padding_mode == 'zeros'
@@ -184,7 +175,112 @@
     def static_op_factory(self):
         """Corresponding Pytorch OP."""
         return nn.Conv2d
 
     def forward(self, x: Tensor) -> Tensor:
         """Forward of OFA's conv2d."""
         return self.forward_mixin(x)
+
+
+@MODELS.register_module()
+class FuseConv2d(nn.Conv2d, FuseConvMixin):
+    """FuseConv2d used in `DCFF`.
+
+    Refers to `Training Compact CNNs for Image Classification
+    using Dynamic-coded Filter Fusion <https://arxiv.org/abs/2107.06916>`_.
+    Attributes:
+        mutable_attrs (ModuleDict[str, BaseMutable]): Mutable attributes,
+            such as `in_channels`. The key of the dict must in
+            ``accepted_mutable_attrs``.
+    """
+    mutable_attrs: nn.ModuleDict
+    accepted_mutable_attrs = {'in_channels', 'out_channels'}
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.mutable_attrs: Dict[str, BaseMutable] = nn.ModuleDict()
+
+    @classmethod
+    def convert_from(cls, module: nn.Conv2d) -> 'FuseConv2d':
+        """Convert an instance of `nn.Conv2d` to a new instance of
+        `FuseConv2d`."""
+        return cls(
+            in_channels=module.in_channels,
+            out_channels=module.out_channels,
+            kernel_size=module.kernel_size,
+            stride=module.stride,
+            padding=module.padding,
+            dilation=module.dilation,
+            groups=module.groups,
+            bias=True if module.bias is not None else False,
+            padding_mode=module.padding_mode)
+
+    @property
+    def conv_func(self) -> Callable:
+        """The function that will be used in ``forward_mixin``."""
+        return F.conv2d
+
+    @property
+    def static_op_factory(self):
+        """Corresponding Pytorch OP."""
+        return nn.Conv2d
+
+    def forward(self, x: Tensor) -> Tensor:
+        """Forward of fused conv2d."""
+        return self.forward_mixin(x)
+
+
+class DynamicConv2dAdaptivePadding(DynamicConv2d):
+    """Dynamic version of mmcv.cnn.bricks.Conv2dAdaptivePadding."""
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        img_h, img_w = x.size()[-2:]
+        kernel_h, kernel_w = self.weight.size()[-2:]
+        stride_h, stride_w = self.stride
+        output_h = math.ceil(img_h / stride_h)
+        output_w = math.ceil(img_w / stride_w)
+        pad_h = (
+            max((output_h - 1) * self.stride[0] +
+                (kernel_h - 1) * self.dilation[0] + 1 - img_h, 0))
+        pad_w = (
+            max((output_w - 1) * self.stride[1] +
+                (kernel_w - 1) * self.dilation[1] + 1 - img_w, 0))
+        if pad_h > 0 or pad_w > 0:
+            x = F.pad(x, [
+                pad_w // 2, pad_w - pad_w // 2, pad_h // 2, pad_h - pad_h // 2
+            ])
+        return super().forward(x)
+
+    @property
+    def static_op_factory(self):
+        from mmcv.cnn.bricks import Conv2dAdaptivePadding
+        return Conv2dAdaptivePadding
+
+    def to_static_op(self) -> nn.Conv2d:
+        self.check_if_mutables_fixed()
+
+        weight, bias, padding = self.get_dynamic_params()
+        groups = self.groups
+        if groups == self.in_channels == self.out_channels and \
+                self.mutable_in_channels is not None:
+            mutable_in_channels = self.mutable_attrs['in_channels']
+            groups = mutable_in_channels.current_mask.sum().item()
+        out_channels = weight.size(0)
+        in_channels = weight.size(1) * groups
+
+        kernel_size = tuple(weight.shape[2:])
+
+        static_conv = self.static_op_factory(
+            in_channels=in_channels,
+            out_channels=out_channels,
+            kernel_size=kernel_size,
+            stride=self.stride,
+            padding=padding,
+            dilation=self.dilation,
+            groups=groups,
+            bias=True if bias is not None else False)
+
+        static_conv.weight = nn.Parameter(weight)
+        if bias is not None:
+            static_conv.bias = nn.Parameter(bias)
+
+        return static_conv
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_linear.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/bricks/dynamic_linear.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/dynamic_ops/mixins/dynamic_mixins.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/dynamic_ops/mixins/dynamic_mixins.py`

 * *Files 20% similar despite different names*

```diff
@@ -70,20 +70,24 @@
 
     def check_if_mutables_fixed(self) -> None:
         """Check if all mutables are fixed.
 
         Raises:
             RuntimeError: Error if a existing mutable is not fixed.
         """
+        from mmrazor.models.mutables import (DerivedMutable,
+                                             MutableChannelContainer)
 
         def check_fixed(mutable: Optional[BaseMutable]) -> None:
             if mutable is not None and not mutable.is_fixed:
                 raise RuntimeError(f'Mutable {type(mutable)} is not fixed.')
 
         for mutable in self.mutable_attrs.values():  # type: ignore
+            if isinstance(mutable, (MutableChannelContainer, DerivedMutable)):
+                continue
             check_fixed(mutable)
 
     def check_mutable_attr_valid(self, attr):
         assert attr in self.attr_mappings or \
                     attr in self.accepted_mutable_attrs
 
     @staticmethod
@@ -111,14 +115,19 @@
     """Base class for dynamic OP with mutable channels.
 
     Note:
         All subclass should implement ``mutable_in_channels`` and
         ``mutable_out_channels`` APIs.
     """
 
+    attr_mappings: Dict[str, str] = {
+        'in_channels': 'in_channels',
+        'out_channels': 'out_channels',
+    }
+
     @staticmethod
     def check_mutable_channels(mutable_channels: BaseMutable) -> None:
         """Check if mutable has `currnet_mask` attribute.
 
         Args:
             mutable_channels (BaseMutable): Mutable to be checked.
 
@@ -257,16 +266,20 @@
             eps=self.eps,
             momentum=self.momentum,
             affine=self.affine,
             track_running_stats=self.track_running_stats)
 
         if running_mean is not None:
             static_bn.running_mean.copy_(running_mean)
+            static_bn.running_mean = static_bn.running_mean.to(
+                running_mean.device)
         if running_var is not None:
             static_bn.running_var.copy_(running_var)
+            static_bn.running_var = static_bn.running_var.to(
+                running_var.device)
         if weight is not None:
             static_bn.weight = nn.Parameter(weight)
         if bias is not None:
             static_bn.bias = nn.Parameter(bias)
 
         return static_bn
 
@@ -393,7 +406,50 @@
             bias=True if bias is not None else False)
 
         static_linear.weight = nn.Parameter(weight)
         if bias is not None:
             static_linear.bias = nn.Parameter(bias)
 
         return static_linear
+
+
+class DynamicResizeMixin(DynamicMixin):
+    """A mixin class for Pytorch InputResizer, which can mutate ``shape``."""
+
+    accepted_mutable_attrs: Set[str] = {'shape'}
+
+    def register_mutable_attr(self, attr, mutable):
+        if attr == 'shape':
+            self._register_mutable_shape(mutable)
+        else:
+            raise NotImplementedError
+
+    def _register_mutable_shape(self, mutable_shape):
+        assert hasattr(self, 'mutable_attrs')
+        current_shape = mutable_shape.current_choice
+        shape_dim = 1 if isinstance(current_shape, int) else len(current_shape)
+        if shape_dim not in [1, 2, 3]:
+            raise ValueError('Expect shape of mutable to be 1, 2 or 3'
+                             f', but got: {shape_dim}.')
+
+        self.mutable_attrs['shape'] = mutable_shape
+
+    def get_dynamic_shape(self):
+        if 'shape' in self.mutable_attrs:
+            current_shape = self.mutable_attrs['shape'].current_choice
+        else:
+            current_shape = None
+        return current_shape
+
+    def to_static_op(self) -> nn.Module:
+        self.check_if_mutables_fixed()
+
+        input_resizer = self.static_op_factory(
+            interpolation_type=self._interpolation_type,  # type:ignore
+            align_corners=self._align_corners,  # type:ignore
+            scale_factor=self._scale_factor)  # type:ignore
+
+        size = self.get_dynamic_shape()
+        if size is not None:
+            input_resizer._size = size
+
+        return input_resizer
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/base_generator.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/dafl_generator.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/dafl_generator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/generators/zskt_generator.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/generators/zskt_generator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/heads/darts_subnet_head.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/heads/darts_subnet_head.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/heads/deit_head.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/heads/deit_head.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/base.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/base.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/common.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/common.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/darts_series.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/darts_series.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/efficientnet_series.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/efficientnet_series.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/gather_tensors.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/gather_tensors.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/architectures/ops/shufflenet_series.py` & `mmrazor-1.0.0rc2/mmrazor/models/architectures/ops/shufflenet_series.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/distillers/base_distiller.py` & `mmrazor-1.0.0rc2/mmrazor/models/distillers/base_distiller.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/distillers/byot_distiller.py` & `mmrazor-1.0.0rc2/mmrazor/models/distillers/byot_distiller.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/distillers/configurable_distiller.py` & `mmrazor-1.0.0rc2/mmrazor/models/distillers/configurable_distiller.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,18 @@
         input can use a different connector in different loss.
 
     Examples:
         >>> distill_losses = dict(
         ...     loss_neck=dict(type='L2Loss', loss_weight=5))
 
         >>> student_recorders = dict(
-        ...     feat = dict(type='ModuleOutputs', sources=['neck.gap']))
+        ...     feat = dict(type='ModuleOutputs', sources='neck.gap'))
 
         >>> teacher_recorders = dict(
-        ...     feat = dict(type='ModuleOutputs', sources=['neck.gap']))
+        ...     feat = dict(type='ModuleOutputs', sources='neck.gap'))
 
         >>> connectors = dict(
         ...     loss_neck_sfeat = dict(
         ...         type='SingleConvConnector', in_channel=32, out_channel=64),
         ...     loss_neck_tfeat = dict(
         ...         type='SingleConvConnector', in_channel=32, out_channel=64))
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/distillers/ofd_distiller.py` & `mmrazor-1.0.0rc2/mmrazor/models/distillers/ofd_distiller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import math
 from operator import attrgetter
 
 import torch
 import torch.nn as nn
-from scipy.stats import norm
+
+try:
+    from scipy.stats import norm
+except ImportError:
+    from mmrazor.utils import get_placeholder
+    norm = get_placeholder('norm')
 
 from mmrazor.registry import MODELS
 from ..architectures.connectors import OFDTeacherConnector
 from ..losses import OFDLoss
 from .configurable_distiller import ConfigurableDistiller
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from .decoupled_kd import DKDLoss
 from .factor_transfer_loss import FTLoss
 from .fbkd_loss import FBKDLoss
 from .kd_soft_ce_loss import KDSoftCELoss
 from .kl_divergence import KLDivergence
 from .l1_loss import L1Loss
 from .l2_loss import L2Loss
+from .mgd_loss import MGDLoss
 from .ofd_loss import OFDLoss
 from .pkd_loss import PKDLoss
 from .relational_kd import AngleWiseRKD, DistanceWiseRKD
 from .weighted_soft_label_distillation import WSLD
 
 __all__ = [
     'ChannelWiseDivergence', 'KLDivergence', 'AngleWiseRKD', 'DistanceWiseRKD',
     'WSLD', 'L2Loss', 'ABLoss', 'DKDLoss', 'KDSoftCELoss', 'ActivationLoss',
     'OnehotLikeLoss', 'InformationEntropyLoss', 'FTLoss', 'ATLoss', 'OFDLoss',
-    'L1Loss', 'FBKDLoss', 'CRDLoss', 'CrossEntropyLoss', 'PKDLoss'
+    'L1Loss', 'FBKDLoss', 'CRDLoss', 'CrossEntropyLoss', 'PKDLoss', 'MGDLoss'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/ab_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/ab_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/at_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/at_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/crd_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/crd_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/cross_entropy_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/cwd.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/cwd.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/dafl_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/dafl_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/decoupled_kd.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/decoupled_kd.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/factor_transfer_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/factor_transfer_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/fbkd_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/fbkd_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/kd_soft_ce_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/kd_soft_ce_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/kl_divergence.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/l1_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/l1_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/l2_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/l2_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/ofd_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/ofd_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/pkd_loss.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/pkd_loss.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/relational_kd.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/relational_kd.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/losses/weighted_soft_label_distillation.py` & `mmrazor-1.0.0rc2/mmrazor/models/losses/weighted_soft_label_distillation.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .base_mutable import BaseMutable
 from .derived_mutable import DerivedMutable
 from .mutable_channel import (BaseMutableChannel, MutableChannelContainer,
                               OneShotMutableChannel, SimpleMutableChannel,
                               SquentialMutableChannel)
-from .mutable_channel.units import (ChannelUnitType, L1MutableChannelUnit,
-                                    MutableChannelUnit,
+from .mutable_channel.units import (ChannelUnitType, DCFFChannelUnit,
+                                    L1MutableChannelUnit, MutableChannelUnit,
                                     OneShotMutableChannelUnit,
                                     SequentialMutableChannelUnit,
                                     SlimmableChannelUnit)
 from .mutable_module import (DiffChoiceRoute, DiffMutableModule, DiffMutableOP,
                              OneHotMutableOP, OneShotMutableModule,
                              OneShotMutableOP)
 from .mutable_value import MutableValue, OneShotMutableValue
@@ -18,9 +18,9 @@
     'OneShotMutableOP', 'OneShotMutableModule', 'DiffMutableOP',
     'DiffChoiceRoute', 'DiffMutableModule', 'DerivedMutable', 'MutableValue',
     'OneShotMutableValue', 'SequentialMutableChannelUnit',
     'L1MutableChannelUnit', 'OneShotMutableChannelUnit',
     'SimpleMutableChannel', 'MutableChannelUnit', 'SlimmableChannelUnit',
     'BaseMutableChannel', 'MutableChannelContainer', 'ChannelUnitType',
     'SquentialMutableChannel', 'OneHotMutableOP', 'OneShotMutableChannel',
-    'BaseMutable'
+    'BaseMutable', 'DCFFChannelUnit'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/base_mutable.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/base_mutable.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/derived_mutable.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/derived_mutable.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,29 +57,36 @@
         expand_ratio: Union[int, float]) -> Callable:  # pragma: no cover
     """Helper function to build `mask_fn` for expand derived mutable."""
     if not hasattr(mutable, 'current_mask'):
         raise ValueError('mutable must have attribute `currnet_mask`')
 
     def fn():
         mask = mutable.current_mask
-        expand_num_channels = int(mask.size(0) * expand_ratio)
-        expand_choice = int(mutable.current_choice * expand_ratio)
+        if isinstance(expand_ratio, int):
+            expand_num_channels = mask.size(0) * expand_ratio
+            expand_choice = mutable.current_choice * expand_ratio
+        elif isinstance(expand_ratio, float):
+            expand_num_channels = int(mask.size(0) * expand_ratio)
+            expand_choice = int(mutable.current_choice * expand_ratio)
+        else:
+            raise NotImplementedError(
+                f'Not support type of expand_ratio: {type(expand_ratio)}')
         expand_mask = torch.zeros(expand_num_channels).bool()
         expand_mask[:expand_choice] = True
 
         return expand_mask
 
     return fn
 
 
 def _divide_and_divise(x: int, ratio: int, divisor: int = 8) -> int:
     """Helper function for divide and divise."""
     new_x = x // ratio
 
-    return make_divisible(new_x, divisor)
+    return make_divisible(new_x, divisor)  # type: ignore
 
 
 def _divide_choice_fn(mutable: MutableProtocol,
                       ratio: int,
                       divisor: int = 8) -> Callable:
     """Helper function to build `choice_fn` for divide derived mutable."""
 
@@ -132,33 +139,70 @@
 
     def derive_same_mutable(self: MutableProtocol) -> 'DerivedMutable':
         """Derive same mutable as the source."""
         return self.derive_expand_mutable(expand_ratio=1)
 
     def derive_expand_mutable(
             self: MutableProtocol,
-            expand_ratio: Union[int, float]) -> 'DerivedMutable':
+            expand_ratio: Union[int, BaseMutable, float]) -> 'DerivedMutable':
         """Derive expand mutable, usually used with `expand_ratio`."""
-        choice_fn = _expand_choice_fn(self, expand_ratio=expand_ratio)
+        # avoid circular import
+        if isinstance(expand_ratio, int):
+            choice_fn = _expand_choice_fn(self, expand_ratio=expand_ratio)
+        elif isinstance(expand_ratio, float):
+            choice_fn = _expand_choice_fn(self, expand_ratio=expand_ratio)
+        elif isinstance(expand_ratio, BaseMutable):
+            current_ratio = expand_ratio.current_choice
+            choice_fn = _expand_choice_fn(self, expand_ratio=current_ratio)
+        else:
+            raise NotImplementedError(
+                f'Not support type of ratio: {type(expand_ratio)}')
 
         mask_fn: Optional[Callable] = None
         if hasattr(self, 'current_mask'):
-            mask_fn = _expand_mask_fn(self, expand_ratio=expand_ratio)
+            if isinstance(expand_ratio, int):
+                mask_fn = _expand_mask_fn(self, expand_ratio=expand_ratio)
+            elif isinstance(expand_ratio, float):
+                mask_fn = _expand_mask_fn(self, expand_ratio=expand_ratio)
+            elif isinstance(expand_ratio, BaseMutable):
+                mask_fn = _expand_mask_fn(self, expand_ratio=current_ratio)
+            else:
+                raise NotImplementedError(
+                    f'Not support type of ratio: {type(expand_ratio)}')
 
         return DerivedMutable(choice_fn=choice_fn, mask_fn=mask_fn)
 
     def derive_divide_mutable(self: MutableProtocol,
-                              ratio: int,
+                              ratio: Union[int, float, BaseMutable],
                               divisor: int = 8) -> 'DerivedMutable':
         """Derive divide mutable, usually used with `make_divisable`."""
-        choice_fn = _divide_choice_fn(self, ratio=ratio, divisor=divisor)
+        from .mutable_channel import BaseMutableChannel
+
+        # avoid circular import
+        if isinstance(ratio, int):
+            choice_fn = _divide_choice_fn(self, ratio=ratio, divisor=divisor)
+            current_ratio = ratio
+        elif isinstance(ratio, float):
+            current_ratio = int(ratio)
+            choice_fn = _divide_choice_fn(self, ratio=current_ratio, divisor=1)
+        elif isinstance(ratio, BaseMutable):
+            current_ratio = int(ratio.current_choice)
+            choice_fn = _divide_choice_fn(self, ratio=current_ratio, divisor=1)
+        else:
+            raise NotImplementedError(
+                f'Not support type of ratio: {type(ratio)}')
 
         mask_fn: Optional[Callable] = None
-        if hasattr(self, 'current_mask'):
-            mask_fn = _divide_mask_fn(self, ratio=ratio, divisor=divisor)
+        if isinstance(self, BaseMutableChannel) and hasattr(
+                self, 'current_mask'):
+            mask_fn = _divide_mask_fn(
+                self, ratio=current_ratio, divisor=divisor)
+        elif getattr(self, 'mask_fn', None):  # OneShotMutableChannel
+            mask_fn = _divide_mask_fn(
+                self, ratio=current_ratio, divisor=divisor)
 
         return DerivedMutable(choice_fn=choice_fn, mask_fn=mask_fn)
 
     @staticmethod
     def derive_concat_mutable(
             mutables: Iterable[MutableChannelProtocol]) -> 'DerivedMutable':
         """Derive concat mutable, usually used with `torch.cat`."""
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .base_mutable_channel import BaseMutableChannel
 from .mutable_channel_container import MutableChannelContainer
-from .oneshot_mutalbe_channel import OneShotMutableChannel
+from .oneshot_mutable_channel import OneShotMutableChannel
 from .sequential_mutable_channel import SquentialMutableChannel
 from .simple_mutable_channel import SimpleMutableChannel
-from .units import (ChannelUnitType, L1MutableChannelUnit, MutableChannelUnit,
-                    OneShotMutableChannelUnit, SequentialMutableChannelUnit,
-                    SlimmableChannelUnit)
+from .units import (ChannelUnitType, DCFFChannelUnit, L1MutableChannelUnit,
+                    MutableChannelUnit, OneShotMutableChannelUnit,
+                    SequentialMutableChannelUnit, SlimmableChannelUnit)
 
 __all__ = [
     'SimpleMutableChannel', 'L1MutableChannelUnit',
     'SequentialMutableChannelUnit', 'MutableChannelUnit',
     'OneShotMutableChannelUnit', 'SlimmableChannelUnit', 'BaseMutableChannel',
     'MutableChannelContainer', 'SquentialMutableChannel', 'ChannelUnitType',
-    'OneShotMutableChannel'
+    'DCFFChannelUnit', 'OneShotMutableChannel'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/base_mutable_channel.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/base_mutable_channel.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/mutable_channel_container.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/mutable_channel_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 
 import torch
 
-from mmrazor.models.architectures.dynamic_ops.mixins import DynamicChannelMixin
 from mmrazor.registry import MODELS
 from mmrazor.utils import IndexDict
+from ...architectures.dynamic_ops.mixins import DynamicChannelMixin
 from .base_mutable_channel import BaseMutableChannel
 from .simple_mutable_channel import SimpleMutableChannel
 
 
 @MODELS.register_module()
 class MutableChannelContainer(BaseMutableChannel):
     """MutableChannelContainer inherits from BaseMutableChannel. However,
@@ -62,30 +62,30 @@
         """Return current mask."""
         return self.current_choice.bool()
 
     # basic extension
 
     def register_mutable(self, mutable_channel: BaseMutableChannel, start: int,
                          end: int):
-        """Register/Store BaseMutableChannel in the MutableChannelContainer  in
+        """Register/Store BaseMutableChannel in the MutableChannelContainer in
         the range [start,end)"""
 
         self.mutable_channels[(start, end)] = mutable_channel
 
     @classmethod
     def register_mutable_channel_to_module(cls,
                                            module: DynamicChannelMixin,
                                            mutable: BaseMutableChannel,
                                            is_to_output_channel=True,
                                            start=0,
                                            end=-1):
         """Register a BaseMutableChannel to a module with
         MutableChannelContainers."""
         if end == -1:
-            end = mutable.num_channels + start
+            end = mutable.current_choice + start
         if is_to_output_channel:
             container: MutableChannelContainer = module.get_mutable_attr(
                 'out_channels')
         else:
             container = module.get_mutable_attr('in_channels')
         assert isinstance(container, MutableChannelContainer)
         container.register_mutable(mutable, start, end)
@@ -96,15 +96,16 @@
         """Assert the current stored BaseMutableChannels are valid to generate
         mask."""
         assert len(self.mutable_channels) > 0
         last_end = 0
         for start, end in self.mutable_channels:
             assert start == last_end
             last_end = end
-        assert last_end == self.num_channels
+        assert last_end == self.num_channels, (
+            f'channel mismatch: {last_end} vs {self.num_channels}')
 
     def _fill_unregistered_range(self):
         """Fill with SimpleMutableChannels in the range without any stored
         BaseMutableChannel.
 
         For example, if a MutableChannelContainer has 10 channels, and only the
         [0,5) is registered with BaseMutableChannels, this method will
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/oneshot_mutalbe_channel.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/oneshot_mutable_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     def __init__(self,
                  num_channels: int,
                  candidate_choices: List[Union[float, int]] = [],
                  choice_mode='number',
                  **kwargs):
         super().__init__(num_channels, choice_mode, **kwargs)
+        candidate_choices.sort()
         self.candidate_choices = candidate_choices
         if candidate_choices == []:
             candidate_choices.append(num_channels if self.is_num_mode else 1.0)
 
     @property
     def current_choice(self) -> Union[int, float]:
         """Get current choice."""
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/sequential_mutable_channel.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/sequential_mutable_channel.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     """
 
     def __init__(self, num_channels: int, choice_mode='number', **kwargs):
 
         super().__init__(num_channels, **kwargs)
         assert choice_mode in ['ratio', 'number']
         self.choice_mode = choice_mode
-        self.mask = torch.ones([self.num_channels]).bool()
 
     @property
     def is_num_mode(self):
         """Get if the choice is number mode."""
         return self.choice_mode == 'number'
 
     @property
@@ -46,22 +45,21 @@
     @current_choice.setter
     def current_choice(self, choice: Union[int, float]):
         """Set choice."""
         if isinstance(choice, float):
             int_choice = self._ratio2num(choice)
         else:
             int_choice = choice
-        mask = torch.zeros([self.num_channels], device=self.mask.device)
-        mask[0:int_choice] = 1
-        self.mask = mask.bool()
+        self.mask.fill_(0.0)
+        self.mask[0:int_choice] = 1.0
 
     @property
     def current_mask(self) -> torch.Tensor:
         """Return current mask."""
-        return self.mask
+        return self.mask.bool()
 
     # methods for
 
     def fix_chosen(self, chosen=...):
         """Fix chosen."""
         if chosen is ...:
             chosen = self.current_choice
@@ -78,28 +76,29 @@
 
         from ..mutable_value import OneShotMutableValue
 
         def expand_choice_fn(mutable1: 'SquentialMutableChannel',
                              mutable2: OneShotMutableValue) -> Callable:
 
             def fn():
-                return mutable1.current_choice * mutable2.current_choice
+                return int(mutable1.current_choice * mutable2.current_choice)
 
             return fn
 
         def expand_mask_fn(mutable1: 'SquentialMutableChannel',
                            mutable2: OneShotMutableValue) -> Callable:
 
             def fn():
                 mask = mutable1.current_mask
                 max_expand_ratio = mutable2.max_choice
                 current_expand_ratio = mutable2.current_choice
-                expand_num_channels = mask.size(0) * max_expand_ratio
+                expand_num_channels = int(mask.size(0) * max_expand_ratio)
 
-                expand_choice = mutable1.current_choice * current_expand_ratio
+                expand_choice = int(mutable1.current_choice *
+                                    current_expand_ratio)
                 expand_mask = torch.zeros(expand_num_channels).bool()
                 expand_mask[:expand_choice] = True
 
                 return expand_mask
 
             return fn
 
@@ -109,18 +108,25 @@
                 mask_fn=expand_mask_fn(self, other))
 
         raise TypeError(f'Unsupported type {type(other)} for mul!')
 
     def __floordiv__(self, other) -> DerivedMutable:
         if isinstance(other, int):
             return self.derive_divide_mutable(other)
+        elif isinstance(other, float):
+            return self.derive_divide_mutable(int(other))
         if isinstance(other, tuple):
             assert len(other) == 2
             return self.derive_divide_mutable(*other)
 
+        from ..mutable_value import OneShotMutableValue
+        if isinstance(other, OneShotMutableValue):
+            ratio = other.current_choice
+            return self.derive_divide_mutable(ratio)
+
         raise TypeError(f'Unsupported type {type(other)} for div!')
 
     def _num2ratio(self, choice: Union[int, float]) -> float:
         """Convert the a number choice to a ratio choice."""
         if isinstance(choice, float):
             return choice
         else:
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/simple_mutable_channel.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/simple_mutable_channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
+from typing import Union
+
 import torch
 
 from mmrazor.registry import MODELS
 from ..derived_mutable import DerivedMutable
 from .base_mutable_channel import BaseMutableChannel
 
 
@@ -14,36 +16,40 @@
 
     Args:
         num_channels (int): number of channels.
     """
 
     def __init__(self, num_channels: int, **kwargs) -> None:
         super().__init__(num_channels, **kwargs)
-        self.mask = torch.ones(num_channels).bool()
+        mask = torch.ones([self.num_channels
+                           ])  # save bool as float for dist training
+        self.register_buffer('mask', mask)
+        self.mask: torch.Tensor
 
     # choice
 
     @property
     def current_choice(self) -> torch.Tensor:
         """Get current choice."""
         return self.mask.bool()
 
     @current_choice.setter
     def current_choice(self, choice: torch.Tensor):
         """Set current choice."""
-        self.mask = choice.to(self.mask.device).bool()
+        self.mask = choice.to(self.mask.device).float()
 
     @property
     def current_mask(self) -> torch.Tensor:
         """Get current mask."""
         return self.current_choice.bool()
 
     # basic extension
 
-    def expand_mutable_channel(self, expand_ratio: int) -> DerivedMutable:
+    def expand_mutable_channel(
+            self, expand_ratio: Union[int, float]) -> DerivedMutable:
         """Get a derived SimpleMutableChannel with expanded mask."""
 
         def _expand_mask():
             mask = self.current_mask
             mask = torch.unsqueeze(
                 mask, -1).expand(list(mask.shape) + [expand_ratio]).flatten(-2)
             return mask
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-
+from .dcff_channel_unit import DCFFChannelUnit
 from .l1_mutable_channel_unit import L1MutableChannelUnit
 from .mutable_channel_unit import ChannelUnitType, MutableChannelUnit
 from .one_shot_mutable_channel_unit import OneShotMutableChannelUnit
 from .sequential_mutable_channel_unit import SequentialMutableChannelUnit
 from .slimmable_channel_unit import SlimmableChannelUnit
 
 __all__ = [
     'L1MutableChannelUnit', 'MutableChannelUnit',
     'SequentialMutableChannelUnit', 'OneShotMutableChannelUnit',
-    'SlimmableChannelUnit', 'ChannelUnitType'
+    'SlimmableChannelUnit', 'ChannelUnitType', 'DCFFChannelUnit'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/channel_unit.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/channel_unit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,135 +1,111 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 from typing import Dict, List
 
 import torch.nn as nn
 from mmengine.model import BaseModule
 
-from mmrazor.structures.graph import ModuleGraph
-from mmrazor.structures.graph.channel_graph import ChannelGraph
-from mmrazor.structures.graph.channel_modules import (BaseChannel,
-                                                      BaseChannelUnit)
-from mmrazor.structures.graph.channel_nodes import \
-    default_channel_node_converter
+from mmrazor.models.architectures.dynamic_ops.mixins import DynamicChannelMixin
+from mmrazor.registry import TASK_UTILS
 
 
 class Channel(BaseModule):
     """Channel records information about channels for pruning.
 
     Args:
         name (str): The name of the channel. When the channel is related with
             a module, the name should be the name of the module in the model.
         module (Any): Module of the channel.
         index (Tuple[int,int]): Index(start,end) of the Channel in the Module
         node (ChannelNode, optional): A ChannelNode corresponding to the
             Channel. Defaults to None.
         is_output_channel (bool, optional): Is the channel output channel.
             Defaults to True.
-        expand_ratio (int, optional): Expand ratio of the mask. Defaults to 1.
     """
 
     # init
 
     def __init__(self,
                  name,
                  module,
                  index,
                  node=None,
-                 is_output_channel=True,
-                 expand_ratio=1) -> None:
+                 is_output_channel=True) -> None:
         super().__init__()
         self.name = name
-        self.module = module
+        self.module: nn.Module = module
         self.index = index
         self.start = index[0]
         self.end = index[1]
 
         self.node = node
 
         self.is_output_channel = is_output_channel
-        self.expand_ratio = expand_ratio
 
     @classmethod
     def init_from_cfg(cls, model: nn.Module, config: Dict):
         """init a Channel using a config which can be generated by
         self.config_template()"""
         name = config['name']
         start = config['start']
         end = config['end']
-        expand_ratio = config['expand_ratio'] \
-            if 'expand_ratio' in config else 1
         is_output_channel = config['is_output_channel']
 
         name2module = dict(model.named_modules())
         name2module.pop('')
         module = name2module[name] if name in name2module else None
         return Channel(
-            name,
-            module, (start, end),
-            is_output_channel=is_output_channel,
-            expand_ratio=expand_ratio)
-
-    @classmethod
-    def init_from_base_channel(cls, base_channel: BaseChannel):
-        """Init from a BaseChannel object."""
-        return cls(
-            base_channel.name,
-            base_channel.module,
-            base_channel.index,
-            node=None,
-            is_output_channel=base_channel.is_output_channel,
-            expand_ratio=base_channel.expand_ratio)
+            name, module, (start, end), is_output_channel=is_output_channel)
 
     # config template
 
     def config_template(self):
         """Generate a config template which can be used to initialize a Channel
         by cls.init_from_cfg(**kwargs)"""
         return {
             'name': self.name,
             'start': self.start,
             'end': self.end,
-            'expand_ratio': self.expand_ratio,
             'is_output_channel': self.is_output_channel
         }
 
     # basic properties
 
     @property
     def num_channels(self) -> int:
         """The number of channels in the Channel."""
         return self.index[1] - self.index[0]
 
     @property
     def is_mutable(self) -> bool:
         """If the channel is prunable."""
-        if isinstance(self.module, nn.Conv2d):
-            # group-wise conv
-            if self.module.groups != 1 and not (self.module.groups ==
-                                                self.module.in_channels ==
-                                                self.module.out_channels):
-                return False
-        return True
+        if self.module is not None:
+            has_prama = len(list(self.module.parameters())) != 0
+            is_dynamic_op = isinstance(self.module, DynamicChannelMixin)
+            return (not has_prama) or is_dynamic_op
+        else:
+            is_unmutable = self.name in [
+                'input_placeholder', 'output_placeholder'
+            ]
+            return not is_unmutable
 
     def __repr__(self) -> str:
         return (f'{self.__class__.__name__}('
                 f'{self.name}, index={self.index}, '
                 f'is_output_channel='
                 f'{"true" if self.is_output_channel else "false"}, '
-                f'expand_ratio={self.expand_ratio}'
                 ')')
 
     def __eq__(self, obj: object) -> bool:
-        if isinstance(obj, BaseChannel):
+        if isinstance(obj, Channel):
             return self.name == obj.name \
                 and self.module == obj.module \
                 and self.index == obj.index \
                 and self.is_output_channel == obj.is_output_channel \
-                and self.expand_ratio == obj.expand_ratio \
                 and self.node == obj.node
         else:
             return False
 
 
 # Channel && ChannelUnit
 
@@ -181,15 +157,15 @@
         if channels is not None:
             for channel_config in channels['input_related']:
                 auto_fill_channel_config(channel_config, False)
                 unit.add_input_related(
                     Channel.init_from_cfg(model, channel_config))
             for channel_config in channels['output_related']:
                 auto_fill_channel_config(channel_config, True)
-                unit.add_ouptut_related(
+                unit.add_output_related(
                     Channel.init_from_cfg(model, channel_config))
         return unit
 
     @classmethod
     def init_from_channel_unit(cls,
                                unit: 'ChannelUnit',
                                args: Dict = {}) -> 'ChannelUnit':
@@ -197,38 +173,24 @@
         args['num_channels'] = unit.num_channels
         mutable_unit = cls(**args)
         mutable_unit.input_related = unit.input_related
         mutable_unit.output_related = unit.output_related
         return mutable_unit
 
     @classmethod
-    def init_from_graph(cls,
-                        graph: ModuleGraph,
-                        unit_args={},
-                        num_input_channel=3) -> List['ChannelUnit']:
-        """Parse a module-graph and get ChannelUnits."""
-
-        def init_from_base_channel_unit(base_channel_unit: BaseChannelUnit):
-            unit = cls(len(base_channel_unit.channel_elems), **unit_args)
-            unit.input_related = [
-                Channel.init_from_base_channel(channel)
-                for channel in base_channel_unit.input_related
-            ]
-            unit.output_related = [
-                Channel.init_from_base_channel(channel)
-                for channel in base_channel_unit.output_related
-            ]
-            return unit
+    def init_from_channel_analyzer(cls, model, analyzer=None):
+        """Init MutableChannelUnits from a ChannelAnalyzer."""
 
-        unit_graph = ChannelGraph.copy_from(graph,
-                                            default_channel_node_converter)
-        unit_graph.forward(num_input_channel)
-        units = unit_graph.collect_units()
-        units = [init_from_base_channel_unit(unit) for unit in units]
-        return units
+        if analyzer is None:
+            from mmrazor.models.task_modules.tracer import ChannelAnalyzer
+            analyzer = ChannelAnalyzer()
+        if isinstance(analyzer, dict):
+            analyzer = TASK_UTILS.build(analyzer)
+        unit_config = analyzer.analyze(model)
+        return [cls.init_from_cfg(model, cfg) for cfg in unit_config.values()]
 
     # tools
 
     @property
     def name(self) -> str:
         """str: name of the unit"""
         if len(self.output_related) + len(self.input_related) > 0:
@@ -255,25 +217,23 @@
             config['init_args'] = {'num_channels': self.num_channels}
         if with_channels:
             config['channels'] = self._channel_dict()
         return config
 
     # node operations
 
-    def add_ouptut_related(self, channel: Channel):
+    def add_output_related(self, channel: Channel):
         """Add a Channel which is output related."""
         assert channel.is_output_channel
-        assert self.num_channels == channel.num_channels
         if channel not in self.output_related:
             self.output_related.append(channel)
 
     def add_input_related(self, channel: Channel):
         """Add a Channel which is input related."""
         assert channel.is_output_channel is False
-        assert self.num_channels == channel.num_channels
         if channel not in self.input_related:
             self.input_related.append(channel)
 
     # others
 
     def extra_repr(self) -> str:
         s = super().extra_repr()
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/l1_mutable_channel_unit.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/l1_mutable_channel_unit.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/mutable_channel_unit.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/mutable_channel_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 """This module defines MutableChannelUnit."""
 import abc
 from collections import Set
 from typing import Dict, List, Type, TypeVar
 
+import torch
 import torch.nn as nn
 
-from mmrazor.models.architectures import dynamic_ops
 from mmrazor.models.architectures.dynamic_ops.mixins import DynamicChannelMixin
 from mmrazor.models.mutables import DerivedMutable
 from mmrazor.models.mutables.mutable_channel import (BaseMutableChannel,
                                                      MutableChannelContainer)
 from .channel_unit import Channel, ChannelUnit
 
 
 class MutableChannelUnit(ChannelUnit):
-
     # init methods
     def __init__(self, num_channels: int, **kwargs) -> None:
         """MutableChannelUnit inherits from ChannelUnit, which manages channels
-        with channel-dependency.
-
-        Compared with ChannelUnit, MutableChannelUnit defines the core
-        interfaces for pruning. By inheriting MutableChannelUnit,
-        we can implement a variant pruning and nas algorithm.
+        with channel-dependency. Compared with ChannelUnit, MutableChannelUnit
+        defines the core interfaces for pruning. By inheriting
+        MutableChannelUnit, we can implement a variant pruning and nas
+        algorithm. These apis includes.
 
-        These apis includes
             - basic property
                 - name
                 - is_mutable
             - before pruning
                 - prepare_for_pruning
             - pruning stage
                 - current_choice
@@ -41,48 +38,61 @@
             num_channels (int): dimension of the channels of the Channel
             objects in the unit.
         """
 
         super().__init__(num_channels)
 
     @classmethod
+    def init_from_cfg(cls, model: nn.Module, config: Dict):
+        """init a Channel using a config which can be generated by
+        self.config_template(), include init choice."""
+        unit = super().init_from_cfg(model, config)
+        # TO DO: add illegal judgement here?
+        if 'choice' in config:
+            unit.current_choice = config['choice']
+        return unit
+
+    @classmethod
     def init_from_mutable_channel(cls, mutable_channel: BaseMutableChannel):
         unit = cls(mutable_channel.num_channels)
         return unit
 
     @classmethod
     def init_from_predefined_model(cls, model: nn.Module):
         """Initialize units using the model with pre-defined dynamicops and
         mutable-channels."""
 
-        def process_container(contanier: MutableChannelContainer,
+        def process_container(container: MutableChannelContainer,
                               module,
                               module_name,
                               mutable2units,
                               is_output=True):
-            for index, mutable in contanier.mutable_channels.items():
+            for index, mutable in container.mutable_channels.items():
+                derived_choices = mutable.current_choice
+                if isinstance(derived_choices, torch.Tensor):
+                    derived_choices = derived_choices.sum().item()
                 if isinstance(mutable, DerivedMutable):
                     source_mutables: Set = \
                         mutable._trace_source_mutables()
                     source_channel_mutables = [
                         mutable for mutable in source_mutables
                         if isinstance(mutable, BaseMutableChannel)
                     ]
                     assert len(source_channel_mutables) == 1, (
                         'only support one mutable channel '
                         'used in DerivedMutable')
-                    mutable = list(source_channel_mutables)[0]
+                    mutable = source_channel_mutables[0]
 
                 if mutable not in mutable2units:
                     mutable2units[mutable] = cls.init_from_mutable_channel(
                         mutable)
 
                 unit: MutableChannelUnit = mutable2units[mutable]
                 if is_output:
-                    unit.add_ouptut_related(
+                    unit.add_output_related(
                         Channel(
                             module_name,
                             module,
                             index,
                             is_output_channel=is_output))
                 else:
                     unit.add_input_related(
@@ -117,15 +127,15 @@
         def traverse(channels: List[Channel]):
             has_dynamic_op = False
             all_channel_prunable = True
             for channel in channels:
                 if channel.is_mutable is False:
                     all_channel_prunable = False
                     break
-                if isinstance(channel.module, dynamic_ops.DynamicChannelMixin):
+                if isinstance(channel.module, DynamicChannelMixin):
                     has_dynamic_op = True
             return has_dynamic_op, all_channel_prunable
 
         input_has_dynamic_op, input_all_prunable = traverse(self.input_related)
         output_has_dynamic_op, output_all_prunable = traverse(
             self.output_related)
 
@@ -219,45 +229,32 @@
                     channel.module = module
 
     @staticmethod
     def _register_channel_container(
             model: nn.Module, container_class: Type[MutableChannelContainer]):
         """register channel container for dynamic ops."""
         for module in model.modules():
-            if isinstance(module, dynamic_ops.DynamicChannelMixin):
+            if isinstance(module, DynamicChannelMixin):
+                in_channels = getattr(module,
+                                      module.attr_mappings['in_channels'], 0)
                 if module.get_mutable_attr('in_channels') is None:
-                    in_channels = 0
-                    if isinstance(module, nn.Conv2d):
-                        in_channels = module.in_channels
-                    elif isinstance(module, nn.modules.batchnorm._BatchNorm):
-                        in_channels = module.num_features
-                    elif isinstance(module, nn.Linear):
-                        in_channels = module.in_features
-                    else:
-                        raise NotImplementedError()
                     module.register_mutable_attr('in_channels',
                                                  container_class(in_channels))
+                out_channels = getattr(module,
+                                       module.attr_mappings['out_channels'], 0)
                 if module.get_mutable_attr('out_channels') is None:
-                    out_channels = 0
-                    if isinstance(module, nn.Conv2d):
-                        out_channels = module.out_channels
-                    elif isinstance(module, nn.modules.batchnorm._BatchNorm):
-                        out_channels = module.num_features
-                    elif isinstance(module, nn.Linear):
-                        out_channels = module.out_features
-                    else:
-                        raise NotImplementedError()
+
                     module.register_mutable_attr('out_channels',
                                                  container_class(out_channels))
 
     def _register_mutable_channel(self, mutable_channel: BaseMutableChannel):
         # register mutable_channel
         for channel in list(self.input_related) + list(self.output_related):
             module = channel.module
-            if isinstance(module, dynamic_ops.DynamicChannelMixin):
+            if isinstance(module, DynamicChannelMixin):
                 container: MutableChannelContainer
                 if channel.is_output_channel and module.get_mutable_attr(
                         'out_channels') is not None:
                     container = module.get_mutable_attr('out_channels')
                 elif channel.is_output_channel is False \
                         and module.get_mutable_attr('in_channels') is not None:
                     container = module.get_mutable_attr('in_channels')
@@ -265,36 +262,38 @@
                     raise NotImplementedError()
 
                 if channel.num_channels == self.num_channels:
                     mutable_channel_ = mutable_channel
                     start = channel.start
                     end = channel.end
                 elif channel.num_channels > self.num_channels:
+
                     if channel.num_channels % self.num_channels == 0:
-                        mutable_channel_ = \
-                            mutable_channel.expand_mutable_channel(
-                                channel.num_channels // self.num_channels)
-                        start = channel.start
-                        end = channel.end
+                        ratio = channel.num_channels // self.num_channels
                     else:
-                        raise NotImplementedError()
+                        ratio = channel.num_channels / self.num_channels
+
+                    mutable_channel_ = \
+                        mutable_channel.expand_mutable_channel(ratio)
+                    start = channel.start
+                    end = channel.end
                 else:
                     raise NotImplementedError()
 
                 if (start, end) in container.mutable_channels:
                     existed = container.mutable_channels[(start, end)]
                     if not isinstance(existed, DerivedMutable):
                         assert mutable_channel is existed
                     else:
                         source_mutables = list(
                             existed._trace_source_mutables())
                         is_same = [
                             mutable_channel is mutable
                             for mutable in source_mutables
                         ]
-                        assert any(is_same)
+                        assert any(is_same), 'existed a mutable channel.'
 
                 else:
                     container.register_mutable(mutable_channel_, start, end)
 
 
 ChannelUnitType = TypeVar('ChannelUnitType', bound=MutableChannelUnit)
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/one_shot_mutable_channel_unit.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/one_shot_mutable_channel_unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import random
 from typing import Dict, List, Union
 
 import torch.nn as nn
 
 from mmrazor.registry import MODELS
-from ..oneshot_mutalbe_channel import OneShotMutableChannel
+from ..oneshot_mutable_channel import OneShotMutableChannel
 from .sequential_mutable_channel_unit import SequentialMutableChannelUnit
 
 
 @MODELS.register_module()
 class OneShotMutableChannelUnit(SequentialMutableChannelUnit):
     """OneShotMutableChannelUnit is for single path supernet such as AutoSlim.
     In single path supernet, each module only has one choice invoked at the
@@ -35,37 +35,41 @@
                  candidate_choices: List[Union[int, float]] = [0.5, 1.0],
                  choice_mode='ratio',
                  divisor=1,
                  min_value=1,
                  min_ratio=0.9) -> None:
         super().__init__(num_channels, choice_mode, divisor, min_value,
                          min_ratio)
+
         candidate_choices = copy.copy(candidate_choices)
         if candidate_choices == []:
             candidate_choices.append(
                 self.num_channels if self.is_num_mode else 1.0)
         self.candidate_choices = self._prepare_candidate_choices(
             candidate_choices, choice_mode)
 
         self.mutable_channel = OneShotMutableChannel(num_channels,
                                                      self.candidate_choices,
                                                      choice_mode)
 
+        self.unit_predefined = False
+
     @classmethod
     def init_from_mutable_channel(cls, mutable_channel: OneShotMutableChannel):
         unit = cls(mutable_channel.num_channels,
                    mutable_channel.candidate_choices,
                    mutable_channel.choice_mode)
         mutable_channel.candidate_choices = unit.candidate_choices
         unit.mutable_channel = mutable_channel
         return unit
 
     def prepare_for_pruning(self, model: nn.Module):
         """Prepare for pruning."""
-        super().prepare_for_pruning(model)
+        if not self.unit_predefined:
+            super().prepare_for_pruning(model)
         self.current_choice = self.max_choice
 
     # ~
 
     def config_template(self,
                         with_init_args=False,
                         with_channels=False) -> Dict:
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/sequential_mutable_channel_unit.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/sequential_mutable_channel_unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import random
 from typing import Dict, Union
 
 import torch.nn as nn
+from mmcv.cnn.bricks import Conv2dAdaptivePadding
 from mmengine import MMLogger
+from mmengine.model.utils import _BatchNormXd
+from mmengine.utils.dl_utils.parrots_wrapper import \
+    SyncBatchNorm as EngineSyncBatchNorm
 
 from mmrazor.models.architectures import dynamic_ops
 from mmrazor.models.utils import make_divisible
 from mmrazor.registry import MODELS
 from ..mutable_channel_container import MutableChannelContainer
 from ..sequential_mutable_channel import SquentialMutableChannel
 from .mutable_channel_unit import MutableChannelUnit
@@ -56,17 +60,22 @@
         return unit
 
     def prepare_for_pruning(self, model: nn.Module):
         """Prepare for pruning, including register mutable channels."""
         # register MutableMask
         self._replace_with_dynamic_ops(
             model, {
+                Conv2dAdaptivePadding:
+                dynamic_ops.DynamicConv2dAdaptivePadding,
                 nn.Conv2d: dynamic_ops.DynamicConv2d,
                 nn.BatchNorm2d: dynamic_ops.DynamicBatchNorm2d,
-                nn.Linear: dynamic_ops.DynamicLinear
+                nn.Linear: dynamic_ops.DynamicLinear,
+                nn.SyncBatchNorm: dynamic_ops.DynamicSyncBatchNorm,
+                EngineSyncBatchNorm: dynamic_ops.DynamicSyncBatchNorm,
+                _BatchNormXd: dynamic_ops.DynamicBatchNormXd,
             })
         self._register_channel_container(model, MutableChannelContainer)
         self._register_mutable_channel(self.mutable_channel)
 
     #  ~
 
     @property
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_channel/units/slimmable_channel_unit.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_channel/units/slimmable_channel_unit.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/diff_mutable_module.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/diff_mutable_module.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/mutable_module.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/mutable_module.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_module/one_shot_mutable_module.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_module/one_shot_mutable_module.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutables/mutable_value/mutable_value.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutables/mutable_value/mutable_value.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         Returns:
             int: Number of choices.
         """
         return len(self.choices)
 
     @property
-    def current_choice(self) -> Optional[Any]:
+    def current_choice(self) -> Value:
         """Current choice of mutable value."""
         return self._current_choice
 
     @current_choice.setter
     def current_choice(self, choice: Any) -> Any:
         """Setter of current choice."""
         if choice not in self.choices:
@@ -112,26 +112,27 @@
 
         self._current_choice = choice
 
     def __rmul__(self, other) -> DerivedMutable:
         """Please refer to method :func:`__mul__`."""
         return self * other
 
-    def __mul__(self, other: int) -> DerivedMutable:
+    def __mul__(self, other: Union[int, float]) -> DerivedMutable:
         """Overload `*` operator.
 
         Args:
             other (int): Expand ratio.
 
         Returns:
             DerivedMutable: Derived expand mutable.
         """
         if isinstance(other, int):
             return self.derive_expand_mutable(other)
-
+        elif isinstance(other, float):
+            return self.derive_expand_mutable(other)
         raise TypeError(f'Unsupported type {type(other)} for mul!')
 
     def __floordiv__(self, other: Union[int, Tuple[int,
                                                    int]]) -> DerivedMutable:
         """Overload `//` operator.
 
         Args:
@@ -139,14 +140,16 @@
                 (divide ratio, divisor) for tuple.
 
         Returns:
             DerivedMutable: Derived divide mutable.
         """
         if isinstance(other, int):
             return self.derive_divide_mutable(other)
+        elif isinstance(other, float):
+            return self.derive_divide_mutable(int(other))
         if isinstance(other, tuple):
             assert len(other) == 2
             return self.derive_divide_mutable(*other)
 
         raise TypeError(f'Unsupported type {type(other)} for div!')
 
     def __repr__(self) -> str:
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutators/base_mutator.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutators/base_mutator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutators/channel_mutator/channel_mutator.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/channel_mutator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
 from typing import Any, Dict, Generic, List, Optional, Tuple, Type, Union
 
 from mmengine import fileio
 from torch.nn import Module, ModuleList
 
-from mmrazor.models.architectures.dynamic_ops import DynamicChannelMixin
 from mmrazor.models.mutables import (ChannelUnitType, MutableChannelUnit,
                                      SequentialMutableChannelUnit)
 from mmrazor.models.mutables.mutable_channel.units.channel_unit import \
     ChannelUnit
-from mmrazor.registry import MODELS
-from mmrazor.structures.graph import ModuleGraph
+from mmrazor.models.task_modules.tracer.channel_analyzer import ChannelAnalyzer
+from mmrazor.registry import MODELS, TASK_UTILS
 from ..base_mutator import BaseMutator
 from ..group_mixin import GroupMixin
 
 
-def is_dynamic_op_for_fx_tracer(module, name):
-    return isinstance(module, DynamicChannelMixin)
-
-
 @MODELS.register_module()
 class ChannelMutator(BaseMutator, Generic[ChannelUnitType], GroupMixin):
     """ChannelMutator manages the pruning structure of a model.
 
     Args:
         channel_unit_cfg (Union[ dict, Type[MutableChannelUnit]], optional):
             The config of ChannelUnits. When the channel_unit_cfg
@@ -42,52 +37,56 @@
             The config template of 'units' can be got using
             MutableChannelUnit.config_template()
             Defaults to SequentialMutableChannelUnit.
 
         parse_cfg (Dict, optional):
             The config to parse the model.
             Defaults to
-                dict( type='BackwardTracer',
-                loss_calculator=dict(type='ImageClassifierPseudoLoss')).
+                dict(
+                     type='ChannelAnalyzer',
+                     demo_input=(1, 3, 224, 224),
+                     tracer_type='BackwardTracer')
 
         custom_groups (list[list[str]], optional): User-defined search groups.
             All searchable modules that are not in ``custom_group`` will be
             grouped separately.
 
         init_cfg (dict, optional): initialization configuration dict for
             BaseModule.
 
     Note:
         There are three ways used in ChannelMutator to parse a model and
         get MutableChannelUnits.
-        1. Using tracer. It needs parse_cfg to be the config of a tracer.
+        1. Using tracer. It needs parse_cfg to be the config of the
+        ChannelAnalyzer.
         2. Using config. When parse_cfg['type']='Config'. It needs that
         channel_unit_cfg['unit']['xxx_unit_name] has a key 'channels'.
         3. Using the model with pre-defined dynamic-ops and mutablechannels:
         When parse_cfg['type']='Predefined'.
     """
 
     # init
 
     def __init__(self,
                  channel_unit_cfg: Union[
                      dict,
                      Type[MutableChannelUnit]] = SequentialMutableChannelUnit,
                  parse_cfg: Dict = dict(
-                     type='BackwardTracer',
-                     loss_calculator=dict(type='ImageClassifierPseudoLoss')),
+                     type='ChannelAnalyzer',
+                     demo_input=(1, 3, 224, 224),
+                     tracer_type='BackwardTracer'),
                  custom_groups: Optional[List[List[str]]] = None,
                  init_cfg: Optional[Dict] = None) -> None:
 
         super().__init__(init_cfg)
 
         # tracer
         if isinstance(parse_cfg, dict):
             assert parse_cfg['type'] in [
-                'RazorFxTracer', 'BackwardTracer', 'Config', 'Predefined'
+                'ChannelAnalyzer', 'Config', 'Predefined'
             ]
         self.parse_cfg = parse_cfg
 
         # units
         self._name2unit: Dict[str, ChannelUnitType] = {}
         self.units: ModuleList[ChannelUnitType] = ModuleList()
 
@@ -104,18 +103,18 @@
     def prepare_from_supernet(self, supernet: Module) -> None:
         """Prepare from a model for pruning.
 
         It includes two steps:
         1. parse the model and get MutableChannelUnits.
         2. call unit.prepare_for_pruning for each unit.
         """
-
         self._name2module = dict(supernet.named_modules())
 
-        if 'Tracer' in self.parse_cfg['type']:
+        if isinstance(self.parse_cfg,
+                      ChannelAnalyzer) or 'Analyzer' in self.parse_cfg['type']:
             units = self._prepare_from_tracer(supernet, self.parse_cfg)
         elif self.parse_cfg['type'] == 'Config':
             units = self._prepare_from_cfg(supernet, self.units_cfg)
         elif self.parse_cfg['type'] == 'Predefined':
             units = self._prepare_from_predefined_model(supernet)
         else:
             raise NotImplementedError()
@@ -209,23 +208,24 @@
         """Get current choices."""
         current_choices = dict()
         for group_id, modules in self.search_groups.items():
             current_choices[group_id] = modules[0].current_choice
 
         return current_choices
 
-    def sample_choices(self) -> Dict[int, Any]:
+    def sample_choices(self, kind: str = 'random') -> Dict[int, Any]:
         """Sampling by search groups.
 
         The sampling result of the first mutable of each group is the sampling
         result of this group.
 
         Returns:
             Dict[int, Any]: Random choices dict.
         """
+        assert kind == 'random', f'unsupported the {kind} sample method.'
         random_choices = dict()
         for group_id, modules in self.search_groups.items():
             random_choices[group_id] = modules[0].sample_choice()
 
         return random_choices
 
     def set_choices(self, choices: Dict[int, Any]) -> None:
@@ -234,14 +234,17 @@
 
         Args:
             choices (Dict[int, Any]): Choices dict. The key is group_id in
                 search groups, and the value is the sampling results
                 corresponding to this group.
         """
         for group_id, modules in self.search_groups.items():
+            if group_id not in choices:
+                # allow optional target_prune_ratio
+                continue
             choice = choices[group_id]
             for module in modules:
                 module.current_choice = choice
 
     @property
     def choice_template(self) -> Dict:
         """Get the chocie template of the Mutator.
@@ -312,28 +315,26 @@
             unit_init_cfg = {}
         else:
             raise NotImplementedError()
         return unit_class, default_unit_args, unit_init_cfg
 
     def _prepare_from_tracer(self, model: Module, parse_cfg: Dict):
         """Initialize units using a tracer."""
-        if 'num_input_channel' in parse_cfg:
-            num_input_channel = parse_cfg.pop('num_input_channel')
-        else:
-            num_input_channel = 3
-        if self.parse_cfg['type'] == 'BackwardTracer':
-            graph = ModuleGraph.init_from_backward_tracer(model, parse_cfg)
-        elif self.parse_cfg['type'] == 'RazorFxTracer':
-            graph = ModuleGraph.init_from_fx_tracer(model, fx_tracer=parse_cfg)
+
+        if isinstance(parse_cfg, Dict):
+            tracer: ChannelAnalyzer = TASK_UTILS.build(parse_cfg)
         else:
-            raise NotImplementedError()
-        self._graph = graph
+            tracer = parse_cfg
+        unit_configs = tracer.analyze(model)
+
         # get ChannelUnits
-        units = ChannelUnit.init_from_graph(
-            graph, num_input_channel=num_input_channel)
+        units = [
+            ChannelUnit.init_from_cfg(model, cfg)
+            for cfg in unit_configs.values()
+        ]
         # convert to MutableChannelUnits
         units = self._convert_channel_unit_to_mutable(units)
         return units
 
     def _prepare_from_cfg(self, model, config: Dict):
         """Initialize units using config dict."""
         assert isinstance(self.channel_unit_cfg, dict)
@@ -354,8 +355,11 @@
 
     def _prepare_from_predefined_model(self, model: Module):
         """Initialize units using the model with pre-defined dynamicops and
         mutable-channels."""
 
         units = self.unit_class.init_from_predefined_model(model)
 
+        for unit in units:
+            unit.unit_predefined = self.unit_default_args.pop(
+                'unit_predefined', False)
         return units
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutators/channel_mutator/slimmable_channel_mutator.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutators/channel_mutator/slimmable_channel_mutator.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,17 @@
         init_cfg (dict, optional): initialization configuration dict for
             BaseModule.
     """
 
     def __init__(self,
                  channel_unit_cfg=dict(type='SlimmableChannelUnit', units={}),
                  parse_cfg=dict(
-                     type='BackwardTracer',
-                     loss_calculator=dict(type='ImageClassifierPseudoLoss')),
+                     type='ChannelAnalyzer',
+                     demo_input=(1, 3, 224, 224),
+                     tracer_type='BackwardTracer'),
                  init_cfg: Optional[Dict] = None) -> None:
 
         super().__init__(channel_unit_cfg, parse_cfg, None, init_cfg)
 
         self.subnets = self._prepare_subnets(self.units_cfg)
 
     def set_choices(self, config: Dict[str, float]):  # type: ignore[override]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/diff_module_mutator.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/diff_module_mutator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/module_mutator.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/module_mutator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/mutators/module_mutator/one_shot_module_mutator.py` & `mmrazor-1.0.0rc2/mmrazor/models/mutators/module_mutator/one_shot_module_mutator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/delivery_manager.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/delivery_manager.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/distill_delivery.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/distill_delivery.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/function_outputs_delivery.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/function_outputs_delivery.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/delivery/method_outputs_delivery.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/delivery/method_outputs_delivery.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/base_estimator.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/base_estimator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/flops_params_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/flops_params_counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,14 +494,17 @@
             print('Warning: variables __flops__ or __params__ are already '
                   'defined for the module' + type(module).__name__ +
                   ' ptflops can affect your code!')
         module.__flops__ = 0
         module.__params__ = 0
 
 
+counter_warning_list = []
+
+
 def get_counter_type(module) -> str:
     """Get counter type of the module based on the module class name.
 
     If the current module counter_type is not in TASK_UTILS._module_dict,
     it will search the base classes of the module to see if it matches any
     base class counter_type.
 
@@ -511,18 +514,21 @@
     counter_type = module.__class__.__name__ + 'Counter'
     if counter_type not in TASK_UTILS._module_dict.keys():
         old_counter_type = counter_type
         assert nn.Module in module.__class__.mro()
         for base_cls in module.__class__.mro():
             if base_cls in get_modules_list():
                 counter_type = base_cls.__name__ + 'Counter'
-                from mmengine import MMLogger
-                logger = MMLogger.get_current_instance()
-                logger.warning(f'`{old_counter_type}` not in op_counters. '
-                               f'Using `{counter_type}` instead.')
+                global counter_warning_list
+                if old_counter_type not in counter_warning_list:
+                    from mmengine import MMLogger
+                    logger = MMLogger.get_current_instance()
+                    logger.warning(f'`{old_counter_type}` not in op_counters. '
+                                   f'Using `{counter_type}` instead.')
+                    counter_warning_list.append(old_counter_type)
                 break
     return counter_type
 
 
 def is_supported_instance(module):
     """Judge whether the module is in TASK_UTILS registry or not."""
     if get_counter_type(module) in TASK_UTILS._module_dict.keys():
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/latency_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/latency_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/activation_layer_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/activation_layer_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/base_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/base_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/conv_layer_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/conv_layer_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/deconv_layer_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/deconv_layer_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/linear_layer_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/linear_layer_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/norm_layer_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/norm_layer_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/pooling_layer_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/pooling_layer_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/counters/op_counters/upsample_layer_counter.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/counters/op_counters/upsample_layer_counter.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/estimators/resource_estimator.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/estimators/resource_estimator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/base_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/base_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/function_inputs_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/function_inputs_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/function_outputs_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/function_outputs_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/method_inputs_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/method_inputs_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/method_outputs_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/method_outputs_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/module_inputs_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/module_inputs_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/module_outputs_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/module_outputs_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/param_recorder.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/param_recorder.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/recorder/recorder_manager.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/recorder/recorder_manager.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/backward_tracer.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/backward_tracer.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/loss_calculator/image_classifier_loss_calculator.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/image_classifier_loss_calculator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/loss_calculator/single_stage_detector_loss_calculator.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/loss_calculator/single_stage_detector_loss_calculator.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/parsers.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/parsers.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/task_modules/tracer/path.py` & `mmrazor-1.0.0rc2/mmrazor/models/task_modules/tracer/path.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/utils/make_divisible.py` & `mmrazor-1.0.0rc2/mmrazor/models/utils/make_divisible.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from typing import Optional
 
+from mmrazor.utils import print_log
+
 warn_once = False
 
 
 def make_divisible(value: int,
                    divisor: int,
                    min_value: Optional[int] = None,
                    min_ratio: float = 0.9) -> int:
@@ -25,19 +27,18 @@
     """
 
     if min_value is None:
         min_value = divisor
     if min_value < divisor:
         global warn_once
         if warn_once is False:
-            from mmengine import MMLogger
-            MMLogger.get_current_instance().warning(
-                (f'min_value=={min_value} should greater or equal to '
-                 f'divisor=={divisor}, '
-                 'so we make min_value equal divisor.'))
+            print_log((f'min_value=={min_value} should greater or equal to '
+                       f'divisor=={divisor}, '
+                       'so we make min_value equal divisor.'),
+                      level='warning')
             warn_once = True
 
         min_value = divisor
 
     new_value = max(min_value, int(value + divisor / 2) // divisor * divisor)
     # Make sure that round down does not go down by more than (1-min_ratio).
     if new_value < min_ratio * value:
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/utils/optim_wrapper.py` & `mmrazor-1.0.0rc2/mmrazor/models/utils/optim_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/models/utils/utils.py` & `mmrazor-1.0.0rc2/mmrazor/models/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/registry/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/registry/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .registry import (DATA_SAMPLERS, DATASETS, HOOKS, LOOPS, METRICS,
                        MODEL_WRAPPERS, MODELS, OPTIM_WRAPPER_CONSTRUCTORS,
                        OPTIM_WRAPPERS, OPTIMIZERS, PARAM_SCHEDULERS,
                        RUNNER_CONSTRUCTORS, RUNNERS, TASK_UTILS, TRANSFORMS,
-                       VISBACKENDS, VISUALIZERS, WEIGHT_INITIALIZERS)
+                       VISBACKENDS, VISUALIZERS, WEIGHT_INITIALIZERS,
+                       sub_model)
 
 __all__ = [
     'RUNNERS', 'RUNNER_CONSTRUCTORS', 'HOOKS', 'DATASETS', 'DATA_SAMPLERS',
     'TRANSFORMS', 'MODELS', 'WEIGHT_INITIALIZERS', 'OPTIMIZERS',
     'OPTIM_WRAPPERS', 'OPTIM_WRAPPER_CONSTRUCTORS', 'TASK_UTILS',
     'PARAM_SCHEDULERS', 'METRICS', 'MODEL_WRAPPERS', 'LOOPS', 'VISBACKENDS',
-    'VISUALIZERS'
+    'VISUALIZERS', 'sub_model'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/registry/registry.py` & `mmrazor-1.0.0rc2/mmrazor/registry/registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 """MMRazor provides 17 registry nodes to support using modules across projects.
 Each node is a child of the root registry in MMEngine.
 
 More details can be found at
 https://mmengine.readthedocs.io/en/latest/tutorials/registry.html.
 """
-from typing import Any, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from mmengine.config import Config, ConfigDict
 from mmengine.registry import DATA_SAMPLERS as MMENGINE_DATA_SAMPLERS
 from mmengine.registry import DATASETS as MMENGINE_DATASETS
 from mmengine.registry import HOOKS as MMENGINE_HOOKS
 from mmengine.registry import LOOPS as MMENGINE_LOOPS
 from mmengine.registry import METRICS as MMENGINE_METRICS
@@ -39,30 +39,22 @@
 
     # TODO relay on mmengine:HAOCHENYE/config_new_feature
     if cfg.get('cfg_path', None) and not cfg.get('type', None):
         from mmengine.hub import get_model
         model = get_model(**cfg)  # type: ignore
         return model
 
-    from mmrazor.structures import load_fix_subnet
-
-    if cfg.get('_fix_subnet_', None):
-        fix_subnet = cfg.pop('_fix_subnet_')
-        mutable_model = build_from_cfg(cfg, registry, default_args)
-        load_fix_subnet(mutable_model, fix_subnet)
-        return mutable_model
+    return_architecture = False
+    if cfg.get('_return_architecture_', None):
+        return_architecture = cfg.pop('_return_architecture_')
+    razor_model = build_from_cfg(cfg, registry, default_args)
+    if return_architecture:
+        return razor_model.architecture
     else:
-        return_architecture = False
-        if cfg.get('_return_architecture_', None):
-            return_architecture = cfg.pop('_return_architecture_')
-        razor_model = build_from_cfg(cfg, registry, default_args)
-        if return_architecture:
-            return razor_model.architecture
-        else:
-            return razor_model
+        return razor_model
 
 
 # Registries For Runner and the related
 # manage all kinds of runners like `EpochBasedRunner` and `IterBasedRunner`
 RUNNERS = Registry('runner', parent=MMENGINE_RUNNERS)
 # manage runner constructors that define how to initialize runners
 RUNNER_CONSTRUCTORS = Registry(
@@ -107,7 +99,40 @@
 TASK_UTILS = Registry('task util', parent=MMENGINE_TASK_UTILS)
 
 # Registries For Visualizer and the related
 # manage visualizer
 VISUALIZERS = Registry('visualizer', parent=MMENGINE_VISUALIZERS)
 # manage visualizer backend
 VISBACKENDS = Registry('vis_backend', parent=MMENGINE_VISBACKENDS)
+
+
+# manage sub models for downstream repos
+@MODELS.register_module()
+def sub_model(cfg,
+              fix_subnet,
+              mode: str = 'mutable',
+              prefix: str = '',
+              extra_prefix: str = '',
+              init_weight_from_supernet: bool = False,
+              init_cfg: Optional[Dict] = None):
+    model = MODELS.build(cfg)
+    # Save path type cfg process, set init_cfg directly.
+    if init_cfg:
+        # update init_cfg when init_cfg is valid.
+        model.init_cfg = init_cfg
+    if init_weight_from_supernet:
+        # Supernet is modified after load_fix_subnet(), init weight here.
+        model.init_weights()
+    from mmrazor.structures import load_fix_subnet
+
+    load_fix_subnet(
+        model,
+        fix_subnet,
+        load_subnet_mode=mode,
+        prefix=prefix,
+        extra_prefix=extra_prefix)
+
+    if init_weight_from_supernet:
+        # Supernet is modified after load_fix_subnet().
+        model.init_cfg = None
+
+    return model
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/structures/graph/base_graph.py` & `mmrazor-1.0.0rc2/mmrazor/structures/graph/base_graph.py`

 * *Files 26% similar despite different names*

```diff
@@ -117,25 +117,35 @@
             return None
 
     def add_node(self, node: BASENODE):
         """Add a node."""
         if node.name not in self.nodes:
             self.nodes[node.name] = node
         else:
-            raise BaseException(f'{node.name} already exists in graph')
+            raise Exception(f'{node.name} already exists in graph')
 
     def connect(self, pre_node: BASENODE, next_node: BASENODE):
         """Add an edge from pre_node to next_node."""
-        assert pre_node in self and next_node in self
+        pre_node_ = self.find_node(pre_node)
+        next_node_ = self.find_node(next_node)
+        assert pre_node_ is not None and next_node_ is not None, \
+            f"{pre_node},{next_node} don't exist in the graph."
+        pre_node = pre_node_
+        next_node = next_node_
         pre_node.add_next_node(next_node)
         next_node.add_prev_node(pre_node)
 
     def disconnect(self, pre_node: BASENODE, next_node: BASENODE):
         """Remove the edge form pre_node to next_node."""
-        assert pre_node in self and next_node in self
+        pre_node_ = self.find_node(pre_node)
+        next_node_ = self.find_node(next_node)
+        assert pre_node_ is not None and next_node_ is not None, \
+            f"{pre_node},{next_node} don't exist in the graph."
+        pre_node = pre_node_
+        next_node = next_node_
         if next_node in pre_node.next_nodes:
             pre_node.next_nodes.remove(next_node)
         if pre_node in next_node.prev_nodes:
             next_node.prev_nodes.remove(pre_node)
 
     def delete_node(self, node: BASENODE):
         """Delete a node with its related edges."""
@@ -181,15 +191,15 @@
         return len(self.nodes)
 
     # other
 
     def __repr__(self):
         res = f'Graph with {len(self)} nodes:\n'
         for node in self:
-            res += '{0:<40} -> {1:^40} -> {2:<40}\n'.format(
+            res += '{0:<80} -> {1:^80} -> {2:<80}\n'.format(
                 str(node.prev_nodes), node.__repr__(), str(node.next_nodes))
         return res
 
     # traverse
 
     def topo_traverse(self) -> Iterator[BASENODE]:
         """Traverse the graph in topologitcal order."""
@@ -200,15 +210,15 @@
                 degree[name] = len(node.prev_nodes)
             return degree
 
         def find_zero_degree_node(in_degree):
             for node_name in in_degree:
                 if in_degree[node_name] == 0:
                     return node_name
-            return None
+            raise Exception(f'no zero degree node\n{in_degree}')
 
         in_degree = _in_degree(self)
 
         while len(in_degree) > 0:
             node_name = find_zero_degree_node(in_degree)  # visit the node
             in_degree.pop(node_name)
             yield self.nodes[node_name]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/structures/graph/channel_graph.py` & `mmrazor-1.0.0rc2/tests/test_core/test_graph/test_channel_graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from typing import Callable, Dict, List
+import unittest
 
-from torch.nn import Module
+import torch
+from torch import nn
 
-from .base_graph import BaseGraph
-from .channel_modules import BaseChannelUnit, ChannelTensor
-from .channel_nodes import ChannelNode, default_channel_node_converter
-from .module_graph import ModuleGraph
-
-
-class ChannelGraph(ModuleGraph[ChannelNode]):
-    """ChannelGraph is used to trace the channel dependency of a model.
-
-    A ChannelGraph generates a ChannelTensor as the input to the model. Then,
-    the tensor can forward through all nodes and collect channel dependency.
-    """
-
-    @classmethod
-    def copy_from(cls,
-                  graph: 'BaseGraph',
-                  node_converter: Callable = default_channel_node_converter):
-        """Copy from a ModuleGraph."""
-        assert isinstance(graph, ModuleGraph)
-        return super().copy_from(graph, node_converter)
-
-    def collect_units(self) -> List[BaseChannelUnit]:
-        """Collect channel units in the graph."""
-        units = list()
-        for node in self.topo_traverse():
-            node.register_channel_to_units()
-        for node in self.topo_traverse():
-            for unit in node.in_channel_tensor.unit_list + \
-                    node.out_channel_tensor.unit_list:
-                if unit not in units:
-                    units.append(unit)
-        return units
-
-    def forward(self, num_input_channel=3):
-        """Generate a ChanneelTensor and let it forwards through the graph."""
-        for node in self.topo_traverse():
-            node.reset_channel_tensors()
-        self._merge_same_module()
-        for i, node in enumerate(self.topo_traverse()):
-            node: ChannelNode
-            if len(node.prev_nodes) == 0:
-                channel_list = ChannelTensor(num_input_channel)
-                node.forward([channel_list])
-            else:
-                node.forward()
-
-    def _merge_same_module(self):
-        """Union all nodes with the same module to the same unit."""
-        module2node: Dict[Module, List[ChannelNode]] = dict()
-        for node in self:
-            if isinstance(node.val, Module):
-                if node.val not in module2node:
-                    module2node[node.val] = []
-                if node not in module2node[node.val]:
-                    module2node[node.val].append(node)
-
-        for module in module2node:
-            if len(module2node[module]) > 1:
-                nodes = module2node[module]
-                input_channel_tensor = ChannelTensor(nodes[0].in_channels)
-                out_channel_tensor = ChannelTensor(nodes[0].out_channels)
-                for node in nodes:
-                    ChannelTensor.union(input_channel_tensor,
-                                        node.in_channel_tensor)
-                    ChannelTensor.union(out_channel_tensor,
-                                        node.out_channel_tensor)
+from mmrazor.models.task_modules import BackwardTracer
+from mmrazor.registry import TASK_UTILS
+from mmrazor.structures.graph import ModuleGraph
+from mmrazor.structures.graph.channel_graph import ChannelGraph
+from mmrazor.structures.graph.channel_nodes import \
+    default_channel_node_converter
+from ...data.models import SingleLineModel
+
+NodeMap = {}
+
+
+@TASK_UTILS.register_module()
+class ImageClassifierPseudoLossWithSixChannel:
+    """Calculate the pseudo loss to trace the topology of a `ImageClassifier`
+    in MMClassification with `BackwardTracer`."""
+
+    def __call__(self, model) -> torch.Tensor:
+        pseudo_img = torch.rand(1, 6, 224, 224)
+        pseudo_output = model(pseudo_img)
+        return sum(pseudo_output)
+
+
+class TestChannelGraph(unittest.TestCase):
+
+    def test_init(self):
+        model = SingleLineModel()
+        module_graph = ModuleGraph.init_from_backward_tracer(model)
+
+        _ = ChannelGraph.copy_from(module_graph,
+                                   default_channel_node_converter)
+
+    # def test_forward(self):
+    #     for model_data in BackwardPassedModelManager.include_models(  # noqa
+    #     ):  # noqa
+    #         with self.subTest(model=model_data):
+    #             model = model_data()
+    #             module_graph = ModuleGraph.init_from_backward_tracer(model)
+
+    #             channel_graph = ChannelGraph.copy_from(
+    #                 module_graph, default_channel_node_converter)
+    #             channel_graph.forward()
+
+    #             # units = channel_graph.collect_units()
+    #             _ = channel_graph.generate_units_config()
+
+    def test_forward_with_config_num_in_channel(self):
+
+        class MyModel(nn.Module):
+
+            def __init__(self) -> None:
+                super().__init__()
+                self.conv1 = nn.Conv2d(6, 3, 3, 1, 1)
+                self.net = SingleLineModel()
+
+            def forward(self, x):
+                return self.net(self.conv1(x))
+
+        model = MyModel()
+        module_graph = ModuleGraph.init_from_backward_tracer(
+            model,
+            backward_tracer=BackwardTracer(
+                loss_calculator=ImageClassifierPseudoLossWithSixChannel()))
+
+        channel_graph = ChannelGraph.copy_from(module_graph,
+                                               default_channel_node_converter)
+        channel_graph.forward(num_input_channel=6)
+
+        _ = channel_graph.generate_units_config
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/structures/graph/channel_nodes.py` & `mmrazor-1.0.0rc2/mmrazor/structures/graph/channel_nodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,378 +1,533 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+"""ChannelNodes are basic node type of ChannelGraph.
 
+Different ChannelNodes represent different modules.
+"""
 import operator
 from abc import abstractmethod
-from typing import Union
+from typing import List, Union
 
 import torch
 import torch.nn as nn
+from mmcv.cnn.bricks import Scale
 from mmengine import MMLogger
 
-from .channel_modules import BaseChannel, BaseChannelUnit, ChannelTensor
+from mmrazor.utils import print_log
+from .channel_flow import ChannelTensor
 from .module_graph import ModuleNode
 
+# error types
+
+
+class ChannelDismatchError(Exception):
+    pass
+
+
+def assert_channel(condition, node):
+    if not condition:
+        raise ChannelDismatchError(node.name)
+
+
+# ChannelNode
+
 
 class ChannelNode(ModuleNode):
     """A ChannelNode is like a torch module. It accepts  a ChannelTensor and
     output a ChannelTensor. The difference is that the torch module transforms
     a tensor, while the ChannelNode records the information of channel
     dependency in the ChannelTensor.
 
     Args:
         name (str): The name of the node.
         val (Union[nn.Module, str]): value of the node.
-        expand_ratio (int, optional): expand_ratio compare with channel
-            mask. Defaults to 1.
         module_name (str, optional): the module name of the module of the
             node.
     """
 
     # init
 
     def __init__(self,
                  name: str,
                  val: Union[nn.Module, str],
-                 expand_ratio: int = 1,
                  module_name='') -> None:
 
-        super().__init__(name, val, expand_ratio, module_name)
-        self.in_channel_tensor = ChannelTensor(self.in_channels)
-        self.out_channel_tensor = ChannelTensor(self.out_channels)
+        super().__init__(name, val, module_name)
+        self.in_channel_tensor: Union[None, ChannelTensor] = None
+        self.out_channel_tensor: Union[None, ChannelTensor] = None
+        self.return_tensor: Union[None, ChannelTensor] = None
 
     @classmethod
     def copy_from(cls, node):
         """Copy from a ModuleNode."""
         assert isinstance(node, ModuleNode)
-        return cls(node.name, node.val, node.expand_ratio, node.module_name)
+        return cls(node.name, node.val, node.module_name)
 
     def reset_channel_tensors(self):
         """Reset the owning ChannelTensors."""
-        self.in_channel_tensor = ChannelTensor(self.in_channels)
-        self.out_channel_tensor = ChannelTensor(self.out_channels)
+        self.in_channel_tensor = None
+        self.out_channel_tensor = None
 
     # forward
 
-    def forward(self, in_channel_tensor=None):
+    def forward(self, in_channel_tensors=None):
         """Forward with ChannelTensors."""
-        assert self.in_channel_tensor is not None and \
-            self.out_channel_tensor is not None
-        if in_channel_tensor is None:
+        if in_channel_tensors is None:
             out_channel_tensors = [
-                node.out_channel_tensor for node in self.prev_nodes
+                node.return_tensor for node in self.prev_nodes
             ]
-
-            in_channel_tensor = out_channel_tensors
-        self.channel_forward(*in_channel_tensor)
-        if self.expand_ratio > 1:
-            self.out_channel_tensor = self.out_channel_tensor.expand(
-                self.expand_ratio)
+            in_channel_tensors = out_channel_tensors
+        try:
+            self.return_tensor = self.channel_forward(in_channel_tensors)
+        except Exception as e:
+            raise Exception(f'{e},{self.name}')
 
     @abstractmethod
-    def channel_forward(self, *channel_tensors: ChannelTensor):
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
         """Forward with ChannelTensors."""
         assert len(channel_tensors) == 1, f'{len(channel_tensors)}'
-        BaseChannelUnit.union_two_units(
-            list(self.in_channel_tensor.unit_dict.values())[0],
-            list(channel_tensors[0].unit_dict.values())[0])
-
-        if self.in_channels == self.out_channels:
-            BaseChannelUnit.union_two_units(
-                self.in_channel_tensor.unit_list[0],
-                self.out_channel_tensor.unit_list[0])
-
-    # register unit
-
-    def register_channel_to_units(self):
-        """Register the module of this node to corresponding units."""
-        name = self.module_name if isinstance(self.val,
-                                              nn.Module) else self.name
-        for index, unit in self.in_channel_tensor.unit_dict.items():
-            channel = BaseChannel(name, self.val, index, None, False,
-                                  self.expand_ratio)
-            if channel not in unit.input_related:
-                unit.input_related.append(channel)
-        for index, unit in self.out_channel_tensor.unit_dict.items():
-            channel = BaseChannel(name, self.val, index, None, True,
-                                  self.expand_ratio)
-            if channel not in unit.output_related:
-                unit.output_related.append(channel)
+
+        self.in_channel_tensor = channel_tensors[0]
+        self.out_channel_tensor = ChannelTensor(self.out_channels)
+        return self.out_channel_tensor
 
     # channels
 
     # @abstractmethod
     @property
     def in_channels(self) -> int:
         """Get the number of input channels of the node."""
-        raise NotImplementedError()
+        try:
+            return self._in_channels
+        except NotImplementedError:
+            return \
+                self._get_in_channels_by_prev_nodes(self.prev_nodes)
 
     # @abstractmethod
     @property
     def out_channels(self) -> int:
         """Get the number of output channels of the node."""
-        raise NotImplementedError()
+        try:
+            return self._out_channels
+        except NotImplementedError:
+            return self._get_out_channel_by_in_channels(self.in_channels)
+
+    def check_channel(self):
+        """Check if the node has a channel error."""
+        for node in self.prev_nodes:
+            assert_channel(node.out_channels == self.in_channels, self)
+
+    @property
+    def _in_channels(self) -> int:
+        """Get in channel number of by the module self."""
+        raise NotImplementedError(
+            f'{self.name}({self.__class__.__name__}) has no _in_channels')
+
+    @property
+    def _out_channels(self) -> int:
+        """Get out channel number of by the module self."""
+        raise NotImplementedError(
+            f'{self.name}({self.__class__.__name__}) has no _out_channels')
+
+    def _get_out_channel_by_in_channels(self, in_channels):
+        """Get output channel number by the input channel number."""
+        return in_channels
+
+    def _get_in_channels_by_prev_nodes(self, prev_nodes):
+        """Get input channel numbers by previous nodes."""
+        if len(prev_nodes) == 0:
+            print_log(
+                (f'As {self.name} '
+                 'has no prev nodes, so we set the in channels of it to 3.'),
+                level='debug')
+            return 3
+        else:
+            return prev_nodes[0].out_channels
+
+    def __repr__(self) -> str:
+        return f'{self.name}_({self.in_channels},{self.out_channels})'
 
 
 # basic nodes
 
 
-class PassChannelNode(ChannelNode):
-    """A PassChannelNode has the same number of input channels and output
+class PassUnionChannelNode(ChannelNode):
+    """A PassUnionChannelNode has the same number of input channels and output
     channels.
 
     Besides, the corresponding input channels and output channels belong to one
     channel unit. Such as  BatchNorm, Relu.
     """
 
-    def channel_forward(self, *in_channel_tensor: ChannelTensor):
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
         """Channel forward."""
-        PassChannelNode._channel_forward(self, *in_channel_tensor)
+        return PassUnionChannelNode._channel_forward(self, channel_tensors[0])
 
-    @property
-    def in_channels(self) -> int:
-        """Get the number of input channels of the node."""
-        if len(self.prev_nodes) > 0:
-            return self.prev_nodes[0].out_channels
-        else:
-            return 0
+    @staticmethod
+    def _channel_forward(node: ChannelNode, tensor: ChannelTensor):
+        """Channel forward."""
+        assert node.in_channels == node.out_channels
+        assert isinstance(tensor, ChannelTensor)
+        node.in_channel_tensor = tensor
+        node.out_channel_tensor = tensor
+        return node.out_channel_tensor
+
+    def __repr__(self) -> str:
+        return super().__repr__() + '_uion'
 
-    @property
-    def out_channels(self) -> int:
-        """Get the number of output channels of the node."""
-        return self.in_channels
+
+class PassChannelNode(ChannelNode):
+
+    def _get_in_channels_by_prev_nodes(self, prev_nodes):
+        assert len(self.prev_nodes) == 1
+        node0: ChannelNode = self.prev_nodes[0]
+        return node0.out_channels
+
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
+        assert len(channel_tensors) == 1
+        self.in_channel_tensor = ChannelTensor(1)
+        self.out_channel_tensor = ChannelTensor(1)
+        return channel_tensors[0]
 
     def __repr__(self) -> str:
         return super().__repr__() + '_pass'
 
-    @staticmethod
-    def _channel_forward(node: ChannelNode, *in_channel_tensor: ChannelTensor):
-        """Channel forward."""
-        assert len(in_channel_tensor) == 1 and \
-            node.in_channels == node.out_channels
-        in_channel_tensor[0].union(node.in_channel_tensor)
-        node.in_channel_tensor.union(node.out_channel_tensor)
-
 
 class MixChannelNode(ChannelNode):
     """A MixChannelNode  has independent input channels and output channels."""
 
-    def channel_forward(self, *in_channel_tensor: ChannelTensor):
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
         """Channel forward."""
-        assert len(in_channel_tensor) <= 1
-        if len(in_channel_tensor) == 1:
-            in_channel_tensor[0].union(self.in_channel_tensor)
-
-    @property
-    def in_channels(self) -> int:
-        """Get the number of input channels of the node."""
-        if len(self.prev_nodes) > 0:
-            return self.prev_nodes[0].in_channels
+        assert len(channel_tensors) <= 1
+        if len(channel_tensors) == 1:
+            self.in_channel_tensor = channel_tensors[0]
+            self.out_channel_tensor = ChannelTensor(self.out_channels)
         else:
-            return 0
-
-    @property
-    def out_channels(self) -> int:
-        """Get the number of output channels of the node."""
-        if len(self.next_nodes) > 0:
-            return self.next_nodes[0].in_channels
-        else:
-            return 0
+            raise NotImplementedError()
+        return self.out_channel_tensor
 
     def __repr__(self) -> str:
         return super().__repr__() + '_mix'
 
 
-class BindChannelNode(PassChannelNode):
+class BindChannelNode(ChannelNode):
     """A BindChannelNode has multiple inputs, and all input channels belong to
     the same channel unit."""
 
-    def channel_forward(self, *in_channel_tensor: ChannelTensor):
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
         """Channel forward."""
-        assert len(in_channel_tensor) > 1
+        assert len(channel_tensors) > 0, f'{self}'
         #  align channel_tensors
-        ChannelTensor.align_tensors(*in_channel_tensor)
-
-        # union tensors
-        node_units = [
-            channel_lis.unit_dict for channel_lis in in_channel_tensor
-        ]
-        for key in node_units[0]:
-            BaseChannelUnit.union_units([units[key] for units in node_units])
-        super().channel_forward(in_channel_tensor[0])
+        for tensor in channel_tensors[1:]:
+            channel_tensors[0].union(tensor)
+        self.in_channel_tensor = channel_tensors[0]
+        self.out_channel_tensor = channel_tensors[0]
+        return self.out_channel_tensor
 
     def __repr__(self) -> str:
-        return super(ChannelNode, self).__repr__() + '_bind'
+        return super().__repr__() + '_bind'
+
+    def check_channel(self):
+        for node in self.prev_nodes:
+            assert_channel(node.out_channels == self.in_channels, self)
 
 
 class CatChannelNode(ChannelNode):
     """A CatChannelNode cat all input channels."""
 
-    def channel_forward(self, *in_channel_tensors: ChannelTensor):
-        BaseChannelUnit.union_two_units(self.in_channel_tensor.unit_list[0],
-                                        self.out_channel_tensor.unit_list[0])
-        num_ch = []
-        for in_ch_tensor in in_channel_tensors:
-            for start, end in in_ch_tensor.unit_dict:
-                num_ch.append(end - start)
-
-        split_units = BaseChannelUnit.split_unit(
-            self.in_channel_tensor.unit_list[0], num_ch)
-
-        i = 0
-        for in_ch_tensor in in_channel_tensors:
-            for in_unit in in_ch_tensor.unit_dict.values():
-                BaseChannelUnit.union_two_units(split_units[i], in_unit)
-                i += 1
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
+        tensor_cat = ChannelTensor.cat(channel_tensors)
+        self.in_channel_tensor = tensor_cat
+        self.out_channel_tensor = tensor_cat
+        return self.out_channel_tensor
+
+    def check_channel(self):
+        in_num = [node.out_channels for node in self.prev_nodes]
+        assert_channel(sum(in_num) == self.in_channels, self)
+
+    def _get_in_channels_by_prev_nodes(self, prev_nodes):
+        assert len(prev_nodes) > 0
+        nums = [node.out_channels for node in prev_nodes]
+        return sum(nums)
 
-    @property
-    def in_channels(self) -> int:
-        """Get the number of input channels of the node."""
-        return sum([node.out_channels for node in self.prev_nodes])
+    def __repr__(self) -> str:
+        return super().__repr__() + '_cat'
+
+
+class ExpandChannelNode(ChannelNode):
+
+    def __init__(self,
+                 name: str,
+                 val: Union[nn.Module, str],
+                 module_name='',
+                 expand_ratio=1) -> None:
+        super().__init__(name, val, module_name)
+        self.expand_ratio = expand_ratio
+
+    def _get_out_channel_by_in_channels(self, in_channels):
+        return in_channels * self.expand_ratio
+
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
+        assert len(channel_tensors) == 1, f'{self}'
+        assert self.out_channels >= self.in_channels, f'{self}'
+        assert self.out_channels % self.in_channels == 0, f'{self}'
+        tensor0 = channel_tensors[0]
+        self.in_channel_tensor = tensor0
+        self.out_channel_tensor = tensor0.expand(self.expand_ratio)
+        return self.out_channel_tensor
+
+    def __repr__(self) -> str:
+        return super().__repr__() + f'_expand({self.expand_ratio})'
+
+
+class InputChannelNode(ChannelNode):
+
+    def __init__(self,
+                 name: str,
+                 val: Union[nn.Module, str],
+                 module_name='',
+                 input_channels=3) -> None:
+        super().__init__(name, val, module_name)
+        self._input_channels = input_channels
+
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
+        input_tensor = ChannelTensor(self._input_channels)
+        self.in_channel_tensor = input_tensor
+        self.out_channel_tensor = input_tensor
+        return input_tensor
 
     @property
-    def out_channels(self) -> int:
-        """Get the number of output channels of the node."""
-        return self.in_channels
+    def _in_channels(self) -> int:
+        return self._input_channels
 
     def __repr__(self) -> str:
-        return super().__repr__() + '_cat'
+        return super().__repr__() + '_input'
+
+
+class EndNode(ChannelNode):
+
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
+        tensor_end = ChannelTensor(1)
+        self.in_channel_tensor = tensor_end
+        self.out_channel_tensor = tensor_end
+        for channel in channel_tensors:
+            channel.union(tensor_end.expand(len(channel)))
+        return self.out_channel_tensor
+
+    def __repr__(self) -> str:
+        return super().__repr__() + '_end'
+
+    def check_channel(self):
+        pass
 
 
 # module nodes
 
 
 class ConvNode(MixChannelNode):
     """A ConvNode corresponds to a Conv2d module.
 
     It can deal with normal conv, dwconv and gwconv.
     """
 
     def __init__(self,
                  name: str,
                  val: Union[nn.Module, str],
-                 expand_ratio: int = 1,
                  module_name='') -> None:
-        super().__init__(name, val, expand_ratio, module_name)
+        super().__init__(name, val, module_name)
         assert isinstance(self.val, nn.Conv2d)
+
+    @property
+    def conv_type(self):
         if self.val.groups == 1:
-            self.conv_type = 'conv'
+            return 'conv'
         elif self.val.in_channels == self.out_channels == self.val.groups:
-            self.conv_type = 'dwconv'
+            return 'dwconv'
         else:
-            self.conv_type = 'gwconv'
+            return 'gwconv'
 
-    def channel_forward(self, *in_channel_tensor: ChannelTensor):
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
         if self.conv_type == 'conv':
-            return super().channel_forward(*in_channel_tensor)
+            return super().channel_forward(channel_tensors)
         elif self.conv_type == 'dwconv':
-            return PassChannelNode._channel_forward(self, *in_channel_tensor)
+            return PassUnionChannelNode._channel_forward(
+                self, channel_tensors[0])
         elif self.conv_type == 'gwconv':
-            return super().channel_forward(*in_channel_tensor)
+            return self._gw_conv_channel_forward(channel_tensors)
         else:
-            pass
+            raise NotImplementedError(f'{self}')
+
+    def _gw_conv_channel_forward(self, channel_tensors: List[ChannelTensor]):
+
+        assert len(channel_tensors) == 1
+        tensor0 = channel_tensors[0]
+        conv: nn.Conv2d = self.val
+        group_union(tensor0, conv.groups)
+        self.in_channel_tensor = tensor0
+        self.out_channel_tensor = ChannelTensor(self.out_channels)
+        group_union(self.out_channel_tensor, conv.groups)
+        return self.out_channel_tensor
 
     @property
-    def in_channels(self) -> int:
+    def _in_channels(self) -> int:
         return self.val.in_channels
 
     @property
-    def out_channels(self) -> int:
+    def _out_channels(self) -> int:
         return self.val.out_channels
 
     def __repr__(self) -> str:
         return super().__repr__() + '_conv'
 
 
 class LinearNode(MixChannelNode):
     """A LinearNode corresponds to a Linear module."""
 
     def __init__(self,
                  name: str,
                  val: Union[nn.Module, str],
-                 expand_ratio: int = 1,
                  module_name='') -> None:
-        super().__init__(name, val, expand_ratio, module_name)
+        super().__init__(name, val, module_name)
         assert isinstance(self.val, nn.Linear)
 
     @property
-    def in_channels(self) -> int:
+    def _in_channels(self) -> int:
         return self.val.in_features
 
     @property
-    def out_channels(self) -> int:
+    def _out_channels(self) -> int:
         return self.val.out_features
 
     def __repr__(self) -> str:
-        return super().__repr__() + 'linear'
+        return super().__repr__() + '_linear'
 
 
-class NormNode(PassChannelNode):
+class BnNode(PassUnionChannelNode):
     """A NormNode corresponds to a BatchNorm2d module."""
 
     def __init__(self,
                  name: str,
                  val: Union[nn.Module, str],
-                 expand_ratio: int = 1,
                  module_name='') -> None:
-        super().__init__(name, val, expand_ratio, module_name)
-        assert isinstance(self.val, nn.BatchNorm2d)
+        super().__init__(name, val, module_name)
+        assert isinstance(self.val,
+                          nn.modules.batchnorm._BatchNorm), f'{type(self.val)}'
 
     @property
-    def in_channels(self) -> int:
+    def _in_channels(self) -> int:
         return self.val.num_features
 
     @property
-    def out_channels(self) -> int:
+    def _out_channels(self) -> int:
         return self.val.num_features
 
     def __repr__(self) -> str:
         return super().__repr__() + '_bn'
 
 
-# converter
+class GroupNormNode(PassUnionChannelNode):
 
+    def __init__(self,
+                 name: str,
+                 val: Union[nn.Module, str],
+                 module_name='') -> None:
+        super().__init__(name, val, module_name)
+        assert isinstance(self.val, nn.GroupNorm)
+        self.val: nn.GroupNorm
+
+    @property
+    def _in_channels(self) -> int:
+        return self.val.num_channels
+
+    @property
+    def _out_channels(self) -> int:
+        return self.val.num_channels
+
+    def channel_forward(self, channel_tensors: List[ChannelTensor]):
+        out_tensor = super().channel_forward(channel_tensors)
+        group_tensor = ChannelTensor(self.in_channels // self.val.num_groups)
+        group_union(out_tensor, self.val.num_groups, group_tensor)
+        return out_tensor
+
+    def __repr__(self) -> str:
+        return super().__repr__() + '_gn'
 
-def default_channel_node_converter(node: ModuleNode) -> ChannelNode:
-    """The default node converter for ChannelNode."""
 
-    def warn(default='PassChannelNode'):
-        logger = MMLogger('mmrazor', 'mmrazor')
-        logger.warn((f"{node.name}({node.val}) node can't find match type of"
-                     'channel_nodes,'
-                     f'replaced with {default} by default.'))
+# converter
 
-    module_mapping = {
+channel_nodes_mapping = {
+    'module': {
         nn.Conv2d: ConvNode,
-        nn.BatchNorm2d: NormNode,
+        nn.modules.batchnorm._BatchNorm: BnNode,
         nn.Linear: LinearNode,
-    }
-    function_mapping = {
+        nn.modules.ReLU: PassChannelNode,
+        nn.modules.Hardtanh: PassChannelNode,
+        # pools
+        nn.modules.pooling._AvgPoolNd: PassChannelNode,
+        nn.modules.pooling._AdaptiveAvgPoolNd: PassChannelNode,
+        nn.modules.pooling._MaxPoolNd: PassChannelNode,
+        nn.modules.pooling._AdaptiveMaxPoolNd: PassChannelNode,
+        Scale: PassChannelNode,
+        nn.modules.GroupNorm: GroupNormNode,
+    },
+    'function': {
         torch.add: BindChannelNode,
         torch.cat: CatChannelNode,
-        operator.add: BindChannelNode
-    }
-    name_mapping = {
+        operator.add: BindChannelNode,
+    },
+    'str': {
         'bind_placeholder': BindChannelNode,
-        'pass_placeholder': PassChannelNode,
+        'pass_placeholder': PassUnionChannelNode,
         'cat_placeholder': CatChannelNode,
-    }
+        'input_placeholder': InputChannelNode,
+        'output_placeholder': EndNode
+    },
+}
+
+
+def default_channel_node_converter(
+        node: ModuleNode,
+        module_mapping=channel_nodes_mapping['module'],
+        function_mapping=channel_nodes_mapping['function'],
+        name_mapping=channel_nodes_mapping['str']) -> ChannelNode:
+    """The default node converter for ChannelNode."""
+
+    def warn(default='PassUnionChannelNode'):
+        logger = MMLogger.get_current_instance()
+        logger.info(
+            (f"{node.name}({node.module_name}) node can't find match type of"
+             'channel_nodes,'
+             f'replaced with {default} by default.'))
+
     if isinstance(node.val, nn.Module):
         # module_mapping
         for module_type in module_mapping:
             if isinstance(node.val, module_type):
                 return module_mapping[module_type].copy_from(node)
 
     elif isinstance(node.val, str):
         for module_type in name_mapping:
             if node.val == module_type:
                 return name_mapping[module_type].copy_from(node)
-
     else:
         for fun_type in function_mapping:
             if node.val == fun_type:
                 return function_mapping[fun_type].copy_from(node)
     if len(node.prev_nodes) > 1:
         warn('BindChannelNode')
         return BindChannelNode.copy_from(node)
     else:
-        warn('PassChannelNode')
-        return PassChannelNode.copy_from(node)
+        warn('PassUnionChannelNode')
+        return PassUnionChannelNode.copy_from(node)
+
+
+# helper functions
+
+
+def group_union(tensor: ChannelTensor, groups: int, group_tensor=None):
+    """Group-wise union for ChannelTensor."""
+    c_per_group = len(tensor) // groups
+    if group_tensor is None:
+        group_tensor = ChannelTensor(c_per_group)
+    assert groups * len(group_tensor) == len(tensor)
+    for i in range(groups):
+        tensor[i * c_per_group:(i + 1) * c_per_group].union(group_tensor)
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/structures/graph/module_graph.py` & `mmrazor-1.0.0rc2/mmrazor/structures/graph/module_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,42 @@
 
 from mmrazor.models.task_modules.tracer.backward_tracer import BackwardTracer
 from mmrazor.models.task_modules.tracer.loss_calculator import \
     ImageClassifierPseudoLoss
 from mmrazor.models.task_modules.tracer.path import (Path, PathConcatNode,
                                                      PathList, PathNode)
 from mmrazor.registry import TASK_UTILS
+from mmrazor.utils import print_log
 from .base_graph import BaseGraph, BaseNode
+from .pseudo_fx_graph import FxBaseNode
+
 
 # ModuleNode && ModuleGraph
+class NoOutputError(Exception):
+    """An error occurs when no output node for a leaf node."""
+
+    def __init__(self, node, *args: object) -> None:
+        super().__init__(f'{node}', *args)
+        self.node = node
+
+    pass
+
+
+class NoInputError(Exception):
+    """An error occurs when no input node for a leaf node."""
+
+    def __init__(self, node, *args: object) -> None:
+        super().__init__(f'{node}', *args)
+        self.node = node
+
+
+def my_assert(condiion, exception):
+    """assert helper function."""
+    if not condiion:
+        raise exception
 
 
 class ModuleNode(BaseNode):
     """A node in a computation graph.
 
     All nodes are divided to four types, the detail of definition can be found
     in functions  self.is_{xxx}_node.
@@ -31,105 +56,45 @@
     pre_defined_node_val_str = [
         'cat_placeholder', 'bind_placeholder', 'pass_placeholder'
     ]
 
     def __init__(self,
                  name: str,
                  val: Union[Module, str],
-                 expand_ratio: int = 1,
                  module_name='') -> None:
         """
         Args:
             name (str): the name of the node
             val (Module | str): content of the node. It can be Module or
             string. If val is a string, the string can only be one of
                 self.pre_defined_node_val_str
-            expand_ratio (int): expand_ratio is used in bind node,
-                where the out_channel is always a multiple of the in_channel.
         Note:
             Here, we give an example of expand_ratio.
             >>> class Pool(nn.Module):
                     def forward(x):
                         return F.adaptive_avg_pool2d(x,2).flatten(1)
             >>> node= ModuleNode('pass_0',Pool(),expand_ratio=4)
             >>> assert node.out_channels == node.in_channels*4
         """
 
-        assert (isinstance(val, Module)
-                or val in self.__class__.pre_defined_node_val_str
-                ), f'{val} node is not allowed'
-        if expand_ratio != 1:
-            assert val == 'pass_placeholder', \
-                'expand != 1 is only valid when val=="pass"'
         super().__init__(name, val)
-        self.expand_ratio = expand_ratio
         self.module_name = module_name
 
-    # channel
-
-    @property
-    def in_channels(self) -> int:
-        """int: the in_channels of the node."""
-        if isinstance(self.val, nn.Module):
-            MAPPING = {
-                nn.Conv2d: 'in_channels',
-                nn.modules.batchnorm._BatchNorm: 'num_features',
-                nn.modules.Linear: 'in_features',
-            }
-            for basetype in MAPPING:
-                if isinstance(self.val, basetype):
-                    return getattr(self.val, MAPPING[basetype])
-            raise NotImplementedError(f'unsupported module: {self.val}')
-        elif self.is_bind_node() or self.is_pass_node():
-            if len(self.prev_nodes) > 0:
-                return self.prev_nodes[0].out_channels
-            else:
-                return 0
-        elif self.is_cat_node():
-            return sum([
-                node.out_channels if node.out_channels is not None else 0
-                for node in self.prev_nodes
-            ])
-        else:
-            raise NotImplementedError(
-                f'unsupported node type: {self.basic_type}')
+    # other
 
     @property
-    def out_channels(self) -> int:
-        """int: the out_channels of the node."""
-        if isinstance(self.val, nn.Module):
-            MAPPING = {
-                nn.Conv2d: 'out_channels',
-                nn.modules.batchnorm._BatchNorm: 'num_features',
-                nn.modules.Linear: 'out_features',
-            }
-            for basetype in MAPPING:
-                if isinstance(self.val, basetype):
-                    return getattr(self.val, MAPPING[basetype])
-            raise NotImplementedError(f'unsupported module: {self.val}')
-        elif self.is_bind_node():
-            if len(self.prev_nodes) > 0:
-                return self.prev_nodes[0].out_channels
-            else:
-                return 0
-        elif self.is_pass_node():
-            return self.in_channels * self.expand_ratio
-        elif self.is_cat_node():
-            return sum([
-                node.out_channels if node.out_channels is not None else 0
-                for node in self.prev_nodes
-            ])
-        else:
-            raise NotImplementedError(
-                f'unsupported node type: {self.basic_type}')
-
-    # other
+    def is_module(self):
+        """Whether the node includes a module."""
+        return isinstance(self.val, nn.Module)
 
     def __repr__(self) -> str:
-        return f'{self.name}_({self.in_channels},{self.out_channels})'
+        repr = f'{self.name}'
+        if self.module_name != '':
+            repr += f'({self.module_name})'
+        return repr
 
     # node type
 
     @property
     def basic_type(self) -> str:
         """The basic type of the node.
 
@@ -146,15 +111,15 @@
                 else:
                     return 'gwconv2d'
             elif isinstance(self.val, nn.modules.batchnorm._BatchNorm):
                 return 'bn'
             elif isinstance(self.val, nn.Linear):
                 return 'linear'
             else:
-                raise NotImplementedError(f'{self}')
+                raise NotImplementedError(f'{self.val}')
         else:
             if self.val in [
                     'cat_placeholder', 'bind_placeholder', 'pass_placeholder'
             ]:
                 return self.val
             else:
                 raise NotImplementedError()
@@ -174,39 +139,33 @@
         return self.basic_type == 'bind_placeholder'
 
     def is_mix_node(self):
         """mix node represents a module that mixs all input channels and
         generete new output channels, such as conv and linear."""
         return self.basic_type in ['conv2d', 'linear', 'gwconv2d']
 
-    # check
+    def is_input(self):
+        """Whether the node is an input node."""
+        return self.val == 'input_placeholder'
+
+    def is_output(self):
+        """Whether the node is an output node."""
+        return self.val == 'output_placeholder'
 
-    def check_channel(self):
-        """Check if the channels of the node is matchable with previous nodes
-        and next nodes."""
-        if self.is_cat_node():
-            pass
-        else:
-            for pre in self.prev_nodes:
-                assert pre.out_channels == self.in_channels, \
-                    f'{self} has channel error'
-
-    def check_type(self):
-        """Check if the node has right number of previous nodes according to
-        their type."""
-        if self.is_pass_node():
-            assert len(self.prev_nodes) <= 1, '{name} pass node error'
-        elif self.is_cat_node():
-            pass
-        elif self.is_bind_node():
-            assert len(self.prev_nodes) > 1, '{name} bind node error'
-        elif self.is_mix_node():
-            assert len(self.prev_nodes) <= 1, '{name} mix node error'
+    def check(self):
+        """Check whether the node has any error."""
+        if self.is_input():
+            assert len(self.prev_nodes) == 0, f'{self}'
+            my_assert(len(self.next_nodes) > 0, NoOutputError(self))
+        elif self.is_output():
+            my_assert(len(self.prev_nodes) > 0, NoInputError(self))
+            assert len(self.next_nodes) == 0, f'{self}'
         else:
-            raise NotImplementedError(f'{self}')
+            my_assert(len(self.prev_nodes) > 0, NoInputError(self))
+            my_assert(len(self.next_nodes) > 0, NoOutputError(self))
 
 
 MODULENODE = TypeVar('MODULENODE', bound=ModuleNode)
 
 
 class ModuleGraph(BaseGraph[MODULENODE]):
     """Computatation Graph."""
@@ -228,63 +187,72 @@
             backward_tracer = TASK_UTILS.build(backward_tracer)
         path_lists = backward_tracer.trace(model)
         converter = PathToGraphConverter(path_lists, model)
         converter.graph.refresh_module_name()
         return converter.graph
 
     @staticmethod
-    def init_from_fx_tracer(model: Module,
-                            fx_tracer={'type': 'RazorFxTracer'}):
-        """init module graph using torch fx tracer."""
-        pass
-
-    @staticmethod
     def init_from_model(model: Module):
         """init module graph from a model which uses connect_module to record
         the relation among modules."""
         pass
 
-    # check
-
-    def check(self):
-        """Check if the graph is valid."""
-        for node in self:
-            node.check_channel()
-            node.check_type()
-
-    # static method for models that can't use tracer
-
-    @staticmethod
-    def connect_module(pre: Module, next: Module):
-        """This function is used to write hardcode in modules to generate Graph
-        object using init_from_model."""
-        if hasattr(pre, '_next'):
-            _next = getattr(pre, '_next')
-            assert isinstance(_next, List)
-        else:
-            pre._next = set()
-        pre._next.add(next)
-
-        if hasattr(next, '_pre'):
-            _pre = getattr(next, '_pre')
-            assert isinstance(_pre, List)
-        else:
-            next._pre = set()
-        next._pre.add(pre)
-
     # others
     def refresh_module_name(self):
+        """Refresh the module name."""
         module2name = {}
         for name, module in self._model.named_modules():
             module2name[module] = name
 
         for node in self:
             if isinstance(node.val, nn.Module):
                 node.module_name = module2name[node.val]
 
+    def check(self, fix=False):
+        """Check whether the Graph has any error."""
+        for node in copy.copy(list(self.topo_traverse())):
+            self._check(node, fix=fix)
+
+    def _check(self, node, fix=False):
+        """Helper method for self.check."""
+        try:
+            node.check()
+        except Exception as e:
+            if not fix:
+                raise e
+            else:
+                try:
+                    raise e
+                except NoOutputError as e:
+                    print_log(
+                        f'add a output after {node}, error: {e}',
+                        level='debug')
+                    self._add_output_after(node)
+                except NoInputError as e:
+                    print_log(
+                        f'add a input before {node}, error: {e}',
+                        level='debug')
+                    self._add_input_before(node)
+
+                self._check(node, fix=True)
+
+    def _add_input_before(self, node):
+        """Add an input node before a node."""
+        input_node = ModuleNode('auto_input',
+                                'input_placeholder')  # type: ignore
+        input_node = self.add_or_find_node(input_node)
+        self.connect(input_node, node)
+
+    def _add_output_after(self, node):
+        """Add an output node after a node."""
+        output_node = ModuleNode('auto_output',
+                                 'output_placeholder')  # type: ignore
+        output_node = self.add_or_find_node(output_node)
+        self.connect(node, output_node)
+
 
 # Converter
 
 
 class GraphConverter:
     """Base class for converters for ModuleGraph."""
 
@@ -310,15 +278,15 @@
             num = self.pass_placeholder_num
             self.pass_placeholder_num += 1
         elif type == 'bind_placeholder':
             num = self.bind_placeholder_num
             self.bind_placeholder_num += 1
         else:
             pass
-        node = ModuleNode(f'{type}_{num}', type, expand_ratio=expand_ratio)
+        node = ModuleNode(f'{type}_{num}', type)
         self.graph.add_or_find_node(node)
         return node
 
     # insert nodes
 
     def _insert_node_before(self, node: ModuleNode, new_node: ModuleNode):
         """Insert a new node before a node."""
@@ -345,15 +313,16 @@
 
     def _insert_pass_nodes(self):
         """Add pass nodes where the channel conflict."""
         for node in copy.copy(list(self.graph.nodes.values())):
             if len(node.prev_nodes) == 1:
                 pre: ModuleNode = node.prev_nodes[0]
                 if node.in_channels != pre.out_channels:
-                    assert node.in_channels % pre.out_channels == 0
+                    assert node.in_channels % pre.out_channels == 0, \
+                        f'{node.name} channel error'
                     pass_node = self._new_placeholder_node(
                         'pass_placeholder',
                         node.in_channels // pre.out_channels)
                     self._insert_node_before(node, pass_node)
 
     def _remove_redundant_pass_nodes(self):
         """Remove redundant pass nodes, which do not change number of channels
@@ -389,17 +358,16 @@
                 pass
             sorted_nodes[node.name] = node
         self.graph.nodes = sorted_nodes
 
     # other
     def _post_process(self):
         """Some post process after init a basic module graph."""
-        self._remove_redundant_pass_nodes()
+        # self._remove_redundant_pass_nodes()
         self._insert_bind_nodes()
-        self._insert_pass_nodes()
         self._topo_rename()
 
 
 class PathToGraphConverter(GraphConverter):
     """The class converts pathlist, which is generated by backward tracer, to a
     module graph."""
 
@@ -411,15 +379,16 @@
         """
         super().__init__(model)
         self.path_list = path_list
         self.cat_dict: Dict[str, str] = {}
         self.name2module = dict(model.named_modules())
         self._parse(self.path_list)
 
-        self._post_process()
+        self._insert_bind_nodes()
+        self._topo_rename()
 
     def _parse(self, path_list: PathList):
         """Parse path list."""
         self._parse_helper(path_list, [])
 
     def _parse_helper(self, path_unit: Union[PathList, Path, PathNode],
                       next_nodes: List[ModuleNode]):
@@ -490,7 +459,49 @@
             module = self.name2module[name]
             return self.graph.add_or_find_node(ModuleNode(name, module))
 
     def _connect_nexts(self, node, nexts: List[ModuleNode]):
         """Connext the node and the nodes in nexts."""
         for next in nexts:
             self.graph.connect(node, next)
+
+
+class FxTracerToGraphConverter(GraphConverter):
+    """Use fx tracer to parse model, and generate module-graph."""
+
+    def __init__(self, base_graph, model=None) -> None:
+        """
+        Args:
+            model (Module): the model which will be parsed
+            is_extra_leaf_module (Callable): a function used to determine,
+             if a module is a leaf module except torch pre-defined modules
+        """
+        super().__init__(model)
+        self.base_graph = base_graph
+        self._convert_graph()
+
+    def _node_converter(self, node: FxBaseNode):
+        """Convert a fxnode to a module-node."""
+        if node.is_function():
+            val = node.function()
+        elif node.is_input():
+            val = 'input_placeholder'
+        elif node.is_output():
+            val = 'output_placeholder'
+        elif node.is_method():
+            val = node.method()
+        elif node.is_get_attr():
+            val = 'get_attr'
+        elif node.is_module():
+            val = node.module()
+        else:
+            raise NotImplementedError(f'{node} is unsupported')
+
+        new_node = ModuleNode(node.name, val)
+        return new_node
+
+    def _convert_graph(self):
+        """Convert a torch-graph to a module-graph."""
+        base_graph = self.base_graph
+        # copy_nodes and connect
+        module_graph = ModuleGraph.copy_from(base_graph, self._node_converter)
+        self.graph = module_graph
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/testing/_fast_stop_training_hook.py` & `mmrazor-1.0.0rc2/mmrazor/testing/_fast_stop_training_hook.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/utils/__init__.py` & `mmrazor-1.0.0rc2/mmrazor/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from .index_dict import IndexDict
+from .log_tools import get_level, print_log
 from .misc import find_latest_checkpoint
 from .placeholder import get_placeholder
 from .setup_env import register_all_modules, setup_multi_processes
 from .typing import (FixMutable, MultiMutatorsRandomSubnet,
                      SingleMutatorRandomSubnet, SupportRandomSubnet,
                      ValidFixMutable)
 
 __all__ = [
     'find_latest_checkpoint', 'setup_multi_processes', 'register_all_modules',
     'FixMutable', 'ValidFixMutable', 'SingleMutatorRandomSubnet',
     'MultiMutatorsRandomSubnet', 'SupportRandomSubnet', 'get_placeholder',
-    'IndexDict'
+    'IndexDict', 'get_level', 'print_log'
 ]
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/utils/index_dict.py` & `mmrazor-1.0.0rc2/mmrazor/utils/index_dict.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/utils/misc.py` & `mmrazor-1.0.0rc2/mmrazor/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/utils/placeholder.py` & `mmrazor-1.0.0rc2/mmrazor/utils/placeholder.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     Raises:
         ImportError: raise it when the dependency is not installed properly.
 
     Returns:
         object: PlaceHolder instance.
     """
 
-    class PlaceHolder:
+    def raise_import_error(package_name):
+        raise ImportError(
+            f'`{package_name}` is not installed properly, plz check.')
 
-        def __init__(self, *args, **kwargs) -> None:
-            raise ImportError(
-                f'`{string}` is not installed properly, plz check.')
+    class PlaceHolder():
+
+        def __init__(self) -> None:
+            raise_import_error(string)
 
     return PlaceHolder
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/utils/setup_env.py` & `mmrazor-1.0.0rc2/mmrazor/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/utils/typing.py` & `mmrazor-1.0.0rc2/mmrazor/utils/typing.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor/version.py` & `mmrazor-1.0.0rc2/mmrazor/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved
 
-__version__ = '1.0.0rc1'
+__version__ = '1.0.0rc2'
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `mmrazor-1.0.0rc1/mmrazor/visualization/local_visualizer.py` & `mmrazor-1.0.0rc2/mmrazor/visualization/local_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/mmrazor.egg-info/PKG-INFO` & `mmrazor-1.0.0rc2/mmrazor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmrazor
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: OpenMMLab Model Compression Toolbox and Benchmark
 Home-page: https://github.com/open-mmlab/mmrazor
 Author: MMRazor Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmrazor-logo.png" width="600"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmrazor Version: 1.0.0rc1 Summary: OpenMMLab Model
+Metadata-Version: 2.1 Name: mmrazor Version: 1.0.0rc2 Summary: OpenMMLab Model
 Compression Toolbox and Benchmark Home-page: https://github.com/open-mmlab/
 mmrazor Author: MMRazor Contributors Author-email: openmmlab@gmail.com License:
 Apache License 2.0 Description:
                          [resources/mmrazor-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
```

### Comparing `mmrazor-1.0.0rc1/mmrazor.egg-info/SOURCES.txt` & `mmrazor-1.0.0rc2/mmrazor.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,29 @@
 mmrazor.egg-info/dependency_links.txt
 mmrazor.egg-info/not-zip-safe
 mmrazor.egg-info/requires.txt
 mmrazor.egg-info/top_level.txt
 mmrazor/.mim/model-index.yml
 mmrazor/.mim/configs/_base_/datasets/mmcls/cifar100_bs16_auto_aug.py
 mmrazor/.mim/configs/_base_/datasets/mmcls/pipelines/auto_aug_cifar.py
+mmrazor/.mim/configs/_base_/nas_backbones/attentive_mobilenetv3_supernet.py
 mmrazor/.mim/configs/_base_/nas_backbones/darts_supernet.py
 mmrazor/.mim/configs/_base_/nas_backbones/dsnas_shufflenet_supernet.py
+mmrazor/.mim/configs/_base_/nas_backbones/ofa_mobilenetv3_supernet.py
 mmrazor/.mim/configs/_base_/nas_backbones/spos_mobilenet_supernet.py
 mmrazor/.mim/configs/_base_/nas_backbones/spos_shufflenet_supernet.py
 mmrazor/.mim/configs/_base_/settings/cifar10_darts_subnet.py
 mmrazor/.mim/configs/_base_/settings/cifar10_darts_supernet.py
 mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_dsnas.py
 mmrazor/.mim/configs/_base_/settings/imagenet_bs1024_spos.py
+mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_AdamW.py
 mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_autoslim.py
 mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_autoslim_pil.py
+mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_bignas.py
+mmrazor/.mim/configs/_base_/settings/imagenet_bs2048_ofa.py
 mmrazor/.mim/configs/_base_/vanilla_models/wrn16_2_cifar10.py
 mmrazor/.mim/configs/distill/mmcls/abloss/abloss_logits_resnet50_resnet18_8xb32_in1k.py
 mmrazor/.mim/configs/distill/mmcls/abloss/abloss_pretrain_backbone_resnet50_resnet18_8xb32_in1k.py
 mmrazor/.mim/configs/distill/mmcls/abloss/metafile.yml
 mmrazor/.mim/configs/distill/mmcls/byot/byot_resnet18_8xb16_cifar100.py
 mmrazor/.mim/configs/distill/mmcls/byot/metafile.yml
 mmrazor/.mim/configs/distill/mmcls/crd/crd_neck_r50_r18_8xb16_cifar10.py
@@ -59,148 +64,207 @@
 mmrazor/.mim/configs/distill/mmdet/cwd/cwd_cls_head_gfl_r101_fpn_gfl_r50_fpn_1x_coco.py
 mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_frcnn_r101_frcnn_r50_1x_coco.py
 mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco.py
 mmrazor/.mim/configs/distill/mmdet/cwd/cwd_fpn_retina_r101_retina_r50_1x_coco_visualization.py
 mmrazor/.mim/configs/distill/mmdet/cwd/metafile.yml
 mmrazor/.mim/configs/distill/mmdet/fbkd/fbkd_fpn_faster-rcnn_r101_faster-rcnn_r50_1x_coco.py
 mmrazor/.mim/configs/distill/mmdet/fbkd/metafile.yml
+mmrazor/.mim/configs/distill/mmdet/mgd/mgd_fpn_retina_x101_retina_r50_2x_coco.py
 mmrazor/.mim/configs/distill/mmdet/pkd/metafile.yml
 mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_faster-rcnn_r101_faster-rcnn_r50_2x_coco.py
 mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_fcos_x101_retina_r50_1x_coco.py
 mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_mask-rcnn_swin_retina_r50_2x_coco.py
 mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_reppoints_x101-dcn_reppoints_r50_2x_coco.py
 mmrazor/.mim/configs/distill/mmdet/pkd/pkd_fpn_retina_x101_retina_r50_2x_coco.py
 mmrazor/.mim/configs/distill/mmdet3d/pkd/metafile.yml
 mmrazor/.mim/configs/distill/mmdet3d/pkd/pkd_fpn_fcos3d_r101_fcos3d_r50_8xb2-1x_nus-mono3d.py
 mmrazor/.mim/configs/distill/mmseg/cwd/cwd_logits_pspnet_r101-d8_pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
 mmrazor/.mim/configs/distill/mmseg/cwd/metafile.yml
+mmrazor/.mim/configs/nas/mmcls/autoformer/autoformer_search_8xb128_in1k.py
+mmrazor/.mim/configs/nas/mmcls/autoformer/autoformer_supernet_32xb256_in1k.py
+mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_search_8xb256_in1k.py
 mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_slimmable_subnet_8xb256_in1k.py
 mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-220M.py
 mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-320M.py
 mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_subnet_8xb256_in1k_flops-530M.py
 mmrazor/.mim/configs/nas/mmcls/autoslim/autoslim_mbv2_1.5x_supernet_8xb256_in1k.py
 mmrazor/.mim/configs/nas/mmcls/autoslim/metafile.yml
+mmrazor/.mim/configs/nas/mmcls/bignas/attentive_mobilenet_search_8xb128_in1k.py
+mmrazor/.mim/configs/nas/mmcls/bignas/attentive_mobilenet_subnet_8xb256_in1k.py
+mmrazor/.mim/configs/nas/mmcls/bignas/attentive_mobilenet_supernet_32xb64_in1k.py
 mmrazor/.mim/configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0.py
+mmrazor/.mim/configs/nas/mmcls/darts/darts_subnet_1xb96_cifar10_2.0_mmrazor.py
 mmrazor/.mim/configs/nas/mmcls/darts/darts_supernet_unroll_1xb96_cifar10.py
 mmrazor/.mim/configs/nas/mmcls/darts/metafile.yml
 mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_subnet_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmcls/dsnas/dsnas_supernet_8xb128_in1k.py
+mmrazor/.mim/configs/nas/mmcls/onceforall/ofa_mobilenet_search_8xb128_in1k.py
+mmrazor/.mim/configs/nas/mmcls/onceforall/ofa_mobilenet_subnet_8xb256_in1k.py
+mmrazor/.mim/configs/nas/mmcls/onceforall/ofa_mobilenet_supernet_32xb64_in1k.py
+mmrazor/.mim/configs/nas/mmcls/spos/faster-rcnn_nas_backbone_fpn_1x_coco.py
 mmrazor/.mim/configs/nas/mmcls/spos/metafile.yml
 mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_search_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_subnet_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmcls/spos/spos_mobilenet_supernet_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_search_8xb128_in1k.py
+mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_search_predictor_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_subnet_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmcls/spos/spos_shufflenet_supernet_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_search_coco_1x.py
 mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_subnet_coco_1x.py
 mmrazor/.mim/configs/nas/mmdet/detnas/detnas_frcnn_shufflenet_supernet_coco_1x.py
 mmrazor/.mim/configs/nas/mmdet/detnas/detnas_retina_shufflenet_supernet_coco_1x.py
 mmrazor/.mim/configs/nas/mmdet/detnas/detnas_shufflenet_subnet_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmdet/detnas/detnas_shufflenet_supernet_8xb128_in1k.py
 mmrazor/.mim/configs/nas/mmdet/detnas/metafile.yml
-mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k.py
+mmrazor/.mim/configs/pruning/mmcls/dcff/dcff_compact_resnet_8xb32_in1k.py
+mmrazor/.mim/configs/pruning/mmcls/dcff/dcff_resnet_8xb32_in1k.py
+mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k_a.py
+mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k_b.py
+mmrazor/.mim/configs/pruning/mmcls/l1-norm/l1-norm_resnet34_8xb32_in1k_c.py
+mmrazor/.mim/configs/pruning/mmdet/dcff/dcff_compact_faster_rcnn_resnet50_8xb4_coco.py
+mmrazor/.mim/configs/pruning/mmdet/dcff/dcff_faster_rcnn_resnet50_8xb4_coco.py
+mmrazor/.mim/configs/pruning/mmdet/dcff/dcff_faster_rcnn_resnet50_fpn.py
+mmrazor/.mim/configs/pruning/mmpose/dcff/dcff_compact_topdown_heatmap_resnet50_coco.py
+mmrazor/.mim/configs/pruning/mmpose/dcff/dcff_topdown_heatmap_resnet50_coco.py
+mmrazor/.mim/configs/pruning/mmseg/dcff/dcff_compact_pointrend_resnet50_8xb2_cityscapes.py
+mmrazor/.mim/configs/pruning/mmseg/dcff/dcff_pointrend_resnet50_8xb2_cityscapes.py
+mmrazor/.mim/configs/pruning/mmseg/dcff/pointrend_resnet50.py
 mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn16-w2_b16x8_cifar10.py
 mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn22-w4_b16x8_cifar10.py
 mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn28-w4_b16x8_cifar10.py
 mmrazor/.mim/configs/vanilla/mmcls/wide-resnet/wrn40-w2_b16x8_cifar10.py
 mmrazor/.mim/tools/dist_test.sh
 mmrazor/.mim/tools/dist_train.sh
-mmrazor/.mim/tools/get_channel_units.py
 mmrazor/.mim/tools/slurm_test.sh
 mmrazor/.mim/tools/slurm_train.sh
 mmrazor/.mim/tools/test.py
 mmrazor/.mim/tools/train.py
 mmrazor/.mim/tools/misc/print_config.py
+mmrazor/.mim/tools/model_converters/convert_attentivenas_nas_ckpt.py
+mmrazor/.mim/tools/model_converters/convert_bignas_gml_ckpt.py
 mmrazor/.mim/tools/model_converters/convert_kd_ckpt.py
+mmrazor/.mim/tools/model_converters/convert_kd_ckpt_to_student.py
+mmrazor/.mim/tools/model_converters/convert_ofa_ckpt.py
+mmrazor/.mim/tools/model_converters/convert_supernet2subnet.py
 mmrazor/.mim/tools/model_converters/publish_model.py
+mmrazor/.mim/tools/pruning/get_channel_units.py
+mmrazor/.mim/tools/pruning/get_l1_prune_config.py
 mmrazor/.mim/tools/visualizations/feature_diff_visualization.py
 mmrazor/.mim/tools/visualizations/feature_visualization.py
 mmrazor/.mim/tools/visualizations/vis_scheduler.py
 mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_diff_visualization.py
 mmrazor/.mim/tools/visualizations/vis_configs/backbone_feature_visualization.py
 mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_diff_visualization.py
 mmrazor/.mim/tools/visualizations/vis_configs/fpn_feature_visualization.py
 mmrazor/datasets/__init__.py
 mmrazor/datasets/crd_dataset_wrapper.py
 mmrazor/datasets/transforms/__init__.py
+mmrazor/datasets/transforms/auto_augment.py
+mmrazor/datasets/transforms/auto_augmentv2.py
 mmrazor/datasets/transforms/formatting.py
 mmrazor/engine/__init__.py
 mmrazor/engine/hooks/__init__.py
 mmrazor/engine/hooks/dump_subnet_hook.py
 mmrazor/engine/hooks/estimate_resources_hook.py
 mmrazor/engine/hooks/visualization_hook.py
 mmrazor/engine/optimizers/__init__.py
 mmrazor/engine/optimizers/optimizer_constructor.py
 mmrazor/engine/runner/__init__.py
-mmrazor/engine/runner/autoslim_val_loop.py
+mmrazor/engine/runner/autoslim_greedy_search_loop.py
 mmrazor/engine/runner/darts_loop.py
 mmrazor/engine/runner/distill_val_loop.py
 mmrazor/engine/runner/evolution_search_loop.py
+mmrazor/engine/runner/iteprune_val_loop.py
 mmrazor/engine/runner/slimmable_val_loop.py
 mmrazor/engine/runner/subnet_sampler_loop.py
+mmrazor/engine/runner/subnet_val_loop.py
 mmrazor/engine/runner/utils/__init__.py
+mmrazor/engine/runner/utils/calibrate_bn_mixin.py
 mmrazor/engine/runner/utils/check.py
 mmrazor/engine/runner/utils/genetic.py
 mmrazor/models/__init__.py
 mmrazor/models/algorithms/__init__.py
 mmrazor/models/algorithms/base.py
 mmrazor/models/algorithms/distill/__init__.py
 mmrazor/models/algorithms/distill/configurable/__init__.py
 mmrazor/models/algorithms/distill/configurable/datafree_distillation.py
 mmrazor/models/algorithms/distill/configurable/fpn_teacher_distill.py
 mmrazor/models/algorithms/distill/configurable/overhaul_feature_distillation.py
 mmrazor/models/algorithms/distill/configurable/self_distill.py
 mmrazor/models/algorithms/distill/configurable/single_teacher_distill.py
 mmrazor/models/algorithms/nas/__init__.py
+mmrazor/models/algorithms/nas/autoformer.py
 mmrazor/models/algorithms/nas/autoslim.py
+mmrazor/models/algorithms/nas/bignas.py
 mmrazor/models/algorithms/nas/darts.py
 mmrazor/models/algorithms/nas/dsnas.py
 mmrazor/models/algorithms/nas/spos.py
 mmrazor/models/algorithms/pruning/__init__.py
+mmrazor/models/algorithms/pruning/dcff.py
 mmrazor/models/algorithms/pruning/ite_prune_algorithm.py
 mmrazor/models/algorithms/pruning/slimmable_network.py
 mmrazor/models/architectures/__init__.py
 mmrazor/models/architectures/backbones/__init__.py
 mmrazor/models/architectures/backbones/darts_backbone.py
-mmrazor/models/architectures/backbones/searchable_mobilenet.py
+mmrazor/models/architectures/backbones/searchable_autoformer.py
+mmrazor/models/architectures/backbones/searchable_mobilenet_v2.py
+mmrazor/models/architectures/backbones/searchable_mobilenet_v3.py
 mmrazor/models/architectures/backbones/searchable_shufflenet_v2.py
 mmrazor/models/architectures/backbones/wideresnet.py
+mmrazor/models/architectures/classifiers/__init__.py
+mmrazor/models/architectures/classifiers/image.py
 mmrazor/models/architectures/connectors/__init__.py
 mmrazor/models/architectures/connectors/base_connector.py
 mmrazor/models/architectures/connectors/byot_connector.py
 mmrazor/models/architectures/connectors/convmodule_connector.py
 mmrazor/models/architectures/connectors/crd_connector.py
 mmrazor/models/architectures/connectors/factor_transfer_connectors.py
 mmrazor/models/architectures/connectors/fbkd_connector.py
+mmrazor/models/architectures/connectors/mgd_connector.py
 mmrazor/models/architectures/connectors/ofd_connector.py
 mmrazor/models/architectures/connectors/torch_connector.py
 mmrazor/models/architectures/dynamic_ops/__init__.py
 mmrazor/models/architectures/dynamic_ops/bricks/__init__.py
+mmrazor/models/architectures/dynamic_ops/bricks/dynamic_container.py
 mmrazor/models/architectures/dynamic_ops/bricks/dynamic_conv.py
+mmrazor/models/architectures/dynamic_ops/bricks/dynamic_embed.py
+mmrazor/models/architectures/dynamic_ops/bricks/dynamic_function.py
 mmrazor/models/architectures/dynamic_ops/bricks/dynamic_linear.py
+mmrazor/models/architectures/dynamic_ops/bricks/dynamic_multi_head_attention.py
 mmrazor/models/architectures/dynamic_ops/bricks/dynamic_norm.py
+mmrazor/models/architectures/dynamic_ops/bricks/dynamic_relative_position.py
+mmrazor/models/architectures/dynamic_ops/head/__init__.py
+mmrazor/models/architectures/dynamic_ops/head/dynamic_linear_head.py
 mmrazor/models/architectures/dynamic_ops/mixins/__init__.py
 mmrazor/models/architectures/dynamic_ops/mixins/dynamic_conv_mixins.py
+mmrazor/models/architectures/dynamic_ops/mixins/dynamic_layernorm_mixins.py
 mmrazor/models/architectures/dynamic_ops/mixins/dynamic_mixins.py
 mmrazor/models/architectures/generators/__init__.py
 mmrazor/models/architectures/generators/base_generator.py
 mmrazor/models/architectures/generators/dafl_generator.py
 mmrazor/models/architectures/generators/zskt_generator.py
 mmrazor/models/architectures/heads/__init__.py
 mmrazor/models/architectures/heads/darts_subnet_head.py
 mmrazor/models/architectures/heads/deit_head.py
+mmrazor/models/architectures/necks/__init__.py
+mmrazor/models/architectures/necks/squeezemean_with_dropout.py
 mmrazor/models/architectures/ops/__init__.py
 mmrazor/models/architectures/ops/base.py
 mmrazor/models/architectures/ops/common.py
 mmrazor/models/architectures/ops/darts_series.py
 mmrazor/models/architectures/ops/efficientnet_series.py
+mmrazor/models/architectures/ops/function.py
 mmrazor/models/architectures/ops/gather_tensors.py
 mmrazor/models/architectures/ops/mobilenet_series.py
 mmrazor/models/architectures/ops/shufflenet_series.py
+mmrazor/models/architectures/ops/transformer_series.py
+mmrazor/models/architectures/utils/__init__.py
+mmrazor/models/architectures/utils/mutable_register.py
+mmrazor/models/architectures/utils/set_dropout.py
 mmrazor/models/distillers/__init__.py
 mmrazor/models/distillers/base_distiller.py
 mmrazor/models/distillers/byot_distiller.py
 mmrazor/models/distillers/configurable_distiller.py
 mmrazor/models/distillers/ofd_distiller.py
 mmrazor/models/losses/__init__.py
 mmrazor/models/losses/ab_loss.py
@@ -212,57 +276,68 @@
 mmrazor/models/losses/decoupled_kd.py
 mmrazor/models/losses/factor_transfer_loss.py
 mmrazor/models/losses/fbkd_loss.py
 mmrazor/models/losses/kd_soft_ce_loss.py
 mmrazor/models/losses/kl_divergence.py
 mmrazor/models/losses/l1_loss.py
 mmrazor/models/losses/l2_loss.py
+mmrazor/models/losses/mgd_loss.py
 mmrazor/models/losses/ofd_loss.py
 mmrazor/models/losses/pkd_loss.py
 mmrazor/models/losses/relational_kd.py
 mmrazor/models/losses/weighted_soft_label_distillation.py
 mmrazor/models/mutables/__init__.py
 mmrazor/models/mutables/base_mutable.py
 mmrazor/models/mutables/derived_mutable.py
 mmrazor/models/mutables/mutable_channel/__init__.py
 mmrazor/models/mutables/mutable_channel/base_mutable_channel.py
 mmrazor/models/mutables/mutable_channel/mutable_channel_container.py
-mmrazor/models/mutables/mutable_channel/oneshot_mutalbe_channel.py
+mmrazor/models/mutables/mutable_channel/oneshot_mutable_channel.py
 mmrazor/models/mutables/mutable_channel/sequential_mutable_channel.py
 mmrazor/models/mutables/mutable_channel/simple_mutable_channel.py
 mmrazor/models/mutables/mutable_channel/units/__init__.py
 mmrazor/models/mutables/mutable_channel/units/channel_unit.py
+mmrazor/models/mutables/mutable_channel/units/dcff_channel_unit.py
 mmrazor/models/mutables/mutable_channel/units/l1_mutable_channel_unit.py
 mmrazor/models/mutables/mutable_channel/units/mutable_channel_unit.py
 mmrazor/models/mutables/mutable_channel/units/one_shot_mutable_channel_unit.py
 mmrazor/models/mutables/mutable_channel/units/sequential_mutable_channel_unit.py
 mmrazor/models/mutables/mutable_channel/units/slimmable_channel_unit.py
+mmrazor/models/mutables/mutable_channel/units/utils.py
 mmrazor/models/mutables/mutable_module/__init__.py
 mmrazor/models/mutables/mutable_module/diff_mutable_module.py
 mmrazor/models/mutables/mutable_module/mutable_module.py
 mmrazor/models/mutables/mutable_module/one_shot_mutable_module.py
 mmrazor/models/mutables/mutable_value/__init__.py
 mmrazor/models/mutables/mutable_value/mutable_value.py
 mmrazor/models/mutators/__init__.py
 mmrazor/models/mutators/base_mutator.py
 mmrazor/models/mutators/group_mixin.py
 mmrazor/models/mutators/channel_mutator/__init__.py
 mmrazor/models/mutators/channel_mutator/channel_mutator.py
+mmrazor/models/mutators/channel_mutator/dcff_channel_mutator.py
 mmrazor/models/mutators/channel_mutator/one_shot_channel_mutator.py
 mmrazor/models/mutators/channel_mutator/slimmable_channel_mutator.py
 mmrazor/models/mutators/module_mutator/__init__.py
 mmrazor/models/mutators/module_mutator/diff_module_mutator.py
 mmrazor/models/mutators/module_mutator/module_mutator.py
 mmrazor/models/mutators/module_mutator/one_shot_module_mutator.py
+mmrazor/models/mutators/value_mutator/__init__.py
+mmrazor/models/mutators/value_mutator/dynamic_value_mutator.py
+mmrazor/models/mutators/value_mutator/value_mutator.py
 mmrazor/models/task_modules/__init__.py
 mmrazor/models/task_modules/delivery/__init__.py
 mmrazor/models/task_modules/delivery/delivery_manager.py
 mmrazor/models/task_modules/delivery/distill_delivery.py
 mmrazor/models/task_modules/delivery/function_outputs_delivery.py
 mmrazor/models/task_modules/delivery/method_outputs_delivery.py
+mmrazor/models/task_modules/demo_inputs/__init__.py
+mmrazor/models/task_modules/demo_inputs/default_demo_inputs.py
+mmrazor/models/task_modules/demo_inputs/demo_inputs.py
+mmrazor/models/task_modules/demo_inputs/mmseg_demo_input.py
 mmrazor/models/task_modules/estimators/__init__.py
 mmrazor/models/task_modules/estimators/base_estimator.py
 mmrazor/models/task_modules/estimators/resource_estimator.py
 mmrazor/models/task_modules/estimators/counters/__init__.py
 mmrazor/models/task_modules/estimators/counters/flops_params_counter.py
 mmrazor/models/task_modules/estimators/counters/latency_counter.py
 mmrazor/models/task_modules/estimators/counters/op_counters/__init__.py
@@ -270,78 +345,108 @@
 mmrazor/models/task_modules/estimators/counters/op_counters/base_counter.py
 mmrazor/models/task_modules/estimators/counters/op_counters/conv_layer_counter.py
 mmrazor/models/task_modules/estimators/counters/op_counters/deconv_layer_counter.py
 mmrazor/models/task_modules/estimators/counters/op_counters/linear_layer_counter.py
 mmrazor/models/task_modules/estimators/counters/op_counters/norm_layer_counter.py
 mmrazor/models/task_modules/estimators/counters/op_counters/pooling_layer_counter.py
 mmrazor/models/task_modules/estimators/counters/op_counters/upsample_layer_counter.py
+mmrazor/models/task_modules/predictor/__init__.py
+mmrazor/models/task_modules/predictor/metric_predictor.py
+mmrazor/models/task_modules/predictor/handler/__init__.py
+mmrazor/models/task_modules/predictor/handler/base_handler.py
+mmrazor/models/task_modules/predictor/handler/carts_handler.py
+mmrazor/models/task_modules/predictor/handler/gp_handler.py
+mmrazor/models/task_modules/predictor/handler/mlp_handler.py
+mmrazor/models/task_modules/predictor/handler/rbf_handler.py
 mmrazor/models/task_modules/recorder/__init__.py
 mmrazor/models/task_modules/recorder/base_recorder.py
 mmrazor/models/task_modules/recorder/function_inputs_recorder.py
 mmrazor/models/task_modules/recorder/function_outputs_recorder.py
 mmrazor/models/task_modules/recorder/method_inputs_recorder.py
 mmrazor/models/task_modules/recorder/method_outputs_recorder.py
 mmrazor/models/task_modules/recorder/module_inputs_recorder.py
 mmrazor/models/task_modules/recorder/module_outputs_recorder.py
 mmrazor/models/task_modules/recorder/param_recorder.py
 mmrazor/models/task_modules/recorder/recorder_manager.py
 mmrazor/models/task_modules/tracer/__init__.py
 mmrazor/models/task_modules/tracer/backward_tracer.py
+mmrazor/models/task_modules/tracer/channel_analyzer.py
+mmrazor/models/task_modules/tracer/fx_tracer.py
 mmrazor/models/task_modules/tracer/parsers.py
 mmrazor/models/task_modules/tracer/path.py
 mmrazor/models/task_modules/tracer/loss_calculator/__init__.py
+mmrazor/models/task_modules/tracer/loss_calculator/cascade_encoder_decoder_loss_calculator.py
 mmrazor/models/task_modules/tracer/loss_calculator/image_classifier_loss_calculator.py
 mmrazor/models/task_modules/tracer/loss_calculator/single_stage_detector_loss_calculator.py
+mmrazor/models/task_modules/tracer/loss_calculator/sum_loss_calculator.py
+mmrazor/models/task_modules/tracer/loss_calculator/top_down_pose_estimator_loss_calculator.py
+mmrazor/models/task_modules/tracer/loss_calculator/two_stage_detector_loss_calculator.py
 mmrazor/models/utils/__init__.py
 mmrazor/models/utils/make_divisible.py
 mmrazor/models/utils/misc.py
 mmrazor/models/utils/optim_wrapper.py
+mmrazor/models/utils/parse_values.py
 mmrazor/models/utils/utils.py
 mmrazor/registry/__init__.py
 mmrazor/registry/registry.py
 mmrazor/structures/__init__.py
 mmrazor/structures/graph/__init__.py
 mmrazor/structures/graph/base_graph.py
+mmrazor/structures/graph/channel_flow.py
 mmrazor/structures/graph/channel_graph.py
-mmrazor/structures/graph/channel_modules.py
 mmrazor/structures/graph/channel_nodes.py
 mmrazor/structures/graph/module_graph.py
+mmrazor/structures/graph/pseudo_fx_graph.py
 mmrazor/structures/subnet/__init__.py
 mmrazor/structures/subnet/candidate.py
 mmrazor/structures/subnet/fix_subnet.py
 mmrazor/testing/__init__.py
 mmrazor/testing/_fast_stop_training_hook.py
 mmrazor/utils/__init__.py
 mmrazor/utils/index_dict.py
+mmrazor/utils/log_tools.py
 mmrazor/utils/misc.py
 mmrazor/utils/placeholder.py
 mmrazor/utils/setup_env.py
 mmrazor/utils/typing.py
 mmrazor/visualization/__init__.py
 mmrazor/visualization/local_visualizer.py
 requirements/docs.txt
 requirements/mminstall.txt
 requirements/optional.txt
 requirements/readthedocs.txt
 requirements/runtime.txt
 requirements/tests.txt
 tests/__init__.py
-tests/test_metafiles.py
+tests/test_data.py
+tests/test_doc.py
 tests/data/__init__.py
+tests/data/model_library.py
 tests/data/models.py
+tests/data/tracer_passed_models.py
 tests/test_core/__init__.py
 tests/test_core/test_graph/__init__.py
+tests/test_core/test_graph/test_channel_flow.py
 tests/test_core/test_graph/test_channel_graph.py
 tests/test_core/test_graph/test_graph.py
+tests/test_core/test_graph/test_prune_tracer_model.py
+tests/test_core/test_tracer/__init__.py
+tests/test_core/test_tracer/test_backward_tracer.py
+tests/test_core/test_tracer/test_fx_tracer.py
+tests/test_core/test_tracer/test_loss_calculator.py
+tests/test_core/test_tracer/test_prune_tracer.py
 tests/test_models/__init__.py
 tests/test_models/test_algorithms/__init__.py
+tests/test_models/test_algorithms/test_autoformer.py
 tests/test_models/test_algorithms/test_autoslim.py
 tests/test_models/test_algorithms/test_base_algorithm.py
+tests/test_models/test_algorithms/test_bignas.py
 tests/test_models/test_algorithms/test_darts.py
 tests/test_models/test_algorithms/test_datafree_distill.py
+tests/test_models/test_algorithms/test_dcff_network.py
 tests/test_models/test_algorithms/test_dsnas.py
 tests/test_models/test_algorithms/test_ofd_algo.py
 tests/test_models/test_algorithms/test_prune_algorithm.py
 tests/test_models/test_algorithms/test_self_distill.py
 tests/test_models/test_algorithms/test_single_teacher_distill.py
 tests/test_models/test_algorithms/test_slimmable_network.py
 tests/test_models/test_algorithms/test_spos.py
@@ -350,19 +455,31 @@
 tests/test_models/test_mutables/test_derived_mutable.py
 tests/test_models/test_mutables/test_diffchoiceroute.py
 tests/test_models/test_mutables/test_diffop.py
 tests/test_models/test_mutables/test_gumbelchoiceroute.py
 tests/test_models/test_mutables/test_mutable_value.py
 tests/test_models/test_mutables/test_onehotop.py
 tests/test_models/test_mutables/test_oneshotop.py
+tests/test_models/test_mutables/test_sequential_mutable_channel.py
 tests/test_models/test_mutables/test_mutable_channel/__init__.py
 tests/test_models/test_mutables/test_mutable_channel/test_mutable_channels.py
 tests/test_models/test_mutables/test_mutable_channel/test_sequential_mutable_channel.py
 tests/test_models/test_mutables/test_mutable_channel/test_units/__init__.py
+tests/test_models/test_mutables/test_mutable_channel/test_units/test_dcff_channel_unit.py
 tests/test_models/test_mutables/test_mutable_channel/test_units/test_l1_mutable_channel_unit.py
 tests/test_models/test_mutables/test_mutable_channel/test_units/test_mutable_channel_units.py
 tests/test_models/test_mutables/test_mutable_channel/test_units/test_one_shot_mutable_channel_unit.py
 tests/test_models/test_mutables/test_mutable_channel/test_units/test_sequential_mutable_channel_unit.py
 tests/test_models/test_mutators/__init__.py
 tests/test_models/test_mutators/test_channel_mutator.py
+tests/test_models/test_mutators/test_dcff_mutator.py
 tests/test_models/test_mutators/test_diff_mutator.py
-tests/test_models/test_mutators/test_classical_models/__init__.py
+tests/test_models/test_mutators/test_value_mutator.py
+tests/test_models/test_mutators/test_classical_models/__init__.py
+tests/test_models/test_task_modules/__init__.py
+tests/test_models/test_task_modules/test_demo_inputs/__init__.py
+tests/test_models/test_task_modules/test_demo_inputs/test_demo_inputs.py
+tests/test_tools/__init__.py
+tests/test_tools/test_tools.py
+tests/utils/__init__.py
+tests/utils/set_dist_env.py
+tests/utils/set_torch_thread.py
```

### Comparing `mmrazor-1.0.0rc1/setup.cfg` & `mmrazor-1.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/setup.py` & `mmrazor-1.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_autoslim.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_autoslim.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,24 +25,33 @@
     head=dict(
         type='mmcls.LinearClsHead',
         num_classes=1000,
         in_channels=1920,
         loss=dict(type='mmcls.CrossEntropyLoss', loss_weight=1.0),
         topk=(1, 5)))
 
+ONESHOT_MUTABLE_CFG = dict(
+    type='OneShotMutableChannel',
+    candidate_choices=[1 / 8, 2 / 8, 3 / 8, 4 / 8, 5 / 8, 6 / 8, 7 / 8, 1.0],
+    candidate_mode='ratio')
+ONESHOT_MUTABLE_CFGS = dict(
+    in_features=ONESHOT_MUTABLE_CFG,
+    out_features=ONESHOT_MUTABLE_CFG,
+    in_channels=ONESHOT_MUTABLE_CFG,
+    out_channels=ONESHOT_MUTABLE_CFG,
+    num_features=ONESHOT_MUTABLE_CFG)
+
 MUTATOR_CFG = dict(
     type='OneShotChannelMutator',
     channel_unit_cfg=dict(
         type='OneShotMutableChannelUnit',
         default_args=dict(
             candidate_choices=list(i / 12 for i in range(2, 13)),
             choice_mode='ratio')),
-    parse_cfg=dict(
-        type='BackwardTracer',
-        loss_calculator=dict(type='ImageClassifierPseudoLoss')))
+    parse_cfg=dict(type='ChannelAnalyzer'))
 
 DISTILLER_CFG = dict(
     type='ConfigurableDistiller',
     teacher_recorders=dict(fc=dict(type='ModuleOutputs', source='head.fc')),
     student_recorders=dict(fc=dict(type='ModuleOutputs', source='head.fc')),
     distill_losses=dict(
         loss_kl=dict(type='KLDivergence', tau=1, loss_weight=1)),
@@ -104,18 +113,18 @@
         assert not algo._optim_wrapper_count_status_reinitialized
         losses = algo.train_step(data, optim_wrapper)
 
         assert len(losses) == 7
         assert losses['max_subnet.loss'] > 0
         assert losses['min_subnet.loss'] > 0
         assert losses['min_subnet.loss_kl'] + 1e-5 > 0
-        assert losses['random_subnet_0.loss'] > 0
-        assert losses['random_subnet_0.loss_kl'] + 1e-5 > 0
-        assert losses['random_subnet_1.loss'] > 0
-        assert losses['random_subnet_1.loss_kl'] + 1e-5 > 0
+        assert losses['random0_subnet.loss'] > 0
+        assert losses['random0_subnet.loss_kl'] + 1e-5 > 0
+        assert losses['random1_subnet.loss'] > 0
+        assert losses['random1_subnet.loss_kl'] + 1e-5 > 0
 
         assert algo._optim_wrapper_count_status_reinitialized
         assert optim_wrapper._inner_count == 4
         assert optim_wrapper._max_counts == 400
 
         losses = algo.train_step(data, optim_wrapper)
         assert algo._optim_wrapper_count_status_reinitialized
@@ -129,21 +138,21 @@
 
         return {'inputs': imgs, 'data_samples': data_samples}
 
     def prepare_model(self,
                       mutator_cfg: MUTATOR_TYPE = MUTATOR_CFG,
                       distiller_cfg: DISTILLER_TYPE = DISTILLER_CFG,
                       architecture_cfg: Dict = ARCHITECTURE_CFG,
-                      num_samples: int = 2) -> AutoSlim:
+                      num_random_samples: int = 2) -> AutoSlim:
         model = AutoSlim(
             mutator=mutator_cfg,
             distiller=distiller_cfg,
             architecture=architecture_cfg,
             data_preprocessor=ToyDataPreprocessor(),
-            num_samples=num_samples)
+            num_random_samples=num_random_samples)
         model.to(self.device)
 
         return model
 
 
 class TestAutoSlimDDP(TestAutoSlim):
 
@@ -160,20 +169,20 @@
             backend = 'gloo'
         dist.init_process_group(backend, rank=0, world_size=1)
 
     def prepare_model(self,
                       mutator_cfg: MUTATOR_TYPE = MUTATOR_CFG,
                       distiller_cfg: DISTILLER_TYPE = DISTILLER_CFG,
                       architecture_cfg: Dict = ARCHITECTURE_CFG,
-                      num_samples: int = 2) -> AutoSlim:
+                      num_random_samples: int = 2) -> AutoSlim:
         model = super().prepare_model(
             mutator_cfg=mutator_cfg,
             distiller_cfg=distiller_cfg,
             architecture_cfg=architecture_cfg,
-            num_samples=num_samples)
+            num_random_samples=num_random_samples)
 
         return AutoSlimDDP(module=model, find_unused_parameters=True)
 
     @classmethod
     def tearDownClass(cls) -> None:
         dist.destroy_process_group()
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_base_algorithm.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_base_algorithm.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_darts.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_darts.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_datafree_distill.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_datafree_distill.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_dsnas.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_dsnas.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_ofd_algo.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_ofd_algo.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_self_distill.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_self_distill.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_single_teacher_distill.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_single_teacher_distill.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_slimmable_network.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_slimmable_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,15 @@
         loss=dict(type='CrossEntropyLoss', loss_weight=1.0),
         topk=(1, 5)))
 CHANNEL_CFG_PATH = 'tests/data/MBV2_slimmable_config.json'
 
 MUTATOR_CFG = dict(
     type='SlimmableChannelMutator',
     channel_unit_cfg=dict(type='SlimmableChannelUnit', units=CHANNEL_CFG_PATH),
-    parse_cfg=dict(
-        type='BackwardTracer',
-        loss_calculator=dict(type='ImageClassifierPseudoLoss')))
+    parse_cfg=dict(type='ChannelAnalyzer'))
 
 CHANNEL_CFG_PATHS = [
     'tests/data/MBV2_220M.yaml',
     'tests/data/MBV2_320M.yaml',
     'tests/data/MBV2_530M.yaml',
 ]
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/test_spos.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/test_spos.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_algorithms/toy_models.py` & `mmrazor-1.0.0rc2/tests/test_models/test_algorithms/toy_models.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_derived_mutable.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_derived_mutable.py`

 * *Files 23% similar despite different names*

```diff
@@ -119,14 +119,35 @@
         assert mv_derived.source_mutables == {mv}
 
         mv.current_choice == 128
         assert mv_derived.current_choice == 16
         mv.current_choice == 120
         assert mv_derived.current_choice == 16
 
+        mc_derived = mc // 8.0
+        assert mc_derived.source_mutables == {mc}
+
+        mc.current_choice = 128.
+        assert mc_derived.current_choice == 16
+        assert torch.equal(mc_derived.current_mask,
+                           torch.ones(16, dtype=torch.bool))
+        mc.current_choice = 120.
+        assert mc_derived.current_choice == 16
+        assert torch.equal(mc_derived.current_mask,
+                           torch.ones(16, dtype=torch.bool))
+
+        mv = OneShotMutableValue(value_list=[112, 120, 128])
+        mv_derived = mv // 8.0
+        assert mv_derived.source_mutables == {mv}
+
+        mv.current_choice == 128.
+        assert mv_derived.current_choice == 16
+        mv.current_choice == 120.
+        assert mv_derived.current_choice == 16
+
     def test_source_mutables(self) -> None:
 
         def useless_fn(x):
             return x  # noqa: E731
 
         with pytest.raises(RuntimeError):
             _ = DerivedMutable(choice_fn=useless_fn)
@@ -203,14 +224,51 @@
                            torch.tensor([1, 1, 1, 1, 0], dtype=torch.bool))
 
         assert derived_e.current_choice == 5
         assert torch.equal(
             derived_e.current_mask,
             torch.tensor([1, 0, 1, 1, 1, 1, 0], dtype=torch.bool))
 
+    def test_mutable_channel_value_calculation(self) -> None:
+        mc = SquentialMutableChannel(num_channels=10)
+        mv = OneShotMutableValue(value_list=[2.0, 2.5, 3.0, 3.5])
+        derived_mutable = mc * mv
+        assert derived_mutable.source_mutables == {mv, mc}
+
+        mc.current_choice = 6
+        mv.current_choice = 3.5
+        assert derived_mutable.current_choice == 21
+
+        mc.current_choice = 9
+        mv.current_choice = 3.5
+        assert derived_mutable.current_choice == 31
+
+        mc.current_choice = 7
+        mv.current_choice = 2.5
+        assert derived_mutable.current_choice == 17
+
+        assert isinstance(derived_mutable, BaseMutable)
+        assert isinstance(derived_mutable, DerivedMutable)
+        assert not derived_mutable.is_fixed
+
+        mc.current_choice = mc.num_channels
+        mv.current_choice = mv.min_choice
+        assert derived_mutable.current_choice == \
+            mv.current_choice * mc.num_channels
+        mv.current_choice = mv.max_choice
+        assert derived_mutable.current_choice == \
+            mv.current_choice * mc.current_choice
+
+        with pytest.raises(RuntimeError):
+            derived_mutable.is_fixed = True
+        mc.fix_chosen(mc.dump_chosen().chosen)
+        assert not derived_mutable.is_fixed
+        mv.fix_chosen(mv.dump_chosen().chosen)
+        assert derived_mutable.is_fixed
+
 
 @pytest.mark.parametrize('expand_ratio', [1, 2, 3])
 def test_derived_expand_mutable(expand_ratio: int) -> None:
     mv = OneShotMutableValue(value_list=[3, 5, 7])
 
     mv_derived = mv * expand_ratio
     assert mv_derived.source_mutables == {mv}
@@ -228,7 +286,33 @@
     with pytest.raises(RuntimeError):
         mv_derived.current_choice = 123
     with pytest.raises(RuntimeError):
         _ = mv_derived.current_mask
 
     mv.current_choice = 5
     assert mv_derived.current_choice == 5 * expand_ratio
+
+
+@pytest.mark.parametrize('expand_ratio', [1.5, 2.0, 2.5])
+def test_derived_expand_mutable_float(expand_ratio: float) -> None:
+    mv = OneShotMutableValue(value_list=[3, 5, 7])
+
+    mv_derived = mv * expand_ratio
+    assert mv_derived.source_mutables == {mv}
+
+    assert isinstance(mv_derived, BaseMutable)
+    assert isinstance(mv_derived, DerivedMutable)
+    assert not mv_derived.is_fixed
+    assert mv_derived.num_choices == 1
+
+    mv.current_choice = mv.max_choice
+    assert mv_derived.current_choice == int(mv.current_choice * expand_ratio)
+    mv.current_choice = mv.min_choice
+    assert mv_derived.current_choice == int(mv.current_choice * expand_ratio)
+
+    with pytest.raises(RuntimeError):
+        mv_derived.current_choice = 123
+    with pytest.raises(RuntimeError):
+        _ = mv_derived.current_mask
+
+    mv.current_choice = 5
+    assert mv_derived.current_choice == int(5 * expand_ratio)
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_diffchoiceroute.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_diffchoiceroute.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_diffop.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_diffop.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_gumbelchoiceroute.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_gumbelchoiceroute.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_mutable_channels.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_mutable_channels.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,8 @@
         mutable_channel.dump_chosen()
 
     def test_SimpleMutableChannel(self):
         channel = SimpleMutableChannel(4)
         channel.current_choice = torch.tensor([1, 0, 0, 0]).bool()
         self.assertEqual(channel.activated_channels, 1)
         channel.fix_chosen()
-        # with pytest.raises(NotImplementedError):
-        #     channel.dump_chosen()
+        channel.dump_chosen()
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_sequential_mutable_channel.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_sequential_mutable_channel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from unittest import TestCase
 
 import torch
 
-from mmrazor.models.mutables import SquentialMutableChannel
+from mmrazor.models.mutables import (OneShotMutableValue,
+                                     SquentialMutableChannel)
 
 
 class TestSquentialMutableChannel(TestCase):
 
     def _test_mutable(self,
                       mutable: SquentialMutableChannel,
                       set_choice,
@@ -37,7 +38,20 @@
         self._test_mutable(channel, 5, 5, 5, self._generate_mask(5, 10))
         self._test_mutable(channel, 0.2, 2, 2, self._generate_mask(2, 10))
 
     def test_float_choice(self):
         channel = SquentialMutableChannel(10, choice_mode='ratio')
         self._test_mutable(channel, 0.5, 0.5, 5, self._generate_mask(5, 10))
         self._test_mutable(channel, 2, 0.2, 2, self._generate_mask(2, 10))
+
+    def test_mutable_channel_mul(self):
+        channel = SquentialMutableChannel(2)
+        self.assertEqual(channel.current_choice, 2)
+        mv = OneShotMutableValue(value_list=[1, 2, 3], default_value=3)
+        derived1 = channel * mv
+        derived2 = mv * channel
+        assert derived1.current_choice == 6
+        assert derived2.current_choice == 6
+        mv.current_choice = mv.min_choice
+        assert derived1.current_choice == 2
+        assert derived2.current_choice == 2
+        assert torch.equal(derived1.current_mask, derived2.current_mask)
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/test_l1_mutable_channel_unit.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_one_shot_mutable_channel_unit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from unittest import TestCase
 
-import torch.nn as nn
+from mmrazor.models.mutables import OneShotMutableChannelUnit
+from mmrazor.models.mutators.channel_mutator import ChannelMutator
+from tests.data.models import DynamicAttention
 
-from mmrazor.models.mutables import L1MutableChannelUnit
-from mmrazor.models.mutators import ChannelMutator
-from .....data.models import LineModel
 
-
-class TestL1MutableChannelUnit(TestCase):
+class TestSequentialMutableChannelUnit(TestCase):
 
     def test_init(self):
-        model = LineModel()
+        unit = OneShotMutableChannelUnit(
+            48, [20, 30, 40], choice_mode='number', divisor=8)
+        self.assertSequenceEqual(unit.candidate_choices, [24, 32, 40])
+
+        unit = OneShotMutableChannelUnit(
+            48, [0.3, 0.5, 0.7], choice_mode='ratio', divisor=8)
+        self.assertSequenceEqual(unit.candidate_choices, [1 / 3, 0.5, 2 / 3])
+
+    def test_unit_predefined(self):
+        model = DynamicAttention()
         mutator = ChannelMutator(
             channel_unit_cfg={
-                'type': 'L1MutableChannelUnit',
+                'type': 'OneShotMutableChannelUnit',
                 'default_args': {
-                    'choice_mode': 'ratio'
+                    'unit_predefined': False
                 }
-            })
+            },
+            parse_cfg={'type': 'Predefined'})
         mutator.prepare_from_supernet(model)
-        mutator.set_choices(mutator.sample_choices())
-        print(mutator.units)
-        print(mutator.mutable_units)
-        print(mutator.choice_template)
-
-    def test_convnd(self):
-        unit = L1MutableChannelUnit(8)
-        conv = nn.Conv3d(3, 8, 3)
-        norm = unit._get_l1_norm(conv, 0, 8)
-        self.assertSequenceEqual(norm.shape, [8])
+        choices = mutator.sample_choices()
+        mutator.set_choices(choices)
+        self.assertSequenceEqual(mutator.units[0].candidate_choices,
+                                 [576, 624])
+        self.assertSequenceEqual(mutator.units[1].candidate_choices, [64])
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/test_mutable_channel_units.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_mutable_channel_units.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,46 +4,55 @@
 
 import torch
 import torch.nn as nn
 
 from mmrazor.models.architectures.dynamic_ops.mixins import DynamicChannelMixin
 from mmrazor.models.mutables.mutable_channel import (
     L1MutableChannelUnit, MutableChannelUnit, SequentialMutableChannelUnit)
-from mmrazor.models.mutables.mutable_channel.units.channel_unit import (  # noqa
-    Channel, ChannelUnit)
-from mmrazor.structures.graph import ModuleGraph as ModuleGraph
-from .....data.models import LineModel
-from .....test_core.test_graph.test_graph import TestGraph
+from mmrazor.models.mutables.mutable_channel.units.channel_unit import \
+    ChannelUnit
+from .....data.models import SingleLineModel
+from .....data.tracer_passed_models import backward_passed_library
 
 MUTABLE_CFG = dict(type='SimpleMutablechannel')
 PARSE_CFG = dict(
-    type='BackwardTracer',
-    loss_calculator=dict(type='ImageClassifierPseudoLoss'))
+    type='ChannelAnalyzer',
+    demo_input=(1, 3, 224, 224),
+    tracer_type='BackwardTracer')
 
-# DEVICE = torch.device('cuda:0') if torch.cuda.is_available() \
-#     else torch.device('cpu')
 DEVICE = torch.device('cpu')
-GROUPS: List[MutableChannelUnit] = [
+UNITS: List[MutableChannelUnit] = [
     L1MutableChannelUnit, SequentialMutableChannelUnit
 ]
 
 DefaultChannelUnit = SequentialMutableChannelUnit
 
 
-class TestMutableChannelUnit(TestCase):
+def _test_units(units: List[MutableChannelUnit], model):
+    for unit in units:
+        unit.prepare_for_pruning(model)
+    for unit in units:
+        _ = unit.current_choice
+
+    mutable_units = [unit for unit in units if unit.is_mutable]
+    assert len(mutable_units) >= 1, \
+        'len of mutable units should greater or equal than 0.'
+    for unit in mutable_units:
+        choice = unit.sample_choice()
+        unit.current_choice = choice
+        assert abs(unit.current_choice - choice) < 0.1
+    x = torch.rand([2, 3, 224, 224]).to(DEVICE)
+    y = model(x)
+    assert list(y.shape) == [2, 1000]
 
-    def test_init_from_graph(self):
-        model = LineModel()
-        # init using tracer
-        graph = ModuleGraph.init_from_backward_tracer(model)
-        units = DefaultChannelUnit.init_from_graph(graph)
-        self._test_units(units, model)
+
+class TestMutableChannelUnit(TestCase):
 
     def test_init_from_cfg(self):
-        model = LineModel()
+        model = SingleLineModel()
         # init using tracer
 
         config = {
             'init_args': {
                 'num_channels': 8
             },
             'channels': {
@@ -72,61 +81,52 @@
                     'end': 8,
                     'expand_ratio': 1,
                     'is_output_channel': True
                 }]
             }
         }
         units = [DefaultChannelUnit.init_from_cfg(model, config)]
-        self._test_units(units, model)
+        _test_units(units, model)
 
-    def test_init_from_channel_unit(self):
-        model = LineModel()
-        # init using tracer
-        graph = ModuleGraph.init_from_backward_tracer(model)
-        units: List[ChannelUnit] = ChannelUnit.init_from_graph(graph)
-        mutable_units = [
-            DefaultChannelUnit.init_from_channel_unit(unit) for unit in units
-        ]
-        self._test_units(mutable_units, model)
-
-    def _test_units(self, units: List[MutableChannelUnit], model):
-        for unit in units:
-            unit.prepare_for_pruning(model)
-        mutable_units = [unit for unit in units if unit.is_mutable]
-        self.assertGreaterEqual(len(mutable_units), 1)
-        for unit in mutable_units:
-            choice = unit.sample_choice()
-            unit.current_choice = choice
-            self.assertAlmostEqual(unit.current_choice, choice, delta=0.1)
-        x = torch.rand([2, 3, 224, 224]).to(DEVICE)
-        y = model(x)
-        self.assertSequenceEqual(y.shape, [2, 1000])
-
-    def _test_a_model_from_backward_tracer(self, model):
-        model.eval()
-        model = model.to(DEVICE)
-        graph = ModuleGraph.init_from_backward_tracer(model)
-        self._test_a_graph(model, graph)
-
-    def test_with_backward_tracer(self):
-        test_models = TestGraph.backward_tracer_passed_models()
-        for model_data in test_models:
-            with self.subTest(model=model_data):
-                model = model_data()
-                self._test_a_model_from_backward_tracer(model)
+    def test_init(self):
+        for UnitClass in UNITS:
+            with self.subTest(unit_class=UnitClass):
+
+                def test_units(units, model):
+                    mutable_units = [
+                        UnitClass.init_from_channel_unit(unit)
+                        for unit in units
+                    ]
+                    _test_units(mutable_units, model)
+
+                # init using tracer
+                model = SingleLineModel()
+                units: List[
+                    ChannelUnit] = ChannelUnit.init_from_channel_analyzer(
+                        model)
+                test_units(units, model)
+
+                # init using tracer config
+                model = SingleLineModel()
+                units: List[
+                    ChannelUnit] = ChannelUnit.init_from_channel_analyzer(
+                        model, analyzer=dict(type='ChannelAnalyzer'))
+                test_units(units, model)
+
+                print(units)
 
     def test_replace_with_dynamic_ops(self):
-        model_datas = TestGraph.backward_tracer_passed_models()
+        model_datas = backward_passed_library.include_models()
         for model_data in model_datas:
-            for unit_type in GROUPS:
+            for unit_type in UNITS:
                 with self.subTest(model=model_data, unit=unit_type):
                     model: nn.Module = model_data()
-                    graph = ModuleGraph.init_from_backward_tracer(model)
                     units: List[
-                        MutableChannelUnit] = unit_type.init_from_graph(graph)
+                        MutableChannelUnit] = unit_type.init_from_channel_analyzer(  # noqa
+                            model)
                     for unit in units:
                         unit.prepare_for_pruning(model)
 
                     for module in model.modules():
                         if isinstance(module, nn.Conv2d)\
                             and module.groups == module.in_channels\
                                 and module.groups == 1:
@@ -134,14 +134,7 @@
                                 isinstance(module, DynamicChannelMixin))
                         if isinstance(module, nn.Linear):
                             self.assertTrue(
                                 isinstance(module, DynamicChannelMixin))
                         if isinstance(module, nn.BatchNorm2d):
                             self.assertTrue(
                                 isinstance(module, DynamicChannelMixin))
-
-    def _test_a_graph(self, model, graph):
-        try:
-            units = DefaultChannelUnit.init_from_graph(graph)
-            self._test_units(units, model)
-        except Exception as e:
-            self.fail(f'{e}')
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_channel/test_units/test_sequential_mutable_channel_unit.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_channel/test_units/test_sequential_mutable_channel_unit.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_mutable_value.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_mutable_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,17 +69,14 @@
         assert mul_derived_mv.current_choice == 6
         assert rmul_derived_mv.current_choice == 6
 
         mv.current_choice = 2
         assert mul_derived_mv.current_choice == 4
         assert rmul_derived_mv.current_choice == 4
 
-        with pytest.raises(TypeError):
-            _ = mv * 1.2
-
         mv = MutableValue(value_list=[1, 2, 3], default_value=3)
         mc = SquentialMutableChannel(num_channels=4)
 
         with pytest.raises(TypeError):
             _ = mc * mv
         with pytest.raises(TypeError):
             _ = mv * mc
@@ -110,16 +107,13 @@
 
         derived_mv = mv // (8, 3)
         mv.current_choice = 120
         assert derived_mv.current_choice == 15
         mv.current_choice = 136
         assert derived_mv.current_choice == 18
 
-        with pytest.raises(TypeError):
-            _ = mv // 1.2
-
     def test_repr(self) -> None:
         value_list = [2, 4, 6]
         mv = MutableValue(value_list=value_list)
 
         assert repr(mv) == \
             f'MutableValue(value_list={value_list}, current_choice=2)'
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_onehotop.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_onehotop.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutables/test_oneshotop.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutables/test_oneshotop.py`

 * *Files identical despite different names*

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutators/test_channel_mutator.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_channel_mutator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import copy
-import sys
 import unittest
 from typing import Union
 
 import torch
 
+# from mmrazor.models.mutables import MutableChannelUnit
 from mmrazor.models.mutables.mutable_channel import (
     L1MutableChannelUnit, SequentialMutableChannelUnit)
 from mmrazor.models.mutators.channel_mutator import ChannelMutator
+from mmrazor.models.task_modules import ChannelAnalyzer
 from mmrazor.registry import MODELS
-from ...data.models import DynamicLinearModel
-from ...test_core.test_graph.test_graph import TestGraph
-
-sys.setrecursionlimit(2000)
+from ...data.models import DynamicAttention, DynamicLinearModel, DynamicMMBlock
+from ...data.tracer_passed_models import backward_passed_library
 
 
 @MODELS.register_module()
 class RandomChannelUnit(SequentialMutableChannelUnit):
 
     def generate_mask(self, choice: Union[int, float]) -> torch.Tensor:
         if isinstance(choice, float):
@@ -41,30 +40,37 @@
         choices = mutator.sample_choices()
         mutator.set_choices(choices)
         self.assertGreater(len(mutator.mutable_units), 0)
         x = torch.rand([2, 3, 224, 224])
         y = model(x)
         self.assertEqual(list(y.shape), [2, 1000])
 
+    def test_init(self):
+        model = backward_passed_library.include_models()[0]()
+        mutator = ChannelMutator(parse_cfg=ChannelAnalyzer())
+        mutator.prepare_from_supernet(model)
+        self.assertGreaterEqual(len(mutator.mutable_units), 1)
+        self._test_a_mutator(mutator, model)
+
     def test_sample_subnet(self):
-        data_models = TestGraph.backward_tracer_passed_models()
+        data_models = backward_passed_library.include_models()[:2]
 
         for i, data in enumerate(data_models):
             with self.subTest(i=i, data=data):
                 model = data()
 
                 mutator = ChannelMutator()
                 mutator.prepare_from_supernet(model)
 
                 self.assertGreaterEqual(len(mutator.mutable_units), 1)
 
                 self._test_a_mutator(mutator, model)
 
     def test_generic_support(self):
-        data_models = TestGraph.backward_tracer_passed_models()
+        data_models = backward_passed_library.include_models()
 
         for data_model in data_models[:1]:
             for unit_type in DATA_UNITS:
                 with self.subTest(model=data_model, unit=unit_type):
 
                     model = data_model()
 
@@ -101,15 +107,15 @@
         mutator2 = MODELS.build(config2)
         mutator2.prepare_from_supernet(model2)
         self.assertEqual(
             len(mutator.mutable_units), len(mutator2.mutable_units))
         self._test_a_mutator(mutator2, model2)
 
     def test_mix_config_tracer(self):
-        model = TestGraph.backward_tracer_passed_models()[0]()
+        model = backward_passed_library.include_models()[0]()
 
         model0 = copy.deepcopy(model)
         mutator0 = ChannelMutator()
         mutator0.prepare_from_supernet(model0)
         config = mutator0.config_template(with_unit_init_args=True)
 
         model1 = copy.deepcopy(model)
@@ -131,14 +137,38 @@
                         'type': 'OneShotMutableChannelUnit',
                         'default_args': {}
                     },
                     parse_cfg={'type': 'Predefined'})
                 mutator.prepare_from_supernet(model)
                 self._test_a_mutator(mutator, model)
 
+    def test_models_with_predefined_dynamic_op_without_pruning(self):
+        for Model in [
+                DynamicAttention,
+        ]:
+            with self.subTest(model=Model):
+                model = Model()
+                mutator = ChannelMutator(
+                    channel_unit_cfg={
+                        'type': 'OneShotMutableChannelUnit',
+                        'default_args': {
+                            'unit_predefined': True
+                        }
+                    },
+                    parse_cfg={'type': 'Predefined'})
+                mutator.prepare_from_supernet(model)
+                choices = mutator.sample_choices()
+                mutator.set_choices(choices)
+                self.assertGreater(len(mutator.mutable_units), 0)
+                x = torch.rand([2, 3, 224, 224])
+                y = model(x)
+                self.assertEqual(
+                    list(y.shape),
+                    [2, list(mutator.current_choices.values())[0]])
+
     def test_custom_group(self):
         ARCHITECTURE_CFG = dict(
             type='mmcls.ImageClassifier',
             backbone=dict(type='mmcls.MobileNetV2', widen_factor=1.5),
             neck=dict(type='mmcls.GlobalAveragePooling'),
             head=dict(
                 type='mmcls.LinearClsHead',
@@ -161,7 +191,29 @@
         ]]
 
         model2 = copy.deepcopy(model)
         mutator2 = ChannelMutator(custom_groups=custom_groups)
         mutator2.prepare_from_supernet(model2)
 
         self.assertEqual(len(mutator2.search_groups), 24)
+
+    def test_related_shortcut_layer(self):
+        for Model in [
+                DynamicMMBlock,
+        ]:
+            with self.subTest(model=Model):
+                model = Model()
+                mutator = ChannelMutator(
+                    channel_unit_cfg={
+                        'type': 'OneShotMutableChannelUnit',
+                        'default_args': {
+                            'unit_predefined': True
+                        }
+                    },
+                    parse_cfg={'type': 'Predefined'})
+                mutator.prepare_from_supernet(model)
+                choices = mutator.sample_choices()
+                mutator.set_choices(choices)
+                self.assertGreater(len(mutator.mutable_units), 0)
+                x = torch.rand([2, 3, 224, 224])
+                y = model(x)
+                self.assertEqual(list(y[-1].shape), [2, 1984, 1, 1])
```

### Comparing `mmrazor-1.0.0rc1/tests/test_models/test_mutators/test_diff_mutator.py` & `mmrazor-1.0.0rc2/tests/test_models/test_mutators/test_diff_mutator.py`

 * *Files identical despite different names*

