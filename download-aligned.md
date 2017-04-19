---
layout: page-download
title: SampleSet
permalink: /download/aligned
---
### Aligned face images:
![Alt](../assets/dataset/irc_facealignedsample.jpg "irc_facealignedsample")
**Purpose**: Faces are aligned by MSR's algorithm, and meant to let participants directly train models if they don't have face detector and alignment modules at hand. We will use the same alignment approach on DevSet and MeasurementSet.
* Download link
  * Compressed to one big zip File: 60GB, [download](https://msceleb1mdata.blob.core.windows.net/training/FaceImageCroppedWithAlignment.zip)
  * OneDrive: 8 files, 60GB [download](https://1drv.ms/f/s!AsQPov4_i5H0bOnQmai3Mp3hFBI)  
* Some statistics:
  * \# of Entities: 99,892
  * \# of Lines: 8,456,240
  * Image Resolution: up to 300*300
  * Average Image \# per Entity: 85
  * Total file size (uncompressed): 89 GB
* File format: text files, each line is an image record containing 7 columns, delimited by TAB.
  * Column1: Freebase MID
  * Column2: ImageSearchRank
  * Column3: ImageURL
  * Column4: PageURL
  * Column5: FaceID
  * Column6: FaceRectangle_Base64Encoded (four floats, relative coordinates of UpperLeft and BottomRight corner)
  * Column7: FaceData_Base64Encoded
d Data](https://msceleb.blob.core.windows.net/ms-celeb-v1-samples/MsCelebV1-Faces-Aligned.Samples.zip): 14 entities, 32MBceleb.blob.core.windows.net/ms-celeb-v1-samples/MsCelebV1-Faces-Aligned.Samples.zip): 14 entities, 32MB