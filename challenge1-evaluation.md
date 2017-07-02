---
layout: page-sidebar
title: Dataset
permalink: /celeb1m/evaluation
---
# Recognizing One Million Celebrities 
## Measurement Set

There are several datasets for measurement purpose. 
To clarify, 
we summarize their descriptions in the following table. 

| Dataset                  | Purpose           | Face Aligned or Not     |Random/Hard      |
| -------------------------|-------------------| -------------------|-----------------|
| Face-Aligned-Dev-1       | Development (label provided)      | Face aligned       |Hard selection  |
| Face-Aligned-Dev-2       | Development (label provided)        | Face aligned       |Random selection |
| Face-Cropped-Dev-1       | Development (label provided)        | No alignment       |Hard selection   |
| Face-Cropped-Dev-2       | Development (label provided)        | No alignment       |Random selection |
| Face-Aligned-Test-(part 1)      | Test (no label provided)              | Face aligned       |Hard selection   |
| Face-Aligned-Test-(part 2)      | Test (no label provided)              | Face aligned       |Random selection |
| Face-Cropped-Test-(part 1)      | Test (no label provided)              | No alignment       |Hard selection   |
| Face-Cropped-Test-(part 2)      | Test (no label provided)              | No alignment       |Random selection |


For the dataset with the "development" purpose, 
we release the ground truth label. 
Participants can use this dataset to develop and tune their algorithms. 
The dataset with the "development" purpose could be downloaded [here](/download/devset). 

For the datasets with the "test" purpose, 
we do NOT include the ground truth label. 
Participants need to register [here](http://imhub-eastus2.cloudapp.net:9999/user/sign-in)
to receive the download link for these datasets.
We will send emails with download link one week before the final results announcement (tentatively July 14th). 

## Evaluation
To obtain results with the test set, 
participants need to upload their results after they sign in [here](http://imhub-eastus2.cloudapp.net:9999/user/sign-in). 
We will return results within 24 hours. 

Please provide the experimental results in a tsv file, in which each line has the following format (delimited by tab). 

* Column1: ImageURL
* Column2: FaceID
* Column3: MID estimated 
* Column4: Confidence score

We give sample code and sample result files (obtained with the development set)
[here](https://1drv.ms/f/s!AsQPov4_i5H0gSVo3bxDuWWNRYQU). 
After download, please run the following command to obtain the results shown in the [paper](https://www.microsoft.com/en-us/research/publication/ms-celeb-1m-dataset-benchmark-large-scale-face-recognition-2/). 
> python PrecisionCoverageEst.py -config Curve_Development.config -pthresh 0.95

The sample results file has the following format
* Column1: Freebase MID (ground truth)
* Column2: EntityNameString
* Column3: ImageURL
* Column4: FaceID
* Column5: MID estimated 
* Column6: Confidence score

## More Information
If participants use their own alignment algorithm, 
we recommend to use the dataset with the "no alignment" option and run their own alignment algorithm. 
If participants use our aligned face images for training, 
we recommend to use the dataset with the "face aligned" option. 
The "hard selection" and "random selection" is described [here](/celeb1m/dataset).  









