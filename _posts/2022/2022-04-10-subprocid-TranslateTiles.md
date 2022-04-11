---
layout: subprocess
categories: subprocess
title: TranslateTiles
processurl: subprocid-TranslateTiles
rootprocid: Translate
subprocid: TranslateTiles
author: thomasg
excerpt: Translate tiles using gdal_translate
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
      "processid": "TranslateTiles",
      "parameters": {
        "version": "1.3",
        "asscript": "False",
        "dstEPSG": "0",
        "xoff": "0",
        "yoff": "0",
        "xsize": "0",
        "ysize": "0",
        "tr_xres": "0.0",
        "tr_yres": "0.0",
        "resample": "near",
        "autofitextent": "True",
        "src_min": "0.0",
        "src_max": "0.0",
        "dst_min": "0.0",
        "dst_max": "0.0",
        "exponent": "0.0",
        "unscale": "False",
        "dst_ulx": "0.0",
        "dst_uly": "0.0",
        "dst_lrx": "0.0",
        "dst_lry": "0.0",
        "nodata": "-22.22",
        "celltype": "auto"
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
        "srccomp": "*",
        "layerid": "*"
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
