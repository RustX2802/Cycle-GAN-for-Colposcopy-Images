# Cycle-GAN-for-Colposcopy-Images

## Background

<p align="center">
<img src="./Cycle GAN concept.png" width="458" height="190" alt="General idea of the CycleGAN" />
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
to [this jupyter notebook](./Colposcopy_Cycle_GAN.ipynb).

## Dataset
You can collect the dataset from the following website:
https://screening.iarc.fr/atlascolpo.php

# Columns in info.csv

*Note: some values can be null*

**Image_name**  : {patient_id}_{photo#}

> There can be multiple photos for a patient `ex) 125_1, 125_2, 125_3`

**Age** :

**HPV status** :

- `1` : Positive 
- `0` : Negative

**TZ_Type :**  Transformation_zone

- `1` : type 1
- `2` : type 2
- `3` : type 3

**Solution** :

- `saline` : *normal saline*
- `saline green` : *normal saline with green filter*
- `acetic` : *acetic acid*
- `acetic green` : *acetic acid with green filter*
- `iodine` : *Lugol’s iodine*
- etc..

**label** : Perform the biopsy if the label is not 0 

- `0` : normal 
- `1` : LSIL 
- `2` : HSIL
