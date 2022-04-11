---
layout: subprocess
categories: subprocess
title: resampleSpatialModisRegion
processurl: subprocid-resampleSpatialModisRegion
rootprocid: MODISProc
subprocid: resampleSpatialModisRegion
author: thomasg
excerpt: Tile regional SMAP data to fit modis
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
      "processid": "resampleSpatialModisRegion",
      "parameters": {
        "version": "1.3",
        "asscript": "True",
        "epsg": "6842",
        "xres": "463.313",
        "yres": "463.313",
        "resample": "near",
        "copycomp": "1to1",
        "suffix": "copy",
        "celltype": "auto"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "region",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": "",
            "system": "smap"
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "region",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": "",
            "system": "smap"
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
