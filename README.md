# Cycle-GAN-for-Colposcopy-Images

## Background

<p align="center">
<img src="./attack.png" width="458" height="190" alt="General idea of the CycleGAN" />
</p>

CycleGAN is a very popular GAN architecture primarily
being used to learn transformation between images of
different styles. Here, CycleGAN is applied to learn a
transformation between images of normal and abnormal
cells. Figure above clearly describes the general idea of the
CycleGAN, showcasing how an input normal cell image is
generated into an abnormal cell image and then cycled back
and generated into a normal cell image.

## Getting Started
This repository contains the main code for the generation of high-quality cell images, thereby
solving the problem of insufficient data. It has a
simple API and can be easily used for own projects. The whole project consists
of python code by utilizing PyTorch framework.

### Jupyter Notebook
To implement Cycle GAN on a Colposcopy dataset, please refer
to [this jupyter notebook](./scaleatt/video_scale_attack.ipynb).

## Dataset
You can collect the dataset from the following website:
https://screening.iarc.fr/atlascolpo.php
