---
layout: page-download
title: LSAligned
permalink: /download/lowshot
---

**Purpose**: This data set is used to support the low shot learning challenge [here](/challenge2/2017). We provide aligned version (face region is cropped and aligned) here. If non-aligned version is needed, please use ImageURL to fetch from the cropped version [here](/download/cropped). 
* Download link
  * Base Set: 22GB: [Download](https://msceleb1mdata.blob.core.windows.net/trainingls/TrainData_Base.zip)
  * Novel Set: 26MB: [One image per celebrity](https://msceleb1mdata.blob.core.windows.net/trainingls/TrainValData_lowshot.tsv); We remove datasets which contain two/five images per celebrity since they are no more needed. 
  * Backup download link for both the above datasets: [Onedrive](https://1drv.ms/f/s!AsQPov4_i5H0gTVKQFcprgEeGLOF).
* File format: text files, each line is an image record containing 5 columns, delimited by TAB.
  * Column1: Image ID
  * Column2: FaceData_Base64Encoded
  * Column3: Freebase MID
  * Column4: ImageSearchRank
  * Column5: ImageURL