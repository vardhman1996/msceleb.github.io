---
layout: page-sidebar-c2
title: Challenge @ ICCV Workshop 2017
permalink: /challenge2/evaluation
---
# Low-shot Learning 

## Measurement Set

We prepare both the development set and test set as follows. 

| Dataset                  | Purpose           | Face Aligned or Not     |
| -------------------------|-------------------| -------------------     |
| Development Set   | Development (label provided)    | Face aligned     |
| Test Set      | Test (no label provided)        | Face aligned         |

For the development set, participants can download [here](https://1drv.ms/f/s!AsQPov4_i5H0gS25WJnbzgRqefVU). 
The development set is a tsv file, in which each line 
has the following format (delimited by tab).

* Column1: Base set or novel set
* Column2: Image ID
* Column3: FaceData_Base64Encoded
* Column4: Freebase MID
* Column5: ImageURL

For the test set, 
participants need to register [here](http://imhub-eastus2.cloudapp.net:9999/user/sign-in)
to receive the download link for these datasets.
We will send emails with download link one week before the final results announcement (tentatively July 14th). 
Please provide the experimental results in a tsv file, in which each line has the following format (delimited by tab). 

* Column1: ImageURL
* Column2: FaceID
* Column3: MID estimated 
* Column4: Confidence score

Note that since we focus on low-shot learning in this challenge, 
we only provide the aligned face option for easier comparison.  

## Evaluation Protocol

We will rank all the participants according to their performance on the novel set, 
while monitor the performance on the base set. 
More specifically, first, participants need to achieve at least 98% top-1 accuracy on the base set to make 
their results valid. 
Second, the teams will be ranked according to the coverage at precision = 99% on the novel set. (**Note: evaluate with the one example per novel class option.**)

Please note this year, if the participants achieve 99% top-1 accuracy on the base set, their score will be ranked separately. 
Next year, we will improve the minimum requirement of top-1 accuracy on the base set set to be 99%. 
Since this year is the first time 
we hold this low-shot learning challenge, we lower the minimum requirement to 98% to encourage more participants.

