---
layout: page-download
title: Full
permalink: /download/full
---

### Full ImageThumbnails data
![Alt](../assets/dataset/irc_imagethumbnailssample.jpg "irc_imagethumbnailssample")
**Purpose**: Whole images are down sampled to up to 300*300 thumbnails, which are meant to provide the complete contextual information of the faces.
* Two forms (data are the same)
  * Compressed to one big zip File: 150GB, [download](https://msceleb.blob.core.windows.net/ms-celeb-v1-zip/MsCelebV1-ImageThumbnails.zip), [MD5](https://msceleb.blob.core.windows.net/ms-celeb-v1-zip/MsCelebV1-ImageThumbnails.zip.md5)
  * Split to multiple 20GB files: [File URL List](https://msceleb.blob.core.windows.net/ms-celeb-v1-split?restype=container&amp;comp=list), [MD5](https://msceleb.blob.core.windows.net/ms-celeb-v1-split/MD5.txt)
* Some statistics:
  * \# of Entities: 99,952
  * \# of Lines: 10,490,534
  * Image Resolution: up to 300*300
  * Average Image \# per Entity: 105
  * Total file size (uncompressed): 214GB
* File format: text files, each line is an image record containing 6 columns, delimited by TAB.
  * Column1: Freebase MID
  * Column2: Query/Name
  * Column3: ImageSearchRank
  * Column4: ImageURL
  * Column5: PageURL
  * Column6: ImageData_Base64Encoded