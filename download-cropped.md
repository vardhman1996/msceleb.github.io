---
layout: page-download
title: Cropped
permalink: /download/cropped
---

### Cropped face images

**Purpose**: Faces are cropped with enough background region, and meant to let participants run their own face detector and alignment for more flexibility.
![Alt](../assets/dataset/irc_facecroppedsample.jpg "irc_facecroppedsample")
* Download link
  * OneDrive: 14 files, 106GB [download](https://1drv.ms/f/s!AsQPov4_i5H0a3PQxcNHK39AW70)
* Some statistics:
  * \# of Entities: 99,892
  * \# of Lines: 8,456,240
  * Image Resolution: up to 300*300
  * Average Image\# per Entity: 85
  * Total file size (uncompressed): 152GB
* File format: text files, each line is an image record containing 7 columns, delimited by TAB.
  * Column1: Freebase MID
  * Column2: ImageSearchRank
  * Column3: ImageURL
  * Column4: PageURL
  * Column5: FaceID
  * Column6: FaceRectangle_Base64Encoded (four floats, relative coordinates of UpperLeft and BottomRight corner)
  * Column7: FaceData_Base64Encoded