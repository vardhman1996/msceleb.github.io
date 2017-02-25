---
layout: page-sidebar
title: Challenge
permalink: /challenge/msceleb17
---

## <center>Next: MSCeleb1M 2017</center>
### <center>details will be announced soon</center>
![irc_ms-celeb-1m-sample0](../assets/irc_ms-celeb-1m-sample0.jpg)

## Task Description:

This year we still focus on face recognition task. The contestants are asked to develop image recognition system based on, **but not limited to**, the datasets provided by the Challenge (as training data) to recognize 1M celebrities from their face images.

The 1M celebrities are obtained from Freebase based on their occurrence frequencies (popularities) on the web. Grounding the face recognition task to a knowledge base has many advantages. First, each people entity on Freebase is unique and clearly defined without disambiguation, making it possible to define such a large scale face recognition task. Second, each entity naturally has multiple properties (e.g. gender, date of birth, occupation), providing rich and valuable information for data collecting, cleaning, and multiple task learning.

The measurement set consists of 1000 celebrities sampled from the 1M celebrities, and for each celebrity we have manually labeled up to 20 images scrapped from commercial image search engines. But the identities of these 1000 celebrities will not be disclosed, so that the contestants cannot optimize just for these 1000 celebrities. To obtain high recognition recall and precision rates, the contestants will have to develop a recognizer to cover as many as possible celebrities, which will be of great value to help advance the state of the art in face recognition.

A contesting system is asked to produce 5 or less labels for a test image, ordered by confidence scores. Top one accuracies will be evaluated against a pre-labeled image dataset, which will be used during evaluation stage.

**Note: Commercial/public intelligent services are not allowed to be called during the evaluation, e.g. [Microsoft Cognitive Servcies](https://www.microsoft.com/cognitive-services), etc. We will detect and ban the contestants for this kind of behavior.**