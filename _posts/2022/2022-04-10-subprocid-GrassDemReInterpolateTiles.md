---
layout: subprocess
categories: subprocess
title: GrassDemReInterpolateTiles
processurl: subprocid-GrassDemReInterpolateTiles
rootprocid: GrassDemProc
subprocid: GrassDemReInterpolateTiles
author: thomasg
excerpt: Fill up dem pits
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
      "processid": "GrassDemReInterpolateTiles",
      "parameters": {
        "asscript": "True",
        "mosaic": "True",
        "flags": "4",
        "ew_res": "0",
        "ns_res": "0",
        "overlap": "3",
        "tension": "40",
        "tilesize": "1000",
        "tileoverlap": "10"
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
        "layerid": "*",
        "prefix": "*",
        "srccomp": "*"
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
