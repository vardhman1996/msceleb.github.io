---
layout: page-download
title: Development Set
permalink: /download/devset
---

### Development data set can be downloaded [here](https://msceleb.blob.core.windows.net/ms-celeb-v1-dev?restype=container&amp;comp=list)
**Purpose**: This data has 6 files. Each file contains 500 face images and labels, which can be used to develop/verify your recognition algorithms. They may also be used during the dry-run stage. 
  * DevSet1: "Hard Set" can be used to test the robustness of an algorithm on illumination, pose, resolution, etc. 
  * DevSet2: "Random Set" can be used to test the coverage of an algorithm among the 1M entities. Both of these two sets include cropped and aligned face images.
* Two Forms: (Form1 is extracted from Form2)
  * File format1: two zip files for DevSet1 and DevSet2 respectively. Each zip file contains two folders for 500 cropped or aligned face jpeg files. Each .jpg file is named by the FreeBase MID.
  * File format2: Four text files, each line is an image record containing 6 columns, delimited by TAB.
    * Column1: Freebase MID
    * Column2: EntityNameString
    * Column3: ImageURL
    * Column4: FaceID
    * Column5: FaceRectangle_Base64Encoded (four floats, relative coordinates of UpperLeft and BottomRight corner)
    * Column6: FaceData_Base64Encoded
* Some Statistics:
  * \# of line: 500 lines in each file
  * \# of unique MIDs: 500
  * Total file size: tsv files: 44 MB, zip files: 32MB