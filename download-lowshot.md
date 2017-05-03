---
layout: page-download
title: LSAligned
permalink: /download/lowshot
---

**Purpose**: This data set is used to support the low shot learning challenge [here](/challenge2/2017). We provide aligned version (face region is cropped and aligned) here. If non-aligned version is needed, please use ImageURL to fetch from the cropped version [here](/download/cropped). 
* Download link
  * Base Set: 22GB: [Download](https://msceleb1mdata.blob.core.windows.net/trainingls/TrainData_Base.zip)
  * Novel Set: 26MB: [One image per celebrity](https://msceleb1mdata.blob.core.windows.net/trainingls/TrainValData_lowshot.tsv); 52MB: [Two images per celebrity](https://msceleb1mdata.blob.core.windows.net/trainingls/TrainData_lowshot_top2.tsv);
  131MB: [Five images per celebrity](https://msceleb1mdata.blob.core.windows.net/trainingls/TrainData_lowshot_top5.tsv)
* File format: text files, each line is an image record containing 5 columns, delimited by TAB.
  * Column1: Image ID
  * Column2: FaceData_Base64Encoded
  * Column3: Freebase MID
  * Column4: ImageSearchRank
  * Column5: ImageURL