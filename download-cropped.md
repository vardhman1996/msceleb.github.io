---
layout: page-download
title: Cropped
permalink: /download/cropped
---

### Cropped face images

**Purpose**: Faces are cropped with enough background region, and meant to let participants run their own face detector and alignment for more flexibility.
![Alt](../assets/dataset/irc_facecroppedsample.jpg "irc_facecroppedsample")
* Two forms (data are the same)
  * Compressed to one big zip File: 104GB, [download](https://msceleb.blob.core.windows.net/ms-celeb-v1-zip/MsCelebV1-Faces-Cropped.zip), [MD5](https://msceleb.blob.core.windows.net/ms-celeb-v1-zip/MsCelebV1-Faces-Cropped.zip.md5)
  * Split to multiple 20GB files: [File URL List](https://msceleb.blob.core.windows.net/ms-celeb-v1-cropped-split?restype=container&amp;comp=list), [MD5](https://msceleb.blob.core.windows.net/ms-celeb-v1-cropped-split/md5.txt)
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