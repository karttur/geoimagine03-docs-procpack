---
layout: subprocess
categories: subprocess
title: MosaicTiles
processurl: subprocid-MosaicTiles
rootprocid: Tiling
subprocid: MosaicTiles
author: thomasg
excerpt: Mosaic raster tiles to regions
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
      "processid": "MosaicTiles",
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
        "celltype": "auto",
        "export": "False",
        "movieframes": "False"
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
