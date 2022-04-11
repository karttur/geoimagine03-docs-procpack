---
layout: subprocess
categories: subprocess
title: MosaicModis
processurl: subprocid-MosaicModis
rootprocid: MODISProc
subprocid: MosaicModis
author: thomasg
excerpt: Mosaic mdois raster tiles to region
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
      "processid": "MosaicModis",
      "parameters": {
        "version": "1.3",
        "overlay": "mean",
        "t_epsg": "0",
        "xres": "0",
        "yres": "0",
        "resample": "near",
        "celltype": "auto",
        "export": "False",
        "movieframes": "False",
        "copycomp": "1to1"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "region",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "region",
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
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      }
    }
  ]
}
```
