# Nuclei-segmentation
This repository is related to the [Selected Topics in Visual Recognition using Deep Learning Homework 3](https://docs.google.com/presentation/d/1AO3PtF3oJF1J0VzeowVpUhW50i9CEWHPTcvOYzx5waE/edit#slide=id.gfd55e7c5d5_0_0).

Nuclear segmentation dataset contains 24 training images with 14,598 nuclear and 6 test images with 2,360 nuclear 

Train an instance segmentation model to detect and segment all the nuclei in the image


## Environment
Google Colab

## Data prepare
see VRDL_HW3_dataset.ipynb , or open it on Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_lK0E1X9eJyx2qL402g3P3Bd6Dt3fojX?usp=sharing)

I use 20 images for training and 4 images for validation.

use imantics to deal with the mask image and turn them into COCO format.

[Reference about imantics](https://zhuanlan.zhihu.com/p/427096258)

## Getting started
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1txqjU1ywal8PpNwO_AGO0eo0-6ojGZPM?usp=sharing)

please use colab to open the file "inference.ipynb"
just execute this file on colab,

it will automatically load the model and reproduce submission file



## Training 
see VRDL_HW3_train.ipynb , or open it on Colab

if you want to try this file, please change the file path in code

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19LVdkdQ0CAGWcPlUaBQC2iKCUBsZrjXs?usp=sharing)

pre-train model: "COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml" in model zoo

Hyperparameters:
* Learning algorithm: Stochastic Gradient Descent (SGD)
* Batch size: 2
* Learning rate: 0.00025
* The number of iterations: 20000 

## My training weight

https://drive.google.com/file/d/1RUtuR7hJozGfQciULRCSds9DV3XJcauS/view?usp=sharing

## Reference

https://colab.research.google.com/drive/16jcaJoc6bCFAQ96jDe2HwtXj7BMD_-m5?usp=sharing


