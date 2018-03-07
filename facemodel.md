---
layout: default
title: Recognizing One Million Celebrities
permalink: /facemodel/
---

# Face Model Zoo

### MS-Celeb-1M Challenge 1 Model: from SMILE Lab@NEU 2016


* Model purpose: to recognize large-scale celebrities from their face images

* Training data: the cropped and aligned version of the MS-Celeb-1M dataset, [dataset download page](/download/aligned); no external data used.

* Brief description: quote from the authors "Due to the large amont of training images (~8.5 millions), we reduce the total training epochs to 30 epochs, and lower the learning rate from 0.1 to 0.01 after 10 epochs, and to 0.001 after 20 epochs. All other settings are the same with original ResNet training setting."

* Performance: measured with the benchmark offered by MS-Celeb-1M Challenge 1, described [here](/celeb1m/evaluation);
	* Coverage @ Precision = 0.95, Random set: 0.734
	* Coverage @ Precision = 0.95, Hard set: 0.534

* **Download**: [code](https://github.com/wuyuebupt/MSCeleb1MTensorflowModel); [model](https://drive.google.com/open?id=1-P0umHM4BowoM1qckEVaqEIAI2SHwJzL)

* Reference paper
<dl>
    <pre>
	@INPROCEEDINGS{ACMMMMSCeleb1M-2,
		author = {Wu, Yue and Li, Jun and Kong, Yu and Fu, Yun},
		title = {Deep Convolutional Neural Network with Independent Softmax for Large Scale Face Recognition},
		booktitle = {ACM Multimedia},
		year = {2016},
		location = {Amsterdam, The Netherlands},
		pages = {1063--1067}}</pre>
</dl>

### MS-Celeb-1M Challenge 2 Model: SMILE Lab@NEU 2017

* Model purpose: one-shot face recognition, large-scale celebrities recognition with extremely imbalanced training data

* Training data: MS-Celeb-1M low-shot training dataset, [dataset download page](/download/lowshot); no external data used.

* Brief description: the winner solution (no external data option) for the MS-Celeb-1M Challenge-2 @ ICCV 2017 Workshop  

* Performance: measured with the benchmark offered by MS-Celeb-1M Challenge 2, described [here](/challenge2/evaluation);
	* Base set, Top-1 accuracy: 0.9959
	* One-shot set, Coverage @ Precision = 0.99: 0.9264

* **Download**: [code](https://github.com/wuyuebupt/hybridClassifier) 

* Reference paper
<dl>
    <pre>
	@INPROCEEDINGS{ICCVWorkshop-2,
		author = {Wu, Yue and Hongfu Liu and Fu, Yun},
		title = {Low-shot Face Recognition with Hybrid Classifiers},
		booktitle ={ICCV Workshop} ,
		year = {2017}
	} </pre>
</dl>

### Face Verification Model-v1: Visual Intelligence Group (VIG) at Microsoft

* Model purpose: face feature extraction

* Training data: MS-Celeb-1M low-shot training dataset (only baseset used, about one million images), [dataset download page](/download/lowshot);

* Brief description: ResNet-34  

* Performance: measured with [lfw](http://vis-www.cs.umass.edu/lfw/) verification task;
	* Mean accuracy without cosine bundle: 0.9888 
	* Mean accuracy with cosine bundle: 0.9928 


* Reference paper
<dl>
    <pre>
	@article { lowshotface,
           author = {Guo, Yandong and Zhang, Lei},
           title = {One-shot Face Recognition by Promoting Underrepresented Classes},
           Journal   = {arXiv preprint arXiv:1707.05574},
           Year      = {2017}}</pre>
</dl>


### Face Verification Model-v2: Visual Intelligence Group (VIG) at Microsoft

* Model purpose: face feature extraction

* Training data: MS-Celeb-1M dataset (cleaned version, about four million images), cropped and aligned version [dataset download page](/download/aligned);

* Brief description: standard softmax and cosine bundle, with ResNet-34  
	* Top performer with public data, highly reproducible

* **Performance**: measured with [lfw](http://vis-www.cs.umass.edu/lfw/) verification task ; 
	* Mean accuracy: **0.9971**

* Reference paper
<dl>
    <pre>
	@article {lowshotface,
           author = {Guo, Yandong and Zhang, Lei},
           title = {One-shot Face Recognition by Promoting Underrepresented Classes},
           Journal   = {arXiv preprint arXiv:1707.05574},
           Year      = {2017}}</pre>
</dl>

### Face Verification Model: Visual Geometry Group (VGG)

* Model purpose: face feature extraction

* Training data: VGG Face2 dataset [dataset description page](http://www.robots.ox.ac.uk/~vgg/data/vgg_face2/);

* Brief description: ResNet-50/SE-ResNet-50  
	* Top performer with public data, highly reproducible

* **Performance**: IARPA Janus Benchmark tasks (please refer to the paper for detailed results); 
	* IJB-A, FAR = 0.001, TAR = 0.921
	* IJB-B, FAR = 0.00001, TAR = 0.705

* Reference paper
<dl>
    <pre>
	@article {VGGFace2,
           author = {Qiong Cao and Li Shen and Weidi Xie and Omkar M. Parkhi and Andrew Zisserman},
           title = {VGGFace2: A dataset for recognising faces across pose and age},
           Journal   = {arXiv preprint arXiv:1710.08092},
           Year      = {2017}}</pre>
</dl>
