---
layout: subprocess
categories: subprocess
title: MosaicAdjacentTiles
processurl: subprocid-MosaicAdjacentTiles
rootprocid: Tiling
subprocid: MosaicAdjacentTiles
author: thomasg
excerpt: Expand tiles by mosaic adjacent tiles
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
      "processid": "MosaicAdjacentTiles",
      "parameters": {
        "version": "1.3",
        "asscript": "False",
        "fillnodata": "False",
        "fillmaxdist": "10",
        "fillsmooth": "0",
        "overlay": "mean",
        "tr_xres": "0",
        "tr_yres": "0",
        "resample": "near",
        "overlap": "101"
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
        "srccomp": "*",
        "suffix": "auto"
      },
      "dstpath": {
        "volume": "",
        "hdr": "vrt",
        "dat": ""
      }
    }
  ]
}
```
