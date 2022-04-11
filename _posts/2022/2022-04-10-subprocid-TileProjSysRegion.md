---
layout: subprocess
categories: subprocess
title: TileProjSysRegion
processurl: subprocid-TileProjSysRegion
rootprocid: Tiling
subprocid: TileProjSysRegion
author: thomasg
excerpt: Tile regional data
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
      "processid": "TileProjSysRegion",
      "parameters": {
        "version": "1.3",
        "asscript": "False",
        "src_defregid": "",
        "tr_xres": "463.313",
        "tr_yres": "463.313",
        "resample": "near",
        "celltype": "auto",
        "srcnodata": "-222",
        "dstnodata": "-222",
        "errorthreshold": "0"
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
