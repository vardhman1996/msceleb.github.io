---
layout: page-sidebar-c2
title: Challenge @ ICCV Workshop 2017
permalink: /challenge2/dataset
---
# Low-shot Learning 

## Dataset Description
Download page is [here](/download/lowshot). 

In order to facilitate the second challenge, we provide three datasets as follows.

* **Training set part one:** 
this dataset contains the training images for the base set. This dataset is provided to build models with general facial perceptions. For example, to learn face representation, calculate average face, etc. In this dataset, there are 20K celebrities, each with 50-100 images. We selected these 20K celebrities from our 100K celebrity list and cleaned the dataset by running algorithms to remove outliers. To verify the data accuracy after cleaning, we randomly selected 2000 images from the base dataset and obtained the estimate of the labeling accuracy as about 99.5%.

* **Training set part two:** 
this dataset contains the training images for the novel set. This dataset contains 1000 celebrities, who are NOT included in the 20K celebrity list in the training set one. There are limited number (1, 2, 5) of training images for each celebrity in this dataset. Participants are required to train models using the images in this dataset to recognize the same 1000 celebrities in the test set.

* **Test set**
Our measurement set contains a mixture of test images from both the base set and the novel set. We provide about 5 test images per celebrity in the base set while 20 images per celebrity in the novel set. We have run a de-duplicate algorithm to ensure that no test image is included in either of the training sets.