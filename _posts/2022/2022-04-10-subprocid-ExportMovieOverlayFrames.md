---
layout: subprocess
categories: subprocess
title: ExportMovieOverlayFrames
processurl: subprocid-ExportMovieOverlayFrames
rootprocid: Export
subprocid: ExportMovieOverlayFrames
author: thomasg
excerpt: Convert 2 sets of exported images to movie frames with baselayer and overlayer
date: 2022-04-10
modified: 2022-04-10
comments: true
share: true
---


```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "system"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "ExportMovieOverlayFrames",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "name": "default",
        "basewidth": "0",
        "basecrop": "",
        "overlaywidth": "0",
        "gravity": "northeast",
        "geomx": "0",
        "geomy": "0",
        "emboss": "KARTTUR",
        "embossdims": "",
        "embossptsize": "0",
        "asscript": "True",
        "vector": "NA"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "srccomp": "*",
        "layerid": "copy",
        "prefix": "copy",
        "suffix": "copy"
      },
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      }
    }
  ]
}
```
