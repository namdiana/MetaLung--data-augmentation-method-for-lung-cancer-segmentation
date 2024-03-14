# MetaLung: Meticulous affine-transformation-based lung cancer augmentation method

A novel method has been introduced for lung cancer segmentation, is applicable for lung cancer classification as well. The method has been implemented in Python 3.7.

## Overview

This repository includes a Jupyter Notebook (`EDA+metrics+CNN.ipynb`) that covers the following aspects:
1. Preprocessing of one DICOM image
2. Lung area segmentation with thresholding-based algorithms
3. Application of MetaLung on a single image
4. Comparing baseline models with models using MetaLung involves assessing their performance and effectiveness for lung cancer segmentation based on DICE, IoU, Precision, and Recall


The MetaLung method has been evaluated for lung cancer segmentation based on three CNN models:
- U-Net [1]
- DeepLabV3 [2]
- Mask RCNN [3]

Evaluation metrics include DICE, IoU, Precision, and Recall.

## Provided Weights

Weights have been provided for all three models in the following formats:
- Baseline: The model trained without data augmentation.
- MetaLung: The model trained with the application of MetaLung with the same number of parameters.
  
All weights could be available here [4].

- `deeplabv3_baseline.pth`
- `deeplabv3_all_metalung.pth`
- `maskrcnn_baseline.pth`
- `maskrcnn_all_metalung.pth`
- `u-net_baseline.pth`
- `u-net_all_metalung.pth`

## Visualization

Visualization of MetaLung on a single image with a corresponding labeled mask has been provided.

## Dataset
The dataset is a combination of original Kazakstani data with an open-source LIDC-IDRI dataset [5].
The dataset for training and evaluating models could be available [6].

## References

<br>[1] [U-Net: Convolutional networks for biomedical image segmentation](https://arxiv.org/abs/1505.04597)
<br>[2] [Rethinking Atrous Convolution for Semantic Image Segmentation](https://arxiv.org/abs/1706.05587)
<br>[3] [Mask R-CNN](https://arxiv.org/abs/1703.06870)
<br>[4] [Pre-trained weights for application of MetaLung (Meticulous affine-transformation-based lung cancer augmentation method) and baseline model](https://doi.org/10.5281/zenodo.10800818)
<br>[5] [LIDC-IDRI Dataset](https://doi.org/10.7937/K9/TCIA.2015.LO9QL9SX)
<br>[6] [Lung Cancer Segmentation Dataset with Lung-RADS Class](https://data.mendeley.com/datasets/5rr22hgzwr/1)
