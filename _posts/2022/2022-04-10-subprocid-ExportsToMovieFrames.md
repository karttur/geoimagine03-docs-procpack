---
layout: subprocess
categories: subprocess
title: ExportsToMovieFrames
processurl: subprocid-ExportsToMovieFrames
rootprocid: Export
subprocid: ExportsToMovieFrames
author: thomasg
excerpt: Convert exported images to movie frames
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
      "processid": "ExportsToMovieFrames",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "name": "default",
        "width": "0",
        "crop": "",
        "border": "0",
        "bordercolor": "black",
        "emboss": "KARTTUR",
        "embossdims": "",
        "embossptsize": "",
        "asscript": "True",
        "vectoroverlay": ""
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "layerid": "copy",
        "prefix": "copy",
        "srccomp": "*",
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
