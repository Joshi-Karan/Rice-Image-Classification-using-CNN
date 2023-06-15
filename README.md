# Rice-Image-Classification-using-CNN
![Status](https://img.shields.io/badge/Status-Completed-yellowgreen.svg)

## Dataset

Rice MSC Dataset: <a href="https://www.muratkoklu.com/datasets/">link</a><br>
(Kaggle Link --> <a href="https://www.kaggle.com/datasets/muratkokludataset/rice-image-dataset">link</a>)
<br>

## Dataset Overview

The Rice Image Dataset is a collection of 75,000 images of rice grains, each of which is labeled with one of five rice varieties: Arborio, Basmati, Ipsala, Jasmine, and Karacadag
<br>

## Model Summary
```
Model: "sequential"
_________________________________________________________________

Layer (type)                Output Shape              Param #
=================================================================

 zero_padding2d (ZeroPadding  (None, 226, 226, 3)      0
 2D)

 conv2d (Conv2D)             (None, 224, 224, 32)      896

 batch_normalization (BatchN  (None, 224, 224, 32)     128
 ormalization)

 max_pooling2d (MaxPooling2D  (None, 112, 112, 32)     0
 )

 zero_padding2d_1 (ZeroPaddi  (None, 114, 114, 32)     0
 ng2D)

 conv2d_1 (Conv2D)           (None, 112, 112, 64)      18496

 batch_normalization_1 (Batc  (None, 112, 112, 64)     256
 hNormalization)

 max_pooling2d_1 (MaxPooling  (None, 56, 56, 64)       0
 2D)

 flatten (Flatten)           (None, 200704)            0

 dense (Dense)               (None, 128)               25690240  

 dropout (Dropout)           (None, 128)               0

 dense_1 (Dense)             (None, 64)                8256

 dropout_1 (Dropout)         (None, 64)                0

 dense_2 (Dense)             (None, 32)                2080

 dropout_2 (Dropout)         (None, 32)                0

 dense_3 (Dense)             (None, 5)                 165

=================================================================
Total params: 25,720,517
Trainable params: 25,720,325
Non-trainable params: 192
_________________________________________________________________
```
<br>

## Citation Request
```
1: KOKLU, M., CINAR, I. and TASPINAR, Y. S. (2021). Classification of rice varieties with deep learning methods. Computers and Electronics in Agriculture, 187, 106285.
DOI: https://doi.org/10.1016/j.compag.2021.106285

2: CINAR, I. and KOKLU, M. (2021). Determination of Effective and Specific Physical Features of Rice Varieties by Computer Vision In Exterior Quality Inspection. Selcuk Journal of Agriculture and Food Sciences, 35(3), 229-243.
DOI: https://doi.org/10.15316/SJAFS.2021.252

3: CINAR, I. and KOKLU, M. (2022). Identification of Rice Varieties Using Machine Learning Algorithms. Journal of Agricultural Sciences, 28 (2), 307-325.
DOI: https://doi.org/10.15832/ankutbd.862482

4: CINAR, I. and KOKLU, M. (2019). Classification of Rice Varieties Using Artificial Intelligence Methods. International Journal of Intelligent Systems and Applications in Engineering, 7(3), 188-194.
DOI: https://doi.org/10.18201/ijisae.2019355381
```