## This project is an attempt at establishing a COVID diagnosis using chest x-rays only. This project is based on the following github repository : https://github.com/ieee8023/covid-chestxray-dataset

# Project Description

To infer covid diagnosis from chest x-rays, here is the approach that I took. I divided the task in two main parts: segmenting the chest x-rays in order to keep only the relevant parts, and infering covid diagnosis from the processed x-rays.
If the first task is achieved satisfyingly, it is not the case of the second part. I have stated at the end of the second notebook the reasons I was able to identify that might explain the unsatisfying results obtained.

# How do I run it ?

To run this notebook, one needs to launch Images Diagnosis first, then Images Segmentation. The first notebook processes hundreds of images, which might cause memory errors on certain computers.

# Annotations

[Lung Bounding Boxes](https://github.com/GeneralBlockchain/covid-19-chest-xray-lung-bounding-boxes-dataset) and [Chest X-ray Segmentation](https://github.com/GeneralBlockchain/covid-19-chest-xray-segmentations-dataset) (license: CC BY 4.0) contributed by [General Blockchain, Inc.](https://github.com/GeneralBlockchain)

[Pneumonia severity scores for 94 images](annotations/covid-severity-scores.csv) (license: CC BY-SA) from the paper [Predicting COVID-19 Pneumonia Severity on Chest X-ray with Deep Learning](http://arxiv.org/abs/2005.11856)

[Generated Lung Segmentations](annotations/lungVAE-masks) (license: CC BY-SA) from the paper [Lung Segmentation from Chest X-rays using Variational Data Imputation](https://arxiv.org/abs/2005.10052)

[Brixia score for 192 images](https://github.com/BrixIA/Brixia-score-COVID-19) (license: CC BY-NC-SA) from the paper [End-to-end learning for semiquantitative rating of COVID-19 severity on Chest X-rays](https://arxiv.org/abs/2006.04603)

[Lung and other segmentations for 517 images](https://github.com/v7labs/covid-19-xray-dataset/tree/master/annotations) (license: CC BY) in COCO and raster formats by [v7labs](https://github.com/v7labs/covid-19-xray-dataset)

# References

1. O.Ronneberger, P.Fischer and T.Brox : U-Net: Convolutional Networks for Biomedical Image
Segmentation. In arXiv:1505.04597v1 [cs.CV] 18 May 2015.

2. M.Sandler, A.Howard, M.Zhu, A.Zhmoginov, and L.Chen : MobileNetV2: Inverted Residuals
and Linear Bottlenecks. In arXiv:1801.04381v4 [cs.CV] 21 Mar 2019.

3. P.Isola, J.Zhu, T.Zhou and A.Efros : Image-to-Image Translation with Conditional Adversar-
ial Networks. In arXiv:1611.07004v3 [cs.CV] 26 Nov 2018.

4. Rasmita Lenkaa, Asimananda Khandualb : Application of CNN and gated recurrent network
for visual improvement of dehazing. Materialstoday : proceeding. 16 January 2021.

5. [Priya Dwivedi : Understanding and Coding a ResNet in Keras.](https://towardsdatascience.com/understanding-and-coding-a-resnet-in-keras-446d7ff84d33) 4 June 2016 [online].

6. [Chengwei : How to do Transfer learning with Efficientnet.](https://www.dlology.com/blog/transfer-learning-with-efficientnet/) [online]

7. [Gaurav Singhal : Introduction to DenseNet with TensorFlow.](https://www.pluralsight.com/guides/introduction-to-densenet-with-tensorflow) 6 May 2020 [online].

8. [Detecting and Visualising the Infectious Regions of COVID-19 in X-ray Im-ages and CT scans Using Different Pretrained-Networks in Tensorflow 2.x.](https://github.com/zeeshannisar/COVID-19) 20 July 2020 [online].

9. [Pham, T.D. : A comprehensive study on classification of COVID-19 on computed tomography with pretrained convolutional neural networks. Sci Rep 10, 16942.](https://doi.org/10.1038/s41598-020-74164-z) 09 October 2020 [online].
