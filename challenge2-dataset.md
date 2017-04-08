---
layout: page-sidebar-c2
title: Challenge @ ICCV Workshop 2017
permalink: /challenge2/dataset
---
# Low-shot Learning 

## Dataset Description
Download link coming soon. 

In order to facilitate the second challenge, we provide three datasets as follows. 

1, Base set

This dataset is provided to build models with general facial perceptions. For example, to learn face representation, calculate average face, etc. In this dataset, there are 20K celebrities, each with 60-100 images. We selected these 20K celebrities from our 100K celebrity list and cleaned the dataset by running algorithms to remove outliers. To verify the data accuracy after cleaning, we randomly selected 2000 images from the base dataset and obtained the estimate of the labeling accuracy as about 99%. 

2, Novel set

This dataset contains 1000 celebrities, who are NOT included in the 20K celebrity list in the base set. There are limited number (1, 2, 5) 
of training images for each celebrity in this dataset. Participants are required to train models using the images in this dataset to recognize the same 1000 celebrities in the test set.  

3, Test set

The test set is used to evaluate the performance of the recognizer on the 1000 celebrities in the novel set. We provide 10 images per celebrity so there are 10,000 test images in total. We have run a de-duplicate algorithm to ensure that no test image is included in the novel set. 
